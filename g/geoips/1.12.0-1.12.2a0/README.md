# Comparing `tmp/geoips-1.12.0.tar.gz` & `tmp/geoips-1.12.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoips-1.12.0.tar", max compression
+gzip compressed data, was "geoips-1.12.2a0.tar", max compression
```

## Comparing `geoips-1.12.0.tar` & `geoips-1.12.2a0.tar`

### file list

```diff
@@ -1,535 +1,540 @@
--rw-r--r--   0        0        0     1558 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/bandit.yaml
--rw-r--r--   0        0        0     1612 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/black.yaml
--rw-r--r--   0        0        0     2992 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/build-html-docs.yaml
--rw-r--r--   0        0        0     2304 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/changelog-templates-unchanged.yaml
--rw-r--r--   0        0        0     1775 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/flake8.yaml
--rw-r--r--   0        0        0      814 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/package-and-publish.yaml
--rw-r--r--   0        0        0     4639 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/pytest-short.yaml
--rw-r--r--   0        0        0      934 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/release-note-update.yaml
--rw-r--r--   0        0        0     3131 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows/test-interfaces.yaml
--rw-r--r--   0        0        0     1083 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows_archived/docker-build-test-push.yaml
--rw-r--r--   0        0        0      559 2024-02-13 20:24:57.959904 geoips-1.12.0/.github/workflows_archived/validate-pull-request.yaml
--rw-r--r--   0        0        0     1968 2024-02-13 20:24:57.963904 geoips-1.12.0/LICENSE
--rw-r--r--   0        0        0     3226 2024-02-13 20:24:57.963904 geoips-1.12.0/README.md
--rw-r--r--   0        0        0    12015 2024-02-13 20:24:57.967903 geoips-1.12.0/docs/source/_templates/conf_PKG.py
--rw-r--r--   0        0        0     1141 2024-02-13 20:24:58.079904 geoips-1.12.0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml
--rw-r--r--   0        0        0     1131 2024-02-13 20:24:58.079904 geoips-1.12.0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1147 2024-02-13 20:24:58.079904 geoips-1.12.0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1188 2024-02-13 20:24:58.079904 geoips-1.12.0/docs/source/yaml/abi_test.yaml
--rw-r--r--   0        0        0     1474 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/__init__.py
--rw-r--r--   0        0        0      755 2024-02-13 20:25:07.963933 geoips-1.12.0/geoips/_version.py
--rw-r--r--   0        0        0     9234 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/cli.py
--rw-r--r--   0        0        0      684 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/commandline/__init__.py
--rw-r--r--   0        0        0    39007 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/commandline/args.py
--rw-r--r--   0        0        0     2199 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/commandline/create_sector_image.py
--rw-r--r--   0        0        0     3111 2024-02-13 20:24:58.079904 geoips-1.12.0/geoips/commandline/list_available_plugins.py
--rw-r--r--   0        0        0     3584 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/commandline/log_setup.py
--rw-r--r--   0        0        0     4007 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/commandline/run_procflow.py
--rwxr-xr-x   0        0        0     8764 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/commandline/test_interfaces.py
--rw-r--r--   0        0        0     1118 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/commandline/update_tc_tracks_database.py
--rw-r--r--   0        0        0    39861 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/create_plugin_registries.py
--rw-r--r--   0        0        0      691 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/data_manipulations/__init__.py
--rw-r--r--   0        0        0     2128 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/data_manipulations/conversions.py
--rw-r--r--   0        0        0    17008 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/data_manipulations/corrections.py
--rw-r--r--   0        0        0     1654 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/data_manipulations/info.py
--rw-r--r--   0        0        0     9017 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/data_manipulations/merge.py
--rw-r--r--   0        0        0      669 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/dev/__init__.py
--rw-r--r--   0        0        0    17285 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/dev/output_config.py
--rw-r--r--   0        0        0     9114 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/dev/product.py
--rw-r--r--   0        0        0     1129 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/errors.py
--rw-r--r--   0        0        0      682 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/filenames/__init__.py
--rwxr-xr-x   0        0        0    10039 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/filenames/base_paths.py
--rw-r--r--   0        0        0     2907 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/filenames/duplicate_files.py
--rw-r--r--   0        0        0    15385 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/geoips_utils.py
--rw-r--r--   0        0        0      677 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/image_utils/__init__.py
--rw-r--r--   0        0        0    11301 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/image_utils/colormap_utils.py
--rw-r--r--   0        0        0    21379 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/image_utils/maps.py
--rw-r--r--   0        0        0    25463 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/image_utils/mpl_utils.py
--rw-r--r--   0        0        0     2763 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/__init__.py
--rw-r--r--   0        0        0    35733 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/base.py
--rw-r--r--   0        0        0      689 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/__init__.py
--rw-r--r--   0        0        0     1874 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/algorithms.py
--rw-r--r--   0        0        0     1459 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/colormappers.py
--rw-r--r--   0        0        0     1437 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/coverage_checkers.py
--rw-r--r--   0        0        0     2753 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/filename_formatters.py
--rw-r--r--   0        0        0     1173 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/interpolators.py
--rw-r--r--   0        0        0    44684 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/output_checkers.py
--rw-r--r--   0        0        0     3334 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/output_formatters.py
--rw-r--r--   0        0        0     1424 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/procflows.py
--rw-r--r--   0        0        0     1173 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/readers.py
--rw-r--r--   0        0        0     1353 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/sector_adjusters.py
--rw-r--r--   0        0        0     1292 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/sector_metadata_generators.py
--rw-r--r--   0        0        0     1324 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/sector_spec_generators.py
--rw-r--r--   0        0        0     1013 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/module_based/title_formatters.py
--rw-r--r--   0        0        0      687 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/__init__.py
--rw-r--r--   0        0        0      935 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/feature_annotators.py
--rw-r--r--   0        0        0      941 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/gridline_annotators.py
--rw-r--r--   0        0        0      933 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/product_defaults.py
--rw-r--r--   0        0        0     7564 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/products.py
--rw-r--r--   0        0        0     3746 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/interfaces/yaml_based/sectors.py
--rw-r--r--   0        0        0    16543 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugin_registry.py
--rw-r--r--   0        0        0      673 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/__init__.py
--rw-r--r--   0        0        0      688 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/__init__.py
--rw-r--r--   0        0        0      683 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/__init__.py
--rw-r--r--   0        0        0      689 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py
--rw-r--r--   0        0        0     2123 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py
--rw-r--r--   0        0        0     2081 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py
--rw-r--r--   0        0        0     2581 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py
--rw-r--r--   0        0        0     2621 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py
--rw-r--r--   0        0        0      687 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py
--rw-r--r--   0        0        0     4150 2024-02-13 20:24:58.083904 geoips-1.12.0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py
--rw-r--r--   0        0        0     6821 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/single_channel.py
--rw-r--r--   0        0        0     3505 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis.py
--rw-r--r--   0        0        0     2414 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py
--rw-r--r--   0        0        0     3665 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py
--rw-r--r--   0        0        0     3463 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py
--rw-r--r--   0        0        0      688 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/algorithms/visir/__init__.py
--rw-r--r--   0        0        0      685 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/__init__.py
--rw-r--r--   0        0        0     1581 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/cmap_rgb.py
--rw-r--r--   0        0        0     5880 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py
--rw-r--r--   0        0        0      723 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py
--rw-r--r--   0        0        0     3353 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py
--rw-r--r--   0        0        0     3429 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py
--rw-r--r--   0        0        0     3428 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py
--rw-r--r--   0        0        0     3390 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py
--rw-r--r--   0        0        0     2984 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py
--rw-r--r--   0        0        0     3327 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py
--rw-r--r--   0        0        0     3326 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py
--rw-r--r--   0        0        0     3365 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py
--rw-r--r--   0        0        0     3356 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py
--rw-r--r--   0        0        0     3488 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py
--rw-r--r--   0        0        0     3069 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py
--rw-r--r--   0        0        0      706 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/tpw/__init__.py
--rw-r--r--   0        0        0     2518 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py
--rw-r--r--   0        0        0     3811 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/visir/IR_BD.py
--rw-r--r--   0        0        0     3592 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/visir/Infrared.py
--rw-r--r--   0        0        0     3557 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/visir/WV.py
--rw-r--r--   0        0        0      698 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/visir/__init__.py
--rw-r--r--   0        0        0      695 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/winds/__init__.py
--rw-r--r--   0        0        0     3806 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py
--rw-r--r--   0        0        0      690 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/__init__.py
--rw-r--r--   0        0        0     4301 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/center_radius.py
--rw-r--r--   0        0        0     2565 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py
--rw-r--r--   0        0        0     1545 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/masked_arrays.py
--rw-r--r--   0        0        0     1527 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py
--rw-r--r--   0        0        0     1540 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/rgba.py
--rw-r--r--   0        0        0     1761 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/coverage_checkers/windbarbs.py
--rw-r--r--   0        0        0      692 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/__init__.py
--rw-r--r--   0        0        0     1976 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/basic_fname.py
--rw-r--r--   0        0        0     7459 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/geoips_fname.py
--rw-r--r--   0        0        0     4224 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py
--rw-r--r--   0        0        0     2052 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/geotiff_fname.py
--rw-r--r--   0        0        0     3107 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py
--rw-r--r--   0        0        0     2951 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py
--rw-r--r--   0        0        0    14732 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/tc_fname.py
--rw-r--r--   0        0        0     1972 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py
--rw-r--r--   0        0        0     3811 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py
--rw-r--r--   0        0        0     4231 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py
--rw-r--r--   0        0        0      706 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/utils/__init__.py
--rw-r--r--   0        0        0     8187 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py
--rw-r--r--   0        0        0      686 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/__init__.py
--rw-r--r--   0        0        0      697 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py
--rw-r--r--   0        0        0     4411 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py
--rw-r--r--   0        0        0     4822 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py
--rw-r--r--   0        0        0      698 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py
--rw-r--r--   0        0        0     2985 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py
--rw-r--r--   0        0        0      692 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/utils/__init__.py
--rwxr-xr-x   0        0        0    39645 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py
--rw-r--r--   0        0        0     4693 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py
--rw-r--r--   0        0        0     5097 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/interpolators/utils/interp_scipy.py
--rw-r--r--   0        0        0     5866 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_checkers/geotiff.py
--rw-r--r--   0        0        0     8982 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_checkers/image.py
--rw-r--r--   0        0        0    10127 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_checkers/netcdf.py
--rw-r--r--   0        0        0     6182 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_checkers/text.py
--rw-r--r--   0        0        0      689 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/__init__.py
--rw-r--r--   0        0        0     3986 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/full_disk_image.py
--rw-r--r--   0        0        0     3988 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/geotiff_standard.py
--rw-r--r--   0        0        0     6729 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_annotated.py
--rw-r--r--   0        0        0     2899 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_clean.py
--rw-r--r--   0        0        0    12540 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py
--rw-r--r--   0        0        0     1630 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py
--rw-r--r--   0        0        0     5804 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/metadata_default.py
--rw-r--r--   0        0        0     7877 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/metadata_tc.py
--rw-r--r--   0        0        0     1409 2024-02-13 20:24:58.087904 geoips-1.12.0/geoips/plugins/modules/output_formatters/netcdf_geoips.py
--rw-r--r--   0        0        0     4888 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/output_formatters/netcdf_xarray.py
--rw-r--r--   0        0        0     7831 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/output_formatters/text_winds.py
--rw-r--r--   0        0        0     2870 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/output_formatters/unprojected_image.py
--rw-r--r--   0        0        0      681 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/procflows/__init__.py
--rw-r--r--   0        0        0    79036 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/procflows/config_based.py
--rw-r--r--   0        0        0    79608 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/procflows/single_source.py
--rw-r--r--   0        0        0      680 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/__init__.py
--rw-r--r--   0        0        0     6447 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/abi_l2_netcdf.py
--rw-r--r--   0        0        0    43052 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/abi_netcdf.py
--rw-r--r--   0        0        0    63703 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/ahi_hsd.py
--rw-r--r--   0        0        0    15704 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/amsr2_netcdf.py
--rw-r--r--   0        0        0     4886 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py
--rw-r--r--   0        0        0    10502 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/amsub_hdf.py
--rw-r--r--   0        0        0    19598 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/amsub_mirs.py
--rw-r--r--   0        0        0    15023 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py
--rw-r--r--   0        0        0    11734 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/atms_hdf5.py
--rw-r--r--   0        0        0    10157 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/ewsg_netcdf.py
--rw-r--r--   0        0        0     3105 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/geoips_netcdf.py
--rw-r--r--   0        0        0     9758 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/gmi_hdf5.py
--rw-r--r--   0        0        0     7409 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/imerg_hdf5.py
--rw-r--r--   0        0        0     4466 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/mimic_netcdf.py
--rw-r--r--   0        0        0    34987 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/modis_hdf4.py
--rw-r--r--   0        0        0     7592 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/saphir_hdf5.py
--rw-r--r--   0        0        0    11767 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/sar_winds_netcdf.py
--rw-r--r--   0        0        0    10592 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py
--rw-r--r--   0        0        0    10365 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py
--rwxr-xr-x   0        0        0    30586 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/seviri_hrit.py
--rw-r--r--   0        0        0     5176 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/sfc_winds_text.py
--rw-r--r--   0        0        0     4811 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py
--rw-r--r--   0        0        0    10319 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/smos_winds_netcdf.py
--rw-r--r--   0        0        0    23045 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/ssmi_binary.py
--rw-r--r--   0        0        0    48302 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/ssmis_binary.py
--rw-r--r--   0        0        0      685 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/utils/__init__.py
--rw-r--r--   0        0        0    24613 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py
--rw-r--r--   0        0        0    39075 2024-02-13 20:24:58.091904 geoips-1.12.0/geoips/plugins/modules/readers/utils/hrit_reader.py
--rw-r--r--   0        0        0     4800 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/readers/utils/remss_reader.py
--rwxr-xr-x   0        0        0    26736 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/readers/viirs_netcdf.py
--rw-r--r--   0        0        0     7650 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/readers/wfabba_ascii.py
--rw-r--r--   0        0        0    20795 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/readers/windsat_idr37_binary.py
--rw-r--r--   0        0        0     4256 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py
--rw-r--r--   0        0        0      690 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/__init__.py
--rw-r--r--   0        0        0    18201 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py
--rw-r--r--   0        0        0     6041 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py
--rw-r--r--   0        0        0      695 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/sector_spec_generators/__init__.py
--rw-r--r--   0        0        0     3073 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py
--rw-r--r--   0        0        0      689 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/title_formatters/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/title_formatters/static_standard.py
--rw-r--r--   0        0        0     2830 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/title_formatters/tc_copyright.py
--rw-r--r--   0        0        0     3061 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/modules/title_formatters/tc_standard.py
--rwxr-xr-x   0        0        0     2977 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt
--rw-r--r--   0        0        0     3353 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt
--rwxr-xr-x   0        0        0     1083 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt
--rw-r--r--   0        0        0      459 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/feature_annotators/default.yaml
--rw-r--r--   0        0        0      553 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml
--rw-r--r--   0        0        0      478 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/feature_annotators/tc_visir.yaml
--rw-r--r--   0        0        0      551 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml
--rw-r--r--   0        0        0      437 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/default.yaml
--rw-r--r--   0        0        0      473 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/tc_0p25degree.yaml
--rw-r--r--   0        0        0      463 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/tc_pmw.yaml
--rw-r--r--   0        0        0      460 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/tc_visir.yaml
--rw-r--r--   0        0        0      474 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/tc_visir_3200km.yaml
--rw-r--r--   0        0        0      460 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/gridline_annotators/tc_windspeed.yaml
--rw-r--r--   0        0        0     1033 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml
--rw-r--r--   0        0        0      559 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml
--rw-r--r--   0        0        0      554 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml
--rw-r--r--   0        0        0      559 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml
--rw-r--r--   0        0        0      554 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml
--rw-r--r--   0        0        0      559 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml
--rw-r--r--   0        0        0      550 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml
--rw-r--r--   0        0        0      547 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml
--rw-r--r--   0        0        0      543 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml
--rw-r--r--   0        0        0      573 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml
--rw-r--r--   0        0        0      568 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml
--rw-r--r--   0        0        0      579 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml
--rw-r--r--   0        0        0      574 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml
--rw-r--r--   0        0        0      547 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml
--rw-r--r--   0        0        0      547 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml
--rw-r--r--   0        0        0      553 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml
--rw-r--r--   0        0        0      548 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml
--rw-r--r--   0        0        0      467 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/color37.yaml
--rw-r--r--   0        0        0      462 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/color37Nearest.yaml
--rw-r--r--   0        0        0      573 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml
--rw-r--r--   0        0        0      568 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml
--rw-r--r--   0        0        0      579 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml
--rw-r--r--   0        0        0      574 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml
--rw-r--r--   0        0        0      547 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml
--rw-r--r--   0        0        0      563 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml
--rw-r--r--   0        0        0      558 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml
--rw-r--r--   0        0        0      547 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml
--rw-r--r--   0        0        0      557 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml
--rw-r--r--   0        0        0      552 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml
--rw-r--r--   0        0        0      467 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/color89.yaml
--rw-r--r--   0        0        0      462 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/color89Nearest.yaml
--rw-r--r--   0        0        0      560 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml
--rw-r--r--   0        0        0      290 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sectored.yaml
--rw-r--r--   0        0        0     1103 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml
--rw-r--r--   0        0        0      945 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml
--rw-r--r--   0        0        0      604 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml
--rw-r--r--   0        0        0      590 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml
--rw-r--r--   0        0        0      613 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml
--rw-r--r--   0        0        0      786 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml
--rw-r--r--   0        0        0      791 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml
--rw-r--r--   0        0        0      519 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml
--rw-r--r--   0        0        0      267 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/unmodified.yaml
--rw-r--r--   0        0        0      296 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/unsectored.yaml
--rw-r--r--   0        0        0      598 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml
--rw-r--r--   0        0        0      722 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml
--rw-r--r--   0        0        0      607 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml
--rw-r--r--   0        0        0      662 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml
--rw-r--r--   0        0        0      483 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR-GeoIPS1.yaml
--rw-r--r--   0        0        0      459 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR.yaml
--rw-r--r--   0        0        0      759 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml
--rw-r--r--   0        0        0     1053 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml
--rw-r--r--   0        0        0      599 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml
--rw-r--r--   0        0        0      599 2024-02-13 20:24:58.095904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml
--rw-r--r--   0        0        0      587 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV.yaml
--rw-r--r--   0        0        0     2429 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/abi.yaml
--rw-r--r--   0        0        0     3827 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/ahi.yaml
--rw-r--r--   0        0        0     4992 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/amsr-e.yaml
--rw-r--r--   0        0        0     7947 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/amsr2.yaml
--rw-r--r--   0        0        0     2844 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/amsu-b.yaml
--rw-r--r--   0        0        0     2244 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/ascat.yaml
--rw-r--r--   0        0        0     2280 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/ascatuhr.yaml
--rw-r--r--   0        0        0     1709 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/atms.yaml
--rw-r--r--   0        0        0    10713 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/gmi.yaml
--rw-r--r--   0        0        0     1070 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/gvar.yaml
--rw-r--r--   0        0        0     1167 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/hscat.yaml
--rw-r--r--   0        0        0      587 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/imerg.yaml
--rw-r--r--   0        0        0     2928 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/mhs.yaml
--rw-r--r--   0        0        0      824 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/mimic.yaml
--rw-r--r--   0        0        0     2186 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/modis.yaml
--rw-r--r--   0        0        0     1040 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/oscat.yaml
--rw-r--r--   0        0        0     1330 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/saphir.yaml
--rw-r--r--   0        0        0     1345 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/sar-spd.yaml
--rw-r--r--   0        0        0     2249 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/seviri.yaml
--rw-r--r--   0        0        0      881 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/smap-spd.yaml
--rw-r--r--   0        0        0      881 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/smos-spd.yaml
--rw-r--r--   0        0        0     8612 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/ssmi.yaml
--rw-r--r--   0        0        0    11093 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/ssmis.yaml
--rw-r--r--   0        0        0     8555 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/tmi.yaml
--rw-r--r--   0        0        0     2349 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/viirs.yaml
--rw-r--r--   0        0        0     3935 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/products/windsat.yaml
--rw-r--r--   0        0        0      400 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_1km_1024x1024.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_2km_1024x1024.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_1km_1400x1400.yaml
--rw-r--r--   0        0        0      400 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_2km_1400x1400.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_2km_1600x1600.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_4km_1600x1600.yaml
--rw-r--r--   0        0        0      395 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_256x256/tc_4km_256x256.yaml
--rw-r--r--   0        0        0      390 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_2km_512x512.yaml
--rw-r--r--   0        0        0      392 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_4km_512x512.yaml
--rw-r--r--   0        0        0      390 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_2km_800x800.yaml
--rw-r--r--   0        0        0      390 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_4km_800x800.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_0p1km_3200x3200.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_2500x2500.yaml
--rw-r--r--   0        0        0      398 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_3200x3200.yaml
--rw-r--r--   0        0        0      391 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_2km_template.yaml
--rw-r--r--   0        0        0      338 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_50km_barbs_template.yaml
--rw-r--r--   0        0        0      417 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_high_barbs_template.yaml
--rw-r--r--   0        0        0      341 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_low_barbs_template.yaml
--rw-r--r--   0        0        0      409 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascatuhr_barbs_template.yaml
--rw-r--r--   0        0        0      397 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_halfkm_template.yaml
--rw-r--r--   0        0        0      391 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_qkm_template.yaml
--rw-r--r--   0        0        0      340 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/dynamic/tc_web_template.yaml
--rw-r--r--   0        0        0      487 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/abu_dhabi.yaml
--rw-r--r--   0        0        0      454 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/africa.yaml
--rw-r--r--   0        0        0      463 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/african_horn.yaml
--rw-r--r--   0        0        0      463 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/alaska.yaml
--rw-r--r--   0        0        0      448 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/asia.yaml
--rw-r--r--   0        0        0      474 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/australia.yaml
--rw-r--r--   0        0        0      463 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/beijing.yaml
--rw-r--r--   0        0        0      460 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/brazil.yaml
--rw-r--r--   0        0        0      451 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/cairo.yaml
--rw-r--r--   0        0        0      457 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/canada.yaml
--rw-r--r--   0        0        0      454 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/caribbean.yaml
--rw-r--r--   0        0        0      479 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/central_america.yaml
--rw-r--r--   0        0        0      565 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/conus.yaml
--rw-r--r--   0        0        0      443 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/delhi.yaml
--rw-r--r--   0        0        0      476 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/denver.yaml
--rw-r--r--   0        0        0      461 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/e_pacific.yaml
--rw-r--r--   0        0        0      458 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/europe.yaml
--rw-r--r--   0        0        0      531 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/ewsg.yaml
--rw-r--r--   0        0        0      451 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/france.yaml
--rw-r--r--   0        0        0      516 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/global.yaml
--rw-r--r--   0        0        0      554 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/goes_east.yaml
--rw-r--r--   0        0        0      555 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/goes_west.yaml
--rw-r--r--   0        0        0      549 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/himawari.yaml
--rw-r--r--   0        0        0      461 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/indian_basin.yaml
--rw-r--r--   0        0        0      526 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/japan.yaml
--rw-r--r--   0        0        0      474 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/mediterranean.yaml
--rw-r--r--   0        0        0      477 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/melbourne.yaml
--rw-r--r--   0        0        0      491 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/meteosat_africa.yaml
--rw-r--r--   0        0        0      491 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/meteosat_europe.yaml
--rw-r--r--   0        0        0      518 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml
--rw-r--r--   0        0        0      472 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/mexico_city.yaml
--rw-r--r--   0        0        0      472 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/middle_east.yaml
--rw-r--r--   0        0        0      466 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/ne_asia.yaml
--rw-r--r--   0        0        0      458 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/north_pole.yaml
--rw-r--r--   0        0        0      451 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/paris.yaml
--rw-r--r--   0        0        0      496 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/rio_de_janeiro.yaml
--rw-r--r--   0        0        0      446 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/russia.yaml
--rw-r--r--   0        0        0      491 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/saskatchewan.yaml
--rw-r--r--   0        0        0      463 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/se_asia.yaml
--rw-r--r--   0        0        0      514 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/south_america.yaml
--rw-r--r--   0        0        0      460 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/south_pole.yaml
--rw-r--r--   0        0        0      492 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/vancouver.yaml
--rw-r--r--   0        0        0      457 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/victoria.yaml
--rw-r--r--   0        0        0      462 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/w_atlantic.yaml
--rw-r--r--   0        0        0      456 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/plugins/yaml/sectors/static/w_pacific.yaml
--rw-r--r--   0        0        0      119 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/docstring.yaml
--rw-r--r--   0        0        0      121 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/family.yaml
--rw-r--r--   0        0        0      118 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/interface.yaml
--rw-r--r--   0        0        0       96 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/name.yaml
--rw-r--r--   0        0        0      119 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/product_defaults.yaml
--rw-r--r--   0        0        0      322 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/top.yaml
--rw-r--r--   0        0        0      274 2024-02-13 20:24:58.099904 geoips-1.12.0/geoips/schema/bases/valid_identifier.yaml
--rw-r--r--   0        0        0     1215 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0     1811 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0      209 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/algorithm.yaml
--rw-r--r--   0        0        0      245 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      284 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      327 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0     1364 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      328 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      320 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      195 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/unvalidated.yaml
--rw-r--r--   0        0        0      833 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml
--rw-r--r--   0        0        0      218 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/interpolator.yaml
--rw-r--r--   0        0        0      248 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      284 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      228 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/sectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      640 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm.yaml
--rw-r--r--   0        0        0      730 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      824 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      652 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator.yaml
--rw-r--r--   0        0        0      734 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      824 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0       98 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/specs/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      169 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/unmodified.yaml
--rw-r--r--   0        0        0      237 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/unsectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      232 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/unsectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      210 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/product_defaults/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      354 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/algorithm.yaml
--rw-r--r--   0        0        0      390 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      429 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      634 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/bases/product.yaml
--rw-r--r--   0        0        0      363 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/interpolator.yaml
--rw-r--r--   0        0        0      393 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      429 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      220 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/list.yaml
--rw-r--r--   0        0        0      243 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/sectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      233 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/sectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      191 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/single.yaml
--rw-r--r--   0        0        0      179 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/unmodified.yaml
--rw-r--r--   0        0        0      247 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/unsectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      237 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/unsectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      215 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/products/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      369 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/generated.yaml
--rw-r--r--   0        0        0      217 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/atmosriver.yaml
--rw-r--r--   0        0        0      213 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/pyrocb.yaml
--rw-r--r--   0        0        0      316 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/static.yaml
--rw-r--r--   0        0        0      271 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/stitched.yaml
--rw-r--r--   0        0        0      451 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/tc.yaml
--rw-r--r--   0        0        0      244 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/metadata_families/volcano.yaml
--rw-r--r--   0        0        0      770 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/specs/area_definition.yaml
--rw-r--r--   0        0        0      746 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/specs/center.yaml
--rw-r--r--   0        0        0     2016 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/schema/sectors/static.yaml
--rw-r--r--   0        0        0      685 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/__init__.py
--rw-r--r--   0        0        0    11134 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/estimate_area_extent.py
--rw-r--r--   0        0        0    12241 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/overpass_predictor.py
--rw-r--r--   0        0        0     3880 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/projections.py
--rw-r--r--   0        0        0    11052 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/tc_tracks.py
--rw-r--r--   0        0        0    15280 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/tc_tracks_database.py
--rw-r--r--   0        0        0    26958 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/utils.py
--rw-r--r--   0        0        0     6731 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/sector_utils/yaml_utils.py
--rw-r--r--   0        0        0      682 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/utils/__init__.py
--rw-r--r--   0        0        0     2582 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/utils/decorators.py
--rw-r--r--   0        0        0     3494 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/utils/memusg.py
--rw-r--r--   0        0        0      685 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/xarray_utils/__init__.py
--rw-r--r--   0        0        0    30188 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/xarray_utils/data.py
--rw-r--r--   0        0        0     4421 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/xarray_utils/time.py
--rw-r--r--   0        0        0     1111 2024-02-13 20:24:58.103904 geoips-1.12.0/geoips/xarray_utils/xr_to_dtree.py
--rw-r--r--   0        0        0     6679 2024-02-13 20:25:07.963933 geoips-1.12.0/pyproject.toml
--rw-r--r--   0        0        0     1062 2024-02-13 20:24:58.103904 geoips-1.12.0/setup/download_test_data.py
--rw-r--r--   0        0        0     1184 2024-02-13 20:24:58.147904 geoips-1.12.0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1190 2024-02-13 20:24:58.151904 geoips-1.12.0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1188 2024-02-13 20:24:58.163904 geoips-1.12.0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1245 2024-02-13 20:24:58.199904 geoips-1.12.0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml
--rw-r--r--   0        0        0     1667 2024-02-13 20:24:58.203904 geoips-1.12.0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml
--rw-r--r--   0        0        0     1661 2024-02-13 20:24:58.211904 geoips-1.12.0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml
--rw-r--r--   0        0        0     1668 2024-02-13 20:24:58.219904 geoips-1.12.0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml
--rw-r--r--   0        0        0     1662 2024-02-13 20:24:58.227904 geoips-1.12.0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml
--rw-r--r--   0        0        0     1243 2024-02-13 20:24:58.227904 geoips-1.12.0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml
--rw-r--r--   0        0        0     1136 2024-02-13 20:24:58.231904 geoips-1.12.0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1234 2024-02-13 20:24:58.235904 geoips-1.12.0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml
--rw-r--r--   0        0        0     1222 2024-02-13 20:24:58.239904 geoips-1.12.0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml
--rw-r--r--   0        0        0     1556 2024-02-13 20:24:58.243904 geoips-1.12.0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml
--rw-r--r--   0        0        0     1569 2024-02-13 20:24:58.247904 geoips-1.12.0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml
--rw-r--r--   0        0        0     1226 2024-02-13 20:24:58.255904 geoips-1.12.0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml
--rw-r--r--   0        0        0     1382 2024-02-13 20:24:58.283904 geoips-1.12.0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml
--rw-r--r--   0        0        0     1211 2024-02-13 20:24:58.287904 geoips-1.12.0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml
--rw-r--r--   0        0        0     1131 2024-02-13 20:24:58.295904 geoips-1.12.0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1220 2024-02-13 20:24:58.299904 geoips-1.12.0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml
--rw-r--r--   0        0        0     1162 2024-02-13 20:24:58.303904 geoips-1.12.0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml
--rw-r--r--   0        0        0     1144 2024-02-13 20:24:58.303904 geoips-1.12.0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml
--rw-r--r--   0        0        0    54649 2024-02-13 20:24:58.315904 geoips-1.12.0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt
--rw-r--r--   0        0        0     1222 2024-02-13 20:24:58.315904 geoips-1.12.0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml
--rw-r--r--   0        0        0     1347 2024-02-13 20:24:58.327905 geoips-1.12.0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0      690 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml
--rw-r--r--   0        0        0      677 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml
--rw-r--r--   0        0        0      662 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml
--rw-r--r--   0        0        0     8382 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml
--rw-r--r--   0        0        0   224173 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips.yaml
--rw-r--r--   0        0        0     8892 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml
--rw-r--r--   0        0        0     3166 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml
--rw-r--r--   0        0        0     5822 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml
--rw-r--r--   0        0        0     1877 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml
--rw-r--r--   0        0        0     1997 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml
--rw-r--r--   0        0        0      626 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml
--rw-r--r--   0        0        0     2850 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugin_registries/test_plugin_registries.py
--rw-r--r--   0        0        0     2815 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py
--rw-r--r--   0        0        0     1529 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py
--rw-r--r--   0        0        0     1717 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py
--rw-r--r--   0        0        0       21 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/bases/docstring.yaml
--rw-r--r--   0        0        0       91 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/bases/valid_identifier.yaml
--rw-r--r--   0        0        0     2966 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0     1467 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0     2028 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0     2855 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      317 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0     1346 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      317 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      317 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      663 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0     1502 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0     1798 2024-02-13 20:24:58.339904 geoips-1.12.0/tests/unit_tests/schema/bad/products/bases/product.yaml
--rw-r--r--   0        0        0      385 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/bad/products/single.yaml
--rw-r--r--   0        0        0       46 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/bases/valid_identifier.yaml
--rw-r--r--   0        0        0      996 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0      288 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0      283 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      384 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      174 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0      523 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      174 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      174 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      290 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      384 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      529 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/products/bases/product.yaml
--rw-r--r--   0        0        0     1182 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/products/single.yaml
--rw-r--r--   0        0        0      460 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/good/sectors/static.yaml
--rw-r--r--   0        0        0     3650 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/schema/test_yaml_schema.py
--rw-r--r--   0        0        0     1867 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests/xarray_utils/test_dtree.py
--rw-r--r--   0        0        0     2533 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/unit_tests_long/plugins/modules/readers/test_readers.py
--rw-r--r--   0        0        0     1263 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/abi_test.yaml
--rw-r--r--   0        0        0     1500 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/abi_test_low_memory.yaml
--rw-r--r--   0        0        0     4833 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/amsr2_no_compare_full.yaml
--rw-r--r--   0        0        0     1731 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/amsr2_test.yaml
--rw-r--r--   0        0        0     1813 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/amsr2_test_low_memory.yaml
--rw-r--r--   0        0        0     1485 2024-02-13 20:24:58.343905 geoips-1.12.0/tests/yaml_configs/amsr2_test_no_compare.yaml
--rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 geoips-1.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1558 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/bandit.yaml
+-rw-r--r--   0        0        0     1613 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/black.yaml
+-rw-r--r--   0        0        0     2992 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/build-html-docs.yaml
+-rw-r--r--   0        0        0     2304 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/changelog-templates-unchanged.yaml
+-rw-r--r--   0        0        0     1775 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/flake8.yaml
+-rw-r--r--   0        0        0      814 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/package-and-publish.yaml
+-rw-r--r--   0        0        0     4598 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/pytest-short.yaml
+-rw-r--r--   0        0        0     2036 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/release-note-update.yaml
+-rw-r--r--   0        0        0     3131 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/test-interfaces.yaml
+-rw-r--r--   0        0        0     1083 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows_archived/docker-build-test-push.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows_archived/validate-pull-request.yaml
+-rw-r--r--   0        0        0     1968 2024-04-23 23:27:47.593713 geoips-1.12.2a0/LICENSE
+-rw-r--r--   0        0        0     3226 2024-04-23 23:27:47.593713 geoips-1.12.2a0/README.md
+-rw-r--r--   0        0        0    12048 2024-04-23 23:27:47.601713 geoips-1.12.2a0/docs/source/_templates/conf_PKG.py
+-rw-r--r--   0        0        0     1141 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml
+-rw-r--r--   0        0        0     1131 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1147 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1188 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/abi_test.yaml
+-rw-r--r--   0        0        0     1596 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/__init__.py
+-rw-r--r--   0        0        0      761 2024-04-23 23:27:59.649849 geoips-1.12.2a0/geoips/_version.py
+-rw-r--r--   0        0        0     9234 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/cli.py
+-rw-r--r--   0        0        0      684 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/__init__.py
+-rw-r--r--   0        0        0    39007 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/args.py
+-rw-r--r--   0        0        0     2199 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/create_sector_image.py
+-rw-r--r--   0        0        0     3111 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/list_available_plugins.py
+-rw-r--r--   0        0        0     9271 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/log_setup.py
+-rw-r--r--   0        0        0     4007 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/run_procflow.py
+-rwxr-xr-x   0        0        0     8764 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/test_interfaces.py
+-rw-r--r--   0        0        0     1118 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/update_tc_tracks_database.py
+-rw-r--r--   0        0        0    40772 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/create_plugin_registries.py
+-rw-r--r--   0        0        0      691 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/__init__.py
+-rw-r--r--   0        0        0     2128 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/conversions.py
+-rw-r--r--   0        0        0    17008 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/corrections.py
+-rw-r--r--   0        0        0     1654 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/info.py
+-rw-r--r--   0        0        0     9017 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/merge.py
+-rw-r--r--   0        0        0      669 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/dev/__init__.py
+-rw-r--r--   0        0        0    17285 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/dev/output_config.py
+-rw-r--r--   0        0        0     9114 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/dev/product.py
+-rw-r--r--   0        0        0     1129 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/errors.py
+-rw-r--r--   0        0        0      682 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/__init__.py
+-rwxr-xr-x   0        0        0    10039 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/base_paths.py
+-rw-r--r--   0        0        0     2907 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/duplicate_files.py
+-rw-r--r--   0        0        0    15385 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/geoips_utils.py
+-rw-r--r--   0        0        0      677 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/__init__.py
+-rw-r--r--   0        0        0    11301 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/colormap_utils.py
+-rw-r--r--   0        0        0    21379 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/maps.py
+-rw-r--r--   0        0        0    25463 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/mpl_utils.py
+-rw-r--r--   0        0        0     3787 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/__init__.py
+-rw-r--r--   0        0        0    35733 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/base.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/algorithms.py
+-rw-r--r--   0        0        0     1459 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/colormappers.py
+-rw-r--r--   0        0        0     1437 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/coverage_checkers.py
+-rw-r--r--   0        0        0     2753 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/filename_formatters.py
+-rw-r--r--   0        0        0     1173 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/interpolators.py
+-rw-r--r--   0        0        0    43982 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/output_checkers.py
+-rw-r--r--   0        0        0     3334 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/output_formatters.py
+-rw-r--r--   0        0        0     1424 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/procflows.py
+-rw-r--r--   0        0        0     1173 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/readers.py
+-rw-r--r--   0        0        0     1353 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_adjusters.py
+-rw-r--r--   0        0        0     1292 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_metadata_generators.py
+-rw-r--r--   0        0        0     1324 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_spec_generators.py
+-rw-r--r--   0        0        0     1013 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/title_formatters.py
+-rw-r--r--   0        0        0      687 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/feature_annotators.py
+-rw-r--r--   0        0        0      941 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/gridline_annotators.py
+-rw-r--r--   0        0        0      933 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/product_defaults.py
+-rw-r--r--   0        0        0     7564 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/products.py
+-rw-r--r--   0        0        0     3746 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/sectors.py
+-rw-r--r--   0        0        0     9534 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugin_registry.py
+-rw-r--r--   0        0        0      673 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/__init__.py
+-rw-r--r--   0        0        0      683 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py
+-rw-r--r--   0        0        0     2123 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py
+-rw-r--r--   0        0        0     2081 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py
+-rw-r--r--   0        0        0     2581 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py
+-rw-r--r--   0        0        0     2621 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py
+-rw-r--r--   0        0        0      687 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py
+-rw-r--r--   0        0        0     4150 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py
+-rw-r--r--   0        0        0     6821 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/single_channel.py
+-rw-r--r--   0        0        0     3505 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis.py
+-rw-r--r--   0        0        0     2414 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py
+-rw-r--r--   0        0        0     3665 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py
+-rw-r--r--   0        0        0     3463 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py
+-rw-r--r--   0        0        0      688 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/__init__.py
+-rw-r--r--   0        0        0     1581 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/cmap_rgb.py
+-rw-r--r--   0        0        0     5880 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py
+-rw-r--r--   0        0        0      723 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py
+-rw-r--r--   0        0        0     3353 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py
+-rw-r--r--   0        0        0     3429 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py
+-rw-r--r--   0        0        0     3428 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py
+-rw-r--r--   0        0        0     3390 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py
+-rw-r--r--   0        0        0     2984 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py
+-rw-r--r--   0        0        0     3327 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py
+-rw-r--r--   0        0        0     3326 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py
+-rw-r--r--   0        0        0     3365 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py
+-rw-r--r--   0        0        0     3356 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py
+-rw-r--r--   0        0        0     3488 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py
+-rw-r--r--   0        0        0     3069 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py
+-rw-r--r--   0        0        0      706 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/__init__.py
+-rw-r--r--   0        0        0     2518 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py
+-rw-r--r--   0        0        0     3811 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/IR_BD.py
+-rw-r--r--   0        0        0     3592 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/Infrared.py
+-rw-r--r--   0        0        0     3557 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/WV.py
+-rw-r--r--   0        0        0      698 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/__init__.py
+-rw-r--r--   0        0        0     3806 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/__init__.py
+-rw-r--r--   0        0        0     4301 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius.py
+-rw-r--r--   0        0        0     2565 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py
+-rw-r--r--   0        0        0     1545 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/masked_arrays.py
+-rw-r--r--   0        0        0     1527 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py
+-rw-r--r--   0        0        0     1540 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/rgba.py
+-rw-r--r--   0        0        0     1761 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/windbarbs.py
+-rw-r--r--   0        0        0      692 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/__init__.py
+-rw-r--r--   0        0        0     1976 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/basic_fname.py
+-rw-r--r--   0        0        0     7459 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_fname.py
+-rw-r--r--   0        0        0     4224 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py
+-rw-r--r--   0        0        0     2052 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geotiff_fname.py
+-rw-r--r--   0        0        0     3107 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py
+-rw-r--r--   0        0        0     2951 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py
+-rw-r--r--   0        0        0    14732 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_fname.py
+-rw-r--r--   0        0        0     1972 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py
+-rw-r--r--   0        0        0     3811 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py
+-rw-r--r--   0        0        0     4231 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py
+-rw-r--r--   0        0        0      706 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/__init__.py
+-rw-r--r--   0        0        0     8187 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py
+-rw-r--r--   0        0        0      686 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/__init__.py
+-rw-r--r--   0        0        0      697 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py
+-rw-r--r--   0        0        0     4411 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py
+-rw-r--r--   0        0        0     4822 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py
+-rw-r--r--   0        0        0      698 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py
+-rw-r--r--   0        0        0      692 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/__init__.py
+-rwxr-xr-x   0        0        0    39645 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py
+-rw-r--r--   0        0        0     4693 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py
+-rw-r--r--   0        0        0     5097 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_scipy.py
+-rw-r--r--   0        0        0     5679 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/geotiff.py
+-rw-r--r--   0        0        0     8331 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/image.py
+-rw-r--r--   0        0        0    11161 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/netcdf.py
+-rw-r--r--   0        0        0     5952 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/text.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/__init__.py
+-rw-r--r--   0        0        0     3986 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/full_disk_image.py
+-rw-r--r--   0        0        0     3988 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/geotiff_standard.py
+-rw-r--r--   0        0        0     6729 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_annotated.py
+-rw-r--r--   0        0        0     2899 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_clean.py
+-rw-r--r--   0        0        0    12540 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py
+-rw-r--r--   0        0        0     1630 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py
+-rw-r--r--   0        0        0     5804 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_default.py
+-rw-r--r--   0        0        0     7877 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_tc.py
+-rw-r--r--   0        0        0     1409 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_geoips.py
+-rw-r--r--   0        0        0     4888 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_xarray.py
+-rw-r--r--   0        0        0     7831 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/text_winds.py
+-rw-r--r--   0        0        0     2870 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/unprojected_image.py
+-rw-r--r--   0        0        0      681 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/procflows/__init__.py
+-rw-r--r--   0        0        0    79206 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/procflows/config_based.py
+-rw-r--r--   0        0        0    79114 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/procflows/single_source.py
+-rw-r--r--   0        0        0      680 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/__init__.py
+-rw-r--r--   0        0        0     6447 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/abi_l2_netcdf.py
+-rw-r--r--   0        0        0    42928 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/abi_netcdf.py
+-rw-r--r--   0        0        0    63750 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ahi_hsd.py
+-rw-r--r--   0        0        0    15704 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_netcdf.py
+-rw-r--r--   0        0        0     4886 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py
+-rw-r--r--   0        0        0    10502 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_hdf.py
+-rw-r--r--   0        0        0    19598 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_mirs.py
+-rw-r--r--   0        0        0    15023 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py
+-rw-r--r--   0        0        0    11734 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/atms_hdf5.py
+-rw-r--r--   0        0        0    10268 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ewsg_netcdf.py
+-rw-r--r--   0        0        0     3105 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/geoips_netcdf.py
+-rw-r--r--   0        0        0     9758 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/gmi_hdf5.py
+-rw-r--r--   0        0        0     7409 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/imerg_hdf5.py
+-rw-r--r--   0        0        0     4466 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/mimic_netcdf.py
+-rw-r--r--   0        0        0    34756 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/modis_hdf4.py
+-rw-r--r--   0        0        0     7592 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/saphir_hdf5.py
+-rw-r--r--   0        0        0    11767 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/sar_winds_netcdf.py
+-rw-r--r--   0        0        0    10592 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py
+-rw-r--r--   0        0        0    10365 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py
+-rwxr-xr-x   0        0        0    30729 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/seviri_hrit.py
+-rw-r--r--   0        0        0     5176 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/sfc_winds_text.py
+-rw-r--r--   0        0        0     4811 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py
+-rw-r--r--   0        0        0    10319 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/smos_winds_netcdf.py
+-rw-r--r--   0        0        0    23045 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ssmi_binary.py
+-rw-r--r--   0        0        0    48302 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ssmis_binary.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/__init__.py
+-rw-r--r--   0        0        0    24657 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py
+-rw-r--r--   0        0        0    39075 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/hrit_reader.py
+-rw-r--r--   0        0        0     4800 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/remss_reader.py
+-rwxr-xr-x   0        0        0    26859 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/viirs_netcdf.py
+-rw-r--r--   0        0        0     7650 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/wfabba_ascii.py
+-rw-r--r--   0        0        0    20795 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_idr37_binary.py
+-rw-r--r--   0        0        0     4256 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/__init__.py
+-rw-r--r--   0        0        0    18201 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py
+-rw-r--r--   0        0        0     6041 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py
+-rw-r--r--   0        0        0      695 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/__init__.py
+-rw-r--r--   0        0        0     3073 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/__init__.py
+-rw-r--r--   0        0        0     2009 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/static_standard.py
+-rw-r--r--   0        0        0     2830 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_copyright.py
+-rw-r--r--   0        0        0     3061 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_standard.py
+-rwxr-xr-x   0        0        0     2977 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt
+-rw-r--r--   0        0        0     3353 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt
+-rwxr-xr-x   0        0        0     1083 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt
+-rw-r--r--   0        0        0      459 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/default.yaml
+-rw-r--r--   0        0        0      553 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml
+-rw-r--r--   0        0        0      478 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_visir.yaml
+-rw-r--r--   0        0        0      551 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml
+-rw-r--r--   0        0        0      437 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/default.yaml
+-rw-r--r--   0        0        0      438 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/north_pole.yaml
+-rw-r--r--   0        0        0      473 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_0p25degree.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_pmw.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_visir.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_visir_3200km.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_windspeed.yaml
+-rw-r--r--   0        0        0     1033 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml
+-rw-r--r--   0        0        0      543 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml
+-rw-r--r--   0        0        0      573 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml
+-rw-r--r--   0        0        0      568 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml
+-rw-r--r--   0        0        0      579 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml
+-rw-r--r--   0        0        0      574 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml
+-rw-r--r--   0        0        0      553 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml
+-rw-r--r--   0        0        0      548 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml
+-rw-r--r--   0        0        0      467 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/color37.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/color37Nearest.yaml
+-rw-r--r--   0        0        0      573 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml
+-rw-r--r--   0        0        0      568 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml
+-rw-r--r--   0        0        0      579 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml
+-rw-r--r--   0        0        0      574 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml
+-rw-r--r--   0        0        0      563 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml
+-rw-r--r--   0        0        0      558 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml
+-rw-r--r--   0        0        0      557 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml
+-rw-r--r--   0        0        0      467 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/color89.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/color89Nearest.yaml
+-rw-r--r--   0        0        0      560 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml
+-rw-r--r--   0        0        0      290 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sectored.yaml
+-rw-r--r--   0        0        0     1103 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml
+-rw-r--r--   0        0        0      945 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml
+-rw-r--r--   0        0        0      604 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml
+-rw-r--r--   0        0        0      590 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml
+-rw-r--r--   0        0        0      613 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml
+-rw-r--r--   0        0        0      786 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml
+-rw-r--r--   0        0        0      791 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml
+-rw-r--r--   0        0        0      519 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml
+-rw-r--r--   0        0        0      267 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/unmodified.yaml
+-rw-r--r--   0        0        0      296 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/unsectored.yaml
+-rw-r--r--   0        0        0      598 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml
+-rw-r--r--   0        0        0      722 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml
+-rw-r--r--   0        0        0      607 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml
+-rw-r--r--   0        0        0      662 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml
+-rw-r--r--   0        0        0      483 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR-GeoIPS1.yaml
+-rw-r--r--   0        0        0      459 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR.yaml
+-rw-r--r--   0        0        0      759 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml
+-rw-r--r--   0        0        0     1053 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml
+-rw-r--r--   0        0        0      599 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml
+-rw-r--r--   0        0        0      599 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml
+-rw-r--r--   0        0        0      587 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV.yaml
+-rw-r--r--   0        0        0     2429 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/abi.yaml
+-rw-r--r--   0        0        0     3827 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/ahi.yaml
+-rw-r--r--   0        0        0     4992 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsr-e.yaml
+-rw-r--r--   0        0        0     7947 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsr2.yaml
+-rw-r--r--   0        0        0     2844 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsu-b.yaml
+-rw-r--r--   0        0        0     2244 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ascat.yaml
+-rw-r--r--   0        0        0     2280 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ascatuhr.yaml
+-rw-r--r--   0        0        0     1709 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/atms.yaml
+-rw-r--r--   0        0        0    10713 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/gmi.yaml
+-rw-r--r--   0        0        0     1070 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/gvar.yaml
+-rw-r--r--   0        0        0     1167 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/hscat.yaml
+-rw-r--r--   0        0        0      587 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/imerg.yaml
+-rw-r--r--   0        0        0     2928 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/mhs.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/mimic.yaml
+-rw-r--r--   0        0        0     2186 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/modis.yaml
+-rw-r--r--   0        0        0     1040 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/oscat.yaml
+-rw-r--r--   0        0        0     1330 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/saphir.yaml
+-rw-r--r--   0        0        0     1345 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/sar-spd.yaml
+-rw-r--r--   0        0        0     2249 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/seviri.yaml
+-rw-r--r--   0        0        0      881 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/smap-spd.yaml
+-rw-r--r--   0        0        0      881 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/smos-spd.yaml
+-rw-r--r--   0        0        0     8612 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ssmi.yaml
+-rw-r--r--   0        0        0    11093 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ssmis.yaml
+-rw-r--r--   0        0        0     8555 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/tmi.yaml
+-rw-r--r--   0        0        0     2349 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/viirs.yaml
+-rw-r--r--   0        0        0     3935 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/windsat.yaml
+-rw-r--r--   0        0        0      400 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_1km_1024x1024.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_2km_1024x1024.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_1km_1400x1400.yaml
+-rw-r--r--   0        0        0      400 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_2km_1400x1400.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_2km_1600x1600.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_4km_1600x1600.yaml
+-rw-r--r--   0        0        0      395 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_256x256/tc_4km_256x256.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_2km_512x512.yaml
+-rw-r--r--   0        0        0      392 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_4km_512x512.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_2km_800x800.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_4km_800x800.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_0p1km_3200x3200.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_2500x2500.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_3200x3200.yaml
+-rw-r--r--   0        0        0      391 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_2km_template.yaml
+-rw-r--r--   0        0        0      338 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_50km_barbs_template.yaml
+-rw-r--r--   0        0        0      417 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_high_barbs_template.yaml
+-rw-r--r--   0        0        0      341 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_low_barbs_template.yaml
+-rw-r--r--   0        0        0      409 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascatuhr_barbs_template.yaml
+-rw-r--r--   0        0        0      397 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_halfkm_template.yaml
+-rw-r--r--   0        0        0      391 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_qkm_template.yaml
+-rw-r--r--   0        0        0      340 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_template.yaml
+-rw-r--r--   0        0        0      486 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/abu_dhabi.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/africa.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/african_horn.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/alaska.yaml
+-rw-r--r--   0        0        0      448 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/asia.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/australia.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/beijing.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/brazil.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/cairo.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/canada.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/caribbean.yaml
+-rw-r--r--   0        0        0      479 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/central_america.yaml
+-rw-r--r--   0        0        0      565 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/conus.yaml
+-rw-r--r--   0        0        0      443 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/delhi.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/denver.yaml
+-rw-r--r--   0        0        0      461 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/e_pacific.yaml
+-rw-r--r--   0        0        0      458 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/europe.yaml
+-rw-r--r--   0        0        0      531 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ewsg.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/france.yaml
+-rw-r--r--   0        0        0      516 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/global.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_east.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_west.yaml
+-rw-r--r--   0        0        0      549 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/himawari.yaml
+-rw-r--r--   0        0        0      461 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/indian_basin.yaml
+-rw-r--r--   0        0        0      526 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/japan.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/mediterranean.yaml
+-rw-r--r--   0        0        0      477 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/melbourne.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_africa.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_europe.yaml
+-rw-r--r--   0        0        0      518 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml
+-rw-r--r--   0        0        0      472 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/mexico_city.yaml
+-rw-r--r--   0        0        0      472 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/middle_east.yaml
+-rw-r--r--   0        0        0      466 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ne_asia.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/north_pole.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/paris.yaml
+-rw-r--r--   0        0        0      496 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/rio_de_janeiro.yaml
+-rw-r--r--   0        0        0      446 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/russia.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/saskatchewan.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/se_asia.yaml
+-rw-r--r--   0        0        0      514 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_america.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_pole.yaml
+-rw-r--r--   0        0        0      492 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/vancouver.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/victoria.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/w_atlantic.yaml
+-rw-r--r--   0        0        0      456 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/w_pacific.yaml
+-rw-r--r--   0        0        0      119 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/docstring.yaml
+-rw-r--r--   0        0        0      121 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/family.yaml
+-rw-r--r--   0        0        0      118 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/interface.yaml
+-rw-r--r--   0        0        0       96 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/name.yaml
+-rw-r--r--   0        0        0      119 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/product_defaults.yaml
+-rw-r--r--   0        0        0      322 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/top.yaml
+-rw-r--r--   0        0        0      274 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0     1215 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     1811 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      209 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm.yaml
+-rw-r--r--   0        0        0      245 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      284 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      327 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0     1364 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      328 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      320 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      195 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/unvalidated.yaml
+-rw-r--r--   0        0        0      833 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml
+-rw-r--r--   0        0        0      218 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator.yaml
+-rw-r--r--   0        0        0      248 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      284 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      228 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/sectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      640 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm.yaml
+-rw-r--r--   0        0        0      730 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      652 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator.yaml
+-rw-r--r--   0        0        0      734 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0       98 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      169 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unmodified.yaml
+-rw-r--r--   0        0        0      237 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unsectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      232 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unsectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      210 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      354 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      429 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      634 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/bases/product.yaml
+-rw-r--r--   0        0        0      363 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator.yaml
+-rw-r--r--   0        0        0      393 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      429 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      220 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/list.yaml
+-rw-r--r--   0        0        0      243 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/sectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      233 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/sectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      191 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/single.yaml
+-rw-r--r--   0        0        0      179 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unmodified.yaml
+-rw-r--r--   0        0        0      247 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unsectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      237 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unsectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      215 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      369 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/generated.yaml
+-rw-r--r--   0        0        0      217 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/atmosriver.yaml
+-rw-r--r--   0        0        0      213 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/pyrocb.yaml
+-rw-r--r--   0        0        0      316 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/static.yaml
+-rw-r--r--   0        0        0      271 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/stitched.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/tc.yaml
+-rw-r--r--   0        0        0      244 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/volcano.yaml
+-rw-r--r--   0        0        0      770 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/specs/area_definition.yaml
+-rw-r--r--   0        0        0      746 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/specs/center.yaml
+-rw-r--r--   0        0        0     2016 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/static.yaml
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/__init__.py
+-rw-r--r--   0        0        0    11134 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/estimate_area_extent.py
+-rw-r--r--   0        0        0    12241 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/overpass_predictor.py
+-rw-r--r--   0        0        0     3880 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/projections.py
+-rw-r--r--   0        0        0    11052 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/tc_tracks.py
+-rw-r--r--   0        0        0    15280 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/tc_tracks_database.py
+-rw-r--r--   0        0        0    26958 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/utils.py
+-rw-r--r--   0        0        0     6731 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/yaml_utils.py
+-rw-r--r--   0        0        0      682 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/context_managers.py
+-rw-r--r--   0        0        0     2582 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/decorators.py
+-rw-r--r--   0        0        0     3569 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/memusg.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/__init__.py
+-rw-r--r--   0        0        0    33275 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/data.py
+-rw-r--r--   0        0        0     4421 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/time.py
+-rw-r--r--   0        0        0     1111 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/xr_to_dtree.py
+-rw-r--r--   0        0        0     6837 2024-04-23 23:27:59.645849 geoips-1.12.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1062 2024-04-23 23:27:47.737714 geoips-1.12.2a0/setup/download_test_data.py
+-rw-r--r--   0        0        0     1184 2024-04-23 23:27:47.793715 geoips-1.12.2a0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1190 2024-04-23 23:27:47.797715 geoips-1.12.2a0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1188 2024-04-23 23:27:47.809715 geoips-1.12.2a0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1245 2024-04-23 23:27:47.845716 geoips-1.12.2a0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml
+-rw-r--r--   0        0        0     1667 2024-04-23 23:27:47.849716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml
+-rw-r--r--   0        0        0     1661 2024-04-23 23:27:47.857716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml
+-rw-r--r--   0        0        0     1668 2024-04-23 23:27:47.865716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml
+-rw-r--r--   0        0        0     1662 2024-04-23 23:27:47.873716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml
+-rw-r--r--   0        0        0     1243 2024-04-23 23:27:47.873716 geoips-1.12.2a0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml
+-rw-r--r--   0        0        0     1136 2024-04-23 23:27:47.877716 geoips-1.12.2a0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1234 2024-04-23 23:27:47.881716 geoips-1.12.2a0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml
+-rw-r--r--   0        0        0     1222 2024-04-23 23:27:47.885716 geoips-1.12.2a0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml
+-rw-r--r--   0        0        0     1556 2024-04-23 23:27:47.889716 geoips-1.12.2a0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml
+-rw-r--r--   0        0        0     1569 2024-04-23 23:27:47.893716 geoips-1.12.2a0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml
+-rw-r--r--   0        0        0     1226 2024-04-23 23:27:47.901716 geoips-1.12.2a0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml
+-rw-r--r--   0        0        0     1382 2024-04-23 23:27:47.933717 geoips-1.12.2a0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml
+-rw-r--r--   0        0        0     1211 2024-04-23 23:27:47.937717 geoips-1.12.2a0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml
+-rw-r--r--   0        0        0     1131 2024-04-23 23:27:47.945717 geoips-1.12.2a0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1220 2024-04-23 23:27:47.953717 geoips-1.12.2a0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml
+-rw-r--r--   0        0        0     1162 2024-04-23 23:27:47.953717 geoips-1.12.2a0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml
+-rw-r--r--   0        0        0     1144 2024-04-23 23:27:47.957717 geoips-1.12.2a0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml
+-rw-r--r--   0        0        0    54649 2024-04-23 23:27:47.969717 geoips-1.12.2a0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt
+-rw-r--r--   0        0        0     1222 2024-04-23 23:27:47.969717 geoips-1.12.2a0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml
+-rw-r--r--   0        0        0     1347 2024-04-23 23:27:47.977717 geoips-1.12.2a0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     6257 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/commandline/test_log_setup.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml
+-rw-r--r--   0        0        0      677 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml
+-rw-r--r--   0        0        0      662 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml
+-rw-r--r--   0        0        0     8382 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml
+-rw-r--r--   0        0        0   224173 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips.yaml
+-rw-r--r--   0        0        0     8892 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml
+-rw-r--r--   0        0        0     3166 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml
+-rw-r--r--   0        0        0     5822 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml
+-rw-r--r--   0        0        0     1877 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml
+-rw-r--r--   0        0        0     1997 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml
+-rw-r--r--   0        0        0      626 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml
+-rw-r--r--   0        0        0    10936 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/test_plugin_registries.py
+-rw-r--r--   0        0        0     2815 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py
+-rw-r--r--   0        0        0     1529 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py
+-rw-r--r--   0        0        0     1717 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py
+-rw-r--r--   0        0        0       21 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/bases/docstring.yaml
+-rw-r--r--   0        0        0       91 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0     2966 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     1467 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     2028 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0     2855 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0     1346 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      663 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0     1502 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0     1798 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/products/bases/product.yaml
+-rw-r--r--   0        0        0      385 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/products/single.yaml
+-rw-r--r--   0        0        0       46 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0      996 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      288 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      283 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      384 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0      523 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      290 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      384 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      529 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/products/bases/product.yaml
+-rw-r--r--   0        0        0     1182 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/products/single.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/sectors/static.yaml
+-rw-r--r--   0        0        0     3650 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/test_yaml_schema.py
+-rw-r--r--   0        0        0     1446 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/utils/context_managers.py
+-rw-r--r--   0        0        0     3912 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests/xarray_utils/data.py
+-rw-r--r--   0        0        0     1867 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests/xarray_utils/test_dtree.py
+-rw-r--r--   0        0        0     2533 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests_long/plugins/modules/readers/test_readers.py
+-rw-r--r--   0        0        0     1263 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/abi_test.yaml
+-rw-r--r--   0        0        0     1500 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/abi_test_low_memory.yaml
+-rw-r--r--   0        0        0     4833 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_no_compare_full.yaml
+-rw-r--r--   0        0        0     1731 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test.yaml
+-rw-r--r--   0        0        0     1813 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test_low_memory.yaml
+-rw-r--r--   0        0        0     1485 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test_no_compare.yaml
+-rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 geoips-1.12.2a0/PKG-INFO
```

### Comparing `geoips-1.12.0/.github/workflows/bandit.yaml` & `geoips-1.12.2a0/.github/workflows/bandit.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows/black.yaml` & `geoips-1.12.2a0/.github/workflows/black.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 jobs:
   check_code_black:
     runs-on: ${{ vars.RUNNER }}
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: "pypy-3.9"
+          python-version: "pypy-3.10"
           check-latest: true
       - name: Checkout plugin current branch
         uses: actions/checkout@master
       - name: Update pip
         run: pip install --upgrade pip
       - name: Install black
         run: pip install black
```

### Comparing `geoips-1.12.0/.github/workflows/build-html-docs.yaml` & `geoips-1.12.2a0/.github/workflows/build-html-docs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows/changelog-templates-unchanged.yaml` & `geoips-1.12.2a0/.github/workflows/changelog-templates-unchanged.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows/flake8.yaml` & `geoips-1.12.2a0/.github/workflows/flake8.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows/package-and-publish.yaml` & `geoips-1.12.2a0/.github/workflows/package-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows/pytest-short.yaml` & `geoips-1.12.2a0/.github/workflows/pytest-short.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 name: Pytest Short Unit Tests Pull Request
 
 defaults:
   run:
     shell: bash
 
-env:
-  CONDA_ENV: github_actions_pytest
-
 # Can not use variables in the list of branches,
 # GitHub Actions will not recognize, and workflow will not run.
 on:
   # Triggers the workflow when pull request created and updated
   # pull_request:
   #   branches:
   #     - main
```

### Comparing `geoips-1.12.0/.github/workflows/test-interfaces.yaml` & `geoips-1.12.2a0/.github/workflows/test-interfaces.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows_archived/docker-build-test-push.yaml` & `geoips-1.12.2a0/.github/workflows_archived/docker-build-test-push.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/.github/workflows_archived/validate-pull-request.yaml` & `geoips-1.12.2a0/.github/workflows_archived/validate-pull-request.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/LICENSE` & `geoips-1.12.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/README.md` & `geoips-1.12.2a0/README.md`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/docs/source/_templates/conf_PKG.py` & `geoips-1.12.2a0/docs/source/_templates/conf_PKG.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 # ones.
 extensions = [
     "sphinx_design",
     "sphinx.ext.autodoc",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
+    "sphinxcontrib.autoprogram",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
```

### Comparing `geoips-1.12.0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/docs/source/yaml/abi_test.yaml` & `geoips-1.12.2a0/docs/source/yaml/abi_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/__init__.py` & `geoips-1.12.2a0/geoips/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 from geoips import errors
 from geoips import filenames
 from geoips import interfaces
 from geoips import utils
 from geoips import xarray_utils
 from ._version import __version__, __version_tuple__
 
+import logging  # noqa
+from geoips.commandline.log_setup import add_logging_level
+
+
+add_logging_level("INTERACTIVE", 35)
+
 __all__ = [
     "interfaces",
     "errors",
     "filenames",
     "utils",
     "xarray_utils",
     "__version__",
```

### Comparing `geoips-1.12.0/geoips/_version.py` & `geoips-1.12.2a0/geoips/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 # DO NOT EDIT
 # managed by poetry-dynamic-versioning
-__version__ = "1.12.0"
-__version_tuple__ = (1, 12, 0)
+__version__ = "1.12.2a0"
+__version_tuple__ = (1, 12, "2a0")
```

### Comparing `geoips-1.12.0/geoips/cli.py` & `geoips-1.12.2a0/geoips/cli.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/__init__.py` & `geoips-1.12.2a0/geoips/commandline/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/args.py` & `geoips-1.12.2a0/geoips/commandline/args.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/create_sector_image.py` & `geoips-1.12.2a0/geoips/commandline/create_sector_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/list_available_plugins.py` & `geoips-1.12.2a0/geoips/commandline/list_available_plugins.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/run_procflow.py` & `geoips-1.12.2a0/geoips/commandline/run_procflow.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/test_interfaces.py` & `geoips-1.12.2a0/geoips/commandline/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/commandline/update_tc_tracks_database.py` & `geoips-1.12.2a0/geoips/commandline/update_tc_tracks_database.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/create_plugin_registries.py` & `geoips-1.12.2a0/geoips/create_plugin_registries.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from os import remove
 import sys
 import logging
 from geoips.commandline.log_setup import setup_logging
 import geoips.interfaces
 from geoips.errors import PluginRegistryError
 import json
+from argparse import ArgumentParser
 
 LOG = logging.getLogger(__name__)
 
 
 def remove_registries(plugin_packages):
     """Remove all plugin registries if a PluginRegistryError is raised.
 
@@ -289,15 +290,15 @@
         with open(reg_plug_abspath, "w") as plugin_registry:
             LOG.interactive("Writing %s", reg_plug_abspath)
             yaml.safe_dump(plugins, plugin_registry, default_flow_style=False)
     else:
         reg_plug_abspath = osjoin(pkg_dir, "registered_plugins.json")
         with open(reg_plug_abspath, "w") as plugin_registry:
             LOG.interactive("Writing %s", reg_plug_abspath)
-            json.dump(plugins, plugin_registry)
+            json.dump(plugins, plugin_registry, indent=4)
 
 
 def create_plugin_registries(plugin_packages, save_type):
     """Generate all plugin paths associated with every installed GeoIPS packages.
 
     These paths include schema plugins, module_based plugins
     and normal YAML plugins. After these paths are generated, they are sent
@@ -832,29 +833,56 @@
     del module
     # Return the final error message - an exception will be raised at the very
     # end after collecting and reporting on all errors if there were any errors
     # during plugin registry creation.
     return error_message
 
 
+def get_parser():
+    """Create the ArgumentParser for main."""
+    description = (
+        "Creates Plugin Registries for all installed GeoIPS packages. "
+        "The registries will be written to the root directory of each installed "
+        "package. The registries will be named either 'registered_plugins.json' "
+        "or 'registered_plugins.yaml' depending on which format is chosen. "
+        "For additional information on GeoIPS plugin registries please refer to "
+        "the GeoIPS documentation."
+    )
+    parser = ArgumentParser(
+        prog="create_plugin_registries",
+        description=description,
+    )
+    parser.add_argument(
+        "-s",
+        "--save_type",
+        type=str.lower,
+        default="json",
+        choices=["json", "yaml"],
+        help="Format to write registries to. This will also be the file extension.",
+    )
+    return parser
+
+
 def main():
     """Generate all available plugins from all installed GeoIPS packages.
 
     After all plugins have been generated, they are written to registered_plugins.yaml
     containing a dictionary of all the registered GeoIPS plugins. Keys in this
     dictionary are the interface names, following by each plugin name.
 
     Parameters
     ----------
     args: list
         List of strings representing the arguments provided via command line.
     """
-    save_type = "json"
-    if len(sys.argv) > 1 and sys.argv[1].lower() == "yaml":
-        save_type = "yaml"
+    parser = get_parser()
+
+    ARGS = parser.parse_args()
+    save_type = ARGS.save_type
+
     LOG = setup_logging(logging_level="INTERACTIVE")
     # Note: Python 3.9 appears to return duplicates when installed with setuptools.
     # These are filtered within the create_plugin_registries function.
     plugin_packages = get_entry_point_group("geoips.plugin_packages")
     LOG.debug(plugin_packages)
     create_plugin_registries(plugin_packages, save_type)
     sys.exit(0)
```

### Comparing `geoips-1.12.0/geoips/data_manipulations/__init__.py` & `geoips-1.12.2a0/geoips/data_manipulations/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/data_manipulations/conversions.py` & `geoips-1.12.2a0/geoips/data_manipulations/conversions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/data_manipulations/corrections.py` & `geoips-1.12.2a0/geoips/data_manipulations/corrections.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/data_manipulations/info.py` & `geoips-1.12.2a0/geoips/data_manipulations/info.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/data_manipulations/merge.py` & `geoips-1.12.2a0/geoips/data_manipulations/merge.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/dev/__init__.py` & `geoips-1.12.2a0/geoips/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/dev/output_config.py` & `geoips-1.12.2a0/geoips/dev/output_config.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/dev/product.py` & `geoips-1.12.2a0/geoips/dev/product.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/errors.py` & `geoips-1.12.2a0/geoips/errors.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/filenames/__init__.py` & `geoips-1.12.2a0/geoips/filenames/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/filenames/base_paths.py` & `geoips-1.12.2a0/geoips/filenames/base_paths.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/filenames/duplicate_files.py` & `geoips-1.12.2a0/geoips/filenames/duplicate_files.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/geoips_utils.py` & `geoips-1.12.2a0/geoips/geoips_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/image_utils/__init__.py` & `geoips-1.12.2a0/geoips/image_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/image_utils/colormap_utils.py` & `geoips-1.12.2a0/geoips/image_utils/colormap_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/image_utils/maps.py` & `geoips-1.12.2a0/geoips/image_utils/maps.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/image_utils/mpl_utils.py` & `geoips-1.12.2a0/geoips/image_utils/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/__init__.py` & `geoips-1.12.2a0/geoips/interfaces/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -68,7 +68,39 @@
     "feature_annotators",
     "gridline_annotators",
     "product_defaults",
     "products",
     "sectors",
 ]
 __all__ = module_based_interfaces + yaml_based_interfaces
+
+
+def list_available_interfaces():
+    """Return a dictionary of available interfaces.
+
+    Collect and return a dictionary whose keys are the interface types (i.e.
+    module_based, yaml_based, and text_based) and whose values are lists of the
+    available interfaces for each interface type.
+    """
+    # These are buried to avoid polluting the interface module's namespace
+    import inspect
+    from geoips import interfaces
+
+    all_interfaces = {
+        "module_based": [],
+        "text_based": [],
+        "yaml_based": [],
+    }
+    for interface_type in ["module", "text", "yaml"]:
+        try:
+            available_interfaces = [
+                str(mod_info[0])
+                for mod_info in inspect.getmembers(
+                    getattr(interfaces, f"{interface_type}_based"),
+                    inspect.ismodule,
+                )
+            ]
+            all_interfaces[f"{interface_type}_based"] = available_interfaces
+        except AttributeError:
+            continue
+
+    return all_interfaces
```

### Comparing `geoips-1.12.0/geoips/interfaces/base.py` & `geoips-1.12.2a0/geoips/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/__init__.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/algorithms.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/algorithms.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/colormappers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/colormappers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/coverage_checkers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/coverage_checkers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/filename_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/filename_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/interpolators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/interpolators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/output_checkers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/output_checkers.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from geoips.interfaces.base import (
     BaseModuleInterface,
     BaseModulePlugin,
     ValidationError,
 )
 import logging
 from geoips.errors import PluginError
+
+# import subprocess
+from geoips.commandline.log_setup import log_with_emphasis
 import gzip
 from glob import glob
 from os.path import exists, splitext, basename, dirname, isdir, join
 from os import makedirs, getenv
 from shutil import copyfileobj
 from geoips.filenames.base_paths import make_dirs
 
@@ -422,41 +425,14 @@
                 # For display purposes - tifs are easier to view
                 test_basename = basename(goodcomp).replace(".jif", ".tif")
                 test_filename = join(test_path, test_basename)
                 fobj.write(f"cp {goodcomp} {test_filename}\n")
     return 0
 
 
-def log_with_emphasis(log_command, log_lines):
-    """Surround log output with extra emphasis.
-
-    This will eventually be consolidated in a logging utility.
-    For now, include here.
-
-    Parameters
-    ----------
-    log_command : callable
-        ie, LOG.info
-    log_lines : list
-        list of lines to pass to log_command.
-        ie, ["log output line 1", "log output line 2"]
-
-    Returns
-    -------
-    No return values.
-    """
-    log_command("**********************************************")
-    log_command("**********************************************")
-    for log_line in log_lines:
-        log_command(log_line)
-    log_command("**********************************************")
-    log_command("**********************************************")
-    log_command("\n")
-
-
 def get_missing_products(output_products_for_comparison, compare_products):
     """Get list of missing products from compare_products_dictionary.
 
     Parameters
     ----------
     output_products_for_comparison: list
         List of output products from the current run.
@@ -537,16 +513,19 @@
     """
     # If it is already a .gz file, use that.
     if splitext(fname)[-1] in [".gz"]:
         gz_fname = fname
     # Otherwise, see if the .gz version exists.
     elif glob(fname + ".gz"):
         gz_fname = fname + ".gz"
-    LOG.info("**** Gunzipping product for comparisons")
-    LOG.info("gunzip %s", gz_fname)
+
+    messages = ["Gunzipping product for comparisons"]
+    messages.append(f"gunzip {gz_fname}")
+    log_with_emphasis(LOG.info, *messages)
+
     if is_comparison_product:
         save_dir = join(
             getenv("GEOIPS_OUTDIRS"),
             "scratch",
             "gunzipped_products",
             "comparison_products",
         )
@@ -774,15 +753,15 @@
             if is_gz(output_product):
                 output_product_for_comparison = self.gunzip_product(
                     output_product, is_comparison_product=False
                 )
                 remove_temp_files += [output_product_for_comparison]
 
             log_with_emphasis(
-                LOG.info, ["*** COMPARE {basename(output_product_for_comparison)}"]
+                LOG.info, "COMPARE {basename(output_product_for_comparison)}"
             )
             found_one = False
             for compare_product in compare_products:
                 file_for_comparison = compare_products[basename(compare_product)][
                     "file_for_comparison"
                 ]
                 # If the current output product matches the basename of the
@@ -845,17 +824,15 @@
             This gets passed through to the "test_products" method.
 
         Returns
         -------
         int
             Binary code: 0 if all comparisons were completed successfully.
         """
-        log_with_emphasis(
-            LOG.info, [f"*** COMPARISONS OF KNOWN OUTPUTS IN {compare_path}"]
-        )
+        log_with_emphasis(LOG.info, f"COMPARISONS OF KNOWN OUTPUTS IN {compare_path}")
         # We gunzip comparison files to a temporary location, so keep track of
         # all the temporary files so we can remove them at the end.
         remove_temp_files = []
 
         compare_products, curr_remove_temp_files = self.get_compare_products(
             compare_path
         )
@@ -876,15 +853,15 @@
             output_products,
             compare_products,
             **kwargs,
         )
         remove_temp_files += curr_remove_temp_files
         log_with_emphasis(
             LOG.info,
-            [f"*** DONE RUNNING COMPARISONS OF KNOWN OUTPUTS IN {compare_path}"],
+            f"DONE RUNNING COMPARISONS OF KNOWN OUTPUTS IN {compare_path}",
         )
 
         # Identify all missing products based on the list of output products
         # and the dictionary of comparison products
         missingproducts = get_missing_products(
             output_products_for_comparison, compare_products
         )
```

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/output_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/output_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/procflows.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/procflows.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/readers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/readers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/sector_adjusters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_adjusters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/sector_metadata_generators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_metadata_generators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/sector_spec_generators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_spec_generators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/module_based/title_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/title_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/__init__.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/feature_annotators.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/feature_annotators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/gridline_annotators.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/gridline_annotators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/product_defaults.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/product_defaults.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/products.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/products.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/interfaces/yaml_based/sectors.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/sectors.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/__init__.py` & `geoips-1.12.2a0/geoips/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/single_channel.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/single_channel.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/algorithms/visir/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/cmap_rgb.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/cmap_rgb.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/tpw/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/visir/IR_BD.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/IR_BD.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/visir/Infrared.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/Infrared.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/visir/WV.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/WV.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/visir/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/winds/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/center_radius.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/masked_arrays.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/masked_arrays.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/rgba.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/rgba.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/coverage_checkers/windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/basic_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/basic_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/geoips_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/geotiff_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geotiff_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/tc_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/utils/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/utils/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/interpolators/utils/interp_scipy.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_scipy.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_checkers/geotiff.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/geotiff.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 """Test script for representative product comparisons."""
 
 import subprocess
 import logging
 from os.path import splitext
 
+from geoips.commandline.log_setup import log_with_emphasis
+
 LOG = logging.getLogger(__name__)
 
 interface = "output_checkers"
 family = "standard"
 name = "geotiff"
 
 
@@ -127,24 +129,23 @@
 
     call_list = ["diff", output_product, compare_product]
     LOG.info("Running %s", " ".join(call_list))
     retval = subprocess.call(call_list)
 
     # subimg_retval = subprocess.call(call_list)
     if retval != 0:
-        LOG.interactive("    *****************************************")
-        LOG.interactive("    *** BAD geotiffs do NOT match exactly ***")
-        LOG.interactive("    ***   output_product: %s ***", output_product)
-        LOG.interactive("    ***   compare_product: %s ***", compare_product)
-        LOG.interactive("    *****************************************")
+        log_with_emphasis(
+            LOG.interactive,
+            "BAD geotiffs do NOT match exactly",
+            f"output_product: {output_product}",
+            f"compare_product: {compare_product}",
+        )
         return False
 
-    LOG.info("    ***************************")
-    LOG.info("    *** GOOD geotiffs match ***")
-    LOG.info("    ***************************")
+    log_with_emphasis(LOG.info, "GOOD geotiffs match")
     return True
 
 
 def call(plugin, compare_path, output_products):
     """Compare the "correct" geotiffs found the list of current output_products.
 
     Compares files produced in the current processing run with the list of
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_checkers/image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/image.py`

 * *Files 24% similar despite different names*

```diff
@@ -115,39 +115,35 @@
     """
     exact_out_diffimg = plugin.get_out_diff_fname(
         compare_product, output_product, flag="exact_"
     )
     from PIL import Image
     import numpy as np
     from pixelmatch.contrib.PIL import pixelmatch
+    from geoips.commandline.log_setup import log_with_emphasis
 
     LOG.info("**Comparing output_product vs. compare product")
     # Open existing images.
     out_img = Image.open(output_product)
     comp_img = Image.open(compare_product)
     diff_img = Image.new(mode="RGB", size=comp_img.size)
     # Compute the pixel diff between the two images.
     if np.array(comp_img).shape == np.array(out_img).shape:
         diff_arr = np.abs(np.array(comp_img) - np.array(out_img))
     # If shapes of arrays do not match, pixel diff can not be performed.
     # Print the names of the two images and associated shapes, and return False.
     else:
-        LOG.interactive("    ***************************************")
-        LOG.interactive("    *** BAD Images NOT match exactly, different sizes ***")
-        LOG.interactive(
-            "    ***   output_product: %s %s ***",
-            np.array(out_img).shape,
-            output_product,
+        log_with_emphasis(
+            LOG.interactive,
+            "BAD Images NOT match exactly, different sizes",
         )
-        LOG.interactive(
-            "    ***   compare_product: %s %s ***",
-            np.array(comp_img).shape,
-            compare_product,
-        )
-        LOG.interactive("    ***************************************")
+        message = f"output_product: {np.array(out_img).shape} {output_product}"
+        log_with_emphasis(LOG.interactive, message)
+        message = f"compare_product: {np.array(comp_img).shape} {compare_product}"
+        log_with_emphasis(LOG.interactive, message)
         return False
     # Determine the number of pixels that are mismatched
     LOG.info("Using threshold %s", threshold)
     thresholded_retval = pixelmatch(
         out_img, comp_img, diff_img, includeAA=True, alpha=0.33, threshold=threshold
     )
     # Currently, return 0 ONLY if the images are exactly matched.  Eventually
@@ -161,48 +157,42 @@
     diff_img.save(exact_out_diffimg)
     LOG.info("**Done running compare")
 
     # If the images do not match exactly, print the output image, comparison image,
     # and exact diff image to log, for easy viewing.  Return False.
     if thresholded_retval != 0:
         bad_inds = np.where(diff_arr != 0)
-        LOG.interactive("    ***************************************")
-        LOG.interactive("    *** BAD Images do NOT match within tolerance ***")
-        LOG.interactive("    *** ***")
-        LOG.interactive(
-            "    *** %s mismatched pixels exceeding threshold %s ***",
-            thresholded_retval,
-            threshold,
+        log_with_emphasis(LOG.interactive, "BAD Images do NOT match within tolerance")
+        message = f"{thresholded_retval} mismatched pixels "
+        message += f"exceeding threshold {threshold}"
+        log_with_emphasis(
+            LOG.interactive,
+            message,
+            f"{len(diff_arr[bad_inds])} mismatched exact",
+            f"np.where(diff_arr != 0): {bad_inds}",
+            f"diff_arr[bad_inds]: {diff_arr[bad_inds]}",
+            f"output_product: {output_product}",
+            f"compare_product: {compare_product}",
+            f"exact diff image: {exact_out_diffimg}",
         )
-        LOG.interactive("    *** %s mismatched exact ***", len(diff_arr[bad_inds]))
-        LOG.interactive("    *** np.where(diff_arr != 0): %s ***", bad_inds)
-        LOG.interactive("    *** diff_arr[bad_inds]: %s ***", diff_arr[bad_inds])
-        LOG.interactive("    *** ***")
-        LOG.interactive("    ***   output_product: %s ***", output_product)
-        LOG.interactive("    ***   compare_product: %s ***", compare_product)
-        LOG.interactive("    ***   exact dif image: %s ***", exact_out_diffimg)
-        LOG.interactive("    ***************************************")
         return False
 
     # If the images match exactly, just output to GOOD comparison log to info level
     # (only bad comparisons to interactive level)
     if fullimg_retval != 0:
         if thresholded_retval == 0:
             bad_inds = np.where(diff_arr != 0)
-        LOG.interactive("    ******************************************")
-        LOG.interactive("    *** GOOD Images match within tolerance ***")
-        LOG.interactive(
-            "    *** %s mismatched pixels from exact comparison ***",
-            len(diff_arr[bad_inds]),
+        message = f"{len(diff_arr[bad_inds])} mismatched pixels from exact comparison"
+        log_with_emphasis(
+            LOG.interactive,
+            "GOOD Images match within tolerance",
+            message,
         )
-        LOG.interactive("    ******************************************")
     else:
-        LOG.info("    *********************************")
-        LOG.info("    *** GOOD Images match exactly ***")
-        LOG.info("    *********************************")
+        log_with_emphasis(LOG.info, "GOOD Images match exactly")
 
     return True
 
 
 def call(plugin, compare_path, output_products, threshold=0.05):
     """Compare the "correct" imagery found the list of current output_products.
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_checkers/netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/netcdf.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Test script for representative product comparisons."""
 
 import logging
 
+from geoips.commandline.log_setup import log_with_emphasis
+
 LOG = logging.getLogger(__name__)
 
 interface = "output_checkers"
 family = "standard"
 name = "netcdf"
 
 
@@ -126,20 +128,21 @@
     retval = True
     import xarray
 
     out_xobj = xarray.open_dataset(output_product)
     compare_xobj = xarray.open_dataset(compare_product)
 
     if out_xobj.attrs != compare_xobj.attrs:
-        LOG.interactive("    ****************************************************")
-        LOG.interactive(
-            "    *** BAD GeoIPS NetCDF file attributes do NOT match exactly ***"
+        message = "BAD GeoIPS NetCDF file attributes do NOT match exactly"
+        log_with_emphasis(
+            LOG.interactive,
+            message,
+            f"output_product: {output_product}",
+            f"compare_product: {compare_product}",
         )
-        LOG.interactive("    ***   output_product: %s ***", output_product)
-        LOG.interactive("    ***   compare_product: %s ***", compare_product)
         for attr in out_xobj.attrs.keys():
             if attr not in compare_xobj.attrs:
                 diffstr = (
                     f"\nattr {attr}\n\n"
                     f"output\n{out_xobj.attrs[attr]}\n\n"
                     "not in comparison\n"
                 )
@@ -166,83 +169,128 @@
                 diffstr = (
                     f"\nattr {attr}\n\n"
                     f"output\n{out_xobj.attrs[attr]}\n\n"
                     f"comparison\n{compare_xobj.attrs[attr]}\n"
                 )
                 diffout += [diffstr]
                 LOG.interactive(diffstr)
-        LOG.interactive("    ****************************************************")
         diffout += ["\n"]
         retval = False
 
     if retval is False:
         with open(out_difftxt, "w") as fobj:
             fobj.writelines(diffout)
         return False
 
     try:
         xarray.testing.assert_allclose(compare_xobj, out_xobj)
     except AssertionError as resp:
-        LOG.interactive("    ****************************************************")
-        LOG.interactive(
-            "    *** BAD GeoIPS NetCDF files do not match within tolerance *****"
+        message = "BAD GeoIPS NetCDF files do not match within tolerance"
+        log_with_emphasis(
+            LOG.interactive,
+            message,
+            f"output_product: {output_product}",
+            f"compare_product: {compare_product}",
         )
-        LOG.interactive("    ***   output_product: %s ***", output_product)
-        LOG.interactive("    ***   compare_product: %s ***", compare_product)
-        for line in str(resp).split("\n"):
-            LOG.interactive(f"    *** {line} ***")
+        log_with_emphasis(LOG.interactive, *[line for line in str(resp).split("\n")])
         diffout += [
             "\nxarray objects do not match between current output and comparison\n"
         ]
         diffout += [f"\nOut: {out_xobj}\n"]
         diffout += [f"\nCompare: {compare_xobj}\n"]
         diffout += [f"\n{resp}\n"]
         for varname in compare_xobj.variables:
-            maxdiff = (compare_xobj[varname] - out_xobj[varname]).max()
-            mindiff = (compare_xobj[varname] - out_xobj[varname]).min()
-            meandiff = (compare_xobj[varname] - out_xobj[varname]).mean()
-            if mindiff != 0:
-                LOG.interactive(f"    *** mindiff {varname}: {mindiff} ***")
-                diffout += [f"mindiff {varname}: {mindiff}\n"]
-            if maxdiff != 0:
-                LOG.interactive(f"    *** maxdiff {varname}: {maxdiff} ***")
-                diffout += [f"maxdiff {varname}: {maxdiff}\n"]
-            if meandiff != 0:
-                LOG.interactive(f"    *** meandiff {varname}: {meandiff} ***")
-                diffout += [f"meandiff {varname}: {meandiff}\n"]
-        LOG.info("    ****************************************************************")
+            logged_messages = log_object_diff_values(
+                out_xobj, compare_xobj, varname, log_function=LOG.warning
+            )
+            diffout.extend([[m] for m in logged_messages])
         retval = False
 
     try:
         xarray.testing.assert_identical(compare_xobj, out_xobj)
     except AssertionError as resp:
-        LOG.info("    ****************************************************************")
-        LOG.info("    *** INFORMATIONAL ONLY assert_identical differences *****")
+        log_with_emphasis(LOG.info, "INFORMATIONAL ONLY assert_identical differences")
         for line in str(resp).split("\n"):
-            LOG.info(f"    *** {line} ***")
+            log_with_emphasis(LOG.info, line)
         for varname in compare_xobj.variables:
-            maxdiff = (compare_xobj[varname] - out_xobj[varname]).max()
-            mindiff = (compare_xobj[varname] - out_xobj[varname]).min()
-            meandiff = (compare_xobj[varname] - out_xobj[varname]).mean()
-            if mindiff != 0:
-                LOG.info(f"    *** mindiff {varname}: {mindiff} ***")
-            if maxdiff != 0:
-                LOG.info(f"    *** maxdiff {varname}: {maxdiff} ***")
-            if meandiff != 0:
-                LOG.info(f"    *** meandiff {varname}: {meandiff} ***")
-        LOG.info("    ****************************************************************")
+            log_object_diff_values(
+                out_xobj, compare_xobj, varname, log_function=LOG.info
+            )
 
     if retval is False:
         with open(out_difftxt, "w") as fobj:
             fobj.writelines(diffout)
         return False
 
     return True
 
 
+def log_object_diff_values(object1, object2, compare_key, log_function=LOG.info):
+    r"""
+    Log differences two objects via key and returns messages detailing differences.
+
+    Computes the maximum, minimum, and mean differences for the values associated
+    with a specified key in two objects. Generates messages for any non-zero
+    differences and logs these messages. The messages are also returned as a list
+    of strings for further use. Takes in an optional custom logging function,
+    defaults to info logging.
+
+    Objects must expose a min, max, and mean function after the difference
+    between them is computed.
+
+    Parameters
+    ----------
+    object1 : object
+        The first object containing the key for comparison. Must support
+        subscripting with the compare key and arithmetic operations.
+    object2 : object
+        The second object for comparison. Must also support subscripting with the
+        compare key and arithmetic operations.
+    compare_key : str
+        The key for the values to be compared between `object1` and `object2`.
+    log_func : func, optional
+        The function to be used for logging, must take in a list of strings of min
+        length 0.
+
+    Returns
+    -------
+    messages : list of str
+        A list of messages indicating non-zero min, max, and mean differences for
+        the values associated with `compare_key`, formatted as strings.
+
+    Notes
+    -----
+    Only logs and returns messages for non-zero differences. If there are no non-zero
+    differences, an empty list is returned.
+
+    Uses `log_with_emphasis` to log the messages.
+
+    Examples
+    --------
+    Given two objects `obj1` and `obj2` with a key `temp`:
+
+    >>> obj1 = {'temp': np.array([1, 2, 3])}
+    >>> obj2 = {'temp': np.array([2, 3, 4])}
+    >>> log_object_diff_values(obj1, obj2, 'temp')
+    ['mindiff temp: -1\\n', 'maxdiff temp: -1\\n', 'meandiff temp: -1.0\\n']
+
+    This will log and return messages about differences in `temp` values.
+    """
+    maxdiff = (object2[compare_key] - object1[compare_key]).max()
+    mindiff = (object2[compare_key] - object1[compare_key]).min()
+    meandiff = (object2[compare_key] - object1[compare_key]).mean()
+    messages = [
+        f"mindiff {compare_key}: {mindiff}\n",
+        f"maxdiff {compare_key}: {maxdiff}\n",
+        f"meandiff {compare_key}: {meandiff}\n",
+    ]
+    log_with_emphasis(log_function, *messages)
+    return messages
+
+
 def call(plugin, compare_path, output_products):
     """Compare the "correct" netcdfs found the list of current output_products.
 
     Compares files produced in the current processing run with the list of
     "correct" files contained in "compare_path".
 
     Parameters
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_checkers/text.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,35 +125,36 @@
         Full path to "good" comparison product
 
     Returns
     -------
     bool
         Return True if products match, False if they differ
     """
+    from geoips.commandline.log_setup import log_with_emphasis
+
     ret = subprocess.run(
         ["diff", output_product, compare_product],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     LOG.debug(ret.stdout)
     if ret.returncode == 0:
-        LOG.info("    *****************************")
-        LOG.info("    *** GOOD Text files match ***")
-        LOG.info("    *****************************")
+        log_with_emphasis(LOG.info, "GOOD Text files match")
         return True
 
     out_difftxt = plugin.get_out_diff_fname(compare_product, output_product)
     with open(out_difftxt, "w") as fobj:
         subprocess.call(["diff", output_product, compare_product], stdout=fobj)
-    LOG.interactive("    *******************************************")
-    LOG.interactive("    *** BAD Text files do NOT match exactly ***")
-    LOG.interactive("    ***   output_product: %s ***", output_product)
-    LOG.interactive("    ***   compare_product: %s ***", compare_product)
-    LOG.interactive("    ***   out_difftxt: %s ***", out_difftxt)
-    LOG.interactive("    *******************************************")
+    log_with_emphasis(
+        LOG.interactive,
+        "BAD Text files do NOT match exactly",
+        f"output_product: {output_product}",
+        f"compare_product: {compare_product}",
+        f"out_difftxt: {out_difftxt}",
+    )
     return False
 
 
 def call(plugin, compare_path, output_products):
     """Compare the "correct" text found the list of current output_products.
 
     Compares files produced in the current processing run with the list of
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/full_disk_image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/full_disk_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/geotiff_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/geotiff_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_annotated.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_annotated.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_clean.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_clean.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/metadata_default.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_default.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/metadata_tc.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_tc.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/netcdf_geoips.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_geoips.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/netcdf_xarray.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_xarray.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/text_winds.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/text_winds.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/output_formatters/unprojected_image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/unprojected_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/procflows/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/procflows/config_based.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/config_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     get_covg_from_product,
     get_covg_args_from_product,
     get_required_variables,
 )
 from geoips.xarray_utils.data import sector_xarrays
 from geoips.filenames.duplicate_files import remove_duplicates
 from geoips.geoips_utils import replace_geoips_paths
+from geoips.utils.context_managers import import_optional_dependencies
 
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     from geoips_db.utils.database_writes import (
         write_to_database,
         flag_product_as_deleted,
         write_stats_to_database,
     )
-except ImportError:
-    pass
 
 # Old interfaces (YAML, will migrate to new soon)
 from geoips.dev.output_config import (
     get_output_formatter_kwargs,
     get_output_formatter,
     get_minimum_coverage,
     produce_current_time,
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/procflows/single_source.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/single_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,29 +355,14 @@
             xobjs["METADATA"],
             area_def=area_def,
         )
 
     return final_products
 
 
-def print_area_def(area_def, print_str):
-    """Print area def."""
-    LOG.info(
-        "\n\n*************************************************************************"
-        "***********"
-        f"\n***{print_str}\n{area_def}"
-    )
-    for key, value in area_def.sector_info.items():
-        LOG.info(f"{key}: {value}")
-    LOG.info(
-        "*****************************************************************************"
-        "*******"
-    )
-
-
 def pad_area_definition(
     area_def, source_name=None, force_pad=False, x_scale_factor=1.5, y_scale_factor=1.5
 ):
     """Pad area definition."""
     from geoips.sector_utils.utils import is_sector_type
 
     # Always pad TC sectors, and if "force_pad=True" is passed into the function
@@ -735,15 +720,15 @@
         if not hasattr(area_def, "description"):
             setattr(area_def, "description", area_def.name)
 
         area_defs += [area_def]
     LOG.interactive("Getting all area defs from command line args:")
     if "sector_list" in command_line_args:
         sector_list = command_line_args["sector_list"]
-        LOG.interactive("  sector_list: %s", tcdb_sector_list)
+        LOG.interactive("  sector_list: %s", sector_list)
     if "tcdb_sector_list" in command_line_args:
         tcdb_sector_list = command_line_args["tcdb_sector_list"]
         LOG.interactive("  tcdb_sector_list: %s", tcdb_sector_list)
     if "tcdb" in command_line_args:
         tcdb = command_line_args["tcdb"]
         LOG.interactive("  tcdb: %s", tcdb)
     if "trackfile_sector_list" in command_line_args:
@@ -1072,17 +1057,15 @@
             final_xarray = alg_xarray
         # If required, interpolate the result prior to returning
         elif prod_plugin.family == "algorithm_interpolator_colormapper":
             interp_args["varlist"] = [prod_plugin.name]
             LOG.interactive(
                 "  Interpolating data with interpolator '%s'...", interp_plugin.name
             )
-            final_xarray = interp_plugin(
-                area_def, alg_xarray, alg_xarray, **interp_args
-            )
+            final_xarray = interp_plugin(area_def, alg_xarray, None, **interp_args)
 
         # Ensure we have the "adjustment"id" in the filename appropriately
         if "adjustment_id" in area_def.sector_info:
             final_xarray = add_filename_extra_field(
                 alg_xarray, "adjustment_id", area_def.sector_info["adjustment_id"]
             )
         # return here - we are done for either alg_cmap or alg_interp_cmap type
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/abi_l2_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/abi_l2_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/abi_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/abi_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,45 +17,34 @@
 import os
 from glob import glob
 from datetime import datetime, timedelta
 import numpy as np
 
 from scipy.ndimage import zoom
 
+from geoips.utils.context_managers import import_optional_dependencies
 from geoips.plugins.modules.readers.utils.geostationary_geolocation import (
     get_geolocation_cache_filename,
     get_geolocation,
     AutoGenError,
 )
 
 
 LOG = logging.getLogger(__name__)
 # np.seterr(all='raise')
 
 # Installed Libraries
 
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     # If this reader is not installed on the system, don't fail alltogether, just skip
     # this import.  This reader will not work if the import fails and the package will
     # have to be installed to process data of this type.
     import netCDF4 as ncdf
-except ImportError:
-    LOG.info(
-        "Failed import netCDF4 in scifile/readers/abi_ncdf4_reader.py. If you need it,"
-        " install it."
-        ""
-    )
-
-try:
     import numexpr as ne
-except ImportError:
-    LOG.info(
-        "Failed import numexpr in scifile/readers/abi_ncdf4_reader_new.py. "
-        "If you need it, install it."
-    )
 
 interface = "readers"
 family = "standard"
 name = "abi_netcdf"
 
 
 nprocs = 6
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/ahi_hsd.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ahi_hsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,29 +21,25 @@
 
 # Installed Libraries
 import numpy as np
 import xarray
 from scipy.ndimage import zoom
 
 from geoips.utils.memusg import print_mem_usage
+from geoips.utils.context_managers import import_optional_dependencies
 from geoips.plugins.modules.readers.utils.geostationary_geolocation import (
     get_geolocation_cache_filename,
     get_geolocation,
 )
 
 LOG = logging.getLogger(__name__)
 
-
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import numexpr as ne
-except Exception:
-    LOG.info(
-        "Failed numexpr import in scifile/readers/ahi_hsd_reader_new.py. If you need"
-        " it, install it."
-    )
 
 try:
     nprocs = 6
     ne.set_num_threads(nprocs)
 except Exception:
     LOG.info(
         "Failed numexpr.set_num_threads in %s. If numexpr is not installed and you"
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/amsr2_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/amsub_hdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_hdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/amsub_mirs.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_mirs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/atms_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/atms_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/ewsg_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ewsg_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,25 @@
 import os
 
 # Installed Libraries
 import numpy as np
 import xarray as xr
 import calendar
 
+from geoips.utils.context_managers import import_optional_dependencies
 
 # If this reader is not installed on the system, don't fail altogether, just skip this
 # import. This reader will not work if the import fails, and the package will have to be
 # installed to process data of this type.
 
 LOG = logging.getLogger(__name__)
 
-
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import netCDF4 as ncdf
-except ImportError:
-    LOG.info("Failed import netCDF4. If you need it, install it.")
 
 
 # @staticmethod                                     # not sure where it is was used?
 
 # gvar_ch6 has only half scanlines of other channels (1,2,4), we temporally do not read
 # the ch6 in. We will modify this reader if gvar_ch6 is needed in the future.
 VARLIST = [
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/geoips_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/geoips_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/gmi_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/gmi_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/imerg_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/imerg_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/mimic_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/mimic_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/modis_hdf4.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/modis_hdf4.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,37 +34,23 @@
 import logging
 
 
 # Installed Libraries
 import numpy as np
 import xarray as xr
 
+from geoips.utils.context_managers import import_optional_dependencies
+
 LOG = logging.getLogger(__name__)
 
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     from pyhdf.HDF import ishdf
-except ImportError:
-    LOG.info(
-        "Failed import pyhdf in /readers/modis_hdf4.py. "
-        + "If you need it, install it."
-    )
-try:
     from pyhdf.SD import SD, SDC
-except ImportError:
-    LOG.info(
-        "Failed import pyhdf in /readers/modis_hdf4.py. "
-        + "If you need it, install it."
-    )
-try:
     from pyhdf.error import HDF4Error
-except ImportError:
-    LOG.info(
-        "Failed import pyhdf in /readers/modis_hdf4_reader.py. "
-        + "If you need it, install it."
-    )
 
 LOG.info("info on imported functions")
 
 interface = "readers"
 family = "standard"
 name = "modis_hdf4"
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/saphir_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/saphir_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/sar_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/sar_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/seviri_hrit.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/seviri_hrit.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,31 +30,32 @@
 import numpy as np
 from geoips.plugins.modules.readers.utils.hrit_reader import HritFile, HritError
 
 # Installed Libraries
 
 # GeoIPS Libraries
 from geoips.filenames.base_paths import PATHS as gpaths
+from geoips.utils.context_managers import import_optional_dependencies
 from .utils.geostationary_geolocation import (
     get_geolocation,
 )
 
 LOG = logging.getLogger(__name__)
 
-
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import numexpr as ne
-except ImportError:
-    LOG.info("Failed numexpr import in satnav.py. If you need it, install it.")
 
 try:
     NPROC = 6
     ne.set_num_threads(NPROC)
 except NameError:
-    LOG.info("Failed ne.set_num_threads in satnav.py. If you need numexpr, install it.")
+    err_str = "Failed ne.set_num_threads in seviri_hrit.py. "
+    err_str += "If you need numexpr, install it."
+    LOG.info(err_str)
 
 
 # These should be added to the data file object
 BADVALS = {
     "Off_Of_Disk": -999.9,
 }
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/sfc_winds_text.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/sfc_winds_text.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/smos_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/smos_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/ssmi_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ssmi_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/ssmis_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ssmis_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/utils/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,23 @@
 import numpy as np
 from pyresample import utils
 from pyresample.geometry import SwathDefinition
 from pyresample.kd_tree import get_neighbour_info  # , get_sample_from_neighbour_info
 
 from geoips.errors import CoverageError
 from geoips.filenames.base_paths import PATHS as gpaths
+from geoips.utils.context_managers import import_optional_dependencies
 
 LOG = logging.getLogger(__name__)
 
 interface = None
 
-
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import numexpr as ne
-except ImportError:
-    LOG.info(
-        "Failed import numexpr in scifile/readers/abi_ncdf4_reader_new.py."
-        "If you need it, install it."
-    )
 
 
 nprocs = 6
 
 try:
     ne.set_num_threads(nprocs)
 except Exception:
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/utils/hrit_reader.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/hrit_reader.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/utils/remss_reader.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/remss_reader.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/viirs_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/viirs_netcdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,24 +59,24 @@
 import logging
 import os
 
 # Installed Libraries
 import numpy
 import xarray as xr
 
+from geoips.utils.context_managers import import_optional_dependencies
+
 # If this reader is not installed on the system, don't fail altogether, just skip this
 # import. This reader will not work if the import fails, and the package will have to be
 # installed to process data of this type.
 LOG = logging.getLogger(__name__)
 
-
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import netCDF4 as ncdf
-except ImportError:
-    LOG.info("Failed import netCDF4. If you need it, install it.")
 
 
 # @staticmethod                                     # not sure where it is uwas used?
 
 
 VARLIST = {
     "DNB": ["DNB_observations"],
@@ -634,15 +634,16 @@
         for varname in xarrays[dtype].variables.keys():
             xarrays[dtype][varname] = xarrays[dtype][varname].where(
                 ~dataset_masks[dtype]
             )
         if "DNBRad" in list(xarrays[dtype].variables.keys()) and required_chan(
             chans, ["DNBRef"]
         ):
-            try:
+            with import_optional_dependencies(loglevel="info"):
+                """Attempt to import a package log to INFO if the import fails."""
                 from lunarref.lib.liblunarref import lunarref
 
                 lunarref_data = lunarref(
                     xarrays["DNB"]["DNBRad"].to_masked_array(),
                     xarrays["DNB"]["solar_zenith_angle"].to_masked_array(),
                     xarrays["DNB"]["lunar_zenith_angle"].to_masked_array(),
                     xarrays["DNB"].start_datetime.strftime("%Y%m%d%H"),
@@ -651,16 +652,14 @@
                 )
                 lunarref_data = numpy.ma.masked_less_equal(
                     lunarref_data, -999, copy=False
                 )
                 xarrays["DNB"]["DNBRef"] = xr.DataArray(
                     lunarref_data, dims=xarrays["DNB"]["DNBRad"].dims
                 )
-            except ImportError:
-                LOG.info("Failed lunarref in viirs reader.  If you need it, build it")
         # This will not duplicate memory - reference
         xarray_returns[dtype] = xarrays[dtype]
 
     # Force masking of latitude/longitude fill values, otherwise causes issues
     # when sectoring
     # fill_value = -999.9
     for dtype in xarray_returns:
```

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/wfabba_ascii.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/wfabba_ascii.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/windsat_idr37_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_idr37_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/sector_spec_generators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/title_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/title_formatters/static_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/static_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/title_formatters/tc_copyright.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_copyright.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/modules/title_formatters/tc_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/product_defaults/visir/WV.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/abi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/abi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/ahi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ahi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/amsr-e.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsr-e.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/amsr2.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsr2.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/amsu-b.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsu-b.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/ascat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ascat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/ascatuhr.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ascatuhr.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/atms.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/atms.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/gmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/gmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/gvar.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/gvar.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/hscat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/hscat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/imerg.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/imerg.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/mhs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/mhs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/mimic.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/mimic.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/modis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/modis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/oscat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/oscat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/saphir.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/saphir.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/sar-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/sar-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/seviri.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/seviri.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/smap-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/smap-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/smos-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/smos-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/ssmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ssmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/ssmis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ssmis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/tmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/tmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/viirs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/viirs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/products/windsat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/windsat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/conus.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/conus.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/ewsg.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ewsg.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/global.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/global.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/goes_east.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_east.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/goes_west.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_west.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/himawari.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/himawari.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/japan.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/japan.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/plugins/yaml/sectors/static/south_america.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_america.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/geoips/schema/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/gridline_annotators/cartopy.yaml` & `geoips-1.12.2a0/geoips/schema/gridline_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/products/bases/product.yaml` & `geoips-1.12.2a0/geoips/schema/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/sectors/specs/area_definition.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/specs/area_definition.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/sectors/specs/center.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/specs/center.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/schema/sectors/static.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/static.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/__init__.py` & `geoips-1.12.2a0/geoips/sector_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/estimate_area_extent.py` & `geoips-1.12.2a0/geoips/sector_utils/estimate_area_extent.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/overpass_predictor.py` & `geoips-1.12.2a0/geoips/sector_utils/overpass_predictor.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/projections.py` & `geoips-1.12.2a0/geoips/sector_utils/projections.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/tc_tracks.py` & `geoips-1.12.2a0/geoips/sector_utils/tc_tracks.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/tc_tracks_database.py` & `geoips-1.12.2a0/geoips/sector_utils/tc_tracks_database.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/utils.py` & `geoips-1.12.2a0/geoips/sector_utils/utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/sector_utils/yaml_utils.py` & `geoips-1.12.2a0/geoips/sector_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/utils/__init__.py` & `geoips-1.12.2a0/geoips/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/utils/decorators.py` & `geoips-1.12.2a0/geoips/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/utils/memusg.py` & `geoips-1.12.2a0/geoips/utils/memusg.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Utilities for tracking and monitoring memory and resource usage."""
 import logging
 import socket
-
 import resource
 
+from geoips.utils.context_managers import import_optional_dependencies
+
 LOG = logging.getLogger(__name__)
 
 
-try:
+with import_optional_dependencies(loglevel="info"):
+    """Attempt to import a package and print to LOG.info if the import fails."""
     import psutil
-except ImportError:
-    LOG.info(
-        "Failed import psutil in utils/memusg.py. " + "If you need it, install it."
-    )
 
 
 def print_mem_usage(logstr="", verbose=False):
     """Print memory usage to LOG.info.
 
     * By default include psutil output.
     * If verbose is True, include output from both psutil and resource packages.
```

### Comparing `geoips-1.12.0/geoips/xarray_utils/__init__.py` & `geoips-1.12.2a0/geoips/xarray_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/xarray_utils/data.py` & `geoips-1.12.2a0/geoips/xarray_utils/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 """Utilities for manipulating xarray Datasets and DataArrays."""
 
 # Python Standard Libraries
 import logging
 
 # Third Party Installed Libraries
+import numpy
+from pyresample import utils
+import xarray
 
 LOG = logging.getLogger(__name__)
 
 # scipy.interpolate.griddata requires at least 4 points. Don't bother
 # plotting if fewer than 4.
 MIN_POINTS = 4
 
@@ -233,29 +236,30 @@
         time_xarray["time"].size,
     )
     return time_xarray
 
 
 def sector_xarray_spatial(
     full_xarray,
-    extent_lonlat,
+    area_def,
     varnames,
     lon_pad=3,
     lat_pad=0,
     verbose=False,
     drop=False,
 ):
     """Sector an xarray object spatially.  If full_xarray is None, return None.
 
     Parameters
     ----------
     full_xarray : xarray.Dataset
         xarray object to sector spatially
-    extent_lonlat : list of float
-        Area to sector: [MINLON, MINLAT, MAXLON, MAXLAT]
+    area_def: pyresample.AreaDefinition
+        The requested region to sector spatially from the full_xarray.
+        If None, no spatial sectoring required.
     varnames : list of str
         list of variable names that should be sectored based on 'time'
     drop : bool
         Specify whether to remove points with no coverage (rather than masking)
 
     Returns
     -------
@@ -267,38 +271,25 @@
         if verbose:
             LOG.info(
                 "    full_xarray is None - not attempting to sector spatially, "
                 "returning None"
             )
         return None
 
-    import xarray
-
     sector_xarray = xarray.Dataset()
     sector_xarray.attrs = full_xarray.attrs.copy()
 
-    import numpy
-    from pyresample import utils
-
     if verbose:
         LOG.info("    Padding longitudes")
-    # convert extent longitude to be within 0-360 range
-    min_lon = utils.wrap_longitudes(extent_lonlat[0]) - lon_pad
-    max_lon = utils.wrap_longitudes(extent_lonlat[2]) + lon_pad
-    if min_lon > max_lon and max_lon < 0:
-        max_lon = max_lon + 360
-    min_lat = extent_lonlat[1] - lat_pad
-    max_lat = extent_lonlat[3] + lat_pad
     if verbose:
         LOG.info("    Padding latitudes")
-    # Make sure we don't extend latitudes beyond -90 / +90
-    if min_lat < -90.0:
-        min_lat = -90.0
-    if max_lat > 90.0:
-        max_lat = 90.0
+
+    min_lon, min_lat, max_lon, max_lat = get_minmax_latlon_from_area_def(
+        area_def, lon_pad, lat_pad
+    )
 
     if verbose:
         LOG.info("    Wrapping longitudes")
     lons = utils.wrap_longitudes(full_xarray["longitude"])
 
     if verbose:
         LOG.info("    Handling dateline")
@@ -412,14 +403,106 @@
         sector_xarray["latitude"].size,
     )
     # extent_lonlat[0], extent_lonlat[2], extent_lonlat[1], extent_lonlat[3],
     # final_good_points)
     return sector_xarray
 
 
+def get_minmax_latlon_from_area_def(area_def, lon_pad, lat_pad):
+    """Retrieve the Min/Max Lat/Lon from the provided area_def.
+
+    Given a PyResample AreaDefinition Object, retrieve the minimum and maximum
+    latitude and longitude values that should be used to sector the xarray efficiently.
+
+    If the provided area def encapsulates either of the poles, set the min/max latitude
+    value to -90/90 degrees accordingly, and match the other latitude value to what was
+    provided in the area_def bounds.
+
+    For longitudes, if the sector doesn't contain a pole, wrap them to ensure they exist
+    in the 0-360 range, otherwise set to -180, 180.
+
+    Parameters
+    ----------
+    area_def: PyResample AreaDefinition()
+        - The area_definition that defines the bounds of the data we will be sectoring.
+    lon_pad: float
+        - The amount (in degrees) of padding to be added to the longitude bounds.
+    lat_pad: float
+        - The amount (in degrees) of padding to be added to the latitude bounds.
+
+    Returns
+    -------
+    min_lon, min_lat, max_lon, max_lat: float
+        - These degree (float) values will be returned in the order listed above.
+    """
+    extent_lonlat = list(
+        area_def.area_extent_ll
+    )  # [min_lon, min_lat, max_lon, max_lat]
+    min_lon, max_lon = -180, 180
+
+    # Check if the area_def includes either North or South Pole. If it does, we have to
+    # manually adjust the lat_lon extent to reflect the correct extent for both lat/lon.
+    # Otherwise go about business as usual.
+    LOG.info("Checking if area_def includes the North Pole.")
+    if point_in_area_def(area_def, 0, 90):
+        LOG.info("North Pole exists within area_def.")
+        min_lat = extent_lonlat[1] - lat_pad
+        max_lat = 90
+        return min_lon, min_lat, max_lon, max_lat
+
+    LOG.info("North Pole not in area_def, checking South Pole.")
+    if point_in_area_def(area_def, 0, -90):
+        LOG.info("South Pole exists within area_def.")
+        min_lat = -90
+        max_lat = extent_lonlat[3] + lat_pad
+        return min_lon, min_lat, max_lon, max_lat
+
+    LOG.info(
+        "Neither North or South Pole are in area def, using custom bounds.",
+    )
+    # Area Definition doesn't include a pole, get the natural bounds from the area_def.
+    # convert extent longitude to be within [-180, 180] range
+    min_lon = utils.wrap_longitudes(extent_lonlat[0]) - lon_pad
+    max_lon = utils.wrap_longitudes(extent_lonlat[2]) + lon_pad
+    if min_lon > max_lon and max_lon < 0:
+        max_lon = max_lon + 360
+    min_lat = extent_lonlat[1] - lat_pad
+    max_lat = extent_lonlat[3] + lat_pad
+    # Make sure we don't extend latitudes beyond -90 / +90
+    if min_lat < -90.0:
+        min_lat = -90.0
+    if max_lat > 90.0:
+        max_lat = 90.0
+    return min_lon, min_lat, max_lon, max_lat
+
+
+def point_in_area_def(area_def, lon, lat):
+    """Determine whether or not the provided point (in degrees) is within area_def.
+
+    Parameters
+    ----------
+    area_def: PyResample AreaDefinition()
+        - The area_definition that defines the bounds of the data we will be sectoring.
+    lon: float
+        - The longitude value in degrees.
+    lat: float
+        - The latitude value in degrees.
+
+    Returns
+    -------
+    bool:
+        - Whether or not the point is contained in the area definition.
+    """
+    try:
+        area_def.get_array_indices_from_lonlat(lon, lat)
+        return True
+    except ValueError:
+        return False
+
+
 def sector_xarray_dataset(
     full_xarray,
     area_def,
     varnames,
     lon_pad=3,
     lat_pad=0,
     verbose=False,
@@ -512,18 +595,17 @@
             )
         else:
             # If it is not a dynamic sector, and we didn't pass window
             # start/end time, just return all of the data, because all
             # we care about is spatial coverage.
             time_xarray = full_xarray.copy()
 
-        extent_lonlat = list(area_def.area_extent_ll)
         sector_xarray = sector_xarray_spatial(
             time_xarray,
-            extent_lonlat,
+            area_def,
             varnames,
             lon_pad,
             lat_pad,
             verbose=verbose,
             drop=drop,
         )
         if (
```

### Comparing `geoips-1.12.0/geoips/xarray_utils/time.py` & `geoips-1.12.2a0/geoips/xarray_utils/time.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/geoips/xarray_utils/xr_to_dtree.py` & `geoips-1.12.2a0/geoips/xarray_utils/xr_to_dtree.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/pyproject.toml` & `geoips-1.12.2a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # required ones
 name = "geoips"  # geoips package available at the root of the project
-version = "1.12.0"  # 0.0.0 will be auto-updated with poetry dynamic versioning!
+version = "1.12.2a0"  # 0.0.0 will be auto-updated with poetry dynamic versioning!
 description = "Geolocated Information Processing System"
 authors = ["Tom <tom.jerry@colostate.edu>"]
 
 # optional ones
 maintainers = ["Tom <tom.jerry@colostate.edu>"]
 #homepage = "set the url"   // optional
 repository = "https://github.com/NRLMMD-GEOIPS/geoips" #optional
@@ -86,14 +86,15 @@
 # To add a new optional dependency it must be added both here and in one of the "extra"
 # groups below.
 #
 # Doc group
 pydata-sphinx-theme = { version = "*", optional = true }
 sphinx = { version = "<7.2", optional = true }
 sphinx-design = { version = "*", optional = true }
+sphinxcontrib-autoprogram = { version = "*", optional = true }
 # Lint group
 bandit = { version = "*", optional = true }
 black = { version = "*", optional = true }
 pylint = { version = "*", optional = true }
 flake8 = { version = "*", optional = true }
 flake8-rst-docstrings = { version = "*", optional = true }
 flake8-docstrings = { version = "*", optional = true }
@@ -112,14 +113,15 @@
 # nothing at this stage;
 
 [tool.poetry.extras]
 doc = [
     "pydata-sphinx-theme", # Required for building documentation
     "sphinx",              # Required for building documentation, v7.2 errors
     "sphinx-design",       # Required for building documentation
+    "sphinxcontrib-autoprogram", # Required for adding command line options to documentation
 ]
 lint = [
     "bandit",                # Syntax/security checking
     "black",                 # Syntax checking and reformatting
     "pylint",                # Syntax checking
     "flake8",                # Syntax checking
     "flake8-rst-docstrings", # numpy docstring checking
```

### Comparing `geoips-1.12.0/setup/download_test_data.py` & `geoips-1.12.2a0/setup/download_test_data.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml` & `geoips-1.12.2a0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt` & `geoips-1.12.2a0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/bad/products/bases/product.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/good/products/bases/product.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/good/products/single.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/products/single.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/schema/test_yaml_schema.py` & `geoips-1.12.2a0/tests/unit_tests/schema/test_yaml_schema.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests/xarray_utils/test_dtree.py` & `geoips-1.12.2a0/tests/unit_tests/xarray_utils/test_dtree.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/unit_tests_long/plugins/modules/readers/test_readers.py` & `geoips-1.12.2a0/tests/unit_tests_long/plugins/modules/readers/test_readers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/abi_test.yaml` & `geoips-1.12.2a0/tests/yaml_configs/abi_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/abi_test_low_memory.yaml` & `geoips-1.12.2a0/tests/yaml_configs/abi_test_low_memory.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/amsr2_no_compare_full.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_no_compare_full.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/amsr2_test.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/amsr2_test_low_memory.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test_low_memory.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/tests/yaml_configs/amsr2_test_no_compare.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test_no_compare.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.0/PKG-INFO` & `geoips-1.12.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoips
-Version: 1.12.0
+Version: 1.12.2a0
 Summary: Geolocated Information Processing System
 Home-page: https://github.com/NRLMMD-GEOIPS/geoips
 Keywords: GeoIPS,Poetry
 Author: Tom
 Author-email: tom.jerry@colostate.edu
 Maintainer: Tom
 Maintainer-email: tom.jerry@colostate.edu
@@ -52,14 +52,15 @@
 Requires-Dist: rasterio
 Requires-Dist: referencing
 Requires-Dist: satpy
 Requires-Dist: scikit-image
 Requires-Dist: scipy (>1.2)
 Requires-Dist: sphinx (<7.2) ; extra == "doc"
 Requires-Dist: sphinx-design ; extra == "doc"
+Requires-Dist: sphinxcontrib-autoprogram ; extra == "doc"
 Requires-Dist: xarray
 Requires-Dist: xarray-datatree ; extra == "test"
 Project-URL: Repository, https://github.com/NRLMMD-GEOIPS/geoips
 Description-Content-Type: text/markdown
 
     # # # Distribution Statement A. Approved for public release. Distribution unlimited.
     # # #
```

