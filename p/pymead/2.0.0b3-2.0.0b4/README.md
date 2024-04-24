# Comparing `tmp/pymead-2.0.0b3.tar.gz` & `tmp/pymead-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymead-2.0.0b3.tar", last modified: Fri Feb 23 00:01:02 2024, max compression
+gzip compressed data, was "pymead-2.0.0b4.tar", last modified: Wed Apr 24 16:40:38 2024, max compression
```

## Comparing `pymead-2.0.0b3.tar` & `pymead-2.0.0b4.tar`

### file list

```diff
@@ -1,274 +1,280 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.989967 pymead-2.0.0b3/
--rw-rw-rw-   0        0        0     1089 2024-02-19 21:20:01.000000 pymead-2.0.0b3/LICENSE.txt
--rw-rw-rw-   0        0        0     4691 2024-02-23 00:01:02.988966 pymead-2.0.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     3804 2024-02-19 21:20:01.000000 pymead-2.0.0b3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.630967 pymead-2.0.0b3/pymead/
--rw-rw-rw-   0        0        0     5060 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.747966 pymead-2.0.0b3/pymead/analysis/
--rw-rw-rw-   0        0        0      247 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/analysis/__init__.py
--rw-rw-rw-   0        0        0    85307 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/analysis/calc_aero_data.py
--rw-rw-rw-   0        0        0      598 2023-08-24 15:00:55.000000 pymead-2.0.0b3/pymead/analysis/cfd_output_templates.py
--rw-rw-rw-   0        0        0      876 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/analysis/compressible_flow.py
--rw-rw-rw-   0        0        0    17768 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/analysis/read_aero_data.py
--rw-rw-rw-   0        0        0     7689 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/analysis/single_element_inviscid.py
--rw-rw-rw-   0        0        0     1367 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.764966 pymead-2.0.0b3/pymead/core/
--rw-rw-rw-   0        0        0      132 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/__init__.py
--rw-rw-rw-   0        0        0    28189 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/airfoil.py
--rw-rw-rw-   0        0        0    10832 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/bezier.py
--rw-rw-rw-   0        0        0     8664 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/constraint_equations.py
--rw-rw-rw-   0        0        0    14573 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/constraints.py
--rw-rw-rw-   0        0        0    43353 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/gcs.py
--rw-rw-rw-   0        0        0    47323 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/geometry_collection.py
--rw-rw-rw-   0        0        0    10934 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/line.py
--rw-rw-rw-   0        0        0     4253 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/mea.py
--rw-rw-rw-   0        0        0    23595 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/param.py
--rw-rw-rw-   0        0        0     2717 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/parametric_curve.py
--rw-rw-rw-   0        0        0    13397 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/core/point.py
--rw-rw-rw-   0        0        0     3136 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/pymead_obj.py
--rw-rw-rw-   0        0        0     6485 2023-11-03 14:37:46.000000 pymead-2.0.0b3/pymead/core/spline.py
--rw-rw-rw-   0        0        0    10601 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/core/transformation.py
--rw-rw-rw-   0        0        0     2511 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/core/units.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.765966 pymead-2.0.0b3/pymead/data/
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.775965 pymead-2.0.0b3/pymead/examples/
--rw-rw-rw-   0        0        0       69 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/__init__.py
--rw-rw-rw-   0        0        0     6346 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/airfoil_matching.py
--rw-rw-rw-   0        0        0     6575 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/complex_airfoil.py
--rw-rw-rw-   0        0        0    18238 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/high_lift.py
--rw-rw-rw-   0        0        0      520 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/iges_generation.py
--rw-rw-rw-   0        0        0    12568 2023-08-14 18:34:51.000000 pymead-2.0.0b3/pymead/examples/mirrored_subsection.py
--rw-rw-rw-   0        0        0    34050 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/examples/propulsion_airframe_integration.py
--rw-rw-rw-   0        0        0     2388 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/examples/simple_airfoil.py
--rw-rw-rw-   0        0        0     3134 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/examples/symm_airfoil.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.815966 pymead-2.0.0b3/pymead/gui/
--rw-rw-rw-   0        0        0      104 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/__init__.py
--rw-rw-rw-   0        0        0     2208 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/aero_forces_graphs.py
--rw-rw-rw-   0        0        0    44391 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/airfoil_canvas.py
--rw-rw-rw-   0        0        0     2106 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/airfoil_statistics.py
--rw-rw-rw-   0        0        0      803 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/analysis_graph.py
--rw-rw-rw-   0        0        0     1831 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/autocomplete.py
--rw-rw-rw-   0        0        0     3649 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/bounds_values_table.py
--rw-rw-rw-   0        0        0     2547 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/concurrency.py
--rw-rw-rw-   0        0        0    12869 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/constraint_items.py
--rw-rw-rw-   0        0        0     2156 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/custom_context_menu_event.py
--rw-rw-rw-   0        0        0      433 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/custom_graphics_view.py
--rw-rw-rw-   0        0        0    28622 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/default_settings.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.819966 pymead-2.0.0b3/pymead/gui/dialog_widgets/
--rw-rw-rw-   0        0        0     3219 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/dialog_widgets/export_IGES.json
--rw-rw-rw-   0        0        0     1159 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/dialog_widgets/export_control_points_dialog.json
--rw-rw-rw-   0        0        0     4325 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/dialog_widgets/export_coordinates_dialog.json
--rw-rw-rw-   0        0        0      796 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/dialog_widgets/screenshot_dialog.json
--rw-rw-rw-   0        0        0     3150 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/dockable_tab_widget.py
--rw-rw-rw-   0        0        0     5309 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/draggable_point.py
--rw-rw-rw-   0        0        0     3702 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/file_selection.py
--rw-rw-rw-   0        0        0    89297 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/gui.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.823966 pymead-2.0.0b3/pymead/gui/gui_settings/
--rw-rw-rw-   0        0        0     3270 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/gui_settings/buttons.json
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.834967 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/
--rw-rw-rw-   0        0        0     1612 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_constraints_termination_settings.json
--rw-rw-rw-   0        0        0     2822 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_general_settings.json
--rw-rw-rw-   0        0        0     1451 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_save_load_settings.json
--rw-rw-rw-   0        0        0     2284 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_warm_start_batch_settings.json
--rw-rw-rw-   0        0        0     4123 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/genetic_algorithm_settings.json
--rw-rw-rw-   0        0        0     1304 2023-08-24 14:59:26.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mplot_settings.json
--rw-rw-rw-   0        0        0      383 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mses_field_plot_settings.json
--rw-rw-rw-   0        0        0     7260 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mses_settings.json
--rw-rw-rw-   0        0        0     5438 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mset_settings.json
--rw-rw-rw-   0        0        0     3318 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/multi_point_opt_settings.json
--rw-rw-rw-   0        0        0     3401 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/opt_constraints_settings.json
--rw-rw-rw-   0        0        0     5492 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/defaults/xfoil_settings.json
--rw-rw-rw-   0        0        0       45 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/gui_settings/grid_settings.json
--rw-rw-rw-   0        0        0     1661 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/menu.json
--rw-rw-rw-   0        0        0     3260 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/q_settings_descriptions.json
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.836967 pymead-2.0.0b3/pymead/gui/gui_settings/themes/
--rw-rw-rw-   0        0        0     1029 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/themes/dark_theme.json
--rw-rw-rw-   0        0        0     1032 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/gui_settings/themes/light_theme.json
--rw-rw-rw-   0        0        0     4140 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/help_browser.py
--rw-rw-rw-   0        0        0    10342 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/hoverable_curve.py
--rw-rw-rw-   0        0        0      744 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/infty_doublespinbox.py
--rw-rw-rw-   0        0        0   150089 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/input_dialog.py
--rw-rw-rw-   0        0        0     4649 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/main_icon_toolbar.py
--rw-rw-rw-   0        0        0      567 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/message_box.py
--rw-rw-rw-   0        0        0      806 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/opt_airfoil_graph.py
--rw-rw-rw-   0        0        0      789 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/parallel_coords_graph.py
--rw-rw-rw-   0        0        0    41413 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/gui/parameter_tree.py
--rw-rw-rw-   0        0        0     2030 2024-02-21 22:55:37.000000 pymead-2.0.0b3/pymead/gui/permanent_widget.py
--rw-rw-rw-   0        0        0     3924 2024-02-21 22:51:13.000000 pymead-2.0.0b3/pymead/gui/polygon_item.py
--rw-rw-rw-   0        0        0    15974 2024-02-19 23:24:23.000000 pymead-2.0.0b3/pymead/gui/pymeadPColorMeshItem.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.617967 pymead-2.0.0b3/pymead/gui/pyqt_vertical_tab_widget/
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.838967 pymead-2.0.0b3/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/
--rw-rw-rw-   0        0        0       48 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/verticalTabWidget.py
--rw-rw-rw-   0        0        0      955 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/rename_popup.py
--rw-rw-rw-   0        0        0     3592 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/sampling_visualization.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.841966 pymead-2.0.0b3/pymead/gui/scientificspinbox_master/
--rw-rw-rw-   0        0        0     5650 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/scientificspinbox_master/ScientificDoubleSpinBox.py
--rw-rw-rw-   0        0        0     6376 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/scientificspinbox_master/ScientificSpinBox.py
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/scientificspinbox_master/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/selectable_header.py
--rw-rw-rw-   0        0        0      949 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/gui/separation_lines.py
--rw-rw-rw-   0        0        0     1502 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/show_hide.py
--rw-rw-rw-   0        0        0     1934 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/side_grip.py
--rw-rw-rw-   0        0        0     1783 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/text_area.py
--rw-rw-rw-   0        0        0    10871 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/title_bar.py
--rw-rw-rw-   0        0        0     1515 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/gui/worker.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.887967 pymead-2.0.0b3/pymead/icons/
--rw-rw-rw-   0        0        0     1039 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/Add-Icon3.png
--rw-rw-rw-   0        0        0    12154 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/Moon-Icon.png
--rw-rw-rw-   0        0        0     4206 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/add_icon.png
--rw-rw-rw-   0        0        0     1560 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/airfoil_dark.svg
--rw-rw-rw-   0        0        0     1560 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/airfoil_light.svg
--rw-rw-rw-   0        0        0     1582 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/airfoil_slat.png
--rw-rw-rw-   0        0        0     4390 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/anti_parallel_constraint_dark.svg
--rw-rw-rw-   0        0        0     4390 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/anti_parallel_constraint_light.svg
--rw-rw-rw-   0        0        0     8871 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/back.png
--rw-rw-rw-   0        0        0     2132 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/bezier_dark.svg
--rw-rw-rw-   0        0        0     2132 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/bezier_light.svg
--rw-rw-rw-   0        0        0     2014 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/close-dark-mode.svg
--rw-rw-rw-   0        0        0     2014 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/close-light-mode.svg
--rw-rw-rw-   0        0        0     1931 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/closed-arrow-dark.png
--rw-rw-rw-   0        0        0     1932 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/closed-arrow-light.png
--rw-rw-rw-   0        0        0     2015 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/distance_constraint_dark.svg
--rw-rw-rw-   0        0        0     2015 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/distance_constraint_light.svg
--rw-rw-rw-   0        0        0     8608 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/forward.png
--rw-rw-rw-   0        0        0     7089 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/grid_icon.png
--rw-rw-rw-   0        0        0    50516 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/help.png
--rw-rw-rw-   0        0        0    10885 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/home.png
--rw-rw-rw-   0        0        0     2487 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/line_dark.svg
--rw-rw-rw-   0        0        0     2487 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/line_light.svg
--rw-rw-rw-   0        0        0     1915 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/maximize-dark-mode.svg
--rw-rw-rw-   0        0        0     1915 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/maximize-light-mode.svg
--rw-rw-rw-   0        0        0     2507 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/mea_dark.svg
--rw-rw-rw-   0        0        0     2507 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/mea_light.svg
--rw-rw-rw-   0        0        0     1252 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/minimize-dark-mode.svg
--rw-rw-rw-   0        0        0     1252 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/minimize-light-mode.svg
--rw-rw-rw-   0        0        0     2032 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/normal-dark-mode.svg
--rw-rw-rw-   0        0        0     2032 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/normal-light-mode.svg
--rw-rw-rw-   0        0        0     1654 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/opened-arrow-dark.png
--rw-rw-rw-   0        0        0     1635 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/opened-arrow-light.png
--rw-rw-rw-   0        0        0     1256 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/perp3_constraint_dark.svg
--rw-rw-rw-   0        0        0     1256 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/perp3_constraint_light.svg
--rw-rw-rw-   0        0        0     1808 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/point_dark.svg
--rw-rw-rw-   0        0        0     1808 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/point_light.svg
--rw-rw-rw-   0        0        0   143663 2023-08-17 15:22:58.000000 pymead-2.0.0b3/pymead/icons/pymead-logo.png
--rw-rw-rw-   0        0        0    34875 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/icons/pymead-logo_old.png
--rw-rw-rw-   0        0        0     1912 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/rel_angle_constraint_dark.svg
--rw-rw-rw-   0        0        0     1912 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/rel_angle_constraint_light.svg
--rw-rw-rw-   0        0        0    15470 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/reload.png
--rw-rw-rw-   0        0        0     2541 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/roc_constraint_dark.svg
--rw-rw-rw-   0        0        0     2541 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/roc_constraint_light.svg
--rw-rw-rw-   0        0        0    38601 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/stop.png
--rw-rw-rw-   0        0        0     5127 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/symmetry_constraint_dark.svg
--rw-rw-rw-   0        0        0     5127 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/icons/symmetry_constraint_light.svg
--rw-rw-rw-   0        0        0     1873 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/icons/web_airfoil_dark.svg
--rw-rw-rw-   0        0        0     1873 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/icons/web_airfoil_light.svg
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.895966 pymead-2.0.0b3/pymead/optimization/
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/optimization/__init__.py
--rw-rw-rw-   0        0        0     4866 2023-09-05 22:04:31.000000 pymead-2.0.0b3/pymead/optimization/conn_test.py
--rw-rw-rw-   0        0        0     7860 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/objectives_and_constraints.py
--rw-rw-rw-   0        0        0    11296 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/opt_callback.py
--rw-rw-rw-   0        0        0    11637 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/opt_setup.py
--rw-rw-rw-   0        0        0    22127 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/pop_chrom.py
--rw-rw-rw-   0        0        0     8995 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/sampling.py
--rw-rw-rw-   0        0        0    18781 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/optimization/shape_optimization.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.896966 pymead-2.0.0b3/pymead/plugins/
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.903966 pymead-2.0.0b3/pymead/plugins/IGES/
--rw-rw-rw-   0        0        0      162 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/IGES/__init__.py
--rw-rw-rw-   0        0        0     2930 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/IGES/curves.py
--rw-rw-rw-   0        0        0     5773 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/plugins/IGES/entity.py
--rw-rw-rw-   0        0        0     3510 2024-02-22 23:47:55.000000 pymead-2.0.0b3/pymead/plugins/IGES/global_params.py
--rw-rw-rw-   0        0        0     2653 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/IGES/iges_generator.py
--rw-rw-rw-   0        0        0     1164 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/IGES/iges_param.py
--rw-rw-rw-   0        0        0     1198 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/IGES/start_end_section.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.906966 pymead-2.0.0b3/pymead/plugins/NX/
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/NX/__init__.py
--rw-rw-rw-   0        0        0    43953 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/NX/journal_functions.py
--rw-rw-rw-   0        0        0     6633 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/NX/write_journal_function.py
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.911966 pymead-2.0.0b3/pymead/post/
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/post/__init__.py
--rw-rw-rw-   0        0        0      175 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/post/fonts_and_colors.py
--rw-rw-rw-   0        0        0     5009 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/post/mses_field.py
--rw-rw-rw-   0        0        0     3631 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/post/plot_formatters.py
--rw-rw-rw-   0        0        0    51497 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/post/post_process.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.916966 pymead-2.0.0b3/pymead/resources/
--rw-rw-rw-   0        0        0        0 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.920966 pymead-2.0.0b3/pymead/resources/cmcrameri/
--rw-rw-rw-   0        0        0     1191 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/cmcrameri/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/cmcrameri/__init__.py
--rw-rw-rw-   0        0        0     7168 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/cmcrameri/berlin.txt
--rw-rw-rw-   0        0        0      216 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/cmcrameri/cmaps.py
--rw-rw-rw-   0        0        0     7168 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/resources/cmcrameri/vik.txt
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.930966 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/
--rw-rw-rw-   0        0        0      899 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/AUTHORS
--rw-rw-rw-   0        0        0       63 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/BUGS
--rw-rw-rw-   0        0        0     9003 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/LICENSE
--rw-rw-rw-   0        0        0    78464 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/NEWS
--rw-rw-rw-   0        0        0     2623 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.935966 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/
--rw-rw-rw-   0        0        0      892 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans-mono.conf
--rw-rw-rw-   0        0        0      882 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans.conf
--rw-rw-rw-   0        0        0      884 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-serif.conf
--rw-rw-rw-   0        0        0     1571 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans-mono.conf
--rw-rw-rw-   0        0        0     2098 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans.conf
--rw-rw-rw-   0        0        0     1718 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-serif.conf
--rw-rw-rw-   0        0        0    26251 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/langcover.txt
--rw-rw-rw-   0        0        0  1551148 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/status.txt
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.967966 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/
--rw-rw-rw-   0        0        0   577708 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuMathTeXGyre.ttf
--rw-rw-rw-   0        0        0   705684 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Bold.ttf
--rw-rw-rw-   0        0        0   643292 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-BoldOblique.ttf
--rw-rw-rw-   0        0        0   355380 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-ExtraLight.ttf
--rw-rw-rw-   0        0        0   635416 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Oblique.ttf
--rw-rw-rw-   0        0        0   757076 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans.ttf
--rw-rw-rw-   0        0        0   665028 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Bold.ttf
--rw-rw-rw-   0        0        0   611836 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-BoldOblique.ttf
--rw-rw-rw-   0        0        0   599292 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Oblique.ttf
--rw-rw-rw-   0        0        0   680264 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed.ttf
--rw-rw-rw-   0        0        0   331992 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Bold.ttf
--rw-rw-rw-   0        0        0   253580 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-BoldOblique.ttf
--rw-rw-rw-   0        0        0   251932 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Oblique.ttf
--rw-rw-rw-   0        0        0   340712 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono.ttf
--rw-rw-rw-   0        0        0   356088 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Bold.ttf
--rw-rw-rw-   0        0        0   347460 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-BoldItalic.ttf
--rw-rw-rw-   0        0        0   345996 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Italic.ttf
--rw-rw-rw-   0        0        0   380132 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif.ttf
--rw-rw-rw-   0        0        0   331244 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Bold.ttf
--rw-rw-rw-   0        0        0   346508 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-BoldItalic.ttf
--rw-rw-rw-   0        0        0   345324 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Italic.ttf
--rw-rw-rw-   0        0        0   346664 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed.ttf
--rw-rw-rw-   0        0        0    29288 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/unicover.txt
--rw-rw-rw-   0        0        0     2256 2024-02-22 23:43:52.000000 pymead-2.0.0b3/pymead/resources/grid_test.pdf
--rw-rw-rw-   0        0        0      156 2024-02-22 23:43:52.000000 pymead-2.0.0b3/pymead/resources/grid_test.svg
--rw-rw-rw-   0        0        0       17 2024-02-22 23:43:52.000000 pymead-2.0.0b3/pymead/resources/mutool.log
--rw-rw-rw-   0        0        0      490 2024-02-22 23:43:52.000000 pymead-2.0.0b3/pymead/resources/ps2pdf.log
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.970967 pymead-2.0.0b3/pymead/tests/
--rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/tests/__init__.py
--rw-rw-rw-   0        0        0      911 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/tests/run_all_tests.py
--rw-rw-rw-   0        0        0     1006 2023-05-18 19:43:45.000000 pymead-2.0.0b3/pymead/tests/update_MEA.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.986966 pymead-2.0.0b3/pymead/utils/
--rw-rw-rw-   0        0        0       39 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/__init__.py
--rw-rw-rw-   0        0        0     8883 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/airfoil_matching.py
--rw-rw-rw-   0        0        0     4403 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/dict_recursion.py
--rw-rw-rw-   0        0        0     1301 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/downsampling_schemes.py
--rw-rw-rw-   0        0        0     4812 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/file_conversion.py
--rw-rw-rw-   0        0        0     2679 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/geometry.py
--rw-rw-rw-   0        0        0     1880 2023-08-18 18:54:04.000000 pymead-2.0.0b3/pymead/utils/get_airfoil.py
--rw-rw-rw-   0        0        0     1344 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/increment_string_index.py
--rw-rw-rw-   0        0        0     2578 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/misc.py
--rw-rw-rw-   0        0        0      476 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/nchoosek.py
--rw-rw-rw-   0        0        0      818 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/pymead_mp.py
--rw-rw-rw-   0        0        0     1882 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/read_write_files.py
--rw-rw-rw-   0        0        0     1200 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/transformations.py
--rw-rw-rw-   0        0        0     6292 2024-02-19 21:20:01.000000 pymead-2.0.0b3/pymead/utils/version_check.py
--rw-rw-rw-   0        0        0      300 2023-08-14 18:34:52.000000 pymead-2.0.0b3/pymead/utils/widget_recursion.py
--rw-rw-rw-   0        0        0       30 2024-02-23 00:00:34.000000 pymead-2.0.0b3/pymead/version.py
-drwxrwxrwx   0        0        0        0 2024-02-23 00:01:02.987966 pymead-2.0.0b3/pymead.egg-info/
--rw-rw-rw-   0        0        0     4691 2024-02-23 00:01:02.000000 pymead-2.0.0b3/pymead.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13322 2024-02-23 00:01:02.000000 pymead-2.0.0b3/pymead.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 00:01:02.000000 pymead-2.0.0b3/pymead.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-02-23 00:01:02.000000 pymead-2.0.0b3/pymead.egg-info/requires.txt
--rw-rw-rw-   0        0        0      339 2024-02-23 00:01:02.000000 pymead-2.0.0b3/pymead.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 00:01:02.989967 pymead-2.0.0b3/setup.cfg
--rw-rw-rw-   0        0        0     2490 2024-02-19 21:20:01.000000 pymead-2.0.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.356458 pymead-2.0.0b4/
+-rw-rw-rw-   0        0        0     1089 2024-02-19 21:20:01.000000 pymead-2.0.0b4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4691 2024-04-24 16:40:38.355458 pymead-2.0.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0     3804 2024-02-19 21:20:01.000000 pymead-2.0.0b4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:37.900574 pymead-2.0.0b4/pymead/
+-rw-rw-rw-   0        0        0     4819 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.032575 pymead-2.0.0b4/pymead/analysis/
+-rw-rw-rw-   0        0        0      247 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/analysis/__init__.py
+-rw-rw-rw-   0        0        0    97418 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/analysis/calc_aero_data.py
+-rw-rw-rw-   0        0        0      598 2023-08-24 15:00:55.000000 pymead-2.0.0b4/pymead/analysis/cfd_output_templates.py
+-rw-rw-rw-   0        0        0      876 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/analysis/compressible_flow.py
+-rw-rw-rw-   0        0        0    17770 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/analysis/read_aero_data.py
+-rw-rw-rw-   0        0        0     7689 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/analysis/single_element_inviscid.py
+-rw-rw-rw-   0        0        0     1367 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.049574 pymead-2.0.0b4/pymead/core/
+-rw-rw-rw-   0        0        0      132 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/core/__init__.py
+-rw-rw-rw-   0        0        0    29971 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/airfoil.py
+-rw-rw-rw-   0        0        0    12030 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/bezier.py
+-rw-rw-rw-   0        0        0     8819 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/constraint_equations.py
+-rw-rw-rw-   0        0        0    18586 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/constraints.py
+-rw-rw-rw-   0        0        0    50898 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/gcs.py
+-rw-rw-rw-   0        0        0    54022 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/geometry_collection.py
+-rw-rw-rw-   0        0        0    11552 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/line.py
+-rw-rw-rw-   0        0        0     5466 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/mea.py
+-rw-rw-rw-   0        0        0    26980 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/param.py
+-rw-rw-rw-   0        0        0      141 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/param_graph.py
+-rw-rw-rw-   0        0        0     2717 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/core/parametric_curve.py
+-rw-rw-rw-   0        0        0    14342 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/point.py
+-rw-rw-rw-   0        0        0     3266 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/core/pymead_obj.py
+-rw-rw-rw-   0        0        0     6485 2023-11-03 14:37:46.000000 pymead-2.0.0b4/pymead/core/spline.py
+-rw-rw-rw-   0        0        0    10601 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/core/transformation.py
+-rw-rw-rw-   0        0        0     2511 2024-02-28 17:02:41.000000 pymead-2.0.0b4/pymead/core/units.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.050574 pymead-2.0.0b4/pymead/data/
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.059575 pymead-2.0.0b4/pymead/examples/
+-rw-rw-rw-   0        0        0       69 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/__init__.py
+-rw-rw-rw-   0        0        0     6346 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/airfoil_matching.py
+-rw-rw-rw-   0        0        0     6575 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/complex_airfoil.py
+-rw-rw-rw-   0        0        0    18238 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/high_lift.py
+-rw-rw-rw-   0        0        0      520 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/iges_generation.py
+-rw-rw-rw-   0        0        0    12568 2023-08-14 18:34:51.000000 pymead-2.0.0b4/pymead/examples/mirrored_subsection.py
+-rw-rw-rw-   0        0        0    34050 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/examples/propulsion_airframe_integration.py
+-rw-rw-rw-   0        0        0     2388 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/examples/simple_airfoil.py
+-rw-rw-rw-   0        0        0     3134 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/examples/symm_airfoil.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.098579 pymead-2.0.0b4/pymead/gui/
+-rw-rw-rw-   0        0        0      104 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/__init__.py
+-rw-rw-rw-   0        0        0     2208 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/aero_forces_graphs.py
+-rw-rw-rw-   0        0        0    45807 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/airfoil_canvas.py
+-rw-rw-rw-   0        0        0     2101 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/airfoil_statistics.py
+-rw-rw-rw-   0        0        0     1835 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/analysis_graph.py
+-rw-rw-rw-   0        0        0     1831 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/autocomplete.py
+-rw-rw-rw-   0        0        0     3649 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/bounds_values_table.py
+-rw-rw-rw-   0        0        0     2508 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/concurrency.py
+-rw-rw-rw-   0        0        0    13432 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/constraint_items.py
+-rw-rw-rw-   0        0        0     2156 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/custom_context_menu_event.py
+-rw-rw-rw-   0        0        0      433 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/custom_graphics_view.py
+-rw-rw-rw-   0        0        0    28622 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/default_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.104580 pymead-2.0.0b4/pymead/gui/dialog_widgets/
+-rw-rw-rw-   0        0        0     3219 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/dialog_widgets/export_IGES.json
+-rw-rw-rw-   0        0        0     1159 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/dialog_widgets/export_control_points_dialog.json
+-rw-rw-rw-   0        0        0     4325 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/dialog_widgets/export_coordinates_dialog.json
+-rw-rw-rw-   0        0        0      731 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/dialog_widgets/screenshot_dialog.json
+-rw-rw-rw-   0        0        0   161523 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/dialogs.py
+-rw-rw-rw-   0        0        0     3150 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/dockable_tab_widget.py
+-rw-rw-rw-   0        0        0     5511 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/draggable_point.py
+-rw-rw-rw-   0        0        0     3767 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/file_selection.py
+-rw-rw-rw-   0        0        0    98508 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/gui.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.107578 pymead-2.0.0b4/pymead/gui/gui_settings/
+-rw-rw-rw-   0        0        0     3270 2024-02-22 23:47:55.000000 pymead-2.0.0b4/pymead/gui/gui_settings/buttons.json
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.121579 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/
+-rw-rw-rw-   0        0        0     1612 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_constraints_termination_settings.json
+-rw-rw-rw-   0        0        0     2822 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_general_settings.json
+-rw-rw-rw-   0        0        0     1451 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_save_load_settings.json
+-rw-rw-rw-   0        0        0     2284 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_warm_start_batch_settings.json
+-rw-rw-rw-   0        0        0     4123 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/genetic_algorithm_settings.json
+-rw-rw-rw-   0        0        0     1304 2023-08-24 14:59:26.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mplot_settings.json
+-rw-rw-rw-   0        0        0      378 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mses_field_plot_settings.json
+-rw-rw-rw-   0        0        0     7260 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mses_settings.json
+-rw-rw-rw-   0        0        0     5438 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mset_settings.json
+-rw-rw-rw-   0        0        0     3318 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/multi_point_opt_settings.json
+-rw-rw-rw-   0        0        0     3401 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/opt_constraints_settings.json
+-rw-rw-rw-   0        0        0     5492 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/defaults/xfoil_settings.json
+-rw-rw-rw-   0        0        0       45 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/gui_settings/grid_settings.json
+-rw-rw-rw-   0        0        0     1930 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/gui_settings/menu.json
+-rw-rw-rw-   0        0        0     3453 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/gui_settings/q_settings_descriptions.json
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.123578 pymead-2.0.0b4/pymead/gui/gui_settings/themes/
+-rw-rw-rw-   0        0        0     1029 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/themes/dark_theme.json
+-rw-rw-rw-   0        0        0     1032 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/gui_settings/themes/light_theme.json
+-rw-rw-rw-   0        0        0     4140 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/help_browser.py
+-rw-rw-rw-   0        0        0    10352 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/hoverable_curve.py
+-rw-rw-rw-   0        0        0      744 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/infty_doublespinbox.py
+-rw-rw-rw-   0        0        0     4649 2024-02-22 23:47:55.000000 pymead-2.0.0b4/pymead/gui/main_icon_toolbar.py
+-rw-rw-rw-   0        0        0      562 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/message_box.py
+-rw-rw-rw-   0        0        0      806 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/opt_airfoil_graph.py
+-rw-rw-rw-   0        0        0      789 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/parallel_coords_graph.py
+-rw-rw-rw-   0        0        0    46554 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/parameter_tree.py
+-rw-rw-rw-   0        0        0     2030 2024-02-21 22:55:37.000000 pymead-2.0.0b4/pymead/gui/permanent_widget.py
+-rw-rw-rw-   0        0        0     3924 2024-02-21 22:51:13.000000 pymead-2.0.0b4/pymead/gui/polygon_item.py
+-rw-rw-rw-   0        0        0    15974 2024-02-19 23:24:23.000000 pymead-2.0.0b4/pymead/gui/pymeadPColorMeshItem.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:37.885576 pymead-2.0.0b4/pymead/gui/pyqt_vertical_tab_widget/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.125577 pymead-2.0.0b4/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/
+-rw-rw-rw-   0        0        0       48 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/verticalTabWidget.py
+-rw-rw-rw-   0        0        0      955 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/rename_popup.py
+-rw-rw-rw-   0        0        0     3592 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/sampling_visualization.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.128578 pymead-2.0.0b4/pymead/gui/scientificspinbox_master/
+-rw-rw-rw-   0        0        0     5650 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/scientificspinbox_master/ScientificDoubleSpinBox.py
+-rw-rw-rw-   0        0        0     6376 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/scientificspinbox_master/ScientificSpinBox.py
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/scientificspinbox_master/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/selectable_header.py
+-rw-rw-rw-   0        0        0      949 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/gui/separation_lines.py
+-rw-rw-rw-   0        0        0     1497 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/gui/show_hide.py
+-rw-rw-rw-   0        0        0     1934 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/side_grip.py
+-rw-rw-rw-   0        0        0     1783 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/text_area.py
+-rw-rw-rw-   0        0        0    10871 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/title_bar.py
+-rw-rw-rw-   0        0        0     1515 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/gui/worker.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.174577 pymead-2.0.0b4/pymead/icons/
+-rw-rw-rw-   0        0        0     1039 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/Add-Icon3.png
+-rw-rw-rw-   0        0        0    12154 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/Moon-Icon.png
+-rw-rw-rw-   0        0        0     4206 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/add_icon.png
+-rw-rw-rw-   0        0        0     1560 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/airfoil_dark.svg
+-rw-rw-rw-   0        0        0     1560 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/airfoil_light.svg
+-rw-rw-rw-   0        0        0     1582 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/airfoil_slat.png
+-rw-rw-rw-   0        0        0     4390 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/anti_parallel_constraint_dark.svg
+-rw-rw-rw-   0        0        0     4390 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/anti_parallel_constraint_light.svg
+-rw-rw-rw-   0        0        0     8871 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/back.png
+-rw-rw-rw-   0        0        0     2132 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/bezier_dark.svg
+-rw-rw-rw-   0        0        0     2132 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/bezier_light.svg
+-rw-rw-rw-   0        0        0     2014 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/close-dark-mode.svg
+-rw-rw-rw-   0        0        0     2014 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/close-light-mode.svg
+-rw-rw-rw-   0        0        0     1931 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/closed-arrow-dark.png
+-rw-rw-rw-   0        0        0     1932 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/closed-arrow-light.png
+-rw-rw-rw-   0        0        0     2015 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/distance_constraint_dark.svg
+-rw-rw-rw-   0        0        0     2015 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/distance_constraint_light.svg
+-rw-rw-rw-   0        0        0     8608 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/forward.png
+-rw-rw-rw-   0        0        0     7089 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/grid_icon.png
+-rw-rw-rw-   0        0        0    50516 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/help.png
+-rw-rw-rw-   0        0        0    10885 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/home.png
+-rw-rw-rw-   0        0        0     2487 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/line_dark.svg
+-rw-rw-rw-   0        0        0     2487 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/line_light.svg
+-rw-rw-rw-   0        0        0     1915 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/maximize-dark-mode.svg
+-rw-rw-rw-   0        0        0     1915 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/maximize-light-mode.svg
+-rw-rw-rw-   0        0        0     2507 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/mea_dark.svg
+-rw-rw-rw-   0        0        0     2507 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/mea_light.svg
+-rw-rw-rw-   0        0        0     1252 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/minimize-dark-mode.svg
+-rw-rw-rw-   0        0        0     1252 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/minimize-light-mode.svg
+-rw-rw-rw-   0        0        0     2032 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/normal-dark-mode.svg
+-rw-rw-rw-   0        0        0     2032 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/normal-light-mode.svg
+-rw-rw-rw-   0        0        0     1654 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/opened-arrow-dark.png
+-rw-rw-rw-   0        0        0     1635 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/opened-arrow-light.png
+-rw-rw-rw-   0        0        0     1256 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/perp3_constraint_dark.svg
+-rw-rw-rw-   0        0        0     1256 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/perp3_constraint_light.svg
+-rw-rw-rw-   0        0        0     1808 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/point_dark.svg
+-rw-rw-rw-   0        0        0     1808 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/point_light.svg
+-rw-rw-rw-   0        0        0   143663 2023-08-17 15:22:58.000000 pymead-2.0.0b4/pymead/icons/pymead-logo.png
+-rw-rw-rw-   0        0        0    34875 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/icons/pymead-logo_old.png
+-rw-rw-rw-   0        0        0   200571 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/icons/pymead-splash.png
+-rw-rw-rw-   0        0        0     1912 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/rel_angle_constraint_dark.svg
+-rw-rw-rw-   0        0        0     1912 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/rel_angle_constraint_light.svg
+-rw-rw-rw-   0        0        0    15470 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/reload.png
+-rw-rw-rw-   0        0        0     2541 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/roc_constraint_dark.svg
+-rw-rw-rw-   0        0        0     2541 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/roc_constraint_light.svg
+-rw-rw-rw-   0        0        0    38601 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/stop.png
+-rw-rw-rw-   0        0        0     5127 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/symmetry_constraint_dark.svg
+-rw-rw-rw-   0        0        0     5127 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/icons/symmetry_constraint_light.svg
+-rw-rw-rw-   0        0        0     1873 2024-02-22 23:47:55.000000 pymead-2.0.0b4/pymead/icons/web_airfoil_dark.svg
+-rw-rw-rw-   0        0        0     1873 2024-02-22 23:47:55.000000 pymead-2.0.0b4/pymead/icons/web_airfoil_light.svg
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.181578 pymead-2.0.0b4/pymead/optimization/
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/optimization/__init__.py
+-rw-rw-rw-   0        0        0     4866 2023-09-05 22:04:31.000000 pymead-2.0.0b4/pymead/optimization/conn_test.py
+-rw-rw-rw-   0        0        0     7860 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/optimization/objectives_and_constraints.py
+-rw-rw-rw-   0        0        0    11141 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/optimization/opt_callback.py
+-rw-rw-rw-   0        0        0    11632 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/optimization/opt_setup.py
+-rw-rw-rw-   0        0        0    22240 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/optimization/pop_chrom.py
+-rw-rw-rw-   0        0        0     8995 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/optimization/sampling.py
+-rw-rw-rw-   0        0        0    18727 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/optimization/shape_optimization.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.182579 pymead-2.0.0b4/pymead/plugins/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.189581 pymead-2.0.0b4/pymead/plugins/IGES/
+-rw-rw-rw-   0        0        0      162 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/IGES/__init__.py
+-rw-rw-rw-   0        0        0     2930 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/IGES/curves.py
+-rw-rw-rw-   0        0        0     5773 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/plugins/IGES/entity.py
+-rw-rw-rw-   0        0        0     3510 2024-02-22 23:47:55.000000 pymead-2.0.0b4/pymead/plugins/IGES/global_params.py
+-rw-rw-rw-   0        0        0     2653 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/IGES/iges_generator.py
+-rw-rw-rw-   0        0        0     1164 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/IGES/iges_param.py
+-rw-rw-rw-   0        0        0     1198 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/IGES/start_end_section.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.192579 pymead-2.0.0b4/pymead/plugins/NX/
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/NX/__init__.py
+-rw-rw-rw-   0        0        0    43953 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/NX/journal_functions.py
+-rw-rw-rw-   0        0        0     6633 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/NX/write_journal_function.py
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.197579 pymead-2.0.0b4/pymead/post/
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/post/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/post/fonts_and_colors.py
+-rw-rw-rw-   0        0        0     5009 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/post/mses_field.py
+-rw-rw-rw-   0        0        0     3631 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/post/plot_formatters.py
+-rw-rw-rw-   0        0        0    52817 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/post/post_process.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.201579 pymead-2.0.0b4/pymead/resources/
+-rw-rw-rw-   0        0        0        0 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.206579 pymead-2.0.0b4/pymead/resources/cmcrameri/
+-rw-rw-rw-   0        0        0     1191 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/cmcrameri/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/cmcrameri/__init__.py
+-rw-rw-rw-   0        0        0     7168 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/cmcrameri/berlin.txt
+-rw-rw-rw-   0        0        0      216 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/cmcrameri/cmaps.py
+-rw-rw-rw-   0        0        0     7168 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/resources/cmcrameri/vik.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.239577 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/
+-rw-rw-rw-   0        0        0      899 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/AUTHORS
+-rw-rw-rw-   0        0        0       63 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/BUGS
+-rw-rw-rw-   0        0        0     9003 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/LICENSE
+-rw-rw-rw-   0        0        0    78464 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/NEWS
+-rw-rw-rw-   0        0        0     2623 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.245574 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/
+-rw-rw-rw-   0        0        0      892 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans-mono.conf
+-rw-rw-rw-   0        0        0      882 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans.conf
+-rw-rw-rw-   0        0        0      884 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-serif.conf
+-rw-rw-rw-   0        0        0     1571 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans-mono.conf
+-rw-rw-rw-   0        0        0     2098 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans.conf
+-rw-rw-rw-   0        0        0     1718 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-serif.conf
+-rw-rw-rw-   0        0        0    26251 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/langcover.txt
+-rw-rw-rw-   0        0        0  1551148 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/status.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.326456 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/
+-rw-rw-rw-   0        0        0   577708 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuMathTeXGyre.ttf
+-rw-rw-rw-   0        0        0   705684 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Bold.ttf
+-rw-rw-rw-   0        0        0   643292 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-BoldOblique.ttf
+-rw-rw-rw-   0        0        0   355380 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-ExtraLight.ttf
+-rw-rw-rw-   0        0        0   635416 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Oblique.ttf
+-rw-rw-rw-   0        0        0   757076 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans.ttf
+-rw-rw-rw-   0        0        0   665028 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Bold.ttf
+-rw-rw-rw-   0        0        0   611836 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-BoldOblique.ttf
+-rw-rw-rw-   0        0        0   599292 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Oblique.ttf
+-rw-rw-rw-   0        0        0   680264 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed.ttf
+-rw-rw-rw-   0        0        0   331992 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Bold.ttf
+-rw-rw-rw-   0        0        0   253580 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-BoldOblique.ttf
+-rw-rw-rw-   0        0        0   251932 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Oblique.ttf
+-rw-rw-rw-   0        0        0   340712 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono.ttf
+-rw-rw-rw-   0        0        0   356088 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Bold.ttf
+-rw-rw-rw-   0        0        0   347460 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   345996 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Italic.ttf
+-rw-rw-rw-   0        0        0   380132 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif.ttf
+-rw-rw-rw-   0        0        0   331244 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Bold.ttf
+-rw-rw-rw-   0        0        0   346508 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   345324 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Italic.ttf
+-rw-rw-rw-   0        0        0   346664 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed.ttf
+-rw-rw-rw-   0        0        0    29288 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/unicover.txt
+-rw-rw-rw-   0        0        0     2256 2024-04-24 16:06:37.000000 pymead-2.0.0b4/pymead/resources/grid_test.pdf
+-rw-rw-rw-   0        0        0      156 2024-04-24 16:06:37.000000 pymead-2.0.0b4/pymead/resources/grid_test.svg
+-rw-rw-rw-   0        0        0       17 2024-04-24 16:06:37.000000 pymead-2.0.0b4/pymead/resources/mutool.log
+-rw-rw-rw-   0        0        0      490 2024-04-24 16:06:37.000000 pymead-2.0.0b4/pymead/resources/ps2pdf.log
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.329456 pymead-2.0.0b4/pymead/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.333456 pymead-2.0.0b4/pymead/tests/core_tests/
+-rw-rw-rw-   0        0        0    55500 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/tests/core_tests/baseline_joa_complete.jmea
+-rw-rw-rw-   0        0        0     2588 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/tests/core_tests/connected_angles.jmea
+-rw-rw-rw-   0        0        0     3455 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/tests/core_tests/double_angle.jmea
+-rw-rw-rw-   0        0        0     2514 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/tests/core_tests/mirror_ap3_constraint.jmea
+-rw-rw-rw-   0        0        0      911 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/tests/run_all_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.353458 pymead-2.0.0b4/pymead/utils/
+-rw-rw-rw-   0        0        0       39 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/__init__.py
+-rw-rw-rw-   0        0        0     8883 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/airfoil_matching.py
+-rw-rw-rw-   0        0        0     4403 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/dict_recursion.py
+-rw-rw-rw-   0        0        0     1301 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/downsampling_schemes.py
+-rw-rw-rw-   0        0        0     4812 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/file_conversion.py
+-rw-rw-rw-   0        0        0     2679 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/geometry.py
+-rw-rw-rw-   0        0        0     2060 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/utils/get_airfoil.py
+-rw-rw-rw-   0        0        0     1344 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/increment_string_index.py
+-rw-rw-rw-   0        0        0     2578 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/misc.py
+-rw-rw-rw-   0        0        0      476 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/nchoosek.py
+-rw-rw-rw-   0        0        0     1148 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/utils/pymead_mp.py
+-rw-rw-rw-   0        0        0     1882 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/read_write_files.py
+-rw-rw-rw-   0        0        0     1200 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/transformations.py
+-rw-rw-rw-   0        0        0     6292 2024-02-19 21:20:01.000000 pymead-2.0.0b4/pymead/utils/version_check.py
+-rw-rw-rw-   0        0        0      300 2023-08-14 18:34:52.000000 pymead-2.0.0b4/pymead/utils/widget_recursion.py
+-rw-rw-rw-   0        0        0       30 2024-04-24 16:38:35.000000 pymead-2.0.0b4/pymead/version.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:40:38.354458 pymead-2.0.0b4/pymead.egg-info/
+-rw-rw-rw-   0        0        0     4691 2024-04-24 16:40:37.000000 pymead-2.0.0b4/pymead.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13533 2024-04-24 16:40:37.000000 pymead-2.0.0b4/pymead.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:40:37.000000 pymead-2.0.0b4/pymead.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-04-24 16:40:37.000000 pymead-2.0.0b4/pymead.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      339 2024-04-24 16:40:37.000000 pymead-2.0.0b4/pymead.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:40:38.356458 pymead-2.0.0b4/setup.cfg
+-rw-rw-rw-   0        0        0     2549 2024-04-24 16:38:35.000000 pymead-2.0.0b4/setup.py
```

### Comparing `pymead-2.0.0b3/LICENSE.txt` & `pymead-2.0.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/PKG-INFO` & `pymead-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymead
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Python library for generation, aerodynamic analysis, and aerodynamic shape optimization of parametric airfoils and airfoil systems
 Home-page: https://github.com/mlau154/pymead
 Author: Matthew G Lauer
 Author-email: mlauer2015@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymead-2.0.0b3/README.md` & `pymead-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/__init__.py` & `pymead-2.0.0b4/pymead/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,22 +72,24 @@
   curvature continuity, but may be useful in some cases.
 
 """
 import os
 
 from PyQt5.QtCore import QCoreApplication, QSettings
 
-DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
-RESOURCE_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "resources")
-ICON_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "icons")
-PLUGINS_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "plugins")
-INCLUDE_FILES = [os.path.join(os.path.dirname(os.path.abspath(__file__)), "core", "symmetry.py")]
-GUI_DEFAULTS_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "gui", "gui_settings", "defaults")
-GUI_SETTINGS_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "gui", "gui_settings")
-GUI_THEMES_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "gui", "gui_settings", "themes")
-GUI_DEFAULT_AIRFOIL_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "gui", "default_airfoil")
-GUI_DIALOG_WIDGETS_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "gui", "dialog_widgets")
+BASE_DIR = os.path.dirname(os.path.abspath(__file__))
+DATA_DIR = os.path.join(BASE_DIR, "data")
+RESOURCE_DIR = os.path.join(BASE_DIR, "resources")
+ICON_DIR = os.path.join(BASE_DIR, "icons")
+PLUGINS_DIR = os.path.join(BASE_DIR, "plugins")
+INCLUDE_FILES = [os.path.join(BASE_DIR, "core", "symmetry.py")]
+GUI_DEFAULTS_DIR = os.path.join(BASE_DIR, "gui", "gui_settings", "defaults")
+GUI_SETTINGS_DIR = os.path.join(BASE_DIR, "gui", "gui_settings")
+GUI_THEMES_DIR = os.path.join(BASE_DIR, "gui", "gui_settings", "themes")
+GUI_DEFAULT_AIRFOIL_DIR = os.path.join(BASE_DIR, "gui", "default_airfoil")
+GUI_DIALOG_WIDGETS_DIR = os.path.join(BASE_DIR, "gui", "dialog_widgets")
+TEST_DIR = os.path.join(BASE_DIR, "tests")
 
 QCoreApplication.setOrganizationName("mlaero")
 QCoreApplication.setApplicationName("pymead")
 
 q_settings = QSettings()
```

### Comparing `pymead-2.0.0b3/pymead/analysis/calc_aero_data.py` & `pymead-2.0.0b4/pymead/analysis/calc_aero_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-import subprocess
-import os
-import typing
-from copy import deepcopy
-import time
-from collections import namedtuple
-
-import numpy as np
-from matplotlib import pyplot as plt
-from scipy.interpolate import CloughTocher2DInterpolator
-from shapely.geometry import MultiPoint
-
-from pymead.core.mea import MEA
-from pymead.analysis.read_aero_data import read_aero_data_from_xfoil, read_Cp_from_file_xfoil, read_bl_data_from_mses, \
-    read_forces_from_mses, read_grid_stats_from_mses, read_field_from_mses, read_streamline_grid_from_mses, \
-    flow_var_idx, convert_blade_file_to_3d_array, read_actuator_disk_data_mses, read_Mach_from_mses_file
-from pymead.analysis.compressible_flow import calculate_normal_shock_total_pressure_ratio
-from pymead.utils.file_conversion import convert_ps_to_svg
-from pymead.utils.geometry import convert_numpy_array_to_shapely_LineString
-from pymead.utils.read_write_files import save_data
 import os
 import subprocess
 import time
 import typing
 from collections import namedtuple
 from copy import deepcopy
 
@@ -306,18 +286,20 @@
                         run_mplot(airfoil_name, airfoil_coord_dir, mplot_settings, mode=mplot_output_name)
                         if mplot_output_name == 'flow_field':
                             run_mplot(airfoil_name, airfoil_coord_dir, mplot_settings, mode='grid_stats')
 
                 if mplot_settings["CPK"]:
                     try:
                         # outputs_CPK = calculate_CPK_power_consumption(os.path.join(airfoil_coord_dir, airfoil_name))
+                        # outputs_CPK = calculate_CPK_power_consumption_old(os.path.join(airfoil_coord_dir, airfoil_name))
                         outputs_CPK = calculate_CPK_mses_inviscid_only(os.path.join(airfoil_coord_dir, airfoil_name))
                     except Exception as e:
                         print(f"{e = }")
-                        # outputs_CPK = {"CPK": 1e9, "diss_shock": 1e9, "diss_surf": 1e9, "Edot": 1e9, "Cd": 1e9}
+                        # outputs_CPK = {"CPK": 1e9, "diss_shock": 1e9, "diss_surf": 1e9, "Edot": 1e9, "Cd": 1e9,
+                        #                "Edota": 1e9, "Edotp": 1e9}
                         outputs_CPK = {"CPK": 1e9}
                     aero_data = {**aero_data, **outputs_CPK}
 
             t2 = time.time()
             # print(f"Time for stencil point {i}: {t2 - t1} seconds")
 
             if converged:
@@ -346,14 +328,50 @@
 
         if save_aero_data:
             save_data(aero_data, os.path.join(airfoil_coord_dir, airfoil_name, "aero_data.json"))
 
         return aero_data, logs
 
 
+def calculate_Cl_integral_form(x: np.ndarray, y: np.ndarray, Cp: np.ndarray, alfa: float):
+    # Calculate the lift coefficient (integral from 0 to max arc length of Cp*(nhat dot jhat)*dl)
+    panel_length = np.hypot(x[1:] - x[:-1], y[1:] - y[:-1])  # length of the panels
+    panel_nhat_angle = np.arctan2(y[1:] - y[:-1], x[1:] - x[:-1]) + np.pi / 2  # angle of the panel outward normal vector
+    panel_center_x = 0.5 * (x[1:] + x[:-1])
+    panel_center_y = 0.5 * (y[1:] + y[:-1])
+    quarter_chord_center_x = 0.25
+    quarter_chord_center_y = 0.0
+    panel_nhat_jcomp = np.sin(panel_nhat_angle - alfa)  # j-component of the panel normal vector
+    # panel_nhat_icomp = np.cos(panel_nhat_angle - alfa)
+    panel_Cp = (Cp[1:] + Cp[:-1]) / 2  # average pressure coefficient of the panel
+    panel_force = panel_Cp * np.array([np.cos(panel_nhat_angle - np.pi),
+                                       np.sin(panel_nhat_angle - np.pi)]) * panel_length
+    r_vec = np.array([panel_center_x - quarter_chord_center_x, panel_center_y - quarter_chord_center_y])
+    panel_Cm = np.cross(r_vec.T, panel_force.T)
+    Cm = np.sum(panel_Cm)
+    Cl = np.sum(panel_Cp * panel_nhat_jcomp * panel_length)
+    # Cdp = np.sum(panel_Cp * panel_nhat_icomp * panel_length)
+    return Cl, Cm
+
+
+def read_alfa_from_xfoil_cp_file(xfoil_cp_file: str):
+    with open(xfoil_cp_file, "r") as f:
+        lines = f.readlines()
+    return float(lines[1].split()[2])
+
+
+def calculate_Cl_alfa_xfoil_inviscid(airfoil_name: str, base_dir: str):
+    cp_file = os.path.join(base_dir, f"{airfoil_name}_Cp.dat")
+    alfa = read_alfa_from_xfoil_cp_file(cp_file)
+    data = np.loadtxt(cp_file, skiprows=3)
+    x, y, Cp = data[:, 0], data[:, 1], data[:, 2]
+    Cl, Cm = calculate_Cl_integral_form(x, y, Cp, np.deg2rad(alfa))
+    return Cl, Cm, alfa
+
+
 def run_xfoil(airfoil_name: str, base_dir: str, xfoil_settings: dict, coords: np.ndarray,
               export_Cp: bool = True):
     aero_data = {}
 
     if "xtr" not in xfoil_settings.keys():
         xfoil_settings["xtr"] = [1.0, 1.0]
     if 'N' not in xfoil_settings.keys():
@@ -370,18 +388,22 @@
         try:
             np.savetxt(f, coords)
             break
         except OSError:
             time.sleep(0.01)
 
     xfoil_input_file = os.path.join(base_dir, 'xfoil_input.txt')
-    xfoil_input_list = ['', 'oper', f'iter {xfoil_settings["iter"]}', 'visc', str(xfoil_settings['Re']),
-                        f'M {xfoil_settings["Ma"]}',
-                        'vpar', f'xtr {xfoil_settings["xtr"][0]} {xfoil_settings["xtr"][1]}',
-                        f'N {xfoil_settings["N"]}', '']
+
+    if xfoil_settings["visc"]:
+        xfoil_input_list = ['', 'oper', f'iter {xfoil_settings["iter"]}', 'visc', str(xfoil_settings['Re']),
+                            f'M {xfoil_settings["Ma"]}',
+                            'vpar', f'xtr {xfoil_settings["xtr"][0]} {xfoil_settings["xtr"][1]}',
+                            f'N {xfoil_settings["N"]}', '']
+    else:
+        xfoil_input_list = ["", "oper", f"iter {xfoil_settings['iter']}", f"M {xfoil_settings['Ma']}"]
 
     # alpha/Cl input setup (must choose exactly one of alpha, Cl, or CLI)
     if len([0 for prescribed_xfoil_val in (
             'alfa', 'Cl', 'CLI') if prescribed_xfoil_val in xfoil_settings.keys()]) != 1:
         raise ValueError('Either none or more than one of alpha, Cl, or CLI was set. '
                          'Choose exactly one for XFOIL analysis.')
     alpha = None
@@ -449,20 +471,27 @@
                 h.write('After timeout, \nOutput: \n'.encode('utf-8'))
                 h.write(outs)
                 h.write('\nErrors:\n'.encode('utf-8'))
                 h.write(errs)
             aero_data['timed_out'] = True
             aero_data['converged'] = False
         finally:
-            if not aero_data['timed_out'] and aero_data["converged"]:
-                line1, line2 = read_aero_data_from_xfoil(xfoil_log, aero_data)
-                if line1 is not None:
-                    convert_xfoil_string_to_aero_data(line1, line2, aero_data)
+            if xfoil_settings["visc"]:
+                if not aero_data['timed_out'] and aero_data["converged"]:
+                    line1, line2 = read_aero_data_from_xfoil(xfoil_log, aero_data)
+                    if line1 is not None:
+                        convert_xfoil_string_to_aero_data(line1, line2, aero_data)
+                        if export_Cp:
+                            aero_data['Cp'] = read_Cp_from_file_xfoil(os.path.join(base_dir, f"{airfoil_name}_Cp.dat"))
+            else:
+                if not aero_data["timed_out"] and aero_data["converged"]:
+                    aero_data["Cl"], aero_data["Cm"], aero_data["alf"] = calculate_Cl_alfa_xfoil_inviscid(
+                        airfoil_name=airfoil_name, base_dir=base_dir)
                     if export_Cp:
-                        aero_data['Cp'] = read_Cp_from_file_xfoil(os.path.join(base_dir, f"{airfoil_name}_Cp.dat"))
+                        aero_data["Cp"] = read_Cp_from_file_xfoil(os.path.join(base_dir, f"{airfoil_name}_Cp.dat"))
 
     return aero_data, xfoil_log
 
 
 def run_mset(name: str, base_dir: str, mset_settings: dict, mea_airfoil_names: typing.List[str],
              coords: typing.List[np.ndarray] = None, mea: MEA = None):
     r"""
@@ -670,31 +699,42 @@
             mplot_input_list = ['3', '3', 'M', '', '9', 'B', '', '6', '-0.441', '0.722', '1.937', '-0.626', '3', 'M',
                                 f'{min_contour} {max_contour} {n_intervals}', '8', '', '0']
         mplot_log = os.path.join(base_dir, name, 'mplot_mach.log')
     else:
         raise Exception("Invalid MPLOT mode!")
     mplot_input_file = os.path.join(base_dir, name, mplot_input_name)
     write_input_file(mplot_input_file, mplot_input_list)
-    with open(mplot_log, 'wb') as f:
-        with open(mplot_input_file, 'r') as g:
-            process = subprocess.Popen(['mplot', name], stdin=g, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-                                       cwd=os.path.join(base_dir, name))
+
+    mplot_attempts = 0
+    mplot_max_attempts = 100
+    while mplot_attempts < mplot_max_attempts:
         try:
-            outs, errs = process.communicate(timeout=mplot_settings['timeout'])
-            f.write('Output:\n'.encode('utf-8'))
-            f.write(outs)
-            f.write('\nErrors:\n'.encode('utf-8'))
-            f.write(errs)
-        except subprocess.TimeoutExpired:
-            process.kill()
-            outs, errs = process.communicate()
-            f.write('After timeout, \nOutput: \n'.encode('utf-8'))
-            f.write(outs)
-            f.write('\nErrors:\n'.encode('utf-8'))
-            f.write(errs)
+            with open(mplot_log, 'wb') as f:
+                with open(mplot_input_file, 'r') as g:
+                    process = subprocess.Popen(['mplot', name], stdin=g, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                                               cwd=os.path.join(base_dir, name))
+                try:
+                    outs, errs = process.communicate(timeout=mplot_settings['timeout'])
+                    f.write('Output:\n'.encode('utf-8'))
+                    f.write(outs)
+                    f.write('\nErrors:\n'.encode('utf-8'))
+                    f.write(errs)
+                except subprocess.TimeoutExpired:
+                    process.kill()
+                    outs, errs = process.communicate()
+                    f.write('After timeout, \nOutput: \n'.encode('utf-8'))
+                    f.write(outs)
+                    f.write('\nErrors:\n'.encode('utf-8'))
+                    f.write(errs)
+            break
+        except OSError:
+            # In case any of the log files cannot be created/read temporarily, wait a short period of time and try again
+            time.sleep(0.01)
+            mplot_attempts += 1
+
     if mode in ["Mach", "mach", "M", "m", "Mach contours", "Mach Contours", "mach contours"]:
         convert_ps_to_svg(os.path.join(base_dir, name),
                           'plot.ps',
                           'Mach_contours.pdf',
                           'Mach_contours.svg')
     elif mode in ['grid', 'Grid', 'GRID']:
         convert_ps_to_svg(os.path.join(base_dir, name), 'plot.ps', 'grid.pdf', 'grid.svg')
@@ -772,15 +812,23 @@
             mea_coords = np.row_stack((mea_coords, np.array([999.0, 999.0])))  # MSES-specific airfoil delimiter
             mea_coords = np.row_stack((mea_coords, airfoil_coords))  # Append this airfoil's coordinates to the mat.
 
     # Generate the full file path
     blade_file_path = os.path.join(base_dir, name, f"blade.{name}")
 
     # Save the coordinates to file
-    np.savetxt(blade_file_path, mea_coords, header=header, comments="")
+    attempt = 0
+    max_attempts = 100
+    while attempt < max_attempts:
+        try:
+            np.savetxt(blade_file_path, mea_coords, header=header, comments="")
+            break
+        except OSError:
+            time.sleep(0.01)
+            attempt += 1
 
     # Get the airfoil name order
     airfoil_name_order = [mea_airfoil_names[idx] for idx in airfoil_order]
 
     return blade_file_path, airfoil_name_order
 
 
@@ -803,37 +851,45 @@
     =======
     str
       Path of the created grid parameter file
     """
     if not os.path.exists(os.path.join(base_folder, name)):  # if specified directory doesn't exist,
         os.mkdir(os.path.join(base_folder, name))  # create it
     gridpar_file = os.path.join(base_folder, name, 'gridpar.' + name)
-    with open(gridpar_file, 'w') as f:  # Open the gridpar_file with write permission
-        f.write(f"{int(mset_settings['airfoil_side_points'])}\n")
-        f.write(f"{mset_settings['exp_side_points']}\n")
-        f.write(f"{int(mset_settings['inlet_pts_left_stream'])}\n")
-        f.write(f"{int(mset_settings['outlet_pts_right_stream'])}\n")
-        f.write(f"{int(mset_settings['num_streams_top'])}\n")
-        f.write(f"{int(mset_settings['num_streams_bot'])}\n")
-        f.write(f"{int(mset_settings['max_streams_between'])}\n")
-        f.write(f"{mset_settings['elliptic_param']}\n")
-        f.write(f"{mset_settings['stag_pt_aspect_ratio']}\n")
-        f.write(f"{mset_settings['x_spacing_param']}\n")
-        f.write(f"{mset_settings['alf0_stream_gen']}\n")
-
-        multi_airfoil_grid = mset_settings['multi_airfoil_grid']
-
-        for a in airfoil_name_order:
-            f.write(f"{multi_airfoil_grid[a]['dsLE_dsAvg']} {multi_airfoil_grid[a]['dsTE_dsAvg']} "
-                    f"{multi_airfoil_grid[a]['curvature_exp']}\n")
-
-        for a in airfoil_name_order:
-            f.write(f"{multi_airfoil_grid[a]['U_s_smax_min']} {multi_airfoil_grid[a]['U_s_smax_max']} "
-                    f"{multi_airfoil_grid[a]['L_s_smax_min']} {multi_airfoil_grid[a]['L_s_smax_max']} "
-                    f"{multi_airfoil_grid[a]['U_local_avg_spac_ratio']} {multi_airfoil_grid[a]['L_local_avg_spac_ratio']}\n")
+    attempt = 0
+    max_attempts = 100
+    while attempt < max_attempts:
+        try:
+            with open(gridpar_file, 'w') as f:  # Open the gridpar_file with write permission
+                f.write(f"{int(mset_settings['airfoil_side_points'])}\n")
+                f.write(f"{mset_settings['exp_side_points']}\n")
+                f.write(f"{int(mset_settings['inlet_pts_left_stream'])}\n")
+                f.write(f"{int(mset_settings['outlet_pts_right_stream'])}\n")
+                f.write(f"{int(mset_settings['num_streams_top'])}\n")
+                f.write(f"{int(mset_settings['num_streams_bot'])}\n")
+                f.write(f"{int(mset_settings['max_streams_between'])}\n")
+                f.write(f"{mset_settings['elliptic_param']}\n")
+                f.write(f"{mset_settings['stag_pt_aspect_ratio']}\n")
+                f.write(f"{mset_settings['x_spacing_param']}\n")
+                f.write(f"{mset_settings['alf0_stream_gen']}\n")
+
+                multi_airfoil_grid = mset_settings['multi_airfoil_grid']
+
+                for a in airfoil_name_order:
+                    f.write(f"{multi_airfoil_grid[a]['dsLE_dsAvg']} {multi_airfoil_grid[a]['dsTE_dsAvg']} "
+                            f"{multi_airfoil_grid[a]['curvature_exp']}\n")
+
+                for a in airfoil_name_order:
+                    f.write(f"{multi_airfoil_grid[a]['U_s_smax_min']} {multi_airfoil_grid[a]['U_s_smax_max']} "
+                            f"{multi_airfoil_grid[a]['L_s_smax_min']} {multi_airfoil_grid[a]['L_s_smax_max']} "
+                            f"{multi_airfoil_grid[a]['U_local_avg_spac_ratio']} {multi_airfoil_grid[a]['L_local_avg_spac_ratio']}\n")
+            break
+        except OSError:
+            time.sleep(0.01)
+            attempt += 1
 
     return gridpar_file
 
 
 def write_mses_file(name: str, base_folder: str, mses_settings: dict, airfoil_name_order: typing.List[str]):
     """
     Writes MSES flow parameters to a file
@@ -869,47 +925,55 @@
     elif F['inverse_side'] == 0:
         F['ISMOVE'] = 0
         F['ISPRES'] = 0
     else:
         F['ISMOVE'] = 2
         F['ISPRES'] = 2
 
-    with open(mses_file, 'w') as f:
-        if F['target'] == 'alfa':
-            global_constraint_target = 5  # Tell MSES to specify the angle of attack in degrees given by 'ALFIN'
-        elif F['target'] == 'Cl':
-            global_constraint_target = 6  # Tell MSES to target the lift coefficient specified by 'CLIFIN'
-        else:
-            raise ValueError('Invalid value for \'target\' (must be either \'alfa\' or \'Cl\')')
-
-        if not F['inverse_flag']:
-            f.write(f'3 4 5 7\n3 4 {global_constraint_target} 7\n')
-        else:
-            f.write(f'3 4 5 7 11 12\n3 4 {global_constraint_target} 7 11 12\n')
-
-        f.write(f"{F['MACHIN']} {F['CLIFIN']} {F['ALFAIN']}\n")
-        f.write(f"{int(F['ISMOM'])} {int(F['IFFBC'])}\n")
-        f.write(f"{F['REYNIN']} {F['ACRIT']}\n")
-
-        for idx, airfoil_name in enumerate(airfoil_name_order):
-            f.write(f"{F['XTRSupper'][airfoil_name]} {F['XTRSlower'][airfoil_name]}")
-            if idx == len(airfoil_name_order) - 1:
-                f.write("\n")
-            else:
-                f.write(" ")
-
-        f.write(f"{F['MCRIT']} {F['MUCON']}\n")
-
-        if any([bool(flag) for flag in F['AD_flags']]) or bool(F['inverse_flag']):
-            f.write(f"{int(F['ISMOVE'])} {int(F['ISPRES'])}\n")
-            f.write(f"{int(F['NMODN'])} {int(F['NPOSN'])}\n")
-
-        for idx, flag in enumerate(F['AD_flags']):
-            if bool(flag):
-                f.write(f"{int(F['ISDELH'][idx])} {F['XCDELH'][idx]} {F['PTRHIN'][idx]} {F['ETAH'][idx]}\n")
+    attempt = 0
+    max_attempts = 100
+    while attempt < max_attempts:
+        try:
+            with open(mses_file, 'w') as f:
+                if F['target'] == 'alfa':
+                    global_constraint_target = 5  # Tell MSES to specify the angle of attack in degrees given by 'ALFIN'
+                elif F['target'] == 'Cl':
+                    global_constraint_target = 6  # Tell MSES to target the lift coefficient specified by 'CLIFIN'
+                else:
+                    raise ValueError('Invalid value for \'target\' (must be either \'alfa\' or \'Cl\')')
+
+                if not F['inverse_flag']:
+                    f.write(f'3 4 5 7\n3 4 {global_constraint_target} 7\n')
+                else:
+                    f.write(f'3 4 5 7 11 12\n3 4 {global_constraint_target} 7 11 12\n')
+
+                f.write(f"{F['MACHIN']} {F['CLIFIN']} {F['ALFAIN']}\n")
+                f.write(f"{int(F['ISMOM'])} {int(F['IFFBC'])}\n")
+                f.write(f"{F['REYNIN']} {F['ACRIT']}\n")
+
+                for idx, airfoil_name in enumerate(airfoil_name_order):
+                    f.write(f"{F['XTRSupper'][airfoil_name]} {F['XTRSlower'][airfoil_name]}")
+                    if idx == len(airfoil_name_order) - 1:
+                        f.write("\n")
+                    else:
+                        f.write(" ")
+
+                f.write(f"{F['MCRIT']} {F['MUCON']}\n")
+
+                if any([bool(flag) for flag in F['AD_flags']]) or bool(F['inverse_flag']):
+                    f.write(f"{int(F['ISMOVE'])} {int(F['ISPRES'])}\n")
+                    f.write(f"{int(F['NMODN'])} {int(F['NPOSN'])}\n")
+
+                for idx, flag in enumerate(F['AD_flags']):
+                    if bool(flag):
+                        f.write(f"{int(F['ISDELH'][idx])} {F['XCDELH'][idx]} {F['PTRHIN'][idx]} {F['ETAH'][idx]}\n")
+            break
+        except OSError:
+            time.sleep(0.01)
+            attempt += 1
 
     mses_settings = F
 
     return mses_file, mses_settings
 
 
 def write_input_file(input_file: str, input_list: typing.List[str]):
@@ -921,18 +985,26 @@
     input_file: str
       File where inputs are written
 
     input_list: typing.List[str]
       List of inputs to write. For example, passing ``["1", "", "12", "13"]`` is equivalent to typing the command
       sequence ``1, RETURN, RETURN, 12, RETURN, 13, RETURN`` into the shell or terminal.
     """
-    with open(input_file, 'w') as f:
-        for input_ in input_list:
-            f.write(input_)
-            f.write('\n')
+    attempt = 0
+    max_attempts = 100
+    while attempt < max_attempts:
+        try:
+            with open(input_file, 'w') as f:
+                for input_ in input_list:
+                    f.write(input_)
+                    f.write('\n')
+            break
+        except OSError:
+            time.sleep(0.01)
+            attempt += 1
 
 
 def convert_xfoil_string_to_aero_data(line1: str, line2: str, aero_data: dict):
     """
     Extracts aerodynamic data from strings pulled from XFOIL log files. The two string inputs are the string outputs
     from ``pymead.analysis.read_aero_data.read_aero_data_from_xfoil``
 
@@ -1230,14 +1302,106 @@
     dl = np.cumsum(dl)
 
     # Integrate
     integral = np.trapz(integrand, dl)
     return integral
 
 
+def line_integral_Edota_inviscid_TP(rho: np.ndarray, u: np.ndarray, v: np.ndarray, x: np.ndarray, y: np.ndarray):
+    """
+    ... according to
+    Drela's "Power Balance in Aerodynamic Flows", a 2009 AIAA Journal article
+
+    Parameters
+    ==========
+    rho: np.ndarray
+        Node-centered density field
+
+    u: np.ndarray
+        Node-centered x-velocity field
+
+    v: np.ndarray
+        Node-centered y-velocity field
+
+    x: np.ndarray
+        1-d array of x-coordinates of the line along which to compute the line integral
+
+    y: np.ndarray
+        1-d array of y-coordinates of the line along which to compute the line integral
+    """
+    # Calculate the direction of n_hat
+    with np.errstate(divide="ignore", invalid="ignore"):
+        angle = np.arctan2(1, np.gradient(x, y))
+
+    perp_angle = -np.pi / 2
+    n_hat = np.column_stack((np.cos(angle + perp_angle), np.sin(angle + perp_angle)))
+    V_vec = np.column_stack((u, v))
+
+    # Compute the dot product V_vec * n_hat
+    dot_product = np.array([np.dot(V_vec_i, n_hat_i) for V_vec_i, n_hat_i in zip(V_vec, n_hat)])
+    u_perturb = dot_product.flatten() - 1
+    # print(f"{u_perturb = }")
+    integrand = rho * u_perturb ** 2 * (1 + u_perturb)
+
+    # Build the length increment vector (dl)
+    dl = np.array([0.0])
+    dl = np.append(dl, np.hypot(x[1:] - x[:-1], y[1:] - y[:-1]))  # compute incremental length along x and y
+    dl = np.cumsum(dl)
+
+    # Integrate
+    integral = np.trapz(integrand, dl)
+    return integral
+
+
+def line_integral_Edotp_inviscid_TP(Cp: np.ndarray, u: np.ndarray, v: np.ndarray, x: np.ndarray,
+                                    y: np.ndarray):
+    """
+    ... according to
+    Drela's "Power Balance in Aerodynamic Flows", a 2009 AIAA Journal article
+
+    Parameters
+    ==========
+    Cp: np.ndarray
+        Node-centered pressure coefficient field
+
+    u: np.ndarray
+        Node-centered x-velocity field
+
+    v: np.ndarray
+        Node-centered y-velocity field
+
+    x: np.ndarray
+        1-d array of x-coordinates of the line along which to compute the line integral
+
+    y: np.ndarray
+        1-d array of y-coordinates of the line along which to compute the line integral
+    """
+    # Calculate the direction of n_hat
+    with np.errstate(divide="ignore", invalid="ignore"):
+        angle = np.arctan2(1, np.gradient(x, y))
+
+    perp_angle = -np.pi / 2
+    n_hat = np.column_stack((np.cos(angle + perp_angle), np.sin(angle + perp_angle)))
+    V_vec = np.column_stack((u, v))
+
+    # Compute the dot product V_vec * n_hat
+    dot_product = np.array([np.dot(V_vec_i, n_hat_i) for V_vec_i, n_hat_i in zip(V_vec, n_hat)])
+    u_perturb = dot_product.flatten() - 1
+    integrand = Cp * u_perturb
+
+    # Build the length increment vector (dl)
+    dl = np.array([0.0])
+    dl = np.append(dl, np.hypot(x[1:] - x[:-1], y[1:] - y[:-1]))  # compute incremental length along x and y
+    dl = np.cumsum(dl)
+
+    # Integrate
+    integral = np.trapz(integrand, dl)
+    return integral
+
+
 def viscous_Edot(last_BL_point: typing.Dict[str, np.ndarray]):
     """
     Eq. (75) of Drela's Power Balance in Aerodynamic Flows in 2-D form
     """
     if any([k not in last_BL_point.keys() for k in ("rhoe/rhoinf", "Ue/Uinf", "theta", "theta*")]):
         raise ValueError(f"Missing a boundary layer key in the Edot calculation. {last_BL_point.keys() = }")
 
@@ -1562,15 +1726,15 @@
             rho = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                          field[flow_var_idx["rho"]][:, start_idx:end_idx])
             u = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                        field[flow_var_idx["u"]][:, start_idx:end_idx])
             v = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                        field[flow_var_idx["v"]][:, start_idx:end_idx])
             V = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
-                                                       field[flow_var_idx["q"]][:, start_idx:end_idx])
+                                                       field[flow_var_idx["V"]][:, start_idx:end_idx])
             M = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                        field[flow_var_idx["M"]][:, start_idx:end_idx])
 
             if calculate_capSS or calculate_exit_plane_Mach_array:
                 if capSS in [None, -1]:
                     capSS = -1
                     if np.any(M > 1.0):
@@ -1649,15 +1813,15 @@
     #     return CPK, capSS
     # else:
     #     return CPK
 
     return {"CPK": CPK, "capSS": capSS, "epma": epma}
 
 
-def calculate_CPK_power_consumption(analysis_subdir: str):
+def calculate_CPK_power_consumption_old(analysis_subdir: str):
     """
     A specialized function that calculates the mechanical flow power coefficient for an underwing trailing edge
     aero-propulsive configuration.
     """
     airfoil_system_name = os.path.split(analysis_subdir)[-1]
     field_file = os.path.join(analysis_subdir, f'field.{airfoil_system_name}')
     grid_stats_file = os.path.join(analysis_subdir, 'mplot_grid_stats.log')
@@ -1687,15 +1851,15 @@
         rho = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                      field[flow_var_idx["rho"]][:, start_idx:end_idx])
         u = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                    field[flow_var_idx["u"]][:, start_idx:end_idx])
         v = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
                                                    field[flow_var_idx["v"]][:, start_idx:end_idx])
         V = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
-                                                   field[flow_var_idx["q"]][:, start_idx:end_idx])
+                                                   field[flow_var_idx["V"]][:, start_idx:end_idx])
         x = x_grid[flow_section_idx]
         y = y_grid[flow_section_idx]
 
         # Integrate over the propulsor outlet for the given flow section
 
         outlet_integral = line_integral_Edot_inviscid(Cp[-1, :], rho[-1, :], u[-1, :], v[-1, :], V[-1, :], x[-1, :],
                                              y[-1, :], n_hat_dir="right")
@@ -1737,15 +1901,15 @@
         for side in bl_data:
             for k in ("rhoe/rhoinf", "Ue/Uinf", "theta", "theta*", "K"):
                 if k not in last_BL_point.keys():
                     last_BL_point[k] = []
                 val = side[k][last_point_idx]
                 if val <= 1e-12 and k == "K":
                     end_point_counter += 1
-                    print(f"Decrementing last_point_idx...")
+                    # print(f"Decrementing last_point_idx...")
                     last_point_idx -= 1
                     continue
                 last_BL_point[k].append(val)
 
         for k, v in last_BL_point.items():
             last_BL_point[k] = np.array(v)
         break
@@ -1783,20 +1947,131 @@
     #     return CPK, capSS
     # else:
     #     return CPK
 
     return {"CPK": CPK, "Edot": Edot, "diss_surf": surface_diss, "diss_shock": shock_diss, "Cd": forces["Cd"]}
 
 
+def calculate_CPK_power_consumption(analysis_subdir: str):
+    """
+    A specialized function that calculates the mechanical flow power coefficient
+    """
+    airfoil_system_name = os.path.split(analysis_subdir)[-1]
+    field_file = os.path.join(analysis_subdir, f'field.{airfoil_system_name}')
+    grid_stats_file = os.path.join(analysis_subdir, 'mplot_grid_stats.log')
+    grid_file = os.path.join(analysis_subdir, f'grid.{airfoil_system_name}')
+    blade_file = os.path.join(analysis_subdir, f"blade.{airfoil_system_name}")
+    bl_file = os.path.join(analysis_subdir, f"bl.{airfoil_system_name}")
+    mses_file = os.path.join(analysis_subdir, f"mses.{airfoil_system_name}")
+    mses_log_file = os.path.join(analysis_subdir, "mses.log")
+    coords = convert_blade_file_to_3d_array(blade_file)
+    mplot_log_file = os.path.join(analysis_subdir, "mplot.log")
+
+    M_inf = read_Mach_from_mses_file(mses_file)
+    gam = 1.4  # Hard-coded specific heat ratio
+    forces = read_forces_from_mses(mplot_log_file)
+    field = read_field_from_mses(field_file, M_inf=M_inf, gam=gam)
+    bl_data = read_bl_data_from_mses(bl_file)
+    grid_stats = read_grid_stats_from_mses(grid_stats_file)
+    x_grid, y_grid = read_streamline_grid_from_mses(grid_file, grid_stats)
+
+    Edot = 0.0
+    Edota = 0.0
+    Edotp = 0.0
+
+    start_idx, end_idx = 0, x_grid[0].shape[1] - 1
+
+    for flow_section_idx in range(grid_stats["numel"] + 1):
+        Cp = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
+                                                   field[flow_var_idx["Cp"]][:, start_idx:end_idx])
+        rho = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
+                                                     field[flow_var_idx["rho"]][:, start_idx:end_idx])
+        u = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
+                                                   field[flow_var_idx["u"]][:, start_idx:end_idx])
+        v = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
+                                                   field[flow_var_idx["v"]][:, start_idx:end_idx])
+        V = convert_cell_centered_to_edge_centered(x_grid[flow_section_idx].shape,
+                                                   field[flow_var_idx["V"]][:, start_idx:end_idx])
+        x = x_grid[flow_section_idx]
+        y = y_grid[flow_section_idx]
+
+        # Integrate over the propulsor outlet for the given flow section
+
+        # outlet_integral = line_integral_Edot_inviscid(Cp[-1, :], rho[-1, :], u[-1, :], v[-1, :], V[-1, :], x[-1, :],
+        #                                      y[-1, :], n_hat_dir="right")
+        #
+        # Edot += outlet_integral
+
+        Edota += line_integral_Edota_inviscid_TP(rho[-1, :], u[-1, :], v[-1, :], x[-1, :], y[-1, :])
+        Edotp += line_integral_Edotp_inviscid_TP(Cp[-1, :], u[-1, :], v[-1, :], x[-1, :], y[-1, :])
+        # print(f"{Edota = }, {Edotp = }, {np.mean(rho[-1, :]) = }, {np.max(rho[-1, :]) = }, {np.min(rho[-1, :]) = }")
+        # print(f"{np.mean(Cp[-1, :]) = }, {np.max(Cp[-1, :]) = }, {np.min(Cp[-1, :]) = }")
+        # print(f"{np.mean(u[-1, :]) = }, {np.max(u[-1, :]) = }, {np.min(u[-1, :]) = }")
+        # print(f"{np.mean(v[-1, :]) = }, {np.max(v[-1, :]) = }, {np.min(v[-1, :]) = }")
+        # print(f"{np.mean(x[-1, :]) = }, {np.max(x[-1, :]) = }, {np.min(x[-1, :]) = }")
+        # print(f"{np.mean(y[-1, :]) = }, {np.max(y[-1, :]) = }, {np.min(y[-1, :]) = }")
+
+        if flow_section_idx < grid_stats["numel"]:
+            start_idx = end_idx
+            end_idx += x_grid[flow_section_idx + 1].shape[1] - 1
+
+    end_point_counter = 0
+    last_point_idx = -1
+    max_end_point_attempts = 10
+
+    while True:
+        if end_point_counter > max_end_point_attempts:
+            raise ValueError("Reached maximum attempts for setting the boundary layer end point.")
+
+        last_BL_point = {}
+        for side in bl_data:
+            for k in ("rhoe/rhoinf", "Ue/Uinf", "theta", "theta*", "K"):
+                if k not in last_BL_point.keys():
+                    last_BL_point[k] = []
+                val = side[k][last_point_idx]
+                if val <= 1e-12 and k == "K":
+                    end_point_counter += 1
+                    # print(f"Decrementing last_point_idx...")
+                    last_point_idx -= 1
+                    continue
+                last_BL_point[k].append(val)
+
+        for k, v in last_BL_point.items():
+            last_BL_point[k] = np.array(v)
+        break
+
+    Edota_visc = viscous_Edot(last_BL_point=last_BL_point)
+
+    Edota += Edota_visc
+
+    # TODO: need to find a way to add the pressure component from the boundary layer region (Edotp_visc)
+
+    surface_diss = surface_dissipation(last_BL_point=last_BL_point)
+
+    shock_diss = shock_dissipation(x_edge=x_grid, y_edge=y_grid, u=field[flow_var_idx["u"]][:, :],
+                                   v=field[flow_var_idx["v"]][:, :], M=field[flow_var_idx["M"]][:, :],
+                                   Cpt=field[flow_var_idx["Cpt"]][:, :], dCpt=field[flow_var_idx["dCpt"]][:, :],
+                                   dCp=field[flow_var_idx["dCp"]][:, :], gam=gam)
+
+    # CPK = Edot + surface_diss + shock_diss - forces["Cd"]
+    CPK = Edota + Edotp + surface_diss + shock_diss - forces["Cd"]
+
+    if np.isnan(CPK):
+        CPK = 1e9
+
+    return {"CPK": CPK, "Edota": Edota, "Edotp": Edotp, "diss_surf": surface_diss, "diss_shock": shock_diss,
+            "Cd": forces["Cd"]}
+
+
 def calculate_CPK_mses_inviscid_only(analysis_subdir: str):
     """
     Calculates the mechanical flower power coefficient input to the control volume across the airfoil system control
     surface. Assumes that the control surface wraps just around the actuator disk and that the normal vectors point
-    into the propulsor. Also assumes that there is no change in the kinetic defect across the actuator disk (and thus
-    no change in CPK due to the boundary layer).
+    into the propulsor. Also assumes that there is no change in the kinetic energy defect across the actuator disk
+    (and thus no change in CPK due to the boundary layer).
     """
 
     airfoil_system_name = os.path.split(analysis_subdir)[-1]
     field_file = os.path.join(analysis_subdir, f'field.{airfoil_system_name}')
     grid_stats_file = os.path.join(analysis_subdir, 'mplot_grid_stats.log')
     grid_file = os.path.join(analysis_subdir, f'grid.{airfoil_system_name}')
     mses_log_file = os.path.join(analysis_subdir, "mses.log")
@@ -1813,16 +2088,16 @@
         Cp_down = field[flow_var_idx["Cp"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         rho_up = field[flow_var_idx["rho"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         rho_down = field[flow_var_idx["rho"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         u_up = field[flow_var_idx["u"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         u_down = field[flow_var_idx["u"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         v_up = field[flow_var_idx["v"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         v_down = field[flow_var_idx["v"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
-        V_up = field[flow_var_idx["q"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
-        V_down = field[flow_var_idx["q"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
+        V_up = field[flow_var_idx["V"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
+        V_down = field[flow_var_idx["V"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         x = x_grid[data["flow_section_idx"]][data["field_i_up"]:data["field_i_up"] + 3, :]
         y = y_grid[data["flow_section_idx"]][data["field_i_up"]:data["field_i_up"] + 3, :]
         CPK += line_integral_CPK_inviscid(Cp_up, Cp_down, rho_up, rho_down, u_up, u_down,
                                           v_up, v_down, V_up, V_down, x, y)
 
     if np.isnan(CPK):
         CPK = 1e9
@@ -1858,16 +2133,16 @@
         Cp_down = field[flow_var_idx["Cp"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         rho_up = field[flow_var_idx["rho"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         rho_down = field[flow_var_idx["rho"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         u_up = field[flow_var_idx["u"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         u_down = field[flow_var_idx["u"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         v_up = field[flow_var_idx["v"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
         v_down = field[flow_var_idx["v"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
-        V_up = field[flow_var_idx["q"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
-        V_down = field[flow_var_idx["q"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
+        V_up = field[flow_var_idx["V"]][data["field_i_up"], data["field_j_start"]:data["field_j_end"] + 1]
+        V_down = field[flow_var_idx["V"]][data["field_i_down"], data["field_j_start"]:data["field_j_end"] + 1]
         x = x_grid[data["flow_section_idx"]][data["field_i_up"]:data["field_i_up"] + 3, :]
         y = y_grid[data["flow_section_idx"]][data["field_i_up"]:data["field_i_up"] + 3, :]
         CPK += line_integral_CPK_inviscid(Cp_up, Cp_down, rho_up, rho_down, u_up, u_down,
                                           v_up, v_down, V_up, V_down, x, y)
 
         # Calculate the bounding boundary layer sides corresponding to the given flow section index
         n_airfoils = len(x_grid) - 1
```

### Comparing `pymead-2.0.0b3/pymead/analysis/cfd_output_templates.py` & `pymead-2.0.0b4/pymead/analysis/cfd_output_templates.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/analysis/compressible_flow.py` & `pymead-2.0.0b4/pymead/analysis/compressible_flow.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/analysis/read_aero_data.py` & `pymead-2.0.0b4/pymead/analysis/read_aero_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import typing
 
 import pandas as pd
 import numpy as np
 
 
-flow_var_idx = {'M': 7, 'Cp': 8, 'p': 3, 'rho': 2, 'u': 4, 'v': 5, 'q': 6, "Cpt": 9, "dCpt": 10, "dCp": 11}
+flow_var_idx = {"M": 7, "Cp": 8, "p": 3, "rho": 2, "u": 4, "v": 5, "V": 6, "Cpt": 9, "dCpt": 10, "dCp": 11}
 
 
 def read_Cp_from_file_xfoil(fname: str):
     """
     Reads the :math:`C_p` data from the format output by XFOIL and converts it to a *numpy* array
 
     Parameters
@@ -353,15 +353,15 @@
 
     * 0: :math:`x`
     * 1: :math:`y`
     * 2: :math:`\rho/\rho_\infty` (density)
     * 3: :math:`p/p_\infty` (pressure)
     * 4: :math:`u/V_\infty` (:math:`x`-velocity)
     * 5: :math:`v/V_\infty` (:math:`y`-velocity)
-    * 6: :math:`q/V_\infty` (velocity magnitude)
+    * 6: :math:`|V|/V_\infty` (velocity magnitude)
     * 7: :math:`M` (Mach number)
     * 8: :math:`C_p` (pressure coefficient)
     * 9: :math:`C_{p_t}` (total pressure coefficient)
     * 10: :math:`\Delta C_{p_t}` (change in total pressure coefficient relative to the previous streamwise cell)
     * 11: :math:`\Delta C_p` (change in pressure coefficient relative to the previous streamwise cell)
 
     Note that for :math:`\Delta C_{p_t}` and :math:`\Delta C_p`, the value of the first streamwise cells (the cells
```

### Comparing `pymead-2.0.0b3/pymead/analysis/single_element_inviscid.py` & `pymead-2.0.0b4/pymead/analysis/single_element_inviscid.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/analysis/utils.py` & `pymead-2.0.0b4/pymead/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/core/airfoil.py` & `pymead-2.0.0b4/pymead/core/airfoil.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,14 +278,56 @@
             rotation_units="rad",
             order="t,s,r"
         )
 
         coords = self.get_coords_selig_format(max_airfoil_points, curvature_exp) if coords is None else coords
         return transformation.transform(coords)
 
+    def get_scaled_coords(self, coords: np.ndarray = None, max_airfoil_points: int = None,
+                                curvature_exp: float = 2.0) -> np.ndarray:
+        """
+        Gets the chord-relative values of the airfoil coordinates. The airfoil is transformed such that the leading
+        edge is at :math:`(0,0)` and the trailing edge is at :math:`(1,0)`.
+
+        Parameters
+        ----------
+        coords: np.ndarray or None
+            Optional Selig format airfoil coordinates (only specified if computational speed is important).
+            If the coordinates are not specified, they are calculated.
+
+        max_airfoil_points: int
+            Optional value specifying the maximum number of airfoil points. If this value is left as ``None``,
+            no downsampling will be performed. Default: ``None``
+
+        curvature_exp: float
+            Optional value specifying the curvature exponent used in the ``downsample`` method. If
+            ``max_airfoil_points`` is left as ``None``, this value will be ignored. Default: 2
+
+        Returns
+        -------
+        np.ndarray
+            An :math:`N \times 2` array of transformed airfoil coordinates
+        """
+        # Get the chord length and angle of attack
+        chord_length = self.measure_chord()
+
+        # Get the transformation object
+        transformation = Transformation2D(
+            tx=[0.0],
+            ty=[0.0],
+            r=[0.0],
+            sx=[1 / chord_length],
+            sy=[1 / chord_length],
+            rotation_units="rad",
+            order="t,s,r"
+        )
+
+        coords = self.get_coords_selig_format(max_airfoil_points, curvature_exp) if coords is None else coords
+        return transformation.transform(coords)
+
     @staticmethod
     def convert_coords_to_shapely_format(coords: np.ndarray) -> typing.List[tuple]:
         r"""
         Converts a set of airfoil coordinates to the ``shapely`` native data format (list of tuples).
 
         Parameters
         ----------
```

### Comparing `pymead-2.0.0b3/pymead/core/bezier.py` & `pymead-2.0.0b4/pymead/core/bezier.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pymead.core.parametric_curve import ParametricCurve, PCurveData
 from pymead.core.point import PointSequence, Point
 from pymead.utils.nchoosek import nchoosek
 
 
 class Bezier(ParametricCurve):
 
-    def __init__(self, point_sequence: PointSequence, name: str or None = None, **kwargs):
+    def __init__(self, point_sequence: PointSequence, name: str or None = None, t_start: float = None,
+                 t_end: float = None, **kwargs):
         r"""
         Computes the Bézier curve through the control points ``P`` according to
 
         .. math::
 
             \vec{C}(t)=\sum_{i=0}^n \vec{P}_i B_{i,n}(t)
 
@@ -59,43 +60,34 @@
         line passing through :math:`P_0` and :math:`P_1`. Similarly, the local slope at :math:`P_3` is equal to
         the slope of the line passing through :math:`P_2` and :math:`P_3`. These properties of Bézier curves allow us to
         easily enforce :math:`G^0` and :math:`G^1` continuity at Bézier curve "joints" (common endpoints of
         connected Bézier curves).
 
         Parameters
         ==========
-        P: numpy.ndarray
-          Array of ``shape=(n+1, 2)``, where ``n`` is the degree of the Bézier curve and ``n+1`` is
-          the number of control points in the Bézier curve. The two columns represent the :math:`x`-
-          and :math:`y`-components of the control points.
-
-        nt: int
-          The number of points in the :math:`t` vector (defines the resolution of the curve). Default: ``100``.
-
-        t: numpy.ndarray
-          Parameter vector describing where the Bézier curve should be evaluated. This vector should be a 1-D array
-          beginning and should monotonically increase from 0 to 1. If not specified, ``numpy.linspace(0, 1, nt)`` will
-          be used.
+        point_sequence: PointSequence
+            Sequence of points defining the control points for the Bézier curve
 
-        Returns
-        =======
-        dict
-            A dictionary of ``numpy`` arrays of ``shape=nt`` containing information related to the created Bézier curve:
-
-            .. math::
+        name: str or ``None``
+            Optional name for the curve. Default: ``None``
 
-                C_x(t), C_y(t), C'_x(t), C'_y(t), C''_x(t), C''_y(t), \kappa(t)
-
-            where the :math:`x` and :math:`y` subscripts represent the :math:`x` and :math:`y` components of the
-            vector-valued functions :math:`\vec{C}(t)`, :math:`\vec{C}'(t)`, and :math:`\vec{C}''(t)`.
+        t_start: float or ``None``
+            Optional starting parameter vector value for the Bézier curve. Not specifying this value automatically
+            gives a value of ``0.0``. Default: ``None``
+
+        t_end: float or ``None``
+            Optional ending parameter vector value for the Bézier curve. Not specifying this value automatically
+            gives a value of ``1.0``. Default: ``None``
         """
         super().__init__(sub_container="bezier", **kwargs)
         self._point_sequence = None
         self.degree = None
         self.set_point_sequence(point_sequence)
+        self.t_start = t_start
+        self.t_end = t_end
         name = "Bezier-1" if name is None else name
         self.set_name(name)
         self.curve_connections = []
         self._add_references()
 
     def _add_references(self):
         for idx, point in enumerate(self.point_sequence().points()):
@@ -199,68 +191,110 @@
                 return finite_diff_recursive(_k - 1, _i + 1) - finite_diff_recursive(_k - 1, _i)
             else:
                 return P[_i + 1, :] - P[_i, :]
 
         return finite_diff_recursive(k, i)
 
     def derivative(self, P: np.ndarray, t: np.ndarray, degree: int, order: int):
-        """
+        r"""
         Calculates an arbitrary-order derivative of the Bézier curve
 
         Parameters
         ==========
         P: np.ndarray
             The control point array
 
         t: np.ndarray
             The parameter vector
 
         degree: int
             The degree of the Bézier curve
 
         order: int
-          The derivative order. For example, ``order=2`` returns the second derivative.
+            The derivative order. For example, ``order=2`` returns the second derivative.
 
         Returns
         =======
         np.ndarray
-          An array of ``shape=(N,2)`` where ``N`` is the number of evaluated points specified by the :math:`t` vector.
-          The columns represent :math:`C^{(m)}_x(t)` and :math:`C^{(m)}_y(t)`, where :math:`m` is the
-          derivative order.
+            An array of ``shape=(N,2)`` where ``N`` is the number of evaluated points specified by the :math:`t` vector.
+            The columns represent :math:`C^{(m)}_x(t)` and :math:`C^{(m)}_y(t)`, where :math:`m` is the
+            derivative order.
         """
         return np.sum(np.array([np.prod(np.array([degree - idx for idx in range(order)])) *
                                 np.array([self.finite_diff_P(P, order, i)]).T *
                                 np.array([self.bernstein_poly(degree - order, i, t)])
                                 for i in range(degree + 1 - order)]), axis=0).T
 
     def evaluate(self, t: np.array or None = None, **kwargs):
+        r"""
+        Evaluates the curve using an optionally specified parameter vector.
+
+        Parameters
+        ==========
+        t: np.ndarray or ``None``
+            Optional direct specification of the parameter vector for the curve. Not specifying this value
+            gives a linearly spaced parameter vector from ``t_start`` or ``t_end`` with the default size.
+            Default: ``None``
+
+        Returns
+        =======
+        PCurveData
+            Data class specifying the following information about the Bézier curve:
+
+            .. math::
+
+                    C_x(t), C_y(t), C'_x(t), C'_y(t), C''_x(t), C''_y(t), \kappa(t)
+
+            where the :math:`x` and :math:`y` subscripts represent the :math:`x` and :math:`y` components of the
+            vector-valued functions :math:`\vec{C}(t)`, :math:`\vec{C}'(t)`, and :math:`\vec{C}''(t)`.
+        """
+        # Pass the starting and ending parameter vector values to the parameter vector generator if they were
+        # specified directly
+        if self.t_start is not None:
+            kwargs["start"] = self.t_start
+        if self.t_end is not None:
+            kwargs["end"] = self.t_end
+
+        # Generate the parameter vector
         t = ParametricCurve.generate_t_vec(**kwargs) if t is None else t
+
+        # Number of control points, curve degree, control point array
         n_ctrl_points = len(self.point_sequence())
         degree = n_ctrl_points - 1
         P = self.point_sequence().as_array()
+
+        # Evaluate the curve
         x, y = np.zeros(t.shape), np.zeros(t.shape)
         for i in range(n_ctrl_points):
             # Calculate the x- and y-coordinates of the Bézier curve given the input vector t
             x += P[i, 0] * self.bernstein_poly(degree, i, t)
             y += P[i, 1] * self.bernstein_poly(degree, i, t)
         xy = np.column_stack((x, y))
 
+        # Calculate the first derivative
         first_deriv = self.derivative(P=P, t=t, degree=degree, order=1)
         xp = first_deriv[:, 0]
         yp = first_deriv[:, 1]
+
+        # Calculate the second derivative
         second_deriv = self.derivative(P=P, t=t, degree=degree, order=2)
         xpp = second_deriv[:, 0]
         ypp = second_deriv[:, 1]
+
+        # Combine the derivative x and y data
         xpyp = np.column_stack((xp, yp))
         xppypp = np.column_stack((xpp, ypp))
 
+        # Calculate the curvature
         with np.errstate(divide='ignore', invalid='ignore'):
             # Calculate the curvature of the Bézier curve (k = kappa = 1 / R, where R is the radius of curvature)
             k = np.true_divide((xp * ypp - yp * xpp), (xp ** 2 + yp ** 2) ** (3 / 2))
 
+        # Calculate the radius of curvature: R = 1 / kappa
         with np.errstate(divide='ignore', invalid='ignore'):
             R = np.true_divide(1, k)
 
         return PCurveData(t=t, xy=xy, xpyp=xpyp, xppypp=xppypp, k=k, R=R)
 
     def get_dict_rep(self):
-        return {"points": [pt.name() for pt in self.point_sequence().points()]}
+        return {"points": [pt.name() for pt in self.point_sequence().points()],
+                "t_start": self.t_start, "t_end": self.t_end}
```

### Comparing `pymead-2.0.0b3/pymead/core/constraint_equations.py` & `pymead-2.0.0b4/pymead/core/constraint_equations.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,23 @@
 def measure_radius_of_curvature_bezier(Lt: float, Lc: float, n: int, psi: float):
     return np.abs(np.true_divide(Lt ** 2, Lc * (1 - 1 / n) * np.sin(psi)))
 
 
 def measure_curvature_length_bezier(x1: float, y1: float, x2: float, y2: float, x3: float, y3: float, R: float, n: int):
     Lt = measure_distance(x1, y1, x2, y2)
     psi = measure_rel_angle3(x1, y1, x2, y2, x3, y3)
-    Lc = np.abs(np.true_divide(Lt ** 2, R * (1 - 1 / n) * np.sin(psi)))
+    with np.errstate(divide="ignore"):
+        Lc = np.abs(np.true_divide(Lt ** 2, R * (1 - 1 / n) * np.sin(psi)))
     return Lc
 
 
 def measure_curvature_bezier(Lt: float, Lc: float, n: int, psi: float):
-    return np.abs(np.true_divide(Lc * (1 - 1 / n) * np.sin(psi), Lt ** 2))
+    with np.errstate(divide="ignore"):
+        kappa = np.abs(np.true_divide(Lc * (1 - 1 / n) * np.sin(psi), Lt ** 2))
+    return kappa
 
 
 def measure_data_bezier_curve_joint(xy: np.ndarray, n: np.ndarray):
     phi1 = measure_abs_angle(xy[2, 0], xy[2, 1], xy[1, 0], xy[1, 1])
     phi2 = measure_abs_angle(xy[2, 0], xy[2, 1], xy[3, 0], xy[3, 1])
     theta1 = measure_abs_angle(xy[1, 0], xy[1, 1], xy[0, 0], xy[0, 1])
     theta2 = measure_abs_angle(xy[3, 0], xy[3, 1], xy[4, 0], xy[4, 1])
@@ -78,16 +81,17 @@
     phi_rel = (phi1 - phi2) % (2 * np.pi)
     Lt1 = measure_distance(xy[1, 0], xy[1, 1], xy[2, 0], xy[2, 1])
     Lt2 = measure_distance(xy[2, 0], xy[2, 1], xy[3, 0], xy[3, 1])
     Lc1 = measure_distance(xy[0, 0], xy[0, 1], xy[1, 0], xy[1, 1])
     Lc2 = measure_distance(xy[3, 0], xy[3, 1], xy[4, 0], xy[4, 1])
     kappa1 = measure_curvature_bezier(Lt1, Lc1, n[0], psi1)
     kappa2 = measure_curvature_bezier(Lt2, Lc2, n[1], psi2)
-    R1 = np.true_divide(1, kappa1)
-    R2 = np.true_divide(1, kappa2)
+    with np.errstate(divide="ignore"):
+        R1 = np.true_divide(1, kappa1)
+        R2 = np.true_divide(1, kappa2)
     n1 = n[0]
     n2 = n[1]
     field_names = ["phi1", "phi2", "theta1", "theta2", "psi1", "psi2", "phi_rel", "Lt1", "Lt2", "Lc1", "Lc2",
                    "kappa1", "kappa2", "R1", "R2", "n1", "n2"]
     BezierCurveJointData = namedtuple("BezierCurveJointData", field_names=field_names)
     data = BezierCurveJointData(phi1=phi1, phi2=phi2, theta1=theta1, theta2=theta2, psi1=psi1, psi2=psi2,
                                 phi_rel=phi_rel, Lt1=Lt1, Lt2=Lt2, Lc1=Lc1, Lc2=Lc2, kappa1=kappa1, kappa2=kappa2,
```

### Comparing `pymead-2.0.0b3/pymead/core/constraints.py` & `pymead-2.0.0b4/pymead/core/constraints.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 from dataclasses import dataclass
+from abc import abstractmethod
 
 import numpy as np
 
-from pymead.core.constraint_equations import measure_rel_angle3
+from pymead.core.constraint_equations import measure_rel_angle3, measure_point_line_distance_unsigned
 from pymead.core.line import PolyLine
 from pymead.core.param import Param, AngleParam, LengthParam
 from pymead.core.point import Point
 from pymead.core.pymead_obj import PymeadObj
 
 
 class GeoCon(PymeadObj):
@@ -48,14 +49,18 @@
     def remove_constraint_from_points(self):
         for child_node in self.child_nodes:
             if not isinstance(child_node, Point) or self not in child_node.geo_cons:
                 return
 
             child_node.geo_cons.remove(self)
 
+    @abstractmethod
+    def verify(self) -> bool:
+        pass
+
 
 class DistanceConstraint(GeoCon):
 
     default_name = "DistCon-1"
 
     def __init__(self, p1: Point, p2: Point, value: float or LengthParam = None, name: str = None):
         self.p1 = p1
@@ -67,14 +72,18 @@
     def __repr__(self):
         return f"{self.__class__.__name__} {self.name()}<v={self.param().value()}>"
 
     def get_dict_rep(self) -> dict:
         return {"p1": self.p1.name(), "p2": self.p2.name(), "value": self.param().name(),
                 "constraint_type": self.__class__.__name__}
 
+    def verify(self) -> bool:
+        measured_distance = self.p1.measure_distance(self.p2)
+        return np.isclose(measured_distance, self.param().value(), rtol=1e-14)
+
 
 class AntiParallel3Constraint(GeoCon):
 
     default_name = "AntiPar3Con-1"
 
     def __init__(self, p1: Point, p2: Point, p3: Point, name: str = None, polyline: PolyLine = None,
                  point_on_curve: Point = None):
@@ -94,33 +103,69 @@
 
     def get_dict_rep(self) -> dict:
         return {"p1": self.p1.name(), "p2": self.p2.name(), "p3": self.p3.name(),
                 "constraint_type": self.__class__.__name__,
                 "polyline": self.polyline.name() if self.polyline is not None else None,
                 "point_on_curve": self.point_on_curve.name() if self.point_on_curve is not None else None}
 
+    def verify(self) -> bool:
+        a1 = self.p2.measure_angle(self.p1)
+        a2 = self.p2.measure_angle(self.p3)
+        measured_angle = (a1 - a2) % (2 * np.pi)
+        return np.isclose(measured_angle, np.pi, rtol=1e-14)
+
 
 class SymmetryConstraint(GeoCon):
 
     default_name = "SymCon-1"
 
     def __init__(self, p1: Point, p2: Point, p3: Point, p4: Point, name: str = None):
-        self.p1 = p1
-        self.p2 = p2
-        self.p3 = p3
-        self.p4 = p4
+        self.p1 = p1  # Line start point
+        self.p2 = p2  # Line end point
+        self.p3 = p3  # Tool point
+        self.p4 = p4  # Target point
         super().__init__(param=None, name=name, child_nodes=[self.p1, self.p2, self.p3, self.p4], kind="a4|d")
 
+    @staticmethod
+    def check_if_point_is_symmetric_target(p: Point):
+        for geo_con in p.geo_cons:
+            if isinstance(geo_con, SymmetryConstraint) and geo_con.child_nodes[-1] is p:
+                return True
+        return False
+
     def __repr__(self):
         return f"{self.__class__.__name__} {self.name()}"
 
     def get_dict_rep(self) -> dict:
         return {"p1": self.p1.name(), "p2": self.p2.name(), "p3": self.p3.name(), "p4": self.p4.name(),
                 "constraint_type": self.__class__.__name__}
 
+    def verify(self) -> bool:
+        tool_angle = measure_rel_angle3(self.p3.x().value(), self.p3.y().value(),
+                                        self.p2.x().value(), self.p2.y().value(),
+                                        self.p1.x().value(), self.p1.y().value())
+        target_angle = measure_rel_angle3(self.p1.x().value(), self.p1.y().value(),
+                                          self.p2.x().value(), self.p2.y().value(),
+                                          self.p4.x().value(), self.p4.y().value())
+        if not np.isclose(tool_angle, target_angle, rtol=1e-14):
+            return False
+
+        tool_distance_to_line = measure_point_line_distance_unsigned(
+            self.p1.x().value(), self.p1.y().value(),
+            self.p2.x().value(), self.p2.y().value(),
+            self.p3.x().value(), self.p3.y().value()
+        )
+        target_distance_to_line = measure_point_line_distance_unsigned(
+            self.p1.x().value(), self.p1.y().value(),
+            self.p2.x().value(), self.p2.y().value(),
+            self.p4.x().value(), self.p4.y().value()
+        )
+
+        return np.isclose(tool_distance_to_line, target_distance_to_line, rtol=1e-14)
+
 
 class Perp3Constraint(GeoCon):
 
     default_name = "Perp3Con-1"
 
     def __init__(self, p1: Point, p2: Point, p3: Point, name: str = None):
         self.p1 = p1
@@ -131,14 +176,20 @@
     def __repr__(self):
         return f"{self.__class__.__name__} {self.name()}"
 
     def get_dict_rep(self) -> dict:
         return {"p1": self.p1.name(), "p2": self.p2.name(), "p3": self.p3.name(),
                 "constraint_type": self.__class__.__name__}
 
+    def verify(self) -> bool:
+        a1 = self.p2.measure_angle(self.p1)
+        a2 = self.p2.measure_angle(self.p3)
+        measured_angle = (a1 - a2) % (2 * np.pi)
+        return np.isclose(measured_angle, 0.5 * np.pi, rtol=1e-14)
+
 
 class RelAngle3Constraint(GeoCon):
 
     default_name = "RelAng3Con-1"
 
     def __init__(self, p1: Point, p2: Point, p3: Point, value: float or AngleParam = None, name: str = None):
         self.p1 = p1
@@ -156,14 +207,20 @@
         return f"{self.__class__.__name__} {self.name()}<v={self.param().value()}>"
 
     def get_dict_rep(self) -> dict:
         return {"p1": self.p1.name(), "p2": self.p2.name(),
                 "p3": self.p3.name(), "value": self.param().name(),
                 "constraint_type": self.__class__.__name__}
 
+    def verify(self) -> bool:
+        a1 = self.p2.measure_angle(self.p1)
+        a2 = self.p2.measure_angle(self.p3)
+        measured_angle = (a1 - a2) % (2 * np.pi)
+        return np.isclose(measured_angle, self.param().rad(), rtol=1e-14)
+
 
 @dataclass
 class CurvatureConstraintData:
     Lt1: float
     Lt2: float
     Lc1: float
     Lc2: float
@@ -225,38 +282,53 @@
 
         secondary_params = []
         if self.curve_type_1 == "Bezier":
             secondary_params.append(Param(self.curve_1.degree, "n"))
         if self.curve_type_2 == "Bezier":
             secondary_params.append(Param(self.curve_2.degree, "n"))
 
+        if self.curve_type_1 == "PolyLine" and self.curve_type_2 == "PolyLine":
+            raise ValueError("Cannot create radius of curvature constraint between two polylines")
+
         if self.curve_type_1 == "LineSegment" or self.curve_type_2 == "LineSegment":
             param = None
-        elif self.curve_type_1 == "PolyLine":
+        elif self.curve_type_1 == "PolyLine" or (self.curve_type_1 == "Bezier" and (
+                self.curve_1.t_start is not None or self.curve_1.t_end is not None)):
             data = self.curve_1.evaluate()
             if (np.isclose(data.xy[0, 0], self.curve_joint.x().value()) and
                 np.isclose(data.xy[0, 1], self.curve_joint.y().value())):
                 R = data.R[0]
             else:
                 R = data.R[-1]
 
             param = LengthParam(value=R, name="ROC-1", enabled=False) if not isinstance(value, Param) else value
-        elif self.curve_type_2 == "PolyLine":
+        elif self.curve_type_2 == "PolyLine" or (self.curve_type_2 == "Bezier" and (
+                self.curve_2.t_start is not None or self.curve_2.t_end is not None)):
             data = self.curve_2.evaluate()
             if (np.isclose(data.xy[0, 0], self.curve_joint.x().value()) and
                     np.isclose(data.xy[0, 1], self.curve_joint.y().value())):
                 R = data.R[0]
             else:
                 R = data.R[-1]
             param = LengthParam(value=R, name="ROC-1", enabled=False) if not isinstance(value, Param) else value
         else:
+            enabled = True
             if value is None:
                 curvature_data = self.calculate_curvature_data(self.curve_joint)
-                value = 0.5 * (curvature_data.R1 + curvature_data.R2)
+
+                if not self.is_solving_allowed(self.g2_point_curve_1):
+                    value = curvature_data.R1
+                    enabled = False
+                elif not self.is_solving_allowed(self.g2_point_curve_2):
+                    value = curvature_data.R2
+                    enabled = False
+                else:
+                    value = 0.5 * (curvature_data.R1 + curvature_data.R2)
             param = value if isinstance(value, Param) else LengthParam(value=value, name="ROC-1")
+            param.set_enabled(enabled)
 
         super().__init__(param=param, child_nodes=points, kind="d", name=name,
                          secondary_params=secondary_params)
 
     @staticmethod
     def calculate_curvature_data(curve_joint):
         curve_1 = curve_joint.curves[0]
@@ -310,22 +382,35 @@
             else:
                 R2 = data.R[-1]
 
         data = CurvatureConstraintData(Lt1=Lt1, Lt2=Lt2, Lc1=Lc1, Lc2=Lc2, n1=n1, n2=n2, theta1=theta1, theta2=theta2,
                                        phi1=phi1, phi2=phi2, psi1=psi1, psi2=psi2, R1=R1, R2=R2)
         return data
 
+    @staticmethod
+    def is_solving_allowed(g2_point: Point):
+        symmetry_constraints = [geo_con for geo_con in g2_point.geo_cons if
+                                isinstance(geo_con, SymmetryConstraint)]
+        # Check if the point is the symmetry target point
+        if any([symmetry_constraint.child_nodes[-1] is g2_point for symmetry_constraint in symmetry_constraints]):
+            return False
+        return True
+
     def __repr__(self):
         return f"{self.__class__.__name__} {self.name()} <C1={self.curve_1.name()}, C2={self.curve_2.name()}>"
 
     def get_dict_rep(self):
         value = self.param().name() if self.param() is not None else None
         return {"curve_joint": self.curve_joint.name(), "value": value,
                 "constraint_type": self.__class__.__name__}
 
+    def verify(self) -> bool:
+        data = self.calculate_curvature_data(self.curve_joint)
+        return np.isclose(data.R1, data.R2, rtol=1e-14)
+
 
 class ConstraintValidationError(Exception):
     pass
 
 
 class NoSolutionError(Exception):
     pass
```

### Comparing `pymead-2.0.0b3/pymead/core/gcs.py` & `pymead-2.0.0b4/pymead/core/gcs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import networkx
+from pymead.core.bezier import Bezier
 
 from pymead.core.constraints import *
 from pymead.core.constraint_equations import *
 from pymead.core.line import PolyLine
 from pymead.core.point import Point
 
 
@@ -30,14 +31,15 @@
         Constructor for the geometric constraint solver.
         """
         super().__init__()
         self.points = {}
         self.roots = []
         self.cluster_angle_params = {}
         self.geo_col = None
+        self.partial_symmetry_solves = []
 
     def add_point(self, point: Point):
         """
         Adds a point (node) to the graph (and to the ``"points"`` attribute). Also assigns this graph to the point.
 
         Parameters
         ----------
@@ -109,18 +111,27 @@
 
         """
         u.root = True
         v.rotation_handle = True
         if u not in [edge[0] for edge in self.roots]:
             self.roots.append((u, v))
 
-        # Do not add a cluster angle parameter if the root was created as part of an antiparallel constraint between
-        # a polyline and another curve
-        if any([isinstance(curve, PolyLine) for curve in u.curves]) and not all(
-                [u in curve.point_sequence().points() for curve in u.curves]):
+        cluster_angle_exceptions = [
+            # Do not add a cluster angle parameter if the root was created as part of an antiparallel constraint between
+            # a polyline and another curve
+            any([isinstance(curve, PolyLine) for curve in u.curves]) and not all(
+                [u in curve.point_sequence().points() for curve in u.curves]),
+
+            # Do not add a cluster angle parameter if the root was created as part of an antiparallel constraint between
+            # a curve defined by symmetric constraints and a normal Bézier curve
+            (SymmetryConstraint.check_if_point_is_symmetric_target(u) and
+                SymmetryConstraint.check_if_point_is_symmetric_target(v))
+        ]
+        if any(cluster_angle_exceptions):
+            v.rotation_handle = False  # TODO: check if this change works for other cases
             return
 
         if v.rotation_param is not None:
             param = v.rotation_param
         else:
             param = self.geo_col.add_param(value=u.measure_angle(v), name="ClusterAngle-1", unit_type="angle", root=u,
                                            rotation_handle=v)
@@ -166,14 +177,16 @@
 
         Returns
         -------
         Point
             Root of the constraint cluster
 
         """
+        if not isinstance(rotation_handle, Point):
+            raise ValueError(f"Detected rotation handle that is not a point ({rotation_handle = })")
         in_edges = [edge for edge in self.in_edges(nbunch=rotation_handle)]
         if not len(in_edges) == 1:
             raise ValueError("Invalid rotation handle. Rotation should have exactly one incident edge "
                              "(the cluster root)")
         return in_edges[0][0]
 
     def _identify_rotation_handle(self, root_node: Point):
@@ -260,14 +273,17 @@
         -------
         Point or None
             The root node/point if found, otherwise ``None``
         """
         for node in networkx.bfs_tree(self, source=source_node, reverse=True):
             if node.root:
                 return node
+        for node in networkx.bfs_tree(self, source=source_node, reverse=False):
+            if node.root:
+                return node
         return None
 
     def _orient_flow_away_from_root(self, root: Point) -> typing.List[GeoCon]:
         """
         Orients the flow of the edges away from the given root of a constraint cluster. Critical method that ensures
         the rigid body transformation triggered by a given constraint value change applies to the correct set of points
         to preserve the constraint state.
@@ -412,15 +428,45 @@
             List of constraints to re-assign
 
         Returns
         -------
 
         """
         for constraint in constraints:
-            self._reassign_constraint(constraint)
+            if (isinstance(constraint, DistanceConstraint) or isinstance(constraint, RelAngle3Constraint) or
+                    isinstance(constraint, Perp3Constraint) or isinstance(constraint, AntiParallel3Constraint)):
+                self._reassign_constraint(constraint)
+
+    def _check_distance_constraint_for_duplicates(self, dist_con: DistanceConstraint):
+        for gc in self.geo_col.container()["geocon"].values():
+            if gc is dist_con:
+                continue
+            if not isinstance(gc, DistanceConstraint):
+                continue
+            if (dist_con.p1 is gc.p1 and dist_con.p2 is gc.p2) or (dist_con.p1 is gc.p2 and dist_con.p2 is gc.p1):
+                raise ValueError("A distance constraint already exists between these two points")
+
+    def _check_angle_constraint_for_duplicates(self, angle_con: RelAngle3Constraint or AntiParallel3Constraint or
+                                                                Perp3Constraint):
+        for gc in self.geo_col.container()["geocon"].values():
+            if gc is angle_con:
+                continue
+            if not isinstance(gc, RelAngle3Constraint) and not isinstance(
+                    gc, AntiParallel3Constraint) and not isinstance(gc, Perp3Constraint):
+                continue
+            if (gc.p1 is angle_con.p1 and gc.p3 is angle_con.p3) or (
+                    gc.p1 is angle_con.p3 and gc.p3 is angle_con.p1):
+                raise ValueError("An angle constraint already exists between these three points")
+
+    def check_constraint_for_duplicates(self, geo_con: GeoCon):
+        if isinstance(geo_con, DistanceConstraint):
+            self._check_distance_constraint_for_duplicates(geo_con)
+        elif isinstance(geo_con, RelAngle3Constraint) or isinstance(
+                geo_con, AntiParallel3Constraint) or isinstance(geo_con, Perp3Constraint):
+            self._check_angle_constraint_for_duplicates(geo_con)
 
     def _assign_distance_constraint(self, dist_con: DistanceConstraint):
         """
         Assigns a distance constraint by first adding an edge from ``p1`` to ``p2`` with no data and subsequently
         applying the constraint data.
 
         Parameters
@@ -428,15 +474,23 @@
         dist_con: DistanceConstraint
             Constraint to assign
 
         Returns
         -------
 
         """
-        self.add_edge(dist_con.p1, dist_con.p2)
+        if (SymmetryConstraint.check_if_point_is_symmetric_target(dist_con.p1) and
+            SymmetryConstraint.check_if_point_is_symmetric_target(dist_con.p2)):
+            raise ValueError("Could not assign distance constraint")
+        if SymmetryConstraint.check_if_point_is_symmetric_target(dist_con.p1):
+            self.add_edge(dist_con.p1, dist_con.p2)
+        elif SymmetryConstraint.check_if_point_is_symmetric_target(dist_con.p2):
+            self.add_edge(dist_con.p2, dist_con.p1)
+        else:
+            self.add_edge(dist_con.p1, dist_con.p2)
         self._reassign_distance_constraint(dist_con)
 
     def _assign_angle_constraint(self, angle_con: RelAngle3Constraint or AntiParallel3Constraint or Perp3Constraint):
         """
         Assigns an angle constraint by first adding an edge from either ``p2`` to ``p1`` or ``p2`` to ``p3``
         (depending on which edge already has data) with no data and subsequently applying the constraint data.
 
@@ -446,19 +500,27 @@
         angle_con: RelAngle3Constraint or AntiParallel3Constraint or Perp3Constraint
             Constraint to assign
 
         Returns
         -------
 
         """
-        if not (self.get_edge_data(angle_con.p1, angle_con.p2)
-                or self.get_edge_data(angle_con.p2, angle_con.p1)):
+        if (SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p1) and
+                SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p2) and
+                SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p3)):
+            raise ValueError("Could not add angle constraint")
+        if (not (self.get_edge_data(angle_con.p1, angle_con.p2)
+                or self.get_edge_data(angle_con.p2, angle_con.p1)) and
+                not (SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p1) and
+                     SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p2))):
             self.add_edge(angle_con.p2, angle_con.p1)
-        if not (self.get_edge_data(angle_con.p2, angle_con.p3) or
-                self.get_edge_data(angle_con.p3, angle_con.p2)):
+        if (not (self.get_edge_data(angle_con.p2, angle_con.p3) or
+                 self.get_edge_data(angle_con.p3, angle_con.p2)) and
+                  not (SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p2) and
+                       SymmetryConstraint.check_if_point_is_symmetric_target(angle_con.p3))):
             self.add_edge(angle_con.p2, angle_con.p3)
         self._reassign_angle_constraint(angle_con)
 
     def _add_ghost_edges_to_angle_constraint(
             self, constraint: RelAngle3Constraint or AntiParallel3Constraint or Perp3Constraint):
         """
         Adds any required "ghost" edges (edges with no data) to an angle constraint to ensure that there are edges
@@ -473,18 +535,35 @@
         Returns
         -------
 
         """
         # Only add ghost edges if there is not a concrete edge present (even if facing the wrong direction)
         if not (self.get_edge_data(constraint.p1, constraint.p2)
                 or self.get_edge_data(constraint.p2, constraint.p1)):
-            self.add_edge(constraint.p2, constraint.p1)
+            if (SymmetryConstraint.check_if_point_is_symmetric_target(constraint.p1) and
+                SymmetryConstraint.check_if_point_is_symmetric_target(constraint.p2)):
+                self.add_edge(constraint.p1, constraint.p2)
+                if constraint.p2.root:
+                    self.move_root(constraint.p1)
+            else:
+                self.add_edge(constraint.p2, constraint.p1)
         if not (self.get_edge_data(constraint.p2, constraint.p3) or
                 self.get_edge_data(constraint.p3, constraint.p2)):
-            self.add_edge(constraint.p2, constraint.p3)
+            if (SymmetryConstraint.check_if_point_is_symmetric_target(constraint.p2) and
+                    SymmetryConstraint.check_if_point_is_symmetric_target(constraint.p3)):
+                self.add_edge(constraint.p3, constraint.p2)
+                if constraint.p2.root:
+                    self.move_root(constraint.p3)
+            else:
+                self.add_edge(constraint.p2, constraint.p3)
+
+    # def _assign_symmetry_constraint(self, constraint: SymmetryConstraint):
+    #     self.add_edge(constraint.p1, constraint.p4)
+    #     self.add_edge(constraint.p2, constraint.p4)
+    #     self.add_edge(constraint.p3, constraint.p4)
 
     def _test_if_cluster_is_branching(self, root_node: Point) -> bool:
         """
         Computes the subgraph corresponding to the constraint cluster given by the input root node, and checks if
         this subgraph is branching: each node must have exactly one parent.
 
         Parameters
@@ -543,14 +622,16 @@
 
         if isinstance(constraint, DistanceConstraint):
             self._assign_distance_constraint(constraint)
         elif isinstance(constraint, RelAngle3Constraint) or isinstance(
                 constraint, AntiParallel3Constraint) or isinstance(constraint, Perp3Constraint):
             self._assign_angle_constraint(constraint)
             self._add_ghost_edges_to_angle_constraint(constraint)
+        # elif isinstance(constraint, SymmetryConstraint):
+        #     self._assign_symmetry_constraint(constraint)
 
         if isinstance(constraint, DistanceConstraint) or isinstance(constraint, AntiParallel3Constraint) or isinstance(
                 constraint, Perp3Constraint) or isinstance(constraint, RelAngle3Constraint):
             unique_roots = self._get_unique_roots_from_constraint(constraint)
             merge_clusters = False if len(unique_roots) < 2 else True
             if merge_clusters:
                 root = self._merge_clusters_with_constraint(unique_roots)
@@ -608,16 +689,14 @@
                 edge_data_21.pop("distance")
             else:
                 self.remove_edge(constraint.p2, constraint.p1)
                 edges_removed = [(constraint.p2, constraint.p1)]
 
             return edges_removed
 
-        raise ValueError(f"Failed to remove distance constraint {constraint}")
-
     def _remove_angle_constraint_from_directed_edge(
             self, constraint: RelAngle3Constraint or AntiParallel3Constraint or Perp3Constraint):
         edges_removed = []
         edge_data_21 = self.get_edge_data(constraint.p2, constraint.p1)
         if edge_data_21 is not None and "angle" in edge_data_21.keys() and edge_data_21["angle"] is constraint:
             if "distance" in edge_data_21.keys():
                 edge_data_21.pop("angle")
@@ -645,32 +724,28 @@
             edge_data_12 = self.get_edge_data(constraint.p1, constraint.p2)
             if edge_data_12 is not None and len(edge_data_12) == 0:
                 self.remove_edge(constraint.p1, constraint.p2)
                 edges_removed.append((constraint.p1, constraint.p2))
 
             return edges_removed
 
-        raise ValueError(f"Failed to remove angle constraint {constraint}")
-
     def _assign_new_root_if_required(self, v_of_edge_removed: Point):
         neighbors_of_v = [nbr for nbr in self.adj[v_of_edge_removed]]
         if len(neighbors_of_v) > 0:
             self._set_edge_as_root(v_of_edge_removed, neighbors_of_v[0])
         else:
             pass  # This means we trimmed the end of the branch
 
     def _update_roots_based_on_constraint_removal(self, edges_removed: typing.List[tuple]):
         for edge_removed in edges_removed:
             if edge_removed[1].rotation_handle:
-                edge_removed[1].rotation_handle = False
+                self._delete_root_status(edge_removed[0], edge_removed[1])
                 for out_edge in self.out_edges(nbunch=edge_removed[0]):
-                    out_edge[1].rotation_handle = True
+                    self._set_edge_as_root(out_edge[0], out_edge[1])
                     break
-                else:  # In this case, no more edges were attached to the root, so the root should be deleted
-                    self._identify_and_delete_root(edge_removed[0])
             self._assign_new_root_if_required(edge_removed[1])
 
     def remove_constraint(self, constraint: GeoCon):
 
         edges_removed = None
         if isinstance(constraint, DistanceConstraint):
             edges_removed = self._remove_distance_constraint_from_directed_edge(constraint)
@@ -702,74 +777,79 @@
             point.x().set_value(point.x().value() + dx)
             point.y().set_value(point.y().value() + dy)
             if point not in points_solved:
                 points_solved.append(point)
 
         return points_solved
 
-    def _solve_perp_parallel_constraint(self, source: AntiParallel3Constraint or Perp3Constraint):
-        points_solved = []
-        edge_data_p21 = self.get_edge_data(source.p2, source.p1)
-        edge_data_p23 = self.get_edge_data(source.p2, source.p3)
+    def _solve_angle_constraint(self, source: RelAngle3Constraint or AntiParallel3Constraint or Perp3Constraint):
 
-        old_angle = (source.p2.measure_angle(source.p1) - source.p2.measure_angle(source.p3)) % (2 * np.pi)
-        new_angle = np.pi if isinstance(source, AntiParallel3Constraint) else np.pi / 2
-        d_angle = new_angle - old_angle
-        rotation_point = source.p2
-
-        if edge_data_p21 and "angle" in edge_data_p21 and edge_data_p21["angle"] is source:
-            start = source.p1
-        elif edge_data_p23 and "angle" in edge_data_p23 and edge_data_p23["angle"] is source:
-            start = source.p3
-            d_angle *= -1
-        else:
-            raise ValueError("Somehow no angle constraint found between the three points")
-
-        rotation_mat = np.array([[np.cos(d_angle), -np.sin(d_angle)], [np.sin(d_angle), np.cos(d_angle)]])
-        rotation_point_mat = np.array([[rotation_point.x().value()], [rotation_point.y().value()]])
-
-        for point in networkx.bfs_tree(self, source=start):
-            dx_dy = np.array([[point.x().value() - rotation_point.x().value()],
-                              [point.y().value() - rotation_point.y().value()]])
-            new_xy = (rotation_mat @ dx_dy + rotation_point_mat).flatten()
-            point.x().set_value(new_xy[0])
-            point.y().set_value(new_xy[1])
-            if point not in points_solved:
-                points_solved.append(point)
-        return points_solved
-
-    def _solve_rel_angle3_constraint(self, source: RelAngle3Constraint):
         points_solved = []
         edge_data_p21 = self.get_edge_data(source.p2, source.p1)
         edge_data_p23 = self.get_edge_data(source.p2, source.p3)
 
         old_angle = (source.p2.measure_angle(source.p1) -
                      source.p2.measure_angle(source.p3)) % (2 * np.pi)
-        new_angle = source.param().rad()
+        if isinstance(source, RelAngle3Constraint):
+            new_angle = source.param().rad()
+        elif isinstance(source, AntiParallel3Constraint):
+            new_angle = np.pi
+        elif isinstance(source, Perp3Constraint):
+            new_angle = np.pi / 2
+        else:
+            raise ValueError(f"{type(source)} is not a valid type for angle constraint")
         d_angle = new_angle - old_angle
         rotation_point = source.p2
 
         if edge_data_p21 and "angle" in edge_data_p21 and edge_data_p21["angle"] is source:
-            start = source.p1 if not source.p2.root else source.p2
+            # start = source.p1 if not source.p2.root else source.p2
+            # start = source.p2
+            start = source.p1
         elif edge_data_p23 and "angle" in edge_data_p23 and edge_data_p23["angle"] is source:
-            start = source.p3 if not source.p2.root else source.p2
+            # start = source.p3 if not source.p2.root else source.p2
+            # start = source.p2
+            start = source.p3
             d_angle *= -1
         else:
             raise ValueError("Somehow no angle constraint found between the three points")
 
         rotation_mat = np.array([[np.cos(d_angle), -np.sin(d_angle)], [np.sin(d_angle), np.cos(d_angle)]])
         rotation_point_mat = np.array([[rotation_point.x().value()], [rotation_point.y().value()]])
 
         # Get all the points that might need to rotate
+        additional_branch_starting_points = []
+        if start is not source.p2:
+            for geo_con in start.geo_cons:
+                if geo_con is source:
+                    continue
+                if not (isinstance(geo_con, AntiParallel3Constraint) or isinstance(
+                        geo_con, RelAngle3Constraint) or isinstance(geo_con, Perp3Constraint)):
+                    continue
+                if geo_con.p2 is not source.p2:
+                    continue
+                # if not geo_con.p1 in self.adj[source.p2] or not geo_con.p3 in self.adj[source.p2]:
+                #     continue
+                if start is source.p3 and geo_con.p3 is source.p3:
+                    additional_branch_starting_points.append(geo_con.p1)
+                elif start is source.p3 and geo_con.p1 is source.p3:
+                    additional_branch_starting_points.append(geo_con.p3)
+                elif start is source.p1 and geo_con.p3 is source.p1:
+                    additional_branch_starting_points.append(geo_con.p1)
+                elif start is source.p1 and geo_con.p1 is source.p1:
+                    additional_branch_starting_points.append(geo_con.p3)
+
         all_downstream_points = []
         rotation_handle = None
-        for point in networkx.bfs_tree(self, source=start):
-            all_downstream_points.append(point)
-            if point.rotation_handle:
-                rotation_handle = point
+        # print(f"{start = }, {additional_branch_starting_points = }")
+        for source_point in [start, *additional_branch_starting_points]:
+            for point in networkx.bfs_tree(self, source=source_point):
+                # if point not in points_to_exclude:
+                all_downstream_points.append(point)
+                if not rotation_handle and point.rotation_handle:
+                    rotation_handle = point
 
         # Get the branch to cut, if there is one
         root_rotation_branch = []
         if source.p2.root and rotation_handle is not None:
             root_rotation_branch = [point for point in networkx.bfs_tree(self, source=rotation_handle)]
 
         for point in all_downstream_points:
@@ -782,35 +862,64 @@
             point.y().set_value(new_xy[1])
             if point not in points_solved:
                 points_solved.append(point)
         return points_solved
 
     def solve(self, source: GeoCon):
 
-        # networkx.draw_circular(self, labels={point: point.name() for point in self.nodes})
-        # from matplotlib import pyplot as plt
-        # plt.show()
-
         points_solved = []
         symmetry_points_solved = []
         roc_points_solved = []
         if isinstance(source, DistanceConstraint):
             points_solved.extend(self._solve_distance_constraint(source))
-        elif isinstance(source, AntiParallel3Constraint) or isinstance(source, Perp3Constraint):
-            points_solved.extend(self._solve_perp_parallel_constraint(source))
-        elif isinstance(source, RelAngle3Constraint):
-            points_solved.extend(self._solve_rel_angle3_constraint(source))
+        elif (isinstance(source, RelAngle3Constraint) or isinstance(source, AntiParallel3Constraint) or
+              isinstance(source, Perp3Constraint)):
+            points_solved.extend(self._solve_angle_constraint(source))
         elif isinstance(source, SymmetryConstraint):
-            symmetry_points_solved = self.solve_symmetry_constraint(source)
+            points_solved.extend(self.solve_symmetry_constraint(source))
         elif isinstance(source, ROCurvatureConstraint):
-            roc_points_solved = self.solve_roc_constraint(source)
+            points_solved.extend(self.solve_roc_constraint(source))
+
+        # symmetry_constraints_to_re_solve = []
+        # for roc_point in roc_points_solved:
+        #     for geo_con in roc_point.geo_cons:
+        #         if not isinstance(geo_con, SymmetryConstraint):
+        #             continue
+        #         if geo_con not in symmetry_constraints_to_re_solve:
+        #             symmetry_constraints_to_re_solve.append(geo_con)
+        #
+        # symmetry_points_solved_second_pass = []
+        # for symmetry_constraint in list(set(symmetry_constraints_to_re_solve)):
+        #     symmetry_points_solved_second_pass.extend(self.solve_symmetry_constraint(symmetry_constraint))
+        #
+        # roc_constraints_to_re_solve = []
+        # for symmetry_point in list(set(symmetry_points_solved_second_pass)):
+        #     for geo_con in symmetry_point.geo_cons:
+        #         if not isinstance(geo_con, ROCurvatureConstraint):
+        #             continue
+        #         if geo_con not in roc_constraints_to_re_solve:
+        #             roc_constraints_to_re_solve.append(geo_con)
+        #
+        # roc_points_solved_second_pass = []
+        # for roc_constraint in list(set(roc_constraints_to_re_solve)):
+        #     roc_points_solved_second_pass.extend(self.solve_roc_constraint(roc_constraint))
 
         other_points_solved = self.solve_other_constraints(points_solved)
         other_points_solved = list(
-            set(other_points_solved).union(set(symmetry_points_solved)).union(set(roc_points_solved)))
+            set(other_points_solved).union(
+                set(symmetry_points_solved)).union(
+                set(roc_points_solved))
+        )
+        # other_points_solved = list(
+        #     set(other_points_solved).union(
+        #         set(symmetry_points_solved)).union(
+        #         set(roc_points_solved)).union(
+        #         set(symmetry_points_solved_second_pass)).union(
+        #         set(roc_points_solved_second_pass))
+        # )
 
         points_solved = list(set(points_solved).union(set(other_points_solved)))
 
         return points_solved
 
     def translate_cluster(self, root: Point, dx: float, dy: float):
         if not root.root:
@@ -850,36 +959,44 @@
             point.x().set_value(new_x)
             point.y().set_value(new_y)
             if point not in points_solved:
                 points_solved.append(point)
         self.solve_other_constraints(points_solved)
         return points_solved, root
 
-    @staticmethod
-    def solve_symmetry_constraint(constraint: SymmetryConstraint):
+    def solve_symmetry_constraint(self, constraint: SymmetryConstraint):
+        # This code prevents recursion errors for the case where a new cluster is created from a symmetry constraint
+        # target. The symmetry constraint only gets solved if it has not yet been added to the list of partial solves
+        if constraint in self.partial_symmetry_solves:
+            return []
+        else:
+            self.partial_symmetry_solves.append(constraint)
+
         x1, y1 = constraint.p1.x().value(), constraint.p1.y().value()
         x2, y2 = constraint.p2.x().value(), constraint.p2.y().value()
         x3, y3 = constraint.p3.x().value(), constraint.p3.y().value()
         line_angle = measure_abs_angle(x1, y1, x2, y2)
         tool_angle = measure_rel_angle3(x1, y1, x2, y2, x3, y3)
         if tool_angle < np.pi:
             mirror_angle = line_angle - np.pi / 2
         elif tool_angle > np.pi:
             mirror_angle = line_angle + np.pi / 2
         else:
             # Rare case where the point is coincident with the line: just make p4 = p3
             constraint.p4.request_move(constraint.p3.x().value(), constraint.p3.y().value(), force=True)
-            return
+            return constraint.child_nodes
 
         mirror_distance = 2 * measure_point_line_distance_unsigned(x1, y1, x2, y2, x3, y3)
         constraint.p4.request_move(
             x3 + mirror_distance * np.cos(mirror_angle),
             y3 + mirror_distance * np.sin(mirror_angle), force=True
         )
 
+        self.partial_symmetry_solves.remove(constraint)
+
         return constraint.child_nodes
 
     @staticmethod
     def solve_roc_constraint(constraint: ROCurvatureConstraint):
 
         def solve_for_single_curve(p_g1: Point, p_g2: Point, n: int):
             Lc = measure_curvature_length_bezier(
@@ -899,17 +1016,25 @@
             return constraint.child_nodes
 
         if constraint.curve_type_2 == "Bezier" and constraint.curve_type_1 == "LineSegment":
             solve_for_single_curve_zero_curvature(constraint.g1_point_curve_2, constraint.g2_point_curve_2)
             return constraint.child_nodes
 
         if constraint.curve_type_1 == "Bezier":
-            solve_for_single_curve(constraint.g1_point_curve_1, constraint.g2_point_curve_1, constraint.curve_1.degree)
+            if constraint.is_solving_allowed(constraint.g2_point_curve_1):
+                solve_for_single_curve(constraint.g1_point_curve_1, constraint.g2_point_curve_1, constraint.curve_1.degree)
+            else:
+                R1 = ROCurvatureConstraint.calculate_curvature_data(constraint.curve_joint).R1
+                constraint.param().set_value(R1, force=True)
         if constraint.curve_type_2 == "Bezier":
-            solve_for_single_curve(constraint.g1_point_curve_2, constraint.g2_point_curve_2, constraint.curve_2.degree)
+            if constraint.is_solving_allowed(constraint.g2_point_curve_2):
+                solve_for_single_curve(constraint.g1_point_curve_2, constraint.g2_point_curve_2, constraint.curve_2.degree)
+            else:
+                R2 = ROCurvatureConstraint.calculate_curvature_data(constraint.curve_joint).R2
+                constraint.param().set_value(R2, force=True)
 
         return constraint.child_nodes
 
     def solve_symmetry_constraints(self, points: typing.List[Point]):
         points_solved = []
         symmetry_constraints_solved = []
         for point in points:
@@ -942,16 +1067,16 @@
                         continue
 
                     points_solved.append(roc_point_solved)
 
         return points_solved
 
     def solve_other_constraints(self, points: typing.List[Point]):
-        symmetry_points_solved = self.solve_symmetry_constraints(points)
         roc_points_solved = self.solve_roc_constraints(points)
+        symmetry_points_solved = self.solve_symmetry_constraints(points)
         return list(set(symmetry_points_solved).union(roc_points_solved))
 
     @staticmethod
     def update_canvas_items(points_solved: typing.List[Point]):
 
         curves_to_update = []
         for point in points_solved:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymead-2.0.0b3/pymead/core/geometry_collection.py` & `pymead-2.0.0b4/pymead/core/geometry_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import datetime
 import os
+import random
 import re
 import sys
 import typing
 from copy import copy
 
+from pymead.core.param_graph import ParamGraph
+from pymead.core import UNITS
 from pymead.core.airfoil import Airfoil
 from pymead.core.bezier import Bezier
 from pymead.core.constraints import *
 from pymead.core.gcs import GCS
 from pymead.core.mea import MEA
 from pymead.core.pymead_obj import DualRep, PymeadObj
 from pymead.core.line import LineSegment, PolyLine
@@ -36,14 +39,15 @@
             "bezier": {},
             "airfoils": {},
             "mea": {},
             "geocon": {},
             "dims": {},
         }
         self.gcs = GCS()
+        self.param_graph = ParamGraph()
         self.gcs.geo_col = self
         self.gui_obj = gui_obj
         self.canvas = None
         self.tree = None
         self.selected_objects = {k: [] for k in self._container.keys()}
         self.selected_airfoils = []
         self.single_step = 0.01
@@ -173,15 +177,16 @@
         """
         if pymead_obj.name() not in self.container()[pymead_obj.sub_container]:
             return
         self.container()[pymead_obj.sub_container].pop(pymead_obj.name())
 
     def add_param(self, value: float, name: str or None = None, lower: float or None = None,
                   upper: float or None = None, unit_type: str or None = None, assign_unique_name: bool = True,
-                  point: Point = None, root: Point = None, rotation_handle: Point = None, enabled: bool = True):
+                  point: Point = None, root: Point = None, rotation_handle: Point = None, enabled: bool = True,
+                  equation_str: str = None):
         """
         Adds a parameter to the geometry collection sub-container ``"params"``, and modifies the name to make it
         unique if necessary.
 
         Parameters
         ==========
         value: float
@@ -201,15 +206,15 @@
 
         Returns
         =======
         Param
             The generated parameter
         """
         kwargs = dict(value=value, name=name, lower=lower, upper=upper, setting_from_geo_col=True, point=point,
-                      root=root, rotation_handle=rotation_handle, enabled=enabled)
+                      root=root, rotation_handle=rotation_handle, enabled=enabled, equation_str=equation_str)
         if unit_type is None:
             param = Param(**kwargs)
         elif unit_type == "length":
             param = LengthParam(**kwargs)
         elif unit_type == "angle":
             param = AngleParam(**kwargs)
         else:
@@ -352,19 +357,31 @@
 
         if self.canvas is not None:
             pymead_obj.canvas = self.canvas
             self.canvas.addPymeadCanvasItem(pymead_obj=pymead_obj)
 
         if isinstance(pymead_obj, Point):
             self.gcs.add_point(pymead_obj)
+            for param in [pymead_obj.x(), pymead_obj.y()]:
+                param.param_graph = self.param_graph
+                if param not in param.param_graph.param_list:
+                    param.param_graph.param_list.append(param)
+                param.update_equation(param.equation_str)
+
+        if isinstance(pymead_obj, Param):
+            pymead_obj.param_graph = self.param_graph
+            if pymead_obj not in pymead_obj.param_graph.param_list:
+                pymead_obj.param_graph.param_list.append(pymead_obj)
+            pymead_obj.update_equation(pymead_obj.equation_str)
+            pymead_obj.set_enabled(pymead_obj.enabled())
 
         return pymead_obj
 
     def remove_pymead_obj(self, pymead_obj: PymeadObj, promotion_demotion: bool = False,
-                          constraint_removal: bool = False):
+                          constraint_removal: bool = False, equating_constraints: bool = False):
         """
         Removes a pymead object from the geometry collection.
 
         Parameters
         ==========
         pymead_obj: PymeadObj
             Pymead object to remove
@@ -372,27 +389,39 @@
         promotion_demotion: bool
             When this flag is set to ``True``, the ``ValueError`` normally raised when directly deleting a ``Param``
             associated with a ``GeoCon`` is ignored. Default: ``False``
 
         constraint_removal: bool
             When this flag is set to ``True``, the ``ValueError`` normally raise when directly deleting a ``Param``
             associated with a constraint cluster rotation is ignored. Default: ``False``
+
+        equating_constraints: bool
+            When this flag is set to ``True`` and the ``pymead_obj`` is a ``Param``, the associated constraints are
+            not deleted
         """
         # Type-specific actions
         if isinstance(pymead_obj, Param):
+
             if pymead_obj.rotation_handle and not constraint_removal and not promotion_demotion:
                 error_message = f"This parameter can only be removed by deleting its associated constraint cluster"
                 if self.gui_obj is None:
                     raise ValueError(error_message)
                 else:
                     self.gui_obj.disp_message_box(error_message, message_mode="error")
                     return
 
-            for geo_con in pymead_obj.geo_cons:
-                self.remove_pymead_obj(geo_con)
+            if not promotion_demotion and not equating_constraints:  # Do not remove the constraints if this is a
+                # promotion/demotion action or an equating constraints action
+                for geo_con in pymead_obj.geo_cons:
+                    self.remove_pymead_obj(geo_con)
+
+            if pymead_obj in self.param_graph.param_list:
+                self.param_graph.param_list.remove(pymead_obj)
+            if pymead_obj in self.param_graph.nodes:
+                self.param_graph.remove_node(pymead_obj)
 
         elif isinstance(pymead_obj, Bezier) or isinstance(pymead_obj, LineSegment) or isinstance(pymead_obj, PolyLine):
             # Remove all the references to this curve in each of the curve's points
             for pt in pymead_obj.point_sequence().points():
                 if pymead_obj in pt.curves:
                     pt.curves.remove(pymead_obj)
 
@@ -400,14 +429,19 @@
                 for curve in pymead_obj.airfoil.curves:
                     if pymead_obj is not curve:
                         curve.airfoil = None
                 self.remove_pymead_obj(pymead_obj.airfoil)
 
         elif isinstance(pymead_obj, Point):
 
+            for param in [pymead_obj.x(), pymead_obj.y()]:
+                param.param_graph.param_list.remove(param)
+                if param in param.param_graph.nodes:
+                    param.param_graph.remove_node(param)
+
             for geo_con in pymead_obj.geo_cons:
                 self.remove_pymead_obj(geo_con)
 
             # Loop through the curves associated with this point to see which ones need to be deleted if one point
             # is removed from their point sequence
             curves_to_delete = []
             for curve in pymead_obj.curves:
@@ -423,34 +457,31 @@
 
             # Update any remaining curves
             for curve in pymead_obj.curves:
                 if pymead_obj in curve.point_sequence().points():
                     curve.remove_point(point=pymead_obj)
                     curve.update()
 
-            for dim in pymead_obj.dims:
-                self.remove_pymead_obj(dim)
-
             for geo_con in pymead_obj.geo_cons[::-1]:
                 self.remove_pymead_obj(geo_con)
 
             self.gcs.remove_point(pymead_obj)
 
         elif isinstance(pymead_obj, GeoCon):
             # First, remove the parameter associated with the constraint if necessary (i.e., if that parameter is not
             # tied to any other constraints
             if pymead_obj.param() is not None:
                 pymead_obj.param().geo_cons.remove(pymead_obj)
                 if len(pymead_obj.param().geo_cons) == 0:
                     self.remove_pymead_obj(pymead_obj.param())
 
-            if (isinstance(pymead_obj, DistanceConstraint) or isinstance(pymead_obj, RelAngle3Constraint) or
-                isinstance(pymead_obj, Perp3Constraint) or isinstance(pymead_obj, AntiParallel3Constraint)):
-                if pymead_obj.p2.rotation_handle and pymead_obj.p2.rotation_param is not None:
-                    self.remove_pymead_obj(pymead_obj.p2.rotation_param, constraint_removal=True)
+            # if (isinstance(pymead_obj, DistanceConstraint) or isinstance(pymead_obj, RelAngle3Constraint) or
+            #     isinstance(pymead_obj, Perp3Constraint) or isinstance(pymead_obj, AntiParallel3Constraint)):
+            #     if pymead_obj.p2.rotation_handle and pymead_obj.p2.rotation_param is not None:
+            #         self.remove_pymead_obj(pymead_obj.p2.rotation_param, constraint_removal=True)
 
             # Remove the constraint from the ConstraintGraph
             self.gcs.remove_constraint(pymead_obj)
 
         elif isinstance(pymead_obj, Airfoil):
             for curve in pymead_obj.curves:
                 curve.airfoil = None
@@ -503,16 +534,17 @@
         point = Point(x=x, y=y, name=name)
         point.x().geo_col = self
         point.y().geo_col = self
         self.add_pymead_obj_by_ref(point, assign_unique_name=assign_unique_name)
 
         return point
 
-    def add_bezier(self, point_sequence: PointSequence, name: str or None = None, assign_unique_name: bool = True):
-        bezier = Bezier(point_sequence=point_sequence, name=name)
+    def add_bezier(self, point_sequence: PointSequence, name: str or None = None,
+                   t_start: float = None, t_end: float = None, assign_unique_name: bool = True):
+        bezier = Bezier(point_sequence=point_sequence, name=name, t_start=t_start, t_end=t_end)
 
         return self.add_pymead_obj_by_ref(bezier, assign_unique_name=assign_unique_name)
 
     def add_line(self, point_sequence: PointSequence, name: str or None = None, assign_unique_name: bool = True):
         line = LineSegment(point_sequence=point_sequence, name=name)
 
         return self.add_pymead_obj_by_ref(line, assign_unique_name=assign_unique_name)
@@ -543,15 +575,15 @@
             for point in new_polyline.point_sequence().points():
                 if point not in self.container()["points"].values():
                     self.add_pymead_obj_by_ref(point)
             self.add_pymead_obj_by_ref(new_polyline)
 
     def add_desvar(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
                    unit_type: str or None = None, assign_unique_name: bool = True, point: Point = None,
-                   root: Point = None, rotation_handle: Point = None):
+                   root: Point = None, rotation_handle: Point = None, enabled: bool = True, equation_str: str = None):
         """
         Directly adds a design variable value to the geometry collection.
 
         Parameters
         ==========
         value: float
             Value of the design variable
@@ -572,15 +604,15 @@
 
         Returns
         =======
         DesVar
             The generated design variable
         """
         kwargs = dict(value=value, name=name, lower=lower, upper=upper, setting_from_geo_col=True, point=point,
-                      root=root, rotation_handle=rotation_handle)
+                      root=root, rotation_handle=rotation_handle, enabled=enabled, equation_str=equation_str)
         if unit_type is None:
             desvar = DesVar(**kwargs)
         elif unit_type == "length":
             desvar = LengthDesVar(**kwargs)
         elif unit_type == "angle":
             desvar = AngleDesVar(**kwargs)
         else:
@@ -639,27 +671,22 @@
         elif isinstance(param, AngleParam):
             unit_type = "angle"
         else:
             unit_type = None
 
         desvar = self.add_desvar(value=param.value(), name=param.name(), lower=lower, upper=upper, unit_type=unit_type,
                                  point=copy(param.point), root=param.root,
-                                 rotation_handle=param.rotation_handle)
+                                 rotation_handle=param.rotation_handle, assign_unique_name=False)
 
         # Replace the corresponding x() or y() in parameter with the new design variable
         self.replace_geo_objs(tool=param, target=desvar)
 
         # Make a copy of the geometry object reference lists in the new design variable
         desvar.geo_objs = param.geo_objs.copy()
 
-        # Copy dimension information
-        desvar.dims = param.dims.copy()
-        for dim in desvar.dims:
-            dim.set_param(desvar)
-
         # Copy constraint information
         desvar.geo_cons = param.geo_cons
         desvar.gcs = self.gcs
         for constraint in desvar.geo_cons:
             constraint.set_param(desvar)
         # desvar.gcs.constraint_params[self.gcs.constraint_params.index(param)] = desvar
 
@@ -687,27 +714,22 @@
             unit_type = "length"
         elif isinstance(desvar, AngleDesVar):
             unit_type = "angle"
         else:
             unit_type = None
 
         param = self.add_param(value=desvar.value(), name=desvar.name(), unit_type=unit_type, point=copy(desvar.point),
-                               root=desvar.root, rotation_handle=desvar.rotation_handle)
+                               root=desvar.root, rotation_handle=desvar.rotation_handle, assign_unique_name=False)
 
         # Replace the corresponding x() or y() in parameter with the new parameter
         self.replace_geo_objs(tool=desvar, target=param)
 
         # Make a copy of the geometry object reference list in the new parameter
         param.geo_objs = desvar.geo_objs.copy()
 
-        # Copy dimension information
-        param.dims = desvar.dims.copy()
-        for dim in param.dims:
-            dim.set_param(param)
-
         # Copy constraint information
         param.geo_cons = desvar.geo_cons
         param.gcs = self.gcs
         for constraint in param.geo_cons:
             constraint.set_param(param)
         # param.gcs.constraint_params[self.gcs.constraint_params.index(desvar)] = param
 
@@ -838,14 +860,15 @@
 
     def add_mea(self, airfoils: typing.List[Airfoil], name: str or None = None, assign_unique_name: bool = True):
         mea = MEA(airfoils=airfoils, name=name)
 
         return self.add_pymead_obj_by_ref(mea, assign_unique_name=assign_unique_name)
 
     def add_constraint(self, constraint: GeoCon, assign_unique_name: bool = True, **constraint_kwargs):
+        self.gcs.check_constraint_for_duplicates(constraint)
         self.add_pymead_obj_by_ref(constraint, assign_unique_name=assign_unique_name)
         if (constraint.param() is not None and constraint.param() not in self.container()["params"].values() and
                 constraint.param() not in self.container()["desvar"].values()):
             self.add_pymead_obj_by_ref(constraint.param())
         try:
             self.gcs.add_constraint(constraint)
             if isinstance(constraint, AntiParallel3Constraint):
@@ -864,25 +887,39 @@
             if self.gui_obj is not None:
                 # self.gui_obj.showColoredMessage("Constraint cluster is over-constrained. Removing constraint...",
                 #                                 4000, "#eb4034")
                 self.gui_obj.disp_message_box(str(e), message_mode="error")
             return
         return constraint
 
+    def equate_constraints(self, constraint1: GeoCon, constraint2: GeoCon):
+        if constraint1.__class__.__name__ != constraint2.__class__.__name__:
+            raise ValueError("Constraints must be of the same type to equate")
+
+        self.remove_pymead_obj(constraint2.param(), equating_constraints=True)
+        constraint2.set_param(constraint1.param())
+        constraint1.param().geo_cons.append(constraint2)
+
+        # Manually trigger an update by setting the value to the current value
+        constraint1.param().set_value(constraint1.param().value())
+
     def get_dict_rep(self):
         dict_rep = {k_outer: {k: v.get_dict_rep() for k, v in self.container()[k_outer].items()}
                     for k_outer in self.container().keys()}
         dict_rep["metadata"] = self.get_metadata()
         return dict_rep
 
     @staticmethod
     def get_metadata():
         return {
             "pymead_version": __version__,
-            "save_datetime": str(datetime.datetime.now())
+            "save_datetime": str(datetime.datetime.now()),
+            "length_unit": UNITS.current_length_unit(),
+            "angle_unit": UNITS.current_angle_unit(),
+            "area_unit": UNITS.current_area_unit()
         }
 
     @classmethod
     def set_from_dict_rep(cls, d: dict, canvas=None, tree=None, gui_obj=None):
         geo_col = cls(gui_obj=gui_obj)
         geo_col.canvas = canvas
         geo_col.tree = tree
@@ -928,31 +965,33 @@
         if "polylines" in d:
             for name, polyline_dict in d["polylines"].items():
                 geo_col.add_polyline(point_sequence=PointSequence(
                     points=[geo_col.container()["points"][k] for k in polyline_dict["points"]]),
                     source=polyline_dict["source"], start=polyline_dict["start"], end=polyline_dict["end"], name=name,
                     assign_unique_name=False)
         for name, bezier_dict in d["bezier"].items():
+            t_start = bezier_dict["t_start"] if "t_start" in bezier_dict else None
+            t_end = bezier_dict["t_end"] if "t_end" in bezier_dict else None
             geo_col.add_bezier(point_sequence=PointSequence(
                 points=[geo_col.container()["points"][k] for k in bezier_dict["points"]]),
-                name=name, assign_unique_name=False
+                name=name, t_start=t_start, t_end=t_end, assign_unique_name=False
             )
 
         constraints_added = []
         for name, geocon_dict in d["geocon"].items():
             for k, v in geocon_dict.items():
                 if v in d["points"].keys():
                     geocon_dict[k] = geo_col.container()["points"][v]
                 elif v in d["params"].keys():
                     geocon_dict[k] = geo_col.container()["params"][v]
                 elif v in d["desvar"].keys():
                     geocon_dict[k] = geo_col.container()["desvar"][v]
                 elif v in d["lines"].keys():
                     geocon_dict[k] = geo_col.container()["lines"][v]
-                elif v in d["polylines"].keys():
+                elif "polylines" in d and v in d["polylines"].keys():
                     geocon_dict[k] = geo_col.container()["polylines"][v]
                 elif v in d["bezier"].keys():
                     geocon_dict[k] = geo_col.container()["bezier"][v]
                 else:
                     pass
             constraint_type = geocon_dict.pop("constraint_type")
             constraint = getattr(sys.modules[__name__], constraint_type)(**geocon_dict, name=name)
@@ -966,14 +1005,58 @@
                                 lower_surf_end=geo_col.container()["points"][airfoil_dict["lower_surf_end"]],
                                 name=name, assign_unique_name=False)
         for name, mea_dict in d["mea"].items():
             geo_col.add_mea(airfoils=[geo_col.container()["airfoils"][k] for k in mea_dict["airfoils"]],
                             name=name, assign_unique_name=False)
         return geo_col
 
+    def switch_units(self, unit_type: str, old_unit: str, new_unit: str):
+
+        if old_unit == new_unit:
+            return
+
+        if unit_type == "length":
+            UNITS.set_current_length_unit(new_unit)
+        elif unit_type == "angle":
+            UNITS.set_current_angle_unit(new_unit)
+
+        def switch_unit_for_param(p: Param):
+            if isinstance(p, LengthParam) and unit_type == "length":
+                p.set_unit(new_unit, old_unit)
+
+            elif isinstance(p, AngleParam) and unit_type == "angle":
+                p.set_unit(new_unit, old_unit)
+
+        def switch_unit_for_point(p: Point):
+            if unit_type != "length":
+                return
+
+            new_x = p.x().set_unit(new_unit, old_unit, modify_value=False)
+            new_y = p.y().set_unit(new_unit, old_unit, modify_value=False)
+            p.request_move(new_x, new_y)
+
+        for param in self.container()["params"].values():
+            if param.point is not None:
+                continue
+            switch_unit_for_param(param)
+
+        for desvar in self.container()["desvar"].values():
+            if desvar.point is not None:
+                continue
+            switch_unit_for_param(desvar)
+
+        for point in self.container()["points"].values():
+            switch_unit_for_point(point)
+
+        if unit_type == "length" and self.canvas is not None:
+            x_data_range, y_data_range = self.canvas.getPointRange()
+            self.canvas.plot.getViewBox().setRange(xRange=x_data_range, yRange=y_data_range)
+            self.canvas.plot.setLabel(axis="bottom", text=f"x [{UNITS.current_length_unit()}]")
+            self.canvas.plot.setLabel(axis="left", text=f"y [{UNITS.current_length_unit()}]")
+
     def write_to_iges(self, base_dir: str, file_name: str, translation: typing.List[float] = None,
                       scaling: typing.List[float] = None, rotation: typing.List[float] = None,
                       transformation_order: str = None):
         """
         Writes all the Bézier curves in the geometry collection to an IGES file.
 
         Parameters
@@ -1032,7 +1115,78 @@
         bez_IGES_list = [BezierIGES(P) for P in transformed_cp_list]
 
         # Generate the IGES file
         iges_generator = IGESGenerator(bez_IGES_list)
         iges_generator.generate(full_file)
 
         return full_file
+
+    def verify_constraints(self):
+        for geo_con in self.container()["geocon"].values():
+            assert geo_con.verify()
+
+        return True
+
+    def verify_point_movement(self):
+        random.seed(1)
+        for point in self.container()["points"].values():
+            # Record the starting xy position of the point
+            old_xy = [point.x().value(), point.y().value()]
+            random_xy = [random.uniform(-5.0, 5.0), random.uniform(-5.0, 5.0)]
+            point.request_move(random_xy[0], random_xy[1])
+
+            self.verify_constraints()
+
+            # Return the point to its original position
+            point.request_move(old_xy[0], old_xy[1])
+
+        return True
+
+    def verify_desvar(self):
+        for desvar in self.container()["desvar"].values():
+
+            # Record the starting value of the design variable
+            old_value = desvar.value()
+
+            # To avoid issues with setting a length of 0, set the value close to 0 if the lower bound is 0
+            if isinstance(desvar, LengthParam) and np.isclose(desvar.lower(), 0.0):
+                desvar.set_value(0.0001)
+            else:
+                desvar.set_value(desvar.lower())
+
+            self.verify_constraints()
+
+            desvar.set_value(desvar.upper())
+
+            self.verify_constraints()
+
+            # Set the design variable to its original value
+            desvar.set_value(old_value)
+
+        return True
+
+    def verify_params(self):
+        random.seed(1)
+        for param in self.container()["params"].values():
+            # Record the starting value of the param
+            old_value = param.value()
+
+            if isinstance(param, LengthParam):
+                param.set_value(random.uniform(0.0001, 10.0))
+            elif isinstance(param, AngleParam):
+                param.set_value(random.uniform(0.0, 2 * np.pi))
+            else:
+                param.set_value(random.uniform(-10.0, 10.0))
+
+            self.verify_constraints()
+
+            param.set_value(old_value)
+
+        return True
+
+    def verify_all(self):
+        self.verify_constraints()
+        self.verify_point_movement()
+        self.verify_desvar()
+        self.verify_params()
+
+        return True
```

### Comparing `pymead-2.0.0b3/pymead/core/line.py` & `pymead-2.0.0b4/pymead/core/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,51 +133,63 @@
                         break
 
         return [polyline1, polyline2]
 
     def add_polyline_airfoil(self):
         le = self._add_le()
         te = self._add_te()
-        self._add_trailing_edge_lines(te)
-        self._add_airfoil(le, te)
+        blunt_trailing_edge = self._add_trailing_edge_lines(te)
+        self._add_airfoil(le, te, blunt_trailing_edge=blunt_trailing_edge)
 
     def _add_le(self):
         coords_dist_from_origin = np.hypot(self.coords[:, 0], self.coords[:, 1])
         le_row = np.argmin(coords_dist_from_origin)
         le = self.geo_col.add_point(self.coords[le_row, 0], self.coords[le_row, 1])
         le.curves.append(self)
         return le
 
     def _add_te(self):
+        if len(self.point_sequence().points()) == 1:
+            return self.point_sequence().points()[0]
         if self.coords[0, 1] >= 0.0 >= self.coords[-1, 1]:
             te = self.geo_col.add_point(1.0, 0.0)
         else:
             te = self.geo_col.add_point(0.5 * (self.coords[0, 0] + self.coords[-1, 0]),
                                         0.5 * (self.coords[0, 1] + self.coords[-1, 1]))
         return te
 
     def _add_trailing_edge_lines(self, te: Point):
+        if len(self.point_sequence().points()) == 1:
+            return False
         self.geo_col.add_line(PointSequence(points=[te, self.point_sequence().points()[0]]))
         self.geo_col.add_line(PointSequence(points=[te, self.point_sequence().points()[-1]]))
+        return True
 
-    def _add_airfoil(self, le: Point, te: Point):
-        self.geo_col.add_airfoil(le, te,
-                                 upper_surf_end=self.point_sequence().points()[0],
-                                 lower_surf_end=self.point_sequence().points()[-1])
+    def _add_airfoil(self, le: Point, te: Point, blunt_trailing_edge: bool):
+        if blunt_trailing_edge:
+            self.geo_col.add_airfoil(le, te,
+                                     upper_surf_end=self.point_sequence().points()[0],
+                                     lower_surf_end=self.point_sequence().points()[-1])
+        else:
+            self.geo_col.add_airfoil(le, te, upper_surf_end=te, lower_surf_end=te)
 
     def _get_default_name(self):
         if self.source_type == self.AirfoilTools:
             return f"{self.source}-1"
         return "PolyLine-1"
 
     def _get_original_coords(self):
         if self.source_type == self.AirfoilTools:
             return self._load_coords_from_airfoil_tools()
         elif self.source_type == self.DatFile:
-            return self._load_coords_from_dat_file(self.num_header_rows, self.delimiter)
+            try:
+                return self._load_coords_from_dat_file(self.num_header_rows, self.delimiter)
+            except:
+                self.num_header_rows = 1
+                return self._load_coords_from_dat_file(self.num_header_rows, self.delimiter)
         else:
             raise ValueError("Invalid polyline source type")
 
     def _get_coord_slice(self):
         if self.start is None and isinstance(self.end, int):
             return self.original_coords[:self.end, :]
         elif self.end is None and isinstance(self.start, int):
@@ -190,20 +202,18 @@
     def _load_coords_from_dat_file(self, num_header_rows: int = 0, delimiter: str or None = None):
         return np.loadtxt(self.source, skiprows=num_header_rows, delimiter=delimiter)
 
     def _load_coords_from_airfoil_tools(self):
         return extract_data_from_airfoiltools(self.source)
 
     def _extract_point_sequence_from_coords(self):
+        if Point(self.coords[0, 0], self.coords[0, 1]).is_coincident(Point(self.coords[-1, 0], self.coords[-1, 1])):
+            return PointSequence(points=[Point(self.coords[0, 0], self.coords[0, 1])])
         return PointSequence(points=[Point(self.coords[row, 0], self.coords[row, 1]) for row in [0, -1]])
 
-    def convert_airfoil_tools_airfoil_to_sequence_and_coords(self):
-        points = [Point(self.coords[row, 0], self.coords[row, 1]) for row in [0, 1, -2, -1]]
-        return PointSequence(points=points)
-
     def _add_references(self):
         for idx, point in enumerate(self.point_sequence().points()):
             # Add the object reference to each point in the curve
             if self not in point.curves:
                 point.curves.append(self)
 
     def point_sequence(self):
```

### Comparing `pymead-2.0.0b3/pymead/core/param.py` & `pymead-2.0.0b4/pymead/core/param.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import typing
-
 import networkx
 import numpy as np
 
 from pymead.core import UNITS
 from pymead.core.pymead_obj import PymeadObj
 
 
@@ -11,15 +9,15 @@
     """
     Base-level parameter in ``pymead``. Sub-classed by ``DesVar`` (design variable). Provides operator overloading and
     getter/setter methods.
     """
 
     def __init__(self, value: float or int, name: str, lower: float or None = None, upper: float or None = None,
                  sub_container: str = "params", setting_from_geo_col: bool = False, point=None, root=None,
-                 rotation_handle=None, enabled: bool = True):
+                 rotation_handle=None, enabled: bool = True, equation_str: str = None):
         """
         Parameters
         ==========
         value: float or int
             Starting value for the parameter.
 
         name: str
@@ -33,23 +31,27 @@
         """
         super().__init__(sub_container=sub_container)
 
         self.dtype = type(value).__name__
         self._value = None
         self._lower = None
         self._upper = None
+        self._enabled = None
         self.at_boundary = False
         self.point = point
         self.root = root
-        self.enabled = enabled
+        self.set_enabled(enabled)
         self.rotation_handle = rotation_handle
         if rotation_handle is not None:
             self.rotation_handle.rotation_param = self
         self.geo_objs = []
-        self.gcs = None
+        self.param_graph = None
+        self.equation_str = equation_str
+        self.equation = None
+        self.equation_dict = None
         self.geo_cons = []
         self.dims = []
         self.setting_from_geo_col = setting_from_geo_col
 
         if upper is not None and lower is not None:
             if upper < lower:
                 raise ValueError(f"Specified upper bound ({upper}) smaller than the specified lower bound ({lower})")
@@ -94,27 +96,37 @@
         if bounds_normalized:
             if self.lower() is None or self.upper() is None:
                 raise ValueError("Lower and upper bounds must be set to extract a bounds-normalized value.")
             return (self._value - self._lower) / (self._upper - self._lower)
         else:
             return self._value
 
-    def set_value(self, value: float or int, updated_objs: typing.List[PymeadObj] = None, bounds_normalized: bool = False):
+    def set_value(self, value: float or int, bounds_normalized: bool = False, force: bool = False,
+                  param_graph_update: bool = False):
         """
         Sets the design variable value, adjusting the value to fit inside the bounds if necessary.
 
         Parameters
         ==========
         value: float or int
             Design variable value
 
         bounds_normalized: bool
             Whether the specified value is normalized by the bounds (e.g., 0 if the value is equal to the lower bound,
             1 if the value is equal to the upper bound, or a float between 0.0 and 1.0 if the value is somewhere
             between the bounds). Default: ``False``
+
+        force: bool
+            Whether to force the change in value. This keyword argument should never be set to ``True`` when using
+            the API. Default: ``False``
+
+        param_graph_update: bool
+            Whether this value is being set as part of a parameter graph update. Used to prevent the parameter graph
+            from triggering multiple updates for the same parameter. This keyword argument should never
+            be set to ``True`` when using the API. Default: ``False``
         """
         def rotate_cluster(new_v):
             if self.gcs is None:
                 return
             points_to_update, root = self.gcs.rotate_cluster(self.rotation_handle, new_rotation_angle=new_v)
             constraints_to_update = []
             for point in networkx.dfs_preorder_nodes(self.gcs, source=root):
@@ -142,49 +154,53 @@
                 curve.update()
 
             for airfoil in airfoils_to_update:
                 airfoil.update_coords()
                 if airfoil.canvas_item is not None:
                     airfoil.canvas_item.generatePicture()
 
-        if bounds_normalized:
-            if self.lower() is None or self.upper() is None:
-                raise ValueError("Lower and upper bounds must be set to assign a bounds-normalized value.")
-            value = value * (self._upper - self._lower) + self._lower
+        if not force:
 
-        if self._lower is not None and value < self._lower:  # If below the lower bound,
-            # set the value equal to the lower bound
-            self._value = self._lower
-            self.at_boundary = True
-        elif self._upper is not None and value > self._upper:  # If above the upper bound,
-            # set the value equal to the upper bound
-            self._value = self._upper
-            self.at_boundary = True
-        else:  # Otherwise, use the default behavior for Param.
-            self._value = value
-            self.at_boundary = False
+            if bounds_normalized:
+                if self.lower() is None or self.upper() is None:
+                    raise ValueError("Lower and upper bounds must be set to assign a bounds-normalized value.")
+                value = value * (self._upper - self._lower) + self._lower
+
+            if self._lower is not None and value < self._lower:  # If below the lower bound,
+                # set the value equal to the lower bound
+                self._value = self._lower
+                self.at_boundary = True
+            elif self._upper is not None and value > self._upper:  # If above the upper bound,
+                # set the value equal to the upper bound
+                self._value = self._upper
+                self.at_boundary = True
+            else:  # Otherwise, use the default behavior for Param.
+                self._value = value
+                self.at_boundary = False
 
-        if self.rotation_handle is not None:
-            rotate_cluster(self._value)
+            if self.rotation_handle is not None:
+                rotate_cluster(self._value)
 
-        if self.at_boundary:
-            return
+            if self.at_boundary:
+                return
 
-        updated_objs = [] if updated_objs is None else updated_objs
+            if self.gcs is not None and self.geo_cons:
+                points_solved = []
+                for gc in self.geo_cons:
+                    points_solved.extend(self.gcs.solve(gc))
+                self.gcs.update_canvas_items(list(set(points_solved)))
+
+            if self.param_graph is not None and not param_graph_update and self in self.param_graph.nodes:
+                for node in networkx.dfs_preorder_nodes(self.param_graph, source=self):
+                    if not node.equation_str:
+                        continue
+                    node.evaluate_equation()
 
-        if self in updated_objs:
-            return
         else:
-            updated_objs.append(self)
-            for dim in self.dims:
-                dim.update_points_from_param(updated_objs=updated_objs)
-
-        if self.gcs is not None and self.geo_cons:
-            points_solved = self.gcs.solve(self.geo_cons[0])
-            self.gcs.update_canvas_items(points_solved)
+            self._value = value
 
         if self.tree_item is not None:
             self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setValue(self.value())
 
     def lower(self):
         """
         Returns the lower bound for the design variable
@@ -203,54 +219,109 @@
         Returns
         =======
         float
             DV upper bound
         """
         return self._upper
 
-    def set_lower(self, lower: float):
+    def set_lower(self, lower: float, force: bool = False):
         """
         Sets the lower bound for the design variable. If called from outside ``DesVar.__init__()``, adjust the design
         variable value to fit inside the bounds if necessary.
 
         Parameters
         ==========
         lower: float
             Lower bound for the design variable
+
+        force: bool
+            Setting this argument to ``True`` ignores the check for lower bound greater than value. Default: ``False``
         """
-        if lower > self.value():
+        if lower > self.value() and not force:
             return
 
         self._lower = lower
 
         if self.tree_item is not None:
             self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setMinimum(self.lower())
 
-    def set_upper(self, upper: float):
+    def set_upper(self, upper: float, force: bool = False):
         """
         Sets the upper bound for the design variable. If called from outside ``DesVar.__init__()``, adjust the design
         variable value to fit inside the bounds if necessary.
 
         Parameters
         ==========
         upper: float
             Upper bound for the design variable
+
+        force: bool
+            Setting this argument to ``True`` ignores the check for upper bound less than value. Default: ``False``
         """
-        if upper < self.value():
+        if upper < self.value() and not force:
             return
 
         self._upper = upper
 
         if self.tree_item is not None:
             self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setMaximum(self.upper())
 
+    def enabled(self):
+        return self._enabled
+
+    def set_enabled(self, enabled: bool):
+        self._enabled = enabled
+        if self.tree_item is not None:
+            self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setEnabled(enabled)
+
+    def update_equation(self, equation_str: str = None):
+        if not equation_str:  # Handles both the None and empty-string cases
+            self.equation_str = equation_str
+            self.equation = None
+            self.equation_dict = None
+            return
+        if self.param_graph is None:
+            return
+        self.equation = "def f(): return "
+        self.equation_dict = {"p": {}}
+        equation_split = equation_str.split()
+        param_names = [param.name() for param in self.param_graph.param_list]
+        for idx, sub_str in enumerate(equation_split):
+            if sub_str[0] != "$":
+                self.equation += sub_str
+                continue
+            param_name = sub_str.strip("$")
+            if param_name in param_names:
+                self.equation_dict["p"][param_name] = self.param_graph.param_list[param_names.index(param_name)]
+            else:
+                raise EquationCompileError("Failed to compile")
+            self.equation += f"p['{param_name}'].value()"
+
+        for param in self.equation_dict["p"].values():
+            self.param_graph.add_edge(param, self)
+        if len(self.param_graph.nodes) != 0 and not networkx.is_forest(self.param_graph):
+            # Revert to the original equation string
+            self.update_equation(self.equation_str)
+            raise EquationCompileError("The dependencies for this equation create a closed loop")
+
+        self.evaluate_equation()
+
+        self.equation_str = equation_str
+
+    def evaluate_equation(self):
+        try:
+            exec(self.equation, self.equation_dict)
+            self.set_value(self.equation_dict["f"](), param_graph_update=True)
+        except (NameError, SyntaxError) as e:
+            raise EquationCompileError(str(e))
+
     def get_dict_rep(self):
         return {"value": float(self.value()) if self.dtype == "float" else int(self.value()),
                 "lower": self.lower(), "upper": self.upper(),
-                "unit_type": None, "enabled": self.enabled}
+                "unit_type": None, "enabled": self.enabled(), "equation_str": self.equation_str}
 
     @classmethod
     def set_from_dict_rep(cls, d: dict):
         if "lower" not in d.keys():
             d["lower"] = None
         if "upper" not in d.keys():
             d["upper"] = None
@@ -285,173 +356,147 @@
 
     def __abs__(self):
         return self.__class__(value=abs(self.value()), name="absolute_value_result")
 
     def __pow__(self, power, modulo=None):
         return self.__class__(value=self.value() ** power, name="power_result")
 
-    # def __eq__(self, other):
-    #     return self.value() == other.value()
-    #
-    # def __ne__(self, other):
-    #     return self.value() != other.value()
-
 
 class LengthParam(Param):
     def __init__(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
                  sub_container: str = "params",
-                 setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None, enabled: bool = True):
+                 setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None, enabled: bool = True,
+                 equation_str: str = None):
         self._unit = None
         self.set_unit(UNITS.current_length_unit())
         name = "Length-1" if name is None else name
         super().__init__(value=value, name=name, lower=lower, upper=upper, sub_container=sub_container,
                          setting_from_geo_col=setting_from_geo_col,
-                         point=point, root=root, rotation_handle=rotation_handle, enabled=enabled)
+                         point=point, root=root, rotation_handle=rotation_handle, enabled=enabled,
+                         equation_str=equation_str)
 
     def unit(self):
         return self._unit
 
-    def set_unit(self, unit: str or None = None):
+    def set_unit(self, unit: str or None = None, old_unit: str = None, modify_value: bool = True):
         if unit is not None:
             self._unit = unit
         else:
             self._unit = UNITS.current_length_unit()
 
-    def lower(self):
-        return UNITS.convert_length_from_base(self._lower, self.unit())
+        if old_unit is None:
+            return
 
-    def upper(self):
-        return UNITS.convert_length_from_base(self._upper, self.unit())
+        lower = self.lower()
+        upper = self.upper()
+        value = self.value()
+        if lower is not None:
+            base_lower = UNITS.convert_length_to_base(lower, old_unit)
+            self.set_lower(UNITS.convert_length_from_base(base_lower, unit), force=True)
+        if upper is not None:
+            base_upper = UNITS.convert_length_to_base(upper, old_unit)
+            self.set_upper(UNITS.convert_length_from_base(base_upper, unit), force=True)
 
-    def value(self, bounds_normalized: bool = False):
-        new_value = super().value(bounds_normalized=bounds_normalized)
-        if bounds_normalized:
-            return new_value
-        else:
-            return UNITS.convert_length_from_base(new_value, self.unit())
+        base_value = UNITS.convert_length_to_base(value, old_unit)
+        new_value = UNITS.convert_length_from_base(base_value, unit)
+        if modify_value:
+            self.set_value(new_value)
+
+        if self.tree_item is not None:
+            self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setSuffix(f" {unit}")
+
+        return new_value
 
-    def set_lower(self, lower: float):
+    def set_lower(self, lower: float, force: bool = False):
         if self.point is None and lower < 0.0:
             lower = 0.0
 
-        return super().set_lower(UNITS.convert_length_to_base(lower, self.unit()))
-
-    def set_upper(self, upper: float):
-        return super().set_upper(UNITS.convert_length_to_base(upper, self.unit()))
+        return super().set_lower(lower, force=force)
 
-    def set_value(self, value: float, updated_objs: typing.List[PymeadObj] = None, bounds_normalized: bool = False):
+    def set_value(self, value: float, bounds_normalized: bool = False, force: bool = False,
+                  param_graph_update: bool = False):
 
         # Negative lengths are prohibited unless this represents a point
         if self.point is None and value < 0.0:
             return
 
-        new_value = UNITS.convert_length_to_base(value, self.unit())
-        return super().set_value(new_value, updated_objs=updated_objs, bounds_normalized=bounds_normalized)
+        return super().set_value(value, bounds_normalized=bounds_normalized, force=force,
+                                 param_graph_update=param_graph_update)
 
     def get_dict_rep(self):
         return {"value": float(self.value()), "lower": self.lower(), "upper": self.upper(),
-                "unit_type": "length", "enabled": self.enabled}
+                "unit_type": "length", "enabled": self.enabled(), "equation_str": self.equation_str}
 
 
 class AngleParam(Param):
     def __init__(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
                  sub_container: str = "params",
                  setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None,
-                 enabled: bool = True):
+                 enabled: bool = True, equation_str: str = None):
         self._unit = None
         self.set_unit(UNITS.current_angle_unit())
         name = "Angle-1" if name is None else name
         super().__init__(value=value, name=name, lower=lower, upper=upper, sub_container=sub_container,
                          setting_from_geo_col=setting_from_geo_col, point=point, root=root,
-                         rotation_handle=rotation_handle, enabled=enabled)
+                         rotation_handle=rotation_handle, enabled=enabled, equation_str=equation_str)
 
     def unit(self):
         return self._unit
 
-    def set_unit(self, unit: str or None = None):
+    def set_unit(self, unit: str or None = None, old_unit: str or None = None):
         if unit is not None:
             self._unit = unit
         else:
             self._unit = UNITS.current_angle_unit()
 
-    def lower(self):
-        return UNITS.convert_angle_from_base(self._lower, self.unit())
+        if old_unit is None:
+            return
 
-    def upper(self):
-        return UNITS.convert_angle_from_base(self._upper, self.unit())
+        lower = self.lower()
+        upper = self.upper()
+        value = self.value()
+        if lower is not None:
+            base_lower = UNITS.convert_angle_to_base(lower, old_unit)
+            self.set_lower(UNITS.convert_angle_from_base(base_lower, unit), force=True)
+        if upper is not None:
+            base_upper = UNITS.convert_angle_to_base(upper, old_unit)
+            self.set_upper(UNITS.convert_angle_from_base(base_upper, unit), force=True)
+        base_value = UNITS.convert_angle_to_base(value, old_unit)
+        self.set_value(UNITS.convert_angle_from_base(base_value, unit))
 
-    def value(self, bounds_normalized: bool = False):
-        new_value = super().value(bounds_normalized=bounds_normalized)
-        if bounds_normalized:
-            return new_value
-        else:
-            return UNITS.convert_angle_from_base(new_value, self.unit())
+        if self.tree_item is not None:
+            self.tree_item.treeWidget().itemWidget(self.tree_item, 1).setSuffix(f" {unit}")
 
     def rad(self):
         """
         Returns the value of the angle parameter in radians, the base angle unit of pymead
 
         Returns
         =======
         float
             Angle in radians
         """
-        return self._value
+        return UNITS.convert_angle_to_base(self._value, self.unit())
 
-    def set_lower(self, lower: float):
-        return super().set_lower(UNITS.convert_angle_to_base(lower, self.unit()))
-
-    def set_upper(self, upper: float):
-        return super().set_upper(UNITS.convert_angle_to_base(upper, self.unit()))
-
-    def set_value(self, value: float, updated_objs: typing.List[PymeadObj] = None, bounds_normalized: bool = False):
+    def set_value(self, value: float, bounds_normalized: bool = False, force: bool = False,
+                  param_graph_update: bool = False):
 
         new_value = UNITS.convert_angle_to_base(value, self.unit())
-
         zero_to_2pi_value = new_value % (2 * np.pi)
+        new_value = UNITS.convert_angle_from_base(zero_to_2pi_value, self.unit())
 
-        return super().set_value(zero_to_2pi_value, updated_objs=updated_objs, bounds_normalized=bounds_normalized)
+        return super().set_value(new_value, bounds_normalized=bounds_normalized, force=force,
+                                 param_graph_update=param_graph_update)
 
     def get_dict_rep(self):
         return {"value": float(self.value()), "lower": self.lower(), "upper": self.upper(),
                 "unit_type": "angle",
                 "root": self.root.name() if self.root is not None else None,
                 "rotation_handle": self.rotation_handle.name() if self.rotation_handle is not None else None,
-                "enabled": self.enabled}
-
-
-# class ParamCollection:
-#     """
-#     Collection (list) of Params. Allows for import from/export to array.
-#     """
-#     def __init__(self, params: typing.List[Param]):
-#         self._params = None
-#         self.set_params(params)
-#         self.shape = len(self.params())
-#
-#     def params(self):
-#         return self._params
-#
-#     def set_params(self, params: typing.List[Param]):
-#         self._params = params
-#
-#     def as_array(self):
-#         return np.array([[p.value()] for p in self.params()])
-#
-#     @classmethod
-#     def generate_from_array(cls, arr: np.ndarray):
-#         if arr.ndim == 1:
-#             return cls(params=[Param(value=v, name=f"FromArrayIndex{idx}") for idx, v in enumerate(arr)])
-#         elif arr.ndim == 2:
-#             if arr.shape[1] != 1:
-#                 raise ValueError(f"Shape of the input array must be Nx1 (found {arr.shape = })")
-#             return cls(params=[Param(value=v, name=f"FromArrayIndex{idx}") for idx, v in enumerate(arr[:, 0])])
-#
-#     def __len__(self):
-#         return len(self.params())
+                "enabled": self.enabled(), "equation_str": self.equation_str}
 
 
 def default_lower(value: float):
     if -0.1 <= value <= 0.1:
         return value - 0.02
     else:
         if value < 0.0:
@@ -472,15 +517,15 @@
 
 class DesVar(Param):
     """
     Design variable class; subclasses the base-level Param. Adds lower and upper bound default behavior.
     """
     def __init__(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
                  sub_container: str = "desvar", setting_from_geo_col: bool = False, point=None, root=None,
-                 rotation_handle=None, enabled: bool = True):
+                 rotation_handle=None, enabled: bool = True, equation_str: str = None):
         """
         Parameters
         ==========
         value: float
             Starting value of the design variable
 
         name: str
@@ -502,25 +547,25 @@
 
         # Default behavior for upper bound
         if upper is None:
             upper = default_upper(value)
 
         super().__init__(value=value, name=name, lower=lower, upper=upper, sub_container=sub_container,
                          setting_from_geo_col=setting_from_geo_col, point=point, root=root,
-                         rotation_handle=rotation_handle, enabled=enabled)
+                         rotation_handle=rotation_handle, enabled=enabled, equation_str=equation_str)
 
 
 class LengthDesVar(LengthParam):
     """
     Design variable class for length values; subclasses the base-level Param. Adds lower and upper bound
     default behavior.
     """
     def __init__(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
                  setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None,
-                 enabled: bool = True):
+                 enabled: bool = True, equation_str: str = None):
         """
         Parameters
         ==========
         value: float
             Starting value of the design variable
 
         name: str
@@ -542,28 +587,29 @@
 
         # Default behavior for upper bound
         if upper is None:
             upper = default_upper(value)
 
         super().__init__(value=value, name=name, lower=lower, upper=upper, setting_from_geo_col=setting_from_geo_col,
                          sub_container="desvar", point=point, root=root, rotation_handle=rotation_handle,
-                         enabled=enabled)
+                         enabled=enabled, equation_str=equation_str)
 
     def get_dict_rep(self):
         return {"value": float(self.value()), "lower": self.lower(), "upper": self.upper(),
-                "unit_type": "length", "enabled": self.enabled}
+                "unit_type": "length", "enabled": self.enabled(), "equation_str": self.equation_str}
 
 
 class AngleDesVar(AngleParam):
     """
     Design variable class for angle values; subclasses the base-level Param. Adds lower and upper bound
     default behavior.
     """
     def __init__(self, value: float, name: str, lower: float or None = None, upper: float or None = None,
-                 setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None, enabled: bool = True):
+                 setting_from_geo_col: bool = False, point=None, root=None, rotation_handle=None, enabled: bool = True,
+                 equation_str: str = None):
         """
         Parameters
         ==========
         value: float
             Starting value of the design variable
 
         name: str
@@ -585,25 +631,30 @@
 
         # Default behavior for upper bound
         if upper is None:
             upper = default_upper(value)
 
         super().__init__(value=value, name=name, lower=lower, upper=upper, sub_container="desvar",
                          setting_from_geo_col=setting_from_geo_col, point=point, root=root,
-                         rotation_handle=rotation_handle, enabled=enabled)
+                         rotation_handle=rotation_handle, enabled=enabled, equation_str=equation_str)
 
-    def set_value(self, value: float, updated_objs: typing.List[PymeadObj] = None, bounds_normalized: bool = False):
+    def set_value(self, value: float, bounds_normalized: bool = False, force: bool = False,
+                  param_graph_update: bool = False):
         r"""
         In this special case of ``set_value`` for an ``AngleDesVar``, we skip over the call to the ``set_value``
         method in ``AngleParam`` and directly call the ``set_value`` method in ``Param`` (the grandparent class).
         The reason for this is that ``AngleParam`` always keeps the angle between 0 and :math:`2 \pi`, which is not
         logical behavior for a bounded variable. This method eliminates that restriction.
         """
-        new_value = UNITS.convert_angle_to_base(value, self.unit())
-        return Param.set_value(self, new_value, updated_objs=updated_objs, bounds_normalized=bounds_normalized)
+        return Param.set_value(self, value, bounds_normalized=bounds_normalized, force=force,
+                               param_graph_update=param_graph_update)
 
     def get_dict_rep(self):
         return {"value": float(self.value()), "lower": self.lower(), "upper": self.upper(),
                 "unit_type": "angle",
                 "root": self.root.name() if self.root is not None else None,
                 "rotation_handle": self.rotation_handle.name() if self.rotation_handle is not None else None,
-                "enabled": self.enabled}
+                "enabled": self.enabled(), "equation_str": self.equation_str}
+
+
+class EquationCompileError(Exception):
+    pass
```

### Comparing `pymead-2.0.0b3/pymead/core/parametric_curve.py` & `pymead-2.0.0b4/pymead/core/parametric_curve.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/core/point.py` & `pymead-2.0.0b4/pymead/core/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,30 @@
             if geo_con.__class__.__name__ == "SymmetryConstraint":
                 symmetry_constraints.append(geo_con)
         for symmetry_constraint in symmetry_constraints:
             if self is symmetry_constraint.p4:
                 return False
         return symmetry_constraints
 
+    def _is_symmetry_target_and_has_edges(self) -> bool:
+        if self.gcs is None:
+            return False
+        if (not [edge for edge in self.gcs.in_edges(nbunch=self)] and
+            not [edge for edge in self.gcs.out_edges(nbunch=self)]):
+            return False
+        symmetry_constraints = []
+        for geo_con in self.geo_cons:
+            if geo_con.__class__.__name__ == "SymmetryConstraint":
+                symmetry_constraints.append(geo_con)
+        if not symmetry_constraints:
+            return False
+        if not any([self is symmetry_constraint.p4 for symmetry_constraint in symmetry_constraints]):
+            return False
+        return True
+
     def is_movement_allowed(self) -> bool:
         """
         This method determines if movement is allowed for the point. Movement is allowed in these cases:
 
         - Where the constraint solver has not been set or there are no geometric constraints attached
         - Where the point is a root or rotation handle of a constraint cluster. If a rotation handle, movement is
           allowed, but the movement gets accepted as a rotation about the root point with a fixed distance to the
@@ -267,14 +283,20 @@
                     self.gcs.solve_symmetry_constraint(symmetry_constraint)
                     points_to_update.extend(symmetry_constraint.child_nodes)
                 points_to_update = list(set(points_to_update))  # Get only the unique points
                 for symmetry_constraint in symmetry_constraints:
                     if symmetry_constraint.canvas_item is not None:
                         symmetry_constraint.canvas_item.update()
 
+        if self._is_symmetry_target_and_has_edges():
+            points_solved = []
+            for gc in self.geo_cons:
+                points_solved.extend(self.gcs.solve(gc))
+            self.gcs.update_canvas_items(list(set(points_solved)))
+
         # Update the GUI object, if there is one
         if self.canvas_item is not None:
             self.canvas_item.updateCanvasItem(self.x().value(), self.y().value())
 
         if points_to_update is None:
             return
```

### Comparing `pymead-2.0.0b3/pymead/core/pymead_obj.py` & `pymead-2.0.0b4/pymead/core/pymead_obj.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         memo[id(self)] = result
         for k, v in self.__dict__.items():
 
             # Eliminate any GUI references so the object is deep-copyable
             if k in self.non_serializable_attributes:
                 v = None
 
+            if k == "equation_dict" and isinstance(v, dict) and "__builtins__" in v:
+                v["__builtins__"] = None
+
             setattr(result, k, deepcopy(v, memo))
         return result
 
 
 class PymeadObj(ABC, DualRep):
     """
     Base class for all objects in pymead.
```

### Comparing `pymead-2.0.0b3/pymead/core/spline.py` & `pymead-2.0.0b4/pymead/core/spline.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/core/transformation.py` & `pymead-2.0.0b4/pymead/core/transformation.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/core/units.py` & `pymead-2.0.0b4/pymead/core/units.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/airfoil_matching.py` & `pymead-2.0.0b4/pymead/examples/airfoil_matching.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/complex_airfoil.py` & `pymead-2.0.0b4/pymead/examples/complex_airfoil.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/high_lift.py` & `pymead-2.0.0b4/pymead/examples/high_lift.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/iges_generation.py` & `pymead-2.0.0b4/pymead/examples/iges_generation.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/mirrored_subsection.py` & `pymead-2.0.0b4/pymead/examples/mirrored_subsection.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/propulsion_airframe_integration.py` & `pymead-2.0.0b4/pymead/examples/propulsion_airframe_integration.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/simple_airfoil.py` & `pymead-2.0.0b4/pymead/examples/simple_airfoil.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/examples/symm_airfoil.py` & `pymead-2.0.0b4/pymead/examples/symm_airfoil.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/aero_forces_graphs.py` & `pymead-2.0.0b4/pymead/gui/aero_forces_graphs.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/airfoil_canvas.py` & `pymead-2.0.0b4/pymead/gui/airfoil_canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import numpy as np
 import pyqtgraph as pg
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtSignal, QEventLoop, Qt
 from PyQt5.QtGui import QFont, QBrush, QColor
 from PyQt5.QtWidgets import QApplication
 
+from pymead.utils.get_airfoil import AirfoilNotFoundError
 from pymead.core.line import PolyLine
-from pymead.gui.input_dialog import PlotExportDialog, WebAirfoilDialog, SplitPolylineDialog
+from pymead.gui.dialogs import PlotExportDialog, WebAirfoilDialog, SplitPolylineDialog
 from pymead.gui.polygon_item import PolygonItem
 
 from pymead.core.airfoil import Airfoil
 
 from pymead.core.constraints import *
 from pymead.core.constraint_equations import *
 from pymead.core.geometry_collection import GeometryCollection
@@ -162,15 +163,17 @@
             # Set the style
             point_gui.setScatterStyle("default")
 
             # Connect signals
             point_gui.sigPointClicked.connect(self.pointClicked)
             point_gui.sigPointHovered.connect(self.pointHovered)
             point_gui.sigPointLeaveHovered.connect(self.pointLeaveHovered)
-            point_gui.sigPointMoved.connect(self.pointMoved)
+            point_gui.sigPointStartedMoving.connect(self.pointStartedMoving)
+            point_gui.sigPointMoving.connect(self.pointMoving)
+            point_gui.sigPointFinishedMoving.connect(self.pointFinishedMoving)
 
             # Add the point to the plot
             self.addItem(point_gui)
 
         elif isinstance(pymead_obj, ParametricCurve):
             # Create the canvas item
             curve_item = HoverableCurve(curve_type=pymead_obj.curve_type)
@@ -222,14 +225,22 @@
         if self.enter_connection is None:
             return
 
         self.sigEnterPressed.disconnect(self.enter_connection)
         self.enter_connection = None
 
     @staticmethod
+    def undoRedoAction(action: typing.Callable):
+        def wrapped(self, *args, **kwargs):
+            self.gui_obj.undo_stack.append(deepcopy(self.geo_col.get_dict_rep()))
+            action(self, *args, **kwargs)
+
+        return wrapped
+
+    @staticmethod
     def runSelectionEventLoop(drawing_object: str, starting_message: str, enter_callback: typing.Callable = None):
         drawing_object = drawing_object
         starting_message = starting_message
 
         def decorator(action: typing.Callable):
             def wrapped(self, *args, **kwargs):
                 self.drawing_object = drawing_object
@@ -239,43 +250,51 @@
                 if enter_callback:
                     self.enter_connection = self.sigEnterPressed.connect(partial(enter_callback, self))
                 else:
                     self.sigEnterPressed.connect(loop.quit)
                 self.sigEscapePressed.connect(loop.quit)
                 loop.exec()
                 # if len(self.geo_col.selected_objects["points"]) > 0:
-                action(self, *args, **kwargs)
+
+                try:
+                    action(self, *args, **kwargs)
+                except ValueError as e:
+                    self.gui_obj.disp_message_box(str(e))
+
                 self.clearSelectedObjects()
                 # elif len(self.geo_col.selected_objects["airfoils"]) > 0:
                 #     action(self, *args, **kwargs)
                 #     self.clearSelectedObjects()
                 self.drawing_object = None
                 self.sigStatusBarUpdate.emit("", 0)
                 if enter_callback:
                     self.closeEnterCallbackConnection()
             return wrapped
         return decorator
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="Points", starting_message="Left click on the canvas to draw a point. "
                                                                      "Press Escape to stop drawing points.")
     def drawPoints(self):
         pass
 
+    @undoRedoAction
     def drawBezierNoEvent(self):
         if len(self.geo_col.selected_objects["points"]) < 2:
             msg = f"Choose at least 2 points to define a curve"
             self.sigStatusBarUpdate.emit(msg, 2000)
             return
 
         point_sequence = PointSequence([pt for pt in self.geo_col.selected_objects["points"]])
         self.geo_col.add_bezier(point_sequence=point_sequence)
 
         self.clearSelectedObjects()
         self.sigStatusBarUpdate.emit("Select the first Bezier control point of the next curve", 0)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="Bezier", starting_message="Select the first Bezier control point")
     def drawBezier(self):
         if len(self.geo_col.selected_objects["points"]) < 2:
             msg = f"Choose at least 2 points to define a curve"
             self.sigStatusBarUpdate.emit(msg, 2000)
             return
 
@@ -286,31 +305,34 @@
                            enter_callback=drawBezierNoEvent)
     def drawBeziers(self):
         if len(self.geo_col.selected_objects["points"]) < 2:
             msg = f"Choose at least 2 points to define a curve"
             self.sigStatusBarUpdate.emit(msg, 2000)
             return
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="LineSegment", starting_message="Select the first line endpoint")
     def drawLineSegment(self):
         if len(self.geo_col.selected_objects["points"]) < 2:
             msg = f"Choose at least 2 points to define a curve"
             self.sigStatusBarUpdate.emit(msg, 2000)
             return
 
         point_sequence = PointSequence([pt for pt in self.geo_col.selected_objects["points"]])
         self.geo_col.add_line(point_sequence=point_sequence)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="LineSegments", starting_message="Select the first line endpoint")
     def drawLines(self):
         if len(self.geo_col.selected_objects["points"]) < 2:
             msg = f"Choose at least 2 points to define a curve"
             self.sigStatusBarUpdate.emit(msg, 2000)
             return
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="Airfoil", starting_message="Select the leading edge point")
     def generateAirfoil(self):
         if len(self.geo_col.selected_objects["points"]) not in [2, 4]:
             self.sigStatusBarUpdate.emit(
                 "Choose either 2 points (sharp trailing edge) or 4 points (blunt trailing edge)"
                 " to generate an airfoil", 4000)
             return
@@ -324,30 +346,37 @@
             upper_surf_end = te
             lower_surf_end = te
 
         self.geo_col.add_airfoil(leading_edge=le, trailing_edge=te, upper_surf_end=upper_surf_end,
                                  lower_surf_end=lower_surf_end)
         self.gui_obj.permanent_widget.updateAirfoils()
 
+    @undoRedoAction
     def generateWebAirfoil(self):
         dialog = WebAirfoilDialog(self, theme=self.gui_obj.themes[self.gui_obj.current_theme])
         if dialog.exec_():
-            polyline = self.geo_col.add_polyline(source=dialog.valuesFromWidgets())
+            try:
+                polyline = self.geo_col.add_polyline(source=dialog.value())
+            except AirfoilNotFoundError as e:
+                self.gui_obj.disp_message_box(f"{e}", message_mode="error")
+                return
             polyline.add_polyline_airfoil()
         self.gui_obj.permanent_widget.updateAirfoils()
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="MEA", starting_message="Select the first airfoil")
     def generateMEA(self):
         if len(self.geo_col.selected_objects["airfoils"]) == 0:
             self.sigStatusBarUpdate.emit("Must choose at least 1 airfoil for a multi-element airfoil (MEA) object",
                                          4000)
             return
 
         self.geo_col.add_mea(airfoils=self.geo_col.selected_objects["airfoils"].copy())
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="DistanceConstraint", starting_message="Select the first point")
     def addDistanceConstraint(self):
         if len(self.geo_col.selected_objects["points"]) != 2:
             self.sigStatusBarUpdate.emit("Choose exactly two points to define a distance constraint", 4000)
             return
 
         # p1 = self.geo_col.selected_objects["points"][0]
@@ -355,26 +384,28 @@
         #
         # cnstr = self.geo_col.add_distance_constraint(p1, p2)
         # cnstr.add_constraint_to_gcs()
 
         constraint = DistanceConstraint(*self.geo_col.selected_objects["points"])
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="RelAngle3Constraint", starting_message="Select any point other than "
                                                                                   "the vertex")
     def addRelAngle3Constraint(self):
         if len(self.geo_col.selected_objects["points"]) != 3:
             msg = (f"Choose exactly three points (start, vertex, and end) for a "
                    f"relative angle 3 constraint")
             self.sigStatusBarUpdate.emit(msg, 4000)
             return
 
         constraint = RelAngle3Constraint(*self.geo_col.selected_objects["points"])
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="AntiParallel3Constraint", starting_message="Select any point other than "
                                                                                       "the vertex")
     def addAntiParallel3Constraint(self):
         if len(self.geo_col.selected_objects["points"]) == 3:
             case = 0
         elif len(self.geo_col.selected_objects["points"]) == 2 and len(self.geo_col.selected_objects["polylines"]) == 1:
             case = 1
@@ -404,65 +435,70 @@
 
             args = [point, *self.geo_col.selected_objects["points"]] if point_is_first_arg else \
                 [*self.geo_col.selected_objects["points"], point]
             constraint = AntiParallel3Constraint(*args, polyline=self.geo_col.selected_objects["polylines"][0],
                                                  point_on_curve=point)
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="SymmetryConstraint", starting_message="Select the start point of the "
                                                                                  "mirror axis")
     def addSymmetryConstraint(self):
         if len(self.geo_col.selected_objects["points"]) != 4:
             msg = (f"Choose exactly four points (mirror axis start, mirror axis end, tool point, and target point) "
                    f"for a symmetry constraint")
             self.sigStatusBarUpdate.emit(msg, 4000)
             return
 
         constraint = SymmetryConstraint(*self.geo_col.selected_objects["points"])
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="Perp3Constraint", starting_message="Select the first point (not the vertex)")
     def addPerp3Constraint(self):
         if len(self.geo_col.selected_objects["points"]) != 3:
             msg = f"Choose exactly three points (start, vertex, and end) for a Perp3Constraint"
             self.sigStatusBarUpdate.emit(msg, 4000)
             return
         constraint = Perp3Constraint(*self.geo_col.selected_objects["points"])
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="ROCurvatureConstraint", starting_message="Select the curve joint")
     def addROCurvatureConstraint(self):
         if len(self.geo_col.selected_objects["points"]) != 1:
             msg = (f"Choose exactly one point (the curve joint) for a "
                    f"radius of curvature constraint")
             self.sigStatusBarUpdate.emit(msg, 4000)
             return
 
         constraint = ROCurvatureConstraint(*self.geo_col.selected_objects["points"])
         self.geo_col.add_constraint(constraint)
 
+    @undoRedoAction
     @runSelectionEventLoop(drawing_object="BezierAddPoint",
                            starting_message="First, click the point to add to the curve")
     def addPointToCurve(self, curve_item: HoverableCurve):
         if len(self.geo_col.selected_objects["points"]) != 2:
             msg = (f"Choose exactly two points (the point to add, then the preceding point in the curve) to add"
                    f" a point to a Bezier curve")
             self.sigStatusBarUpdate.emit(msg, 4000)
             return
         bezier_curve = curve_item.parametric_curve
         point_to_add = self.geo_col.selected_objects["points"][0]
         preceding_point = self.geo_col.selected_objects["points"][1]
         bezier_curve.insert_point_after_point(point_to_add, preceding_point)
 
+    @undoRedoAction
     def splitPoly(self, curve_item: HoverableCurve):
         polyline = curve_item.parametric_curve
         dialog = SplitPolylineDialog(self, theme=self.gui_obj.themes[self.gui_obj.current_theme], polyline=polyline,
                                      geo_col=self.geo_col)
         if dialog.exec_():
-            self.geo_col.split_polyline(polyline, dialog.valuesFromWidgets())
+            self.geo_col.split_polyline(polyline, dialog.value())
 
     def appendSelectedPoint(self, plot_data_item: pg.PlotDataItem):
         self.geo_col.selected_objects["points"].append(plot_data_item.point)
 
     def setColorBarData(self, cmap_dict, color_bar, current_theme: str, flow_var: str, min_level_default: float,
                        max_level_default: float):
         self.color_bar_data = dict(cmap_dict=cmap_dict, color_bar=color_bar, current_theme=current_theme,
@@ -485,19 +521,19 @@
             levels[1] = max_level
 
         if levels[0] >= levels[1]:
             raise ValueError("Minimum value cannot be greater than or equal to the maximum value")
         if levels[1] <= levels[0]:
             raise ValueError("Maximum value cannot be less than or equal to the minimum value")
 
-        if self.color_bar_data["flow_var"] == "Cp":
-            Cp_stop = (0.0 - levels[0]) / (levels[1] - levels[0])
-            pos = np.linspace(0.0, Cp_stop, color_data.shape[0] // 2 + 1)
+        if self.color_bar_data["flow_var"] in ["Cp", "v"]:
+            stop = (0.0 - levels[0]) / (levels[1] - levels[0])
+            pos = np.linspace(0.0, stop, color_data.shape[0] // 2 + 1)
             pos = pos[:-1]
-            pos2 = np.linspace(Cp_stop, 1.0, color_data.shape[0] // 2)
+            pos2 = np.linspace(stop, 1.0, color_data.shape[0] // 2)
             for p in pos2:
                 pos = np.append(pos, p)
         else:
             stop = (1.0 - levels[0]) / (levels[1] - levels[0])
             pos = np.linspace(0.0, stop, color_data.shape[0] // 2 + 1)
             pos = pos[:-1]
             pos2 = np.linspace(stop, 1.0, color_data.shape[0] // 2)
@@ -604,21 +640,28 @@
         elif self.drawing_object == "ROCurvatureConstraint":
             self.geo_col.select_object(point_item.point)
             if len(self.geo_col.selected_objects["points"]) == 1:
                 self.sigEnterPressed.emit()
         else:
             self.geo_col.select_object(point_item.point)
 
-    def pointMoved(self, point: DraggablePoint):
+    def pointMoving(self, point: DraggablePoint):
         if self.point_text_item is not None:
             self.removeItem(self.point_text_item)
             self.point_text_item = None
         for curve in point.curveOwners:
             curve.updateCurveItem()
 
+    @undoRedoAction
+    def pointStartedMoving(self, point: DraggablePoint):
+        pass
+
+    def pointFinishedMoving(self, point: DraggablePoint):
+        pass
+
     def setItemStyle(self, item, style: str):
         valid_styles = ["default", "hovered", "selected"]
         if style not in valid_styles:
             raise ValueError(f"Style found ({style}) is not a valid style. Must be one of {valid_styles}.")
 
         if style == "hovered":
             # Point
@@ -738,15 +781,15 @@
             current_max_level = current_levels[1]
 
         dialog = PlotExportDialog(self, gui_obj=self.gui_obj, theme=self.gui_obj.themes[self.gui_obj.current_theme],
                                   current_min_level=current_min_level,
                                   current_max_level=current_max_level)
         if dialog.exec_():
             # Get the inputs from the dialog
-            inputs = dialog.valuesFromWidgets()
+            inputs = dialog.value()
 
             # Create the pyqtgraph ImageExporter object from the airfoil canvas
             exporter = pg.exporters.ImageExporter(self.plot)
 
             # Set the image width parameter
             exporter.parameters()["width"] = inputs["width"]
 
@@ -804,14 +847,16 @@
         addAntiParallel3ConstraintAction = add_constraint_menu.addAction("Add Anti-Parallel 3 Constraint")
         addSymmetryConstraintAction = add_constraint_menu.addAction("Add Symmetry Constraint")
         addROCurvatureConstraintAction = add_constraint_menu.addAction("Add Radius of Curvature Constraint")
         addDistanceConstraintAction = add_constraint_menu.addAction("Add Distance Constraint")
         exportPlotAction = menu.addAction("Export Plot")
         view_pos = self.getPlotItem().getViewBox().mapSceneToView(event.pos())
         res = menu.exec_(event.globalPos())
+        if res is None:
+            return
         if res == drawPointAction:
             self.drawPoint(x=[view_pos.x()], y=[view_pos.y()])
         elif res == drawBezierCurveThroughPointsAction:
             self.drawBezier()
         elif res == drawLineSegmentThroughPointsAction:
             self.drawLineSegment()
         elif res == generateAirfoilAction:
@@ -835,14 +880,15 @@
         elif res == insertCurvePointAction and curve_item is not None:
             self.addPointToCurve(curve_item)
         elif res == splitPolyAction and curve_item is not None:
             self.splitPoly(curve_item)
         elif res == exportPlotAction:
             self.exportPlot()
 
+    @undoRedoAction
     def removeSelectedPoints(self):
         self.geo_col.remove_selected_objects()
 
     def clearSelectedObjects(self):
         self.geo_col.clear_selected_objects()
 
     def onLineItemAdded(self, line_item):
@@ -870,14 +916,18 @@
 
         if not self.drawing_object == "Points":
             return
 
         view_pos = self.getPlotItem().getViewBox().mapSceneToView(ev.pos())
         self.geo_col.add_point(view_pos.x(), view_pos.y())
 
+    @undoRedoAction
+    def removeSelectedObjects(self):
+        self.geo_col.remove_selected_objects()
+
     def canvasShortcuts(self):
         return {
             Qt.Key_P: self.drawPoints,
             Qt.Key_L: self.drawLines,
             Qt.Key_B: self.drawBeziers,
             Qt.Key_F: self.generateAirfoil,
             Qt.Key_W: self.generateWebAirfoil,
@@ -896,13 +946,13 @@
         if key == Qt.Key_Return:
             self.sigEnterPressed.emit()
         elif key == Qt.Key_Escape:
             self.sigEscapePressed.emit()
             self.geo_col.clear_selected_objects()
             self.sigStatusBarUpdate.emit("", 0)
         elif key == Qt.Key_Delete:
-            self.geo_col.remove_selected_objects()
+            self.removeSelectedObjects()
             self.sigStatusBarUpdate.emit("", 0)
         elif key in (Qt.Key_Left, Qt.Key_Right, Qt.Key_Down, Qt.Key_Up) and len(self.geo_col.selected_objects["points"]) > 0:
             self.arrowKeyPointMove(ev.key(), mods)
         elif key in self.canvasShortcuts():
             self.canvasShortcuts()[key]()
```

### Comparing `pymead-2.0.0b3/pymead/gui/airfoil_statistics.py` & `pymead-2.0.0b4/pymead/gui/airfoil_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from PyQt5.QtWidgets import QTextEdit
 
 from pymead.core.geometry_collection import GeometryCollection
-from pymead.gui.input_dialog import PymeadDialog
+from pymead.gui.dialogs import PymeadDialog
 
 
 class AirfoilStatistics:
     def __init__(self, geo_col: GeometryCollection):
         self.geo_col = geo_col
         self.df = None
         self.data = None
```

### Comparing `pymead-2.0.0b3/pymead/gui/analysis_graph.py` & `pymead-2.0.0b4/pymead/gui/opt_airfoil_graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import pyqtgraph as pg
 
 
-class AnalysisGraph:
+class OptAirfoilGraph:
     def __init__(self, pen=None, size: tuple = (1000, 300), background_color: str = 'w'):
         pg.setConfigOptions(antialias=True)
 
         if pen is None:
             pen = pg.mkPen(color='cornflowerblue', width=2)
 
         self.w = pg.GraphicsLayoutWidget(show=True, size=size)
         # self.w.setWindowTitle('Airfoil')
         self.w.setBackground(background_color)
-
         self.v = self.w.addPlot(pen=pen)
-        self.v.invertY(True)
+        self.v.setAspectLocked()
         self.v.setLabel(axis='bottom', text='x')
-        self.v.setLabel(axis='left', text='Cp')
+        self.v.setLabel(axis='left', text='y')
         self.legend = self.v.addLegend(offset=(300, 20))
         # self.v.setAspectLocked()
 
     def set_background(self, background_color: str):
         self.w.setBackground(background_color)
```

### Comparing `pymead-2.0.0b3/pymead/gui/autocomplete.py` & `pymead-2.0.0b4/pymead/gui/autocomplete.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/bounds_values_table.py` & `pymead-2.0.0b4/pymead/gui/bounds_values_table.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/concurrency.py` & `pymead-2.0.0b4/pymead/gui/concurrency.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
                     except EOFError:
                         self.signals.finished.emit(True)
                         self.running = False
                 elif not self.process.is_alive():
                     self.signals.progress.emit("terminated", None)
                     self.running = False
             except (BrokenPipeError, OSError, EOFError):
-                print("Terminating!")
                 self.signals.finished.emit(False)
                 self.running = False
 
 
 class CPUBoundProcess(QObject):
 
     def __init__(self, operation, args=(), parent=None):
```

### Comparing `pymead-2.0.0b3/pymead/gui/constraint_items.py` & `pymead-2.0.0b4/pymead/gui/constraint_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
 
 import pyqtgraph as pg
 from PyQt5.QtCore import Qt, pyqtSignal, QObject
 from PyQt5.QtGui import QFont, QPen, QColor
 
+from pymead.core import UNITS
 from pymead.core.constraints import *
 from pymead.utils.misc import get_setting
 
 
 class ConstraintItem(QObject):
 
     sigItemHovered = pyqtSignal()
@@ -83,31 +84,31 @@
         self.update()
 
     def update(self):
         angle = self.constraint.p1.measure_angle(self.constraint.p2)
         dist = self.constraint.p1.measure_distance(self.constraint.p2)
 
         handle_angle = angle + np.pi / 2
-        arrow_offset = 0.04
+        arrow_offset = 0.04 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
         p1_arrow = (self.constraint.p1.x().value() + arrow_offset * np.cos(handle_angle),
                     self.constraint.p1.y().value() + arrow_offset * np.sin(handle_angle))
         p2_arrow = (self.constraint.p2.x().value() + arrow_offset * np.cos(handle_angle),
                     self.constraint.p2.y().value() + arrow_offset * np.sin(handle_angle))
 
-        text_offset = 0.06
+        text_offset = 0.06 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
         text_angle = np.rad2deg((angle + np.pi / 2) % np.pi - np.pi / 2)
         text_pos = (self.constraint.p1.x().value() + text_offset * np.cos(handle_angle) + 0.5 * dist * np.cos(angle),
                     self.constraint.p1.y().value() + text_offset * np.sin(handle_angle) + 0.5 * dist * np.sin(angle))
 
         line_x = [self.constraint.p1.x().value() + arrow_offset * np.cos(handle_angle),
                   self.constraint.p1.x().value() + arrow_offset * np.cos(handle_angle) + dist * np.cos(angle)]
         line_y = [self.constraint.p1.y().value() + arrow_offset * np.sin(handle_angle),
                   self.constraint.p1.y().value() + arrow_offset * np.sin(handle_angle) + dist * np.sin(angle)]
 
-        handle_offset = 0.05
+        handle_offset = 0.05 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
         handle1_x = [self.constraint.p1.x().value(),
                      self.constraint.p1.x().value() + handle_offset * np.cos(handle_angle)]
         handle1_y = [self.constraint.p1.y().value(),
                      self.constraint.p1.y().value() + handle_offset * np.sin(handle_angle)]
 
         handle2_x = [self.constraint.p2.x().value(),
                      self.constraint.p2.x().value() + handle_offset * np.cos(handle_angle)]
@@ -136,32 +137,34 @@
         canvas_items[1].setFont(QFont("DejaVu Sans", 10))
         for item in canvas_items:
             item.setZValue(-10)
         super().__init__(constraint=constraint, canvas_items=canvas_items, theme=theme)
         self.update()
 
     def update(self):
-        self.canvas_items[0].setPos(self.constraint.p3.x().value() + 0.01, self.constraint.p3.y().value() - 0.01)
-        self.canvas_items[1].setPos(self.constraint.p4.x().value() + 0.01, self.constraint.p4.y().value() - 0.01)
+        dist = 0.01 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
+        self.canvas_items[0].setPos(self.constraint.p3.x().value() + dist, self.constraint.p3.y().value() - dist)
+        self.canvas_items[1].setPos(self.constraint.p4.x().value() + dist, self.constraint.p4.y().value() - dist)
 
 
 class ROCurvatureConstraintItem(ConstraintItem):
     def __init__(self, constraint: ROCurvatureConstraint, theme: dict):
         canvas_items = [
             pg.TextItem("\u24c7"),
         ]
         canvas_items[0].setFont(QFont("DejaVu Sans", 10))
         for item in canvas_items:
             item.setZValue(-10)
         super().__init__(constraint=constraint, canvas_items=canvas_items, theme=theme)
         self.update()
 
     def update(self):
-        self.canvas_items[0].setPos(self.constraint.curve_joint.x().value() - 0.01,
-                                    self.constraint.curve_joint.y().value() - 0.01)
+        dist = 0.01 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
+        self.canvas_items[0].setPos(self.constraint.curve_joint.x().value() - dist,
+                                    self.constraint.curve_joint.y().value() - dist)
 
 
 class AntiParallel3ConstraintItem(ConstraintItem):
     def __init__(self, constraint: AntiParallel3Constraint, theme: dict):
         self.text_style = dict(anchor=(0.5, 0.5))
         pen = pg.mkPen(width=1, style=Qt.DashLine)
         canvas_items = [
@@ -228,15 +231,18 @@
         line2_x = [self.constraint.p2.x().value(), self.constraint.p3.x().value()]
         line2_y = [self.constraint.p2.y().value(), self.constraint.p3.y().value()]
 
         self.canvas_items[0].setData(x=x, y=y)
         self.canvas_items[1].setData(x=line1_x, y=line1_y)
         self.canvas_items[2].setData(x=line2_x, y=line2_y)
         self.canvas_items[3].setPos(text_x, text_y)
-        self.canvas_items[3].setText(f"{np.rad2deg(self.constraint.param().rad()):.2f}\u00b0")
+        text = f"{self.constraint.param().value():.2f}"
+        if self.constraint.param().unit() == "deg":
+            text += "\u00b0"
+        self.canvas_items[3].setText(text)
 
 
 class Perp3ConstraintItem(ConstraintItem):
     def __init__(self, constraint: Perp3Constraint, theme: dict):
         pen = pg.mkPen(width=1, style=Qt.DashLine)
         canvas_items = [
             pg.PlotDataItem(),
@@ -249,15 +255,15 @@
             item.setZValue(-10)
         self.update()
 
     def update(self):
         angle1 = self.constraint.p2.measure_angle(self.constraint.p1)
         angle2 = angle1 - np.pi / 2
 
-        square_side = 0.05
+        square_side = 0.05 * UNITS.convert_length_from_base(1.0, UNITS.current_length_unit())
 
         x1 = [self.constraint.p2.x().value() + square_side * np.cos(angle1),
               self.constraint.p2.x().value() + square_side * np.cos(angle1) + square_side * np.cos(angle2)]
         y1 = [self.constraint.p2.y().value() + square_side * np.sin(angle1),
               self.constraint.p2.y().value() + square_side * np.sin(angle1) + square_side * np.sin(angle2)]
         x2 = [self.constraint.p2.x().value() + square_side * np.cos(angle2),
               self.constraint.p2.x().value() + square_side * np.cos(angle2) + square_side * np.cos(angle1)]
```

### Comparing `pymead-2.0.0b3/pymead/gui/custom_context_menu_event.py` & `pymead-2.0.0b4/pymead/gui/custom_context_menu_event.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/default_settings.py` & `pymead-2.0.0b4/pymead/gui/default_settings.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/dialog_widgets/export_IGES.json` & `pymead-2.0.0b4/pymead/gui/dialog_widgets/export_IGES.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/dialog_widgets/export_control_points_dialog.json` & `pymead-2.0.0b4/pymead/gui/dialog_widgets/export_control_points_dialog.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/dialog_widgets/export_coordinates_dialog.json` & `pymead-2.0.0b4/pymead/gui/dialog_widgets/export_coordinates_dialog.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/dialog_widgets/screenshot_dialog.json` & `pymead-2.0.0b4/pymead/gui/dialog_widgets/screenshot_dialog.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'window'": "{'combobox': {'addItems': []}}"}*

```diff
@@ -31,21 +31,15 @@
             ],
             "text": "",
             "w": "QLineEdit"
         }
     },
     "window": {
         "combobox": {
-            "addItems": [
-                "Full Window",
-                "Parameter Tree",
-                "Geometry",
-                "Analysis",
-                "Console"
-            ],
+            "addItems": [],
             "grid": [
                 0,
                 1,
                 1,
                 2
             ],
             "w": "QComboBox"
```

### Comparing `pymead-2.0.0b3/pymead/gui/dockable_tab_widget.py` & `pymead-2.0.0b4/pymead/gui/dockable_tab_widget.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/draggable_point.py` & `pymead-2.0.0b4/pymead/gui/draggable_point.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 q_settings_descriptions = load_data(os.path.join(GUI_SETTINGS_DIR, "q_settings_descriptions.json"))
 
 
 class DraggablePoint(pg.GraphItem):
     sigPointClicked = pyqtSignal(object, object, object, object)
     sigPointHovered = pyqtSignal(object, object, object, object)
     sigPointLeaveHovered = pyqtSignal(object, object, object, object)
-    sigPointMoved = pyqtSignal(object)
+    sigPointStartedMoving = pyqtSignal(object)
+    sigPointMoving = pyqtSignal(object)
+    sigPointFinishedMoving = pyqtSignal(object)
 
     def __init__(self):
         self.point = None
         self.dragPoint = None
         self.dragOffset = None
         self.curveOwners = []
         self.textItems = []
@@ -41,15 +43,15 @@
         self.data["pos"][0] = np.array([x, y])
         self.updateGraph()
 
     def updateGraph(self):
         pg.GraphItem.setData(self, **self.data)
         for i, item in enumerate(self.textItems):
             item.setPos(*self.data['pos'][i])
-        self.sigPointMoved.emit(self)
+        self.sigPointMoving.emit(self)
 
     def setTexts(self, text):
         for i in self.textItems:
             i.scene().removeItem(i)
         self.textItems = []
         for t in text:
             item = pg.TextItem(t)
@@ -58,14 +60,15 @@
 
     def mouseDragEvent(self, ev):
         if ev.button() != Qt.MouseButton.LeftButton:
             ev.ignore()
             return
 
         if ev.isStart():
+            self.sigPointStartedMoving.emit(self)
             # While dragging, disable hovering for curves
             self.hoverable = False
             for curve in self.curveOwners:
                 curve.hoverable = False
 
             # We are already one step into the drag.
             # Find the point(s) at the mouse cursor when the button was first
@@ -75,14 +78,15 @@
             if len(pts) == 0:
                 ev.ignore()
                 return
             self.dragPoint = pts[0]
             ind = pts[0].data()[0]
             self.dragOffset = self.data['pos'][ind] - pos
         elif ev.isFinish():
+            self.sigPointFinishedMoving.emit(self)
             # Re-enable hovering for curves
             self.hoverable = True
             for curve in self.curveOwners:
                 curve.hoverable = True
 
             self.dragPoint = None
             return
```

### Comparing `pymead-2.0.0b3/pymead/gui/file_selection.py` & `pymead-2.0.0b4/pymead/gui/file_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from PyQt5.QtWidgets import QFileDialog, QLineEdit, QPlainTextEdit
 
 
 def single_file_output_rule(dlg: QFileDialog, line_edit: QLineEdit = None):
     if line_edit is not None:
         if dlg.exec_():
-            line_edit.setText(dlg.selectedFiles()[0])
+            file_name = dlg.selectedFiles()[0]
+            line_edit.setText(file_name)
+            return file_name
     else:
         return dlg
 
 
 def multi_file_output_rule(dlg: QFileDialog, text_edit: QPlainTextEdit = None):
     if text_edit is not None:
         if dlg.exec_():
```

### Comparing `pymead-2.0.0b3/pymead/gui/gui.py` & `pymead-2.0.0b4/pymead/gui/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import typing
 import warnings
 from copy import deepcopy
 from functools import partial
 from threading import Thread
 from pathlib import PureWindowsPath
 
+import networkx
 import numpy as np
 import pyqtgraph as pg
 import requests
 from PyQt5.QtCore import QEvent, QObject, Qt, QThreadPool, QRect
 from PyQt5.QtCore import pyqtSlot
-from PyQt5.QtGui import QIcon, QFont, QFontDatabase, QPainter, QCloseEvent, QTextCursor
+from PyQt5.QtGui import QIcon, QFont, QFontDatabase, QPainter, QCloseEvent, QTextCursor, QImage
 from PyQt5.QtSvg import QSvgWidget
 from PyQt5.QtWidgets import QMainWindow, QApplication, \
     QWidget, QMenu, QStatusBar, QAction, QGraphicsScene, QGridLayout, QDockWidget, QSizeGrip
 
 from pymoo.factory import get_decomposition
 from pyqtgraph.exporters import CSVExporter, SVGExporter
 
@@ -26,28 +27,30 @@
 from pymead import RESOURCE_DIR
 from pymead.analysis.calc_aero_data import SVG_PLOTS, SVG_SETTINGS_TR
 from pymead.analysis.calc_aero_data import calculate_aero_data
 from pymead.analysis.read_aero_data import flow_var_idx
 from pymead.analysis.read_aero_data import read_grid_stats_from_mses, read_field_from_mses, \
     read_streamline_grid_from_mses
 from pymead.analysis.single_element_inviscid import single_element_inviscid
+from pymead.core import UNITS
 from pymead.core.geometry_collection import GeometryCollection
 from pymead.core.mea import MEA
 from pymead.gui.airfoil_canvas import AirfoilCanvas
 from pymead.gui.airfoil_statistics import AirfoilStatisticsDialog, AirfoilStatistics
 from pymead.gui.analysis_graph import AnalysisGraph
 from pymead.gui.concurrency import CPUBoundProcess
 from pymead.gui.custom_graphics_view import CustomGraphicsView
 from pymead.gui.dockable_tab_widget import PymeadDockWidget
 from pymead.gui.help_browser import HelpBrowserWindow
-from pymead.gui.input_dialog import LoadDialog, SaveAsDialog, OptimizationSetupDialog, \
+from pymead.gui.dialogs import LoadDialog, SaveAsDialog, OptimizationSetupDialog, \
     MultiAirfoilDialog, ColorInputDialog, ExportCoordinatesDialog, ExportControlPointsDialog, AirfoilPlotDialog, \
     AirfoilMatchingDialog, MSESFieldPlotDialog, ExportIGESDialog, XFOILDialog, NewGeoColDialog, EditBoundsDialog, \
-    ExitDialog, ScreenshotDialog, LoadAirfoilAlgFile, ExitOptimizationDialog
-from pymead.gui.input_dialog import convert_dialog_to_mset_settings, convert_dialog_to_mses_settings, \
+    ExitDialog, ScreenshotDialog, LoadAirfoilAlgFile, ExitOptimizationDialog, SettingsDialog, LoadPointsDialog, \
+    PanelDialog
+from pymead.gui.dialogs import convert_dialog_to_mset_settings, convert_dialog_to_mses_settings, \
     convert_dialog_to_mplot_settings
 from pymead.gui.main_icon_toolbar import MainIconToolbar
 from pymead.gui.message_box import disp_message_box
 from pymead.gui.parameter_tree import ParameterTree
 from pymead.gui.permanent_widget import PermanentWidget
 from pymead.gui.pymeadPColorMeshItem import PymeadPColorMeshItem
 from pymead.gui.show_hide import ShowHideDialog
@@ -64,24 +67,33 @@
 from pymead.utils.dict_recursion import compare_dicts_floating_precision
 from pymead.utils.get_airfoil import extract_data_from_airfoiltools
 from pymead.utils.misc import get_setting
 from pymead.utils.misc import make_ga_opt_dir
 from pymead.utils.read_write_files import load_data, save_data
 from pymead.utils.version_check import using_latest
 
+q_settings_descriptions = load_data(os.path.join(GUI_SETTINGS_DIR, "q_settings_descriptions.json"))
+
 # Suppress the following DeprecationWarning: sipPyTypeDict() is deprecated, the extension module
 # should use sipPyTypeDictRef() instead
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 
 class GUI(QMainWindow):
     _gripSize = 5
 
     def __init__(self, path=None, parent=None):
         # super().__init__(flags=Qt.FramelessWindowHint)
+        try:
+            import pyi_splash
+            pyi_splash.update_text("Initializing constants...")
+        except:
+            pass
+        UNITS.set_current_length_unit(get_setting("length_unit"))
+        UNITS.set_current_angle_unit(get_setting("angle_unit"))
         super().__init__(parent=parent)
         self.showHideState = None
         self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
         self.windowMaximized = False
         # print(f"Running GUI with {os.getpid() = }")
         self.pool = None
         self.current_opt_folder = None
@@ -99,29 +111,35 @@
             QFontDatabase.addApplicationFont(os.path.join(RESOURCE_DIR, "dejavu-fonts-ttf-2.37", "ttf",
                                                           f"{font_name}.ttf"))
         self.themes = {
             "dark": load_data(os.path.join(GUI_THEMES_DIR, "dark_theme.json")),
             "light": load_data(os.path.join(GUI_THEMES_DIR, "light_theme.json")),
         }
 
+        self.undo_stack = []
+        self.redo_stack = []
+
         self.design_tree = None
         self.dialog = None
         self.opt_settings = None
         self.multi_airfoil_analysis_settings = None
         self.xfoil_settings = None
+        self.panel_settings = None
+        self.screenshot_settings = None
         self.current_settings_save_file = None
         self.current_theme = "dark"
         self.cbar = None
         self.cbar_label_attrs = None
         self.crameri_cmap = None
         self.default_field_dir = None
         self.objectives = []
         self.constraints = []
         self.airfoil_name_list = []
         self.last_analysis_dir = None
+        self.field_plot_variable = None
         self.analysis_graph = None
         self.opt_airfoil_graph = None
         self.parallel_coords_graph = None
         self.drag_graph = None
         self.Cp_graph = None
         self.geometry_plot_handles = {}
         # self.Mach_contour_widget = None
@@ -133,30 +151,14 @@
         self.forces_dict = {}
         self.te_thickness_edit_mode = False
         self.worker = None
         self.n_analyses = 0
         self.n_converged_analyses = 0
         self.threadpool = QThreadPool().globalInstance()
         self.threadpool.setMaxThreadCount(4)
-        self.pens = [
-            ('#d4251c', Qt.SolidLine),
-            ('darkorange', Qt.SolidLine),
-            ('gold', Qt.SolidLine),
-            ('limegreen', Qt.SolidLine),
-            ('cyan', Qt.SolidLine),
-            ('mediumpurple', Qt.SolidLine),
-            ('deeppink', Qt.SolidLine),
-            ('#d4251c', Qt.DashLine),
-            ('darkorange', Qt.DashLine),
-            ('gold', Qt.DashLine),
-            ('limegreen', Qt.DashLine),
-            ('cyan', Qt.DashLine),
-            ('mediumpurple', Qt.DashLine),
-            ('deeppink', Qt.DashLine)
-        ]
 
         # Save/load variables
         self.save_attempts = 0
         self.last_saved_state = None
         self.current_save_name = None
 
         # mandatory for cursor updates
@@ -172,14 +174,19 @@
             SideGrip(self, Qt.BottomEdge),
         ]
         # corner grips should be "on top" of everything, otherwise the side grips
         # will take precedence on mouse events, so we are adding them *after*;
         # alternatively, widget.raise_() can be used
         self.cornerGrips = [QSizeGrip(self) for i in range(4)]
 
+        try:
+            pyi_splash.update_text("Generating pymead widgets...")
+        except:
+            pass
+
         # Dock widget items
         self.dock_widgets = []
         self.dock_widget_names = []
         self.first_dock_widget = None
         self.current_dock_widget = None
         self.tabifiedDockWidgetActivated.connect(self.activated)
         self.setDockNestingEnabled(True)
@@ -226,35 +233,46 @@
         self.statusBar().addPermanentWidget(self.permanent_widget)
         self.permanent_widget.updateAirfoils()
 
         self.parameter_tree.setMaximumWidth(300)
         self.resize(1000, self.title_bar.height() + 600)
         self.parameter_tree.setMaximumWidth(800)
 
+        try:
+            pyi_splash.update_text("Loading geometry information...")
+        except:
+            pass
+
         # Load the airfoil system from the system argument variable if necessary
         if self.path is not None:
             self.load_geo_col_no_dialog(self.path)
         else:
             self.last_saved_state = self.get_geo_col_state()
 
+        try:
+            pyi_splash.close()
+        except:
+            pass
+
         # Check if we are using the most recent release of pymead (notify if not)
         self.check_for_new_version()
 
     def check_for_new_version(self):
         try:
             using_latest_res, latest_ver, current_ver = using_latest()
         except requests.ConnectionError:
             self.disp_message_box("Could not connect to the internet to check for updates", message_mode="info")
             return
 
         if not using_latest_res:
             self.disp_message_box(f"A newer version of pymead ({latest_ver}) is available for download at "
                                   f"<a href='https://github.com/mlau154/pymead/releases' style='color:#45C5E6;'>"
-                                  f"https://github.com/mlau154/pymead/releases</a>", message_mode="info",
-                                  rich_text=True)
+                                  f"https://github.com/mlau154/pymead/releases</a>. If you are using pymead directly"
+                                  f" via Python, you can update with 'pip install pymead --upgrade' in the terminal.",
+                                  message_mode="info", rich_text=True)
 
     def add_new_tab_widget(self, widget, name):
         if not (name in self.dock_widget_names):
             dw = PymeadDockWidget(name, self)
             dw.setAllowedAreas(Qt.AllDockWidgetAreas)
             dw.setWidget(widget)
             dw.setFloating(False)
@@ -463,14 +481,17 @@
             self.cbar.axis.setStyle(tickFont=tick_font)
             self.cbar.axis.setTextPen(pg.mkPen(color=theme["cbar-color"]))
             self.airfoil_canvas.color_bar_data["current_theme"] = self.current_theme
         # if self.analysis_graph is not None:
         #     self.analysis_graph.set_background(theme["graph-background-color"])
         # if self.param_tree_instance is not None:
         #     self.param_tree_instance.set_theme(theme)
+        if self.analysis_graph is not None:
+            self.analysis_graph.set_formatting(theme=self.themes[self.current_theme])
+            self.analysis_graph.set_legend_label_format(theme=self.themes[self.current_theme])
 
         for cnstr in self.geo_col.container()["geocon"].values():
             cnstr.canvas_item.setStyle(theme)
 
         for button_name, button_setting in self.main_icon_toolbar.button_settings.items():
             icon_name = button_setting["icon"]
             if "dark" not in icon_name:
@@ -483,14 +504,34 @@
         if self.cbar is None:
             return
 
         new_values = {} if new_values is None else new_values
         self.cbar.setLabel(axis="right", )
         self.cbar.getAxis("right").setWidth(25 + 1)
 
+    @staticmethod
+    def pen(n: int):
+        pens = [
+            ('#d4251c', Qt.SolidLine),
+            ('darkorange', Qt.SolidLine),
+            ('gold', Qt.SolidLine),
+            ('limegreen', Qt.SolidLine),
+            ('cyan', Qt.SolidLine),
+            ('mediumpurple', Qt.SolidLine),
+            ('deeppink', Qt.SolidLine),
+            ('#d4251c', Qt.DashLine),
+            ('darkorange', Qt.DashLine),
+            ('gold', Qt.DashLine),
+            ('limegreen', Qt.DashLine),
+            ('cyan', Qt.DashLine),
+            ('mediumpurple', Qt.DashLine),
+            ('deeppink', Qt.DashLine)
+        ]
+        return pens[n % len(pens)]
+
     def set_title_and_icon(self):
         self.setWindowTitle("pymead")
         image_path = os.path.join(ICON_DIR, "pymead-logo.png")
         self.setWindowIcon(QIcon(image_path))
 
     def create_menu_bar(self):
         self.menu_bar = self.menuBar()
@@ -521,51 +562,93 @@
                             action.setCheckable(True)
                             action.setChecked(val[2])
                     else:
                         action.triggered.connect(getattr(self, val))
 
         recursively_add_menus(menu_data, self.menu_bar)
 
+    def open_settings(self):
+        dialog = SettingsDialog(parent=self, geo_col=self.geo_col, theme=self.themes[self.current_theme],
+                                settings_override=None)
+        dialog.exec_()
+
+
+    def undo(self):
+        if not self.undo_stack:
+            return
+        self.redo_stack.append(deepcopy(self.geo_col.get_dict_rep()))
+        self.load_geo_col_from_memory(self.undo_stack[-1])
+        self.undo_stack.pop()
+
+    def redo(self):
+        if not self.redo_stack:
+            return
+        self.undo_stack.append(deepcopy(self.geo_col.get_dict_rep()))
+        self.load_geo_col_from_memory(self.redo_stack[-1])
+        self.redo_stack.pop()
+
+    def load_points(self):
+        """
+        Loads a set of :math:`x`-:math:`y` points from a .dat/.txt/.csv file.
+        """
+        dialog = LoadPointsDialog(self, theme=self.themes[self.current_theme])
+
+        if dialog.exec_():
+            # Load the points to an array
+            try:
+                points = np.loadtxt(dialog.value())
+            except ValueError:
+                points = np.loadtxt(dialog.value(), delimiter=",")
+
+            # Add each point from the array to the GeometryCollection
+            for point in points:
+                self.geo_col.add_point(point[0], point[1])
+
+            # Make sure that all the points are in view
+            self.auto_range_geometry()
+
     def take_screenshot(self):
 
-        # if hasattr(self.dockable_tab_window, "current_dock_widget"):
-        if self.current_dock_widget is not None:
-            analysis_id = self.current_dock_widget.winId()
-        else:
-            analysis_id = self.dock_widgets[-1].winId()
+        id_dict = {dw.windowTitle(): dw.winId() for dw in self.dock_widgets}
+        id_dict = {"Full Window": self.winId(), **id_dict}
 
-        id_dict = {
-            "Full Window": self.winId(),
-            # "Parameter Tree": self.param_tree_instance.t.winId(),
-            "Geometry": self.dock_widgets[0].winId(),
-            "Analysis": analysis_id,
-            "Console": self.text_area.winId()
-        }
+        window_widget_dict = {dw.windowTitle(): dw for dw in self.dock_widgets}
+        window_widget_dict = {"Full Window": self, **window_widget_dict}
+
+        dialog = ScreenshotDialog(self, theme=self.themes[self.current_theme], windows=[k for k in id_dict.keys()])
+        if self.screenshot_settings is not None:
+            dialog.setValue(self.screenshot_settings)
 
-        dialog = ScreenshotDialog(self, theme=self.themes[self.current_theme])
         if dialog.exec_():
-            inputs = dialog.getInputs()
+            inputs = dialog.value()
+            self.screenshot_settings = inputs
 
             # Take the screenshot
-            screen = QApplication.primaryScreen()
-            screenshot = screen.grabWindow(id_dict[inputs["window"]])
+            ratio = 5  # Increased device-pixel ratio for better screenshot resolution
+            window_widget = window_widget_dict[inputs["window"]]
+            size = window_widget.size()
+            image = QImage(size.width() * ratio, size.height() * ratio, QImage.Format_ARGB32)
+            image.setDevicePixelRatio(ratio)
+            window_widget.render(image)
 
             # Handle improper directory names and file extensions
             file_path_split = os.path.split(inputs['image_file'])
             dir_name = file_path_split[0]
             file_name = file_path_split[1]
             file_name_no_ext = os.path.splitext(file_name)[0]
             file_ext = os.path.splitext(file_name)[1]
             if file_ext not in [".jpg", ".jpeg"]:
                 file_ext = ".jpg"
 
             final_file_name = os.path.join(dir_name, file_name_no_ext + file_ext)
 
+            # Save the image or raise an error if the file directory is not found
             if os.path.isdir(dir_name):
-                screenshot.save(final_file_name, "jpg")  # Save the screenshot
+                # screenshot.save(final_file_name, "jpg")  # Save the screenshot
+                image.save(final_file_name, "jpg")  # Save the screenshot
                 self.disp_message_box(f"{inputs['window']} window screenshot saved to {final_file_name}",
                                       message_mode="info")
             else:
                 self.disp_message_box(f"Directory {dir_name} for"
                                       f"file {file_name} not found")
 
     def showHidePymeadObjs(self, sub_container: str, show: bool):
@@ -619,15 +702,15 @@
             self.setWindowTitle(f"pymead - {os.path.split(self.current_save_name)[-1]}")
             self.save_attempts = 0
             return True
 
     def deepcopy_geo_col(self):
         return deepcopy(self.geo_col)
 
-    def load_geo_col(self):
+    def load_geo_col(self, file_name: str = None):
 
         if self.changes_made():
             save_dialog = NewGeoColDialog(theme=self.themes[self.current_theme], parent=self,
                                           message="Airfoil has changes. Save?")
             exit_dialog = ExitDialog(theme=self.themes[self.current_theme], parent=self, window_title="Load anyway?",
                                      message="Airfoil not saved.\nAre you sure you want to load a new one?")
             while True:
@@ -638,25 +721,26 @@
                         if exit_dialog.exec_():  # Otherwise, If "Yes" to "Exit the Program Anyway," close the program.
                             break
                     if save_dialog.reject_changes:  # If "No" to "Save Changes," do not load an MEA.
                         return
                 else:  # If "Cancel" to "Save Changes," do not load an MEA
                         return
 
-        dialog = LoadDialog(self, settings_var="jmea_default_open_location")
-
-        if dialog.exec_():
-            file_name = dialog.selectedFiles()[0]
-            file_name_parent_dir = os.path.dirname(file_name)
-            q_settings.setValue(dialog.settings_var, file_name_parent_dir)
-        else:
-            file_name = None
-        if file_name is not None:
+        if not file_name:
+            dialog = LoadDialog(self, settings_var="jmea_default_open_location")
+            if dialog.exec_():
+                file_name = dialog.selectedFiles()[0]
+                file_name_parent_dir = os.path.dirname(file_name)
+                q_settings.setValue(dialog.settings_var, file_name_parent_dir)
+            else:
+                file_name = None
+        if file_name:
             self.load_geo_col_no_dialog(file_name)
             self.setWindowTitle(f"pymead - {os.path.split(file_name)[-1]}")
+            self.current_save_name = file_name
 
     def new_geo_col(self):
 
         def load_blank_geo_col():
             self.load_geo_col_no_dialog()
             self.setWindowTitle(f"pymead")
 
@@ -664,14 +748,17 @@
             dialog = NewGeoColDialog(theme=self.themes[self.current_theme], parent=self)
             if dialog.exec_():
                 load_blank_geo_col()
         else:
             load_blank_geo_col()
 
     def edit_bounds(self):
+        if len(self.geo_col.container()["desvar"]) == 0:
+            self.disp_message_box("No design variables present", message_mode="info")
+            return
         bv_dialog = EditBoundsDialog(geo_col=self.geo_col, theme=self.themes[self.current_theme], parent=self)
         bv_dialog.exec_()
 
     def auto_range_geometry(self):
         """
         Adjusts the range of the airfoil canvas based on the rectangle that just encloses all the Points in the
         geometry collection, plus an offset. If no points are present, default bounds are chosen.
@@ -797,52 +884,70 @@
                     child, pg.ColorBarItem):
                 self.airfoil_canvas.plot.getViewBox().removeItem(child)
         self.cbar = None
         self.cbar_label_attrs = None
         if self.airfoil_canvas.color_bar_data is not None:
             self.airfoil_canvas.color_bar_data.clear()
 
-    def plot_field(self):
-        if self.last_analysis_dir is None and get_setting("plot-field-dir") != "":
-            default_field_dir = get_setting("plot-field-dir")
-        elif self.last_analysis_dir is not None:
-            default_field_dir = self.last_analysis_dir
-        else:
-            default_field_dir = ""
-        dlg = MSESFieldPlotDialog(parent=self, default_field_dir=default_field_dir,
-                                  theme=self.themes[self.current_theme])
-        if dlg.exec_():
-            inputs = dlg.valuesFromWidgets()
+    def plot_field(self, **kwargs):
+        if ("show_dialog" in kwargs and kwargs["show_dialog"]) or "show_dialog" not in kwargs:
+            if self.last_analysis_dir is None and get_setting("plot-field-dir") != "":
+                default_field_dir = get_setting("plot-field-dir")
+            elif self.last_analysis_dir is not None:
+                default_field_dir = self.last_analysis_dir
+            else:
+                default_field_dir = ""
+            dlg = MSESFieldPlotDialog(parent=self, default_field_dir=default_field_dir,
+                                      theme=self.themes[self.current_theme])
+            if dlg.exec_():
+                inputs = dlg.value()
+                self.field_plot_variable = inputs["flow_variable"]
+            else:
+                return
         else:
-            return
+            inputs = {
+                "analysis_dir": self.last_analysis_dir,
+                "flow_variable": self.field_plot_variable
+            }
 
         self.clear_field()
 
         for child in self.airfoil_canvas.plot.allChildItems():
             if hasattr(child, 'setZValue'):
                 child.setZValue(1.0)
 
         analysis_dir = inputs['analysis_dir']
         vBox = self.airfoil_canvas.plot.getViewBox()
         field_file = os.path.join(analysis_dir, f'field.{os.path.split(analysis_dir)[-1]}')
         grid_stats_file = os.path.join(analysis_dir, 'mplot_grid_stats.log')
         grid_file = os.path.join(analysis_dir, f'grid.{os.path.split(analysis_dir)[-1]}')
+        transformation_file = os.path.join(analysis_dir, "transformation.json")
         if not os.path.exists(field_file):
             self.disp_message_box(message=f"Field file {field_file} not found", message_mode='error')
             return
         if not os.path.exists(grid_file):
             self.disp_message_box(message=f"Grid statistics log {grid_file} not found", message_mode='error')
             return
 
         self.default_field_dir = analysis_dir
 
         # data = np.loadtxt(field_file, skiprows=2)
         field = read_field_from_mses(field_file)
         grid_stats = read_grid_stats_from_mses(grid_stats_file)
         x_grid, y_grid = read_streamline_grid_from_mses(grid_file, grid_stats)
+        try:
+            transformation = load_data(transformation_file)
+            x_grid = [x_grid_section / transformation["sx"][0] /
+                      UNITS.convert_length_from_base(1, transformation["length_unit"]) *
+                      UNITS.convert_length_from_base(1, UNITS.current_length_unit()) for x_grid_section in x_grid]
+            y_grid = [y_grid_section / transformation["sy"][0] /
+                      UNITS.convert_length_from_base(1, transformation["length_unit"]) *
+                      UNITS.convert_length_from_base(1, UNITS.current_length_unit()) for y_grid_section in y_grid]
+        except OSError:
+            pass
         flow_var = field[flow_var_idx[inputs['flow_variable']]]
 
         edgecolors = None
         antialiasing = False
         # edgecolors = {'color': 'b', 'width': 1}  # May be uncommented to see edgecolor effect
         # antialiasing = True # May be uncommented to see antialiasing effect
 
@@ -910,37 +1015,84 @@
 
         tick_font = QFont(get_setting("cbar-tick-font-family"), get_setting("cbar-tick-point-size"))
         self.cbar.axis.setStyle(tickFont=tick_font)
         self.cbar.axis.setTextPen(pg.mkPen(color=theme["cbar-color"]))
         self.cbar.getAxis("right").setWidth(20 + 2 * get_setting("axis-label-point-size") +
                                             2 * get_setting("cbar-tick-point-size"))
 
+    def load_geo_col_from_memory(self, dict_rep: dict):
 
+        # Clear the canvas and the tree, and add the high-level containers back to the tree
+        self.airfoil_canvas.clear()
+        self.parameter_tree.clear()
+        self.parameter_tree.addContainers()
+
+        self.geo_col.switch_units("angle", old_unit=UNITS.current_angle_unit(),
+                                  new_unit=dict_rep["metadata"]["angle_unit"]
+                                  if "angle_unit" in dict_rep["metadata"] else "rad")
+        self.geo_col.switch_units("length", old_unit=UNITS.current_length_unit(),
+                                  new_unit=dict_rep["metadata"]["length_unit"]
+                                  if "length_unit" in dict_rep["metadata"] else "m")
+
+        self.geo_col = GeometryCollection.set_from_dict_rep(dict_rep, canvas=self.airfoil_canvas,
+                                                            tree=self.parameter_tree, gui_obj=self)
+        self.permanent_widget.geo_col = self.geo_col
+        self.last_saved_state = self.get_geo_col_state()
+
+        self.geo_col.tree.geo_col = self.geo_col
+        self.geo_col.canvas.geo_col = self.geo_col
+        self.permanent_widget.updateAirfoils()
 
     def load_geo_col_no_dialog(self, file_name: str = None):
 
         # Clear the canvas and the tree, and add the high-level containers back to the tree
         self.airfoil_canvas.clear()
         self.parameter_tree.clear()
         self.parameter_tree.addContainers()
 
         if file_name is not None:
             geo_col_dict = load_data(file_name)
         else:
             geo_col_dict = GeometryCollection().get_dict_rep()
+
+        self.geo_col.switch_units("angle", old_unit=UNITS.current_angle_unit(),
+                                  new_unit=geo_col_dict["metadata"]["angle_unit"]
+                                  if "angle_unit" in geo_col_dict["metadata"] else "rad")
+        self.geo_col.switch_units("length", old_unit=UNITS.current_length_unit(),
+                                  new_unit=geo_col_dict["metadata"]["length_unit"]
+                                  if "length_unit" in geo_col_dict["metadata"] else "m")
+
         self.geo_col = GeometryCollection.set_from_dict_rep(geo_col_dict, canvas=self.airfoil_canvas,
                                                             tree=self.parameter_tree, gui_obj=self)
         self.permanent_widget.geo_col = self.geo_col
         self.last_saved_state = self.get_geo_col_state()
 
         self.geo_col.tree.geo_col = self.geo_col
         self.geo_col.canvas.geo_col = self.geo_col
         self.permanent_widget.updateAirfoils()
         self.auto_range_geometry()
 
+        # self.geo_col.switch_units("angle", old_unit=UNITS.current_angle_unit(),
+        #                           new_unit=geo_col_dict["metadata"]["angle_unit"])
+        # self.geo_col.switch_units("length", old_unit=UNITS.current_length_unit(),
+        #                           new_unit=geo_col_dict["metadata"]["length_unit"])
+
+    def show_constraint_graph(self):
+
+        networkx.draw_circular(self.geo_col.gcs, labels={point: point.name() for point in self.geo_col.gcs.nodes})
+        from matplotlib import pyplot as plt
+        plt.show()
+
+    def show_param_graph(self):
+
+        networkx.draw_circular(self.geo_col.param_graph,
+                               labels={param: param.name() for param in self.geo_col.param_graph.nodes})
+        from matplotlib import pyplot as plt
+        plt.show()
+
     def get_geo_col_state(self):
         return {k: v for k, v in self.geo_col.get_dict_rep().items() if k != "metadata"}
 
     def changes_made(self, atol: float = 1e-15) -> bool:
         return not compare_dicts_floating_precision(self.last_saved_state, self.get_geo_col_state(), atol=atol)
 
     def disp_message_box(self, message: str, message_mode: str = "error", rich_text: bool = False):
@@ -994,47 +1146,57 @@
 
         if selected_airfoil_name == "":
             if plot_cp:
                 self.disp_message_box("Choose an airfoil in the bottom right-hand corner of the screen "
                                       "to perform an incompressible, inviscid analysis", message_mode="info")
             return
 
+        dialog = PanelDialog(self, theme=self.themes[self.current_theme], settings_override=self.panel_settings)
+
+        if dialog.exec_():
+            alpha_add = dialog.value()["alfa"]
+            self.panel_settings = dialog.value()
+        else:
+            return
+
         selected_airfoil = self.geo_col.container()["airfoils"][selected_airfoil_name]
         body_fixed_coords = selected_airfoil.get_chord_relative_coords()
-        alpha = selected_airfoil.measure_alpha() * 180 / np.pi
-        xy, CP, CL = single_element_inviscid(body_fixed_coords,
-                                             alpha=selected_airfoil.measure_alpha() * 180 / np.pi)
+        alpha = selected_airfoil.measure_alpha() * 180 / np.pi + alpha_add
+        xy, CP, CL = single_element_inviscid(body_fixed_coords, alpha=alpha)
 
         if plot_cp:
             self.output_area_text(
                 f"[{str(self.n_analyses).zfill(2)}] ")
-            self.output_area_text(f"PANEL ({selected_airfoil_name}, \u03b1 = {alpha:.3f}): "
+            self.output_area_text(f"PANEL ({selected_airfoil_name}, \u03b1 = {alpha:.3f}\u00b0): "
                                   f"Cl = {CL:+7.4f}".replace("-", "\u2212"), line_break=True)
         else:
             self.statusBar().showMessage(f"CL = {CL:.3f}", 4000)
 
         if not plot_cp:
             return
 
         if self.analysis_graph is None:
-            self.analysis_graph = AnalysisGraph(
+            self.analysis_graph = AnalysisGraph(theme=self.themes[self.current_theme],
                 background_color=self.themes[self.current_theme]["graph-background-color"])
             self.add_new_tab_widget(self.analysis_graph.w, "Analysis")
-        pg_plot_handle = self.analysis_graph.v.plot(pen=pg.mkPen(color=self.pens[self.n_converged_analyses][0],
-                                                                 style=self.pens[self.n_converged_analyses][1]),
-                                                    name=str(self.n_analyses))
+        name = f"[{self.n_analyses}] P ({selected_airfoil_name}, \u03b1 = {alpha:.1f}\u00b0)"
+        pg_plot_handle = self.analysis_graph.v.plot(pen=pg.mkPen(color=self.pen(self.n_converged_analyses)[0],
+                                                                 style=self.pen(self.n_converged_analyses)[1]),
+                                                    name=name)
         pg_plot_handle.setData(xy[:, 0], CP)
+
+        self.analysis_graph.set_legend_label_format(self.themes[self.current_theme])
         self.n_converged_analyses += 1
         self.n_analyses += 1
 
     def export_coordinates(self):
         """Airfoil coordinate exporter"""
         dialog = ExportCoordinatesDialog(self, theme=self.themes[self.current_theme])
         if dialog.exec_():
-            inputs = dialog.valuesFromWidgets()
+            inputs = dialog.value()
             f_ = os.path.join(inputs['choose_dir'], inputs['file_name'])
 
             # Determine if output format should be JSON:
             if os.path.splitext(f_) and os.path.splitext(f_)[-1] == '.json':
                 json = True
             else:
                 json = False
@@ -1066,15 +1228,15 @@
                         if idx < len(airfoils) - 1:
                             f.write(f"{inputs['separator']}")
             self.disp_message_box(f"Airfoil coordinates saved to {f_}", message_mode='info')
 
     def export_control_points(self):
         dialog = ExportControlPointsDialog(self, theme=self.themes[self.current_theme])
         if dialog.exec_():
-            inputs = dialog.valuesFromWidgets()
+            inputs = dialog.value()
             f_ = os.path.join(inputs['choose_dir'], inputs['file_name'])
 
             airfoils = inputs['airfoil_order'].split(',')
 
             control_point_dict = {}
             for a in airfoils:
                 airfoil = self.geo_col.container()["airfoils"][a]
@@ -1091,42 +1253,44 @@
 
     def show_help(self):
         HelpBrowserWindow(parent=self)
 
     def export_IGES(self):
         self.dialog = ExportIGESDialog(parent=self, theme=self.themes[self.current_theme])
         if self.dialog.exec_():
-            inputs = self.dialog.valuesFromWidgets()
+            inputs = self.dialog.value()
             iges_file_path = self.geo_col.write_to_iges(base_dir=inputs["dir"], file_name=inputs["file_name"],
                                                         translation=inputs["translation"], scaling=inputs["scaling"],
                                                         rotation=inputs["rotation"],
                                                         transformation_order=inputs["transformation_order"])
             self.disp_message_box(f"Airfoil geometry saved to {iges_file_path}", message_mode="info")
 
     def single_airfoil_viscous_analysis(self):
         self.dialog = XFOILDialog(parent=self, current_airfoils=[k for k in self.geo_col.container()["airfoils"]],
-                                  theme=self.themes[self.current_theme])
+                                  theme=self.themes[self.current_theme], settings_override=self.xfoil_settings)
         current_airfoils = [k for k in self.geo_col.container()["airfoils"].keys()]
         self.dialog.w.widget_dict["airfoil"]["widget"].addItems(current_airfoils)
         if self.dialog.exec():
-            inputs = self.dialog.valuesFromWidgets()
+            inputs = self.dialog.value()
+            self.xfoil_settings = inputs
         else:
             inputs = None
 
         if inputs is not None:
             xfoil_settings = {'Re': inputs['Re'],
                               'Ma': inputs['Ma'],
                               'prescribe': inputs['prescribe'],
                               'timeout': inputs['timeout'],
                               'iter': inputs['iter'],
                               'xtr': [inputs['xtr_lower'], inputs['xtr_upper']],
                               'N': inputs['N'],
                               'airfoil_analysis_dir': inputs['airfoil_analysis_dir'],
                               'airfoil_coord_file_name': inputs['airfoil_coord_file_name'],
-                              'airfoil': inputs['airfoil']}
+                              'airfoil': inputs['airfoil'],
+                              "visc": inputs["viscous_flag"]}
             if xfoil_settings['prescribe'] == 'Angle of Attack (deg)':
                 xfoil_settings['alfa'] = inputs['alfa']
             elif xfoil_settings['prescribe'] == 'Viscous Cl':
                 xfoil_settings['Cl'] = inputs['Cl']
             elif xfoil_settings['prescribe'] == 'Inviscid Cl':
                 xfoil_settings['CLI'] = inputs['CLI']
 
@@ -1134,15 +1298,15 @@
 
             # coords = tuple(self.mea.deepcopy().airfoils[xfoil_settings['airfoil']].get_coords(
             #     body_fixed_csys=False, as_tuple=True))
 
             if xfoil_settings["airfoil"] == "":
                 self.disp_message_box("An airfoil was not chosen for analysis")
                 return
-            coords = self.geo_col.container()["airfoils"][xfoil_settings["airfoil"]].get_coords_selig_format()
+            coords = self.geo_col.container()["airfoils"][xfoil_settings["airfoil"]].get_scaled_coords()
 
             aero_data, _ = calculate_aero_data(xfoil_settings['airfoil_analysis_dir'],
                                                xfoil_settings['airfoil_coord_file_name'],
                                                coords=coords,
                                                tool="XFOIL",
                                                xfoil_settings=xfoil_settings,
                                                export_Cp=True
@@ -1159,32 +1323,48 @@
                     f"{aero_data['errored_out']} | Timed out = {aero_data['timed_out']}", line_break=True)
             else:
                 self.output_area_text(
                     f"[{str(self.n_analyses).zfill(2)}] ")
                 self.output_area_text(
                     f"<a href='file:///{os.path.join(xfoil_settings['airfoil_analysis_dir'], xfoil_settings['airfoil_coord_file_name'])}'><font family='DejaVu Sans Mono' size='3'>XFOIL</font></a>",
                     mode="html")
-                self.output_area_text(f" ({xfoil_settings['airfoil']}, "
-                                      f"\u03b1 = {aero_data['alf']:.3f}, Re = {xfoil_settings['Re']:.3E}, "
-                                      f"Ma = {xfoil_settings['Ma']:.3f}): "
-                                      f"Cl = {aero_data['Cl']:+7.4f} | Cd = {aero_data['Cd']:+.5f} | Cm = {aero_data['Cm']:+7.4f} "
-                                      f"| L/D = {aero_data['L/D']:+8.4f}".replace("-", "\u2212"), line_break=True)
+                if xfoil_settings["visc"]:
+                    self.output_area_text(f" ({xfoil_settings['airfoil']}, "
+                                          f"\u03b1 = {aero_data['alf']:.3f}\u00b0, Re = {xfoil_settings['Re']:.3E}, "
+                                          f"Ma = {xfoil_settings['Ma']:.3f}): "
+                                          f"Cl = {aero_data['Cl']:+7.4f} | Cd = {aero_data['Cd']:+.5f} | Cm = {aero_data['Cm']:+7.4f} "
+                                          f"| L/D = {aero_data['L/D']:+8.4f}".replace("-", "\u2212"), line_break=True)
+                else:
+                    self.output_area_text(f" ({xfoil_settings['airfoil']}, "
+                                          f"\u03b1 = {aero_data['alf']:.3f}\u00b0, "
+                                          f"Ma = {xfoil_settings['Ma']:.3f}): "
+                                          f"Cl = {aero_data['Cl']:+7.4f} | Cm = {aero_data['Cm']:+7.4f}".replace("-", "\u2212"), line_break=True)
             bar = self.text_area.verticalScrollBar()
             sb = bar
             sb.setValue(sb.maximum())
 
             if aero_data['converged'] and not aero_data['errored_out'] and not aero_data['timed_out']:
                 if self.analysis_graph is None:
                     # Need to set analysis_graph to None if analysis window is closed! Might also not want to allow geometry docking window to be closed
-                    self.analysis_graph = AnalysisGraph(
+                    self.analysis_graph = AnalysisGraph(theme=self.themes[self.current_theme],
                         background_color=self.themes[self.current_theme]["graph-background-color"])
                     self.add_new_tab_widget(self.analysis_graph.w, "Analysis")
-                pg_plot_handle = self.analysis_graph.v.plot(pen=pg.mkPen(color=self.pens[self.n_converged_analyses][0],
-                                                                         style=self.pens[self.n_converged_analyses][1]),
-                                                            name=str(self.n_analyses))
+
+                if xfoil_settings["visc"]:
+                    name = (f"[{str(self.n_analyses)}] X ({xfoil_settings['airfoil']}, \u03b1 = {aero_data['alf']:.1f}\u00b0,"
+                            f" Re = {xfoil_settings['Re']:.1E}, Ma = {xfoil_settings['Ma']:.2f})")
+                else:
+                    name = (f"[{str(self.n_analyses)}] X ({xfoil_settings['airfoil']}, \u03b1 = {aero_data['alf']:.1f}\u00b0,"
+                            f" Ma = {xfoil_settings['Ma']:.2f})")
+
+                pg_plot_handle = self.analysis_graph.v.plot(pen=pg.mkPen(color=self.pen(self.n_converged_analyses)[0],
+                                                                         style=self.pen(self.n_converged_analyses)[1]),
+                                                            name=name)
+                self.analysis_graph.set_legend_label_format(self.themes[self.current_theme])
+
                 pg_plot_handle.setData(aero_data['Cp']['x'], aero_data['Cp']['Cp'])
                 # pen = pg.mkPen(color='green')
                 self.n_converged_analyses += 1
                 self.n_analyses += 1
             else:
                 self.n_analyses += 1
 
@@ -1207,25 +1387,25 @@
         )
         self.dialog.accepted.connect(self.multi_airfoil_analysis_accepted)
         self.dialog.rejected.connect(self.multi_airfoil_analysis_rejected)
         self.dialog.exec_()
 
     def multi_airfoil_analysis_accepted(self):
 
-        inputs = self.dialog.valuesFromWidgets()
+        inputs = self.dialog.value()
         self.multi_airfoil_analysis_settings = inputs
 
         if inputs is not None:
             mset_settings = convert_dialog_to_mset_settings(inputs['MSET'])
             mses_settings = convert_dialog_to_mses_settings(inputs['MSES'])
             mplot_settings = convert_dialog_to_mplot_settings(inputs['MPLOT'])
             self.multi_airfoil_analysis(mset_settings, mses_settings, mplot_settings)
 
     def multi_airfoil_analysis_rejected(self):
-        self.multi_airfoil_analysis_settings = self.dialog.valuesFromWidgets()
+        self.multi_airfoil_analysis_settings = self.dialog.value()
 
     def display_mses_result(self, aero_data: dict, mset_settings: dict, mses_settings: dict):
 
         def display_fail():
             # Throw a GUI error
             self.disp_message_box("MSES Analysis Failed", message_mode='error')
 
@@ -1299,36 +1479,39 @@
                     self.add_new_tab_widget(Mach_contour_widget, name)
                     break
 
         for svg_plot in SVG_PLOTS:
             if mplot_settings[SVG_SETTINGS_TR[svg_plot]]:
                 display_svg()
 
-    def plot_mses_pressure_coefficient_distribution(self, aero_data: dict, mea: MEA):
+    def plot_mses_pressure_coefficient_distribution(self, aero_data: dict, mea: MEA, mses_settings: dict):
         if self.analysis_graph is None:
             # Need to set analysis_graph to None if analysis window is closed
-            self.analysis_graph = AnalysisGraph(
+            self.analysis_graph = AnalysisGraph(theme=self.themes[self.current_theme],
                 background_color=self.themes[self.current_theme]["graph-background-color"])
             self.add_new_tab_widget(self.analysis_graph.w, "Analysis")
 
-        # Get the index of the pen to determine which style to use
-        pen_idx = self.n_converged_analyses % len(self.pens)
-
         # Get the maximum physical extent of the airfoil system in the x-direction (used to prevent showing
         # off-body pressure recovery)
         x_max = mea.get_max_x_extent()
 
         # Plot the Cp distribution for each airfoil side
-        for side in aero_data["BL"]:
+        name = (f"[{self.n_analyses}] M ({mea.name()}, \u03b1 = {aero_data['alf']:.1f}\u00b0, "
+                f"Re = {mses_settings['REYNIN']:.1E}, Ma = {mses_settings['MACHIN']:.2f})")
+
+        for side_idx, side in enumerate(aero_data["BL"]):
+            extra_opts = dict(name=name) if side_idx == 0 else {}
             pg_plot_handle = self.analysis_graph.v.plot(
-                pen=pg.mkPen(color=self.pens[pen_idx][0], style=self.pens[pen_idx][1]), name=str(self.n_analyses)
+                pen=pg.mkPen(color=self.pen(self.n_converged_analyses)[0],
+                             style=self.pen(self.n_converged_analyses)[1]), **extra_opts
             )
             x = side["x"] if isinstance(side["x"], np.ndarray) else np.array(side["x"])
             Cp = side["Cp"] if isinstance(side["Cp"], np.ndarray) else np.array(side["Cp"])
             pg_plot_handle.setData(x[np.where(x <= x_max)[0]], Cp[np.where(x <= x_max)[0]])
+            self.analysis_graph.set_legend_label_format(self.themes[self.current_theme])
 
     def multi_airfoil_analysis(self, mset_settings: dict, mses_settings: dict,
                                mplot_settings: dict):
 
         mea = self.geo_col.container()["mea"][mset_settings["mea"]]
 
         try:
@@ -1343,15 +1526,15 @@
         except OSError as os_error:
             self.disp_message_box(str(os_error), message_mode="error")
             return
 
         self.display_mses_result(aero_data, mset_settings, mses_settings)
 
         if aero_data['converged'] and not aero_data['errored_out'] and not aero_data['timed_out']:
-            self.plot_mses_pressure_coefficient_distribution(aero_data, mea)
+            self.plot_mses_pressure_coefficient_distribution(aero_data, mea, mses_settings)
             self.display_svgs(mset_settings, mplot_settings)
 
             # Update the last successful analysis directory (for easy access in field plotting)
             self.last_analysis_dir = os.path.join(mset_settings["airfoil_analysis_dir"],
                                                   mset_settings["airfoil_coord_file_name"])
 
             # Increment the number of converged analyses and the total number of analyses
@@ -1360,15 +1543,15 @@
         else:
             self.n_analyses += 1
 
     def match_airfoil(self):
         airfoil_names = [a for a in self.geo_col.container()["airfoils"].keys()]
         dialog = AirfoilMatchingDialog(self, airfoil_names=airfoil_names, theme=self.themes[self.current_theme])
         if dialog.exec_():
-            airfoil_match_settings = dialog.valuesFromWidgets()
+            airfoil_match_settings = dialog.value()
             # res = match_airfoil_ga(self.mea, target_airfoil, airfoil_name)
             res = match_airfoil(self.geo_col, airfoil_match_settings["tool_airfoil"],
                                 airfoil_match_settings["target_airfoil"])
             msg_mode = 'error'
             if hasattr(res, 'success') and res.success or hasattr(res, 'F') and res.F is not None:
                 if hasattr(res, 'x'):
                     update_params = res.x
@@ -1380,15 +1563,15 @@
                 self.geo_col.assign_design_variable_values(update_params, bounds_normalized=True)
                 msg_mode = 'info'
             self.disp_message_box(message=res.message, message_mode=msg_mode)
 
     def plot_airfoil_from_airfoiltools(self):
         dialog = AirfoilPlotDialog(self, theme=self.themes[self.current_theme])
         if dialog.exec_():
-            airfoil_name = dialog.valuesFromWidgets()
+            airfoil_name = dialog.value()
             airfoil = extract_data_from_airfoiltools(airfoil_name)
             self.airfoil_canvas.plot.plot(airfoil[:, 0], airfoil[:, 1], pen=pg.mkPen(color='orange', width=1))
 
     def setup_optimization(self):
         self.dialog = OptimizationSetupDialog(self, settings_override=self.opt_settings,
                                               geo_col=self.geo_col, theme=self.themes[self.current_theme])
         self.dialog.accepted.connect(self.optimization_accepted)
@@ -1399,15 +1582,15 @@
         exit_the_dialog = False
         early_return = False
         opt_settings_list = None
         param_dict_list = None
         geo_col_dict_list = None
         files = None
         while not exit_the_dialog and not early_return:
-            self.opt_settings = self.dialog.valuesFromWidgets()
+            self.opt_settings = self.dialog.value()
 
             loop_through_settings = False
 
             if self.opt_settings['General Settings']['batch_mode_active']:
 
                 loop_through_settings = True
 
@@ -1463,27 +1646,28 @@
                     self.disp_message_box('MSES suite executable \'mses\' not found on system path')
                     return
                 if param_dict["tool"] == "MSES" and shutil.which('mplot') is None:
                     self.disp_message_box('MPLOT suite executable \'mplot\' not found on system path')
                     return
 
                 # print(f"{opt_settings['General Settings']['use_current_mea'] = }")
-                if opt_settings['General Settings']['use_current_mea']:
-                    # mea_dict = self.mea.copy_as_param_dict(deactivate_airfoil_graphs=True)
-                    geo_col = self.geo_col.get_dict_rep()
-                else:
-                    mea_file = opt_settings['General Settings']['mea_file']
-                    if not os.path.exists(mea_file):
-                        self.disp_message_box('JMEA parametrization file not found', message_mode='error')
-                        exit_the_dialog = True
-                        early_return = True
-                        continue
-                    else:
-                        # mea_dict = load_data(mea_file)
-                        geo_col = load_data(mea_file)
+                # if opt_settings['General Settings']['use_current_mea']:
+                #     # mea_dict = self.mea.copy_as_param_dict(deactivate_airfoil_graphs=True)
+                #     geo_col = self.geo_col.get_dict_rep()
+                # else:
+                #     mea_file = opt_settings['General Settings']['mea_file']
+                #     if not os.path.exists(mea_file):
+                #         self.disp_message_box('JMEA parametrization file not found', message_mode='error')
+                #         exit_the_dialog = True
+                #         early_return = True
+                #         continue
+                #     else:
+                #         # mea_dict = load_data(mea_file)
+                #         geo_col = load_data(mea_file)
+                geo_col = self.geo_col.get_dict_rep()
 
                 # # Generate the multi-element airfoil from the dictionary
                 # mea = MEA.generate_from_param_dict(mea_dict)
 
                 # TODO: reimplement this logic
                 # norm_val_list = geo_col.extract_design_variable_values(bounds_normalized=True)
                 # if isinstance(norm_val_list, str):
@@ -1598,30 +1782,30 @@
 
         if early_return:
             self.setup_optimization()
 
         if not early_return:
             for (opt_settings, param_dict, geo_col_dict) in zip(opt_settings_list, param_dict_list, geo_col_dict_list):
                 # The next line is just to make sure any calls to the GUI are performed before the optimization
-                self.dialog.setWidgetValuesFromDict(new_inputs=opt_settings)
+                self.dialog.setValue(new_inputs=opt_settings)
 
                 # Need to regenerate the objectives and constraints here since they contain references to
                 # (non-serializable) modules which must be passed through a multiprocessing.Pipe
                 new_obj_list = [obj.func_str for obj in self.objectives]
                 new_constr_list = [constr.func_str for constr in self.constraints]
 
                 # Run the shape optimization in a worker thread
                 self.run_shape_optimization(param_dict, opt_settings,
                                             # mea.copy_as_param_dict(deactivate_airfoil_graphs=True),
                                             geo_col_dict,
                                             new_obj_list, new_constr_list,
                                             )
 
     def optimization_rejected(self):
-        self.opt_settings = self.dialog.valuesFromWidgets()
+        self.opt_settings = self.dialog.value()
         return
 
     @pyqtSlot(str, object)
     def progress_update(self, status: str, data: object):
         bcolor = self.themes[self.current_theme]["graph-background-color"]
         if status == "text" and isinstance(data, str):
             self.output_area_text(data, line_break=True)
@@ -1723,14 +1907,15 @@
 
     @staticmethod
     def shape_opt_progress_callback_fn(progress_object: object):
         if isinstance(progress_object, OptCallback):
             progress_object.exec_callback()
 
     def shape_opt_finished_callback_fn(self, success: bool):
+        self.stop_optimization(completed=True)
         self.forces_dict = {}
         self.pool = None
         self.status_bar.showMessage("Optimization Complete!", 3000)
         first_word = "Completed" if success else "Terminated"
         self.output_area_text(f"{first_word} aerodynamic shape optimization. ")
         self.output_area_text(self.generate_output_folder_link_text(self.current_opt_folder), mode="html")
         self.output_area_text("\n\n")
@@ -1795,15 +1980,15 @@
             self.showNormal()
 
     def keyPressEvent(self, a0):
         if a0.key() == Qt.Key_Escape:
             self.geo_col.clear_selected_objects()
             self.status_bar.clearMessage()
         if a0.key() == Qt.Key_Delete:
-            self.geo_col.remove_selected_objects()
+            self.airfoil_canvas.removeSelectedObjects()
             self.status_bar.clearMessage()
 
 
 # Adjustments for variable monitor resolution (from https://stackoverflow.com/a/47723454)
 if hasattr(Qt, 'AA_EnableHighDpiScaling'):
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
```

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/buttons.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/buttons.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_constraints_termination_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_constraints_termination_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_general_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_general_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_save_load_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_save_load_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/ga_warm_start_batch_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/ga_warm_start_batch_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/genetic_algorithm_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/genetic_algorithm_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mplot_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mplot_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mses_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mses_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/mset_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/mset_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/multi_point_opt_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/multi_point_opt_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/opt_constraints_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/opt_constraints_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/defaults/xfoil_settings.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/defaults/xfoil_settings.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/menu.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/menu.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7604166666666666%*

 * *Differences: {"'Dev'": "OrderedDict([('Show Constraint Graph', 'show_constraint_graph'), ('Show Param Graph', "*

 * *          "'show_param_graph')])",*

 * * "'Edit'": "{'Undo': ['undo', 'Ctrl+Z'], 'Redo': ['redo', 'Ctrl+Y']}",*

 * * "'File'": "{'Import': {'Points from File': 'load_points'}, 'Settings': 'open_settings'}",*

 * * "'Plot'": "{replace: OrderedDict([('Reference Geometry From File', 'plot_geometry')])}"}*

```diff
@@ -17,54 +17,68 @@
             ],
             "Viscous": [
                 "single_airfoil_viscous_analysis",
                 "Ctrl+Alt+V"
             ]
         }
     },
+    "Dev": {
+        "Show Constraint Graph": "show_constraint_graph",
+        "Show Param Graph": "show_param_graph"
+    },
     "Edit": {
         "Bounds": [
             "edit_bounds",
             "Ctrl+B"
+        ],
+        "Redo": [
+            "redo",
+            "Ctrl+Y"
+        ],
+        "Undo": [
+            "undo",
+            "Ctrl+Z"
         ]
     },
     "File": {
         "Export": {
             "Airfoil Coordinates": "export_coordinates",
             "Control Points": "export_control_points",
             "Design Variable Values": "export_design_variable_values",
             "IGES": "export_IGES",
             "NXOpen Macro": "export_nx_macro"
         },
         "Import": {
             "Design Variable Values": "import_design_variable_values",
-            "Optimized Airfoil": "import_algorithm_pkl_file"
+            "Optimized Airfoil": "import_algorithm_pkl_file",
+            "Points from File": "load_points"
         },
         "New": [
             "new_geo_col",
             "Ctrl+N"
         ],
         "Open": [
             "load_geo_col",
             "Ctrl+O"
         ],
         "Save": [
             "save_geo_col",
             "Ctrl+S"
         ],
-        "Save As": "save_as_geo_col"
+        "Save As": "save_as_geo_col",
+        "Settings": "open_settings"
     },
     "Optimization": {
         "Run": [
             "setup_optimization",
             "Ctrl+Alt+O"
         ]
     },
     "Plot": {
-        "Geometry From File": "plot_geometry"
+        "Reference Geometry From File": "plot_geometry"
     },
     "Tools": {
         "Airfoil Statistics": "display_airfoil_statistics",
         "Match Airfoil": "match_airfoil",
         "Plot Airfoil from AirfoilTools": "plot_airfoil_from_airfoiltools",
         "Take Screenshot": [
             "take_screenshot",
```

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/q_settings_descriptions.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/q_settings_descriptions.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'angle_unit'": "['Default angle unit', 'deg']",*

 * * "'length_unit'": "['Default length unit', 'm']",*

 * * "'load_points_default_open_location'": "['Directory where load_points() starts by default', '']"}*

```diff
@@ -1,8 +1,12 @@
 {
+    "angle_unit": [
+        "Default angle unit",
+        "deg"
+    ],
     "axis-label-font-family": [
         "Default axis label font family",
         "DejaVu Sans"
     ],
     "axis-label-point-size": [
         "Default axis label font point size",
         12
@@ -55,14 +59,22 @@
         "Hovered pen width for curves",
         3
     ],
     "dark_theme_checked": "set_theme('dark') used if true, else set_theme('light')",
     "ga-settings-dir": "Directory where GAGeneralSettingsDialogWidget.load_opt_settings starts",
     "geometry_plot_default_open_location": "Directory where plot_geometry() starts by default",
     "jmea_default_open_location": "Directory where load_mea() starts by default",
+    "length_unit": [
+        "Default length unit",
+        "m"
+    ],
+    "load_points_default_open_location": [
+        "Directory where load_points() starts by default",
+        ""
+    ],
     "parameter_list_default_open_location": "Directory where import_parameter_list() starts by default",
     "pkl_file": "Starting value for the .pkl file to extract",
     "pkl_file_dir": "Directory where import_algorithm_pkl_file starts",
     "pkl_index": "Value of the index used to extract parameter vector from optimal set",
     "pkl_use_index": "Whether to extract parameter vector from optimal set by index",
     "pkl_use_weights": "Whether to extract parameter vector from optimal set by weights",
     "pkl_weights": "Value of the weights used to extract parameter vector from optimal set (as a string)",
```

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/themes/dark_theme.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/themes/dark_theme.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/gui_settings/themes/light_theme.json` & `pymead-2.0.0b4/pymead/gui/gui_settings/themes/light_theme.json`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/help_browser.py` & `pymead-2.0.0b4/pymead/gui/help_browser.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/hoverable_curve.py` & `pymead-2.0.0b4/pymead/gui/hoverable_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pyqtgraph as pg
 from PyQt5.QtCore import pyqtSignal
 
 from pymead import q_settings, GUI_SETTINGS_DIR
 from pymead.core.bezier import Bezier
-from pymead.core.line import LineSegment
+from pymead.core.line import LineSegment, PolyLine
 from pymead.core.parametric_curve import PCurveData, ParametricCurve
 from pymead.core.point import PointSequence, Point
 from pymead.gui.draggable_point import DraggablePoint
 from pymead.utils.misc import convert_str_to_Qt_dash_pattern
 from pymead.utils.read_write_files import load_data
 
 q_settings_descriptions = load_data(os.path.join(GUI_SETTINGS_DIR, "q_settings_descriptions.json"))
```

### Comparing `pymead-2.0.0b3/pymead/gui/infty_doublespinbox.py` & `pymead-2.0.0b4/pymead/gui/infty_doublespinbox.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/input_dialog.py` & `pymead-2.0.0b4/pymead/gui/dialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 import PyQt5.QtWidgets
 import numpy as np
 import pyqtgraph as pg
 from PyQt5.QtCore import QEvent
 from PyQt5.QtCore import Qt, pyqtSignal, QObject, QRect
 from PyQt5.QtCore import pyqtSlot, QStandardPaths
-from PyQt5.QtGui import QFont
+from PyQt5.QtGui import QFont, QTextDocument
 from PyQt5.QtWidgets import (QWidget, QGridLayout, QLabel, QPushButton, QCheckBox, QTabWidget, QSpinBox,
                              QDoubleSpinBox, QComboBox, QDialog, QVBoxLayout, QSizeGrip, QDialogButtonBox, QMessageBox,
                              QFormLayout, QRadioButton)
+from pymead.core.airfoil import Airfoil
 
 from pymead import GUI_DEFAULTS_DIR, q_settings, GUI_DIALOG_WIDGETS_DIR
 from pymead.analysis import cfd_output_templates
 from pymead.analysis.utils import viscosity_calculator
+from pymead.core import UNITS
 from pymead.core.geometry_collection import GeometryCollection
 from pymead.core.line import PolyLine
 from pymead.core.mea import MEA
 from pymead.gui.bounds_values_table import BoundsValuesTable
 from pymead.gui.default_settings import xfoil_settings_default
 from pymead.gui.file_selection import *
 from pymead.gui.infty_doublespinbox import InftyDoubleSpinBox
@@ -238,15 +240,15 @@
         # triggered during initialization):
         for w_name, w_dict in self.settings.items():
             widget = self.widget_dict[w_name]['widget']
             if w_dict['widget_type'] in get_set_value_names.keys():
                 getattr(widget, get_set_value_names[w_dict['widget_type']][2]).connect(
                     partial(self.dialogChanged, w_name=w_name))
 
-    def valuesFromWidgets(self):
+    def value(self):
         """This method is used to extract the data from the Dialog"""
         output_dict = {w_name: None for w_name in self.widget_dict.keys()}
         for w_name, w in self.widget_dict.items():
             if self.settings[w_name]['widget_type'] in get_set_value_names.keys():
                 output_dict[w_name] = getattr(w['widget'],
                                               get_set_value_names[self.settings[w_name]['widget_type']][0]
                                               )()
@@ -257,60 +259,60 @@
                 output_dict[w_name] = None
         return output_dict
 
     @staticmethod
     def activate_deactivate_from_checkbox(widget, state):
         widget.setReadOnly(not state)
 
-    def setWidgetValuesFromDict(self, new_values: dict):
+    def setValue(self, new_values: dict):
         for k, v in new_values.items():
             if v is not None:
                 if self.widget_dict[k]['checkbox'] is not None:
                     self.widget_dict[k]['checkbox'].setCheckState(v[1])
                     getattr(self.widget_dict[k]['widget'], get_set_value_names[self.settings[k]['widget_type']][1])(v[0])
                 else:
                     getattr(self.widget_dict[k]['widget'], get_set_value_names[self.settings[k]['widget_type']][1])(v)
 
     def dialogChanged(self, *_, w_name: str):
-        new_inputs = self.valuesFromWidgets()
+        new_inputs = self.value()
         self.updateDialog(new_inputs, w_name)
 
     @abstractmethod
     def updateDialog(self, new_inputs: dict, w_name: str):
-        """Required method which reacts to changes in the dialog inputs. Use the :code:`setWidgetValuesFromDict` method to
+        """Required method which reacts to changes in the dialog inputs. Use the :code:`setValue` method to
         update the dialog at the end of this method if necessary."""
         pass
 
 
 class PymeadDialogHTabWidget(QTabWidget):
 
     sigTabsChanged = pyqtSignal(object)
 
     def __init__(self, parent, widgets: dict, settings_override: dict = None):
         super().__init__()
         self.w_dict = widgets
         self.generateWidgets()
         if settings_override is not None:
-            self.setWidgetValuesFromDict(settings_override)
+            self.setValue(settings_override)
 
     def generateWidgets(self):
         for k, v in self.w_dict.items():
             self.addTab(v, k)
 
     def regenerateWidgets(self):
         self.clear()
         self.generateWidgets()
         self.sigTabsChanged.emit([k for k in self.w_dict.keys()])
 
-    def setWidgetValuesFromDict(self, new_values: dict):
+    def setValue(self, new_values: dict):
         for k, v in new_values.items():
-            self.w_dict[k].setWidgetValuesFromDict(new_values=v)
+            self.w_dict[k].setValue(new_values=v)
 
-    def valuesFromWidgets(self):
-        return {k: v.valuesFromWidgets() for k, v in self.w_dict.items()}
+    def value(self):
+        return {k: v.value() for k, v in self.w_dict.items()}
 
 
 class PymeadLabeledSpinBox(QObject):
 
     sigValueChanged = pyqtSignal(int)
 
     def __init__(self, label: str = "", tool_tip: str = "", minimum: int = None, maximum: int = None,
@@ -380,39 +382,113 @@
     def setReadOnly(self, read_only: bool):
         self.widget.setReadOnly(read_only)
 
     def setActive(self, active: bool):
         self.widget.setReadOnly(not active)
 
 
+class PymeadLabeledScientificDoubleSpinBox(QObject):
+
+    sigValueChanged = pyqtSignal(float)
+
+    def __init__(self, label: str = "", tool_tip: str = "", minimum: float = None, maximum: float = None,
+                 value: float = None, decimals: int = None, single_step: float = None, read_only: bool = None):
+        self.label = QLabel(label)
+        self.widget = ScientificDoubleSpinBox()
+        self.label.setToolTip(tool_tip)
+        self.widget.setToolTip(tool_tip)
+        if minimum is not None:
+            self.widget.setMinimum(minimum)
+        if maximum is not None:
+            self.widget.setMaximum(maximum)
+        if decimals is not None:
+            self.widget.setDecimals(decimals)
+        if value is not None:
+            self.widget.setValue(value)
+        if single_step is not None:
+            self.widget.setSingleStep(single_step)
+        if read_only is not None:
+            self.widget.setReadOnly(read_only)
+        self.push = None
+        super().__init__()
+        self.widget.valueChanged.connect(self.sigValueChanged)
+
+    def setValue(self, value: float):
+        self.widget.setValue(value)
+
+    def value(self):
+        return self.widget.value()
+
+    def setReadOnly(self, read_only: bool):
+        self.widget.setReadOnly(read_only)
+
+    def setActive(self, active: bool):
+        self.widget.setReadOnly(not active)
+
+
 class PymeadLabeledLineEdit(QObject):
 
     sigValueChanged = pyqtSignal(str)
 
-    def __init__(self, label: str = "", tool_tip: str = "", text: str = "", push_label: str = None):
+    def __init__(self, label: str = "", tool_tip: str = "", text: str = "", push_label: str = None,
+                 read_only: bool = None):
         self.label = QLabel(label)
         self.widget = QLineEdit(text)
         self.label.setToolTip(tool_tip)
         self.widget.setToolTip(tool_tip)
         self.push = None
 
         if push_label is not None:
             self.push = QPushButton(push_label)
+        if read_only is not None:
+            self.setReadOnly(read_only)
 
         super().__init__()
         self.widget.textChanged.connect(self.sigValueChanged)
 
     def setValue(self, text: str):
         self.widget.setText(text)
 
     def value(self):
         return self.widget.text()
 
     def setReadOnly(self, read_only: bool):
         self.widget.setReadOnly(read_only)
+        if self.push is not None:
+            self.push.setEnabled(not read_only)
+
+
+class PymeadLabeledPlainTextEdit(QObject):
+
+    sigValueChanged = pyqtSignal()
+
+    def __init__(self, label: str = "", tool_tip: str = "", text: str = "", push_label: str = None,
+                 read_only: bool = None):
+        self.label = QLabel(label)
+        self.widget = QPlainTextEdit(text)
+        self.label.setToolTip(tool_tip)
+        self.widget.setToolTip(tool_tip)
+        self.push = None
+
+        if push_label is not None:
+            self.push = QPushButton(push_label)
+        if read_only is not None:
+            self.setReadOnly(read_only)
+
+        super().__init__()
+        self.widget.textChanged.connect(self.sigValueChanged)
+
+    def setValue(self, text: str):
+        self.widget.setPlainText(text)
+
+    def value(self):
+        return self.widget.toPlainText()
+
+    def setReadOnly(self, read_only: bool):
+        self.widget.setReadOnly(read_only)
 
 
 class PymeadLabeledComboBox(QObject):
 
     sigValueChanged = pyqtSignal(str)
 
     def __init__(self, label: str = "", tool_tip: str = "", items: typing.List[str] = None,
@@ -481,45 +557,71 @@
 
     @staticmethod
     def value():
         return None
 
 
 class PymeadDialogWidget2(QWidget):
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, **kwargs):
         super().__init__(parent=parent)
+        self.widget_dict = None
+        self.lay = QGridLayout()
+        self.setLayout(self.lay)
+        self.initializeWidgets(**kwargs)
+        self.addWidgets(**kwargs)
+        self.establishWidgetConnections()
 
     @abstractmethod
     def initializeWidgets(self, *args, **kwargs):
         pass
 
-    @abstractmethod
-    def setWidgetValuesFromDict(self, *args, **kwargs):
-        pass
+    def addWidgets(self, *args, **kwargs):
+        # Add all the widgets
+        row_count = 0
+        column = 0
+        for widget_name, widget in self.widget_dict.items():
+            row_span = 1
+            col_span = 2 if widget.push is None else 1
+            self.lay.addWidget(widget.label, row_count, column, 1, 1)
+            self.lay.addWidget(widget.widget, row_count, column + 1, row_span, col_span)
 
-    @abstractmethod
-    def valuesFromWidgets(self) -> dict:
+            if widget.push is not None:
+                self.lay.addWidget(widget.push, row_count, column + 2, row_span, col_span)
+
+            row_count += 1
+
+    def establishWidgetConnections(self):
         pass
 
+    def setValue(self, d: dict):
+        for d_name, d_value in d.items():
+            try:
+                self.widget_dict[d_name].setValue(d_value)
+            except KeyError:
+                pass
+
+    def value(self) -> dict:
+        return {k: v.value() for k, v in self.widget_dict.items()}
+
 
 class PymeadDialogVTabWidget(VerticalTabWidget):
     def __init__(self, parent, widgets: dict, settings_override: dict = None):
         super().__init__()
         self.w_dict = widgets
         for k, v in self.w_dict.items():
             self.addTab(v, k)
         if settings_override is not None:
-            self.setWidgetValuesFromDict(settings_override)
+            self.setValue(settings_override)
 
-    def setWidgetValuesFromDict(self, new_values: dict):
+    def setValue(self, new_values: dict):
         for k, v in new_values.items():
-            self.w_dict[k].setWidgetValuesFromDict(v)
+            self.w_dict[k].setValue(v)
 
-    def valuesFromWidgets(self):
-        return {k: v.valuesFromWidgets() for k, v in self.w_dict.items()}
+    def value(self):
+        return {k: v.value() for k, v in self.w_dict.items()}
 
 
 class PymeadDialog(QDialog):
 
     _gripSize = 2
 
     """This subclass of QDialog forces the selection of a WindowTitle and matches the visual format of the GUI"""
@@ -562,19 +664,19 @@
             f"""background-color: qlineargradient(x1: 0.0, y1: 0.5, x2: 1.0, y2: 0.5, 
                     stop: 0 {theme['title-gradient-color']}, 
                     stop: 0.6 {theme['background-color']})""")
 
     # def setInputs(self):
     #     self.w.setInputs()
 
-    def setWidgetValuesFromDict(self, new_inputs):
-        self.w.setWidgetValuesFromDict(new_values=new_inputs)
+    def setValue(self, new_inputs):
+        self.w.setValue(new_values=new_inputs)
 
-    def valuesFromWidgets(self):
-        return self.w.valuesFromWidgets()
+    def value(self):
+        return self.w.value()
 
     def create_button_box(self):
         """Creates a ButtonBox to add to the Layout. Can be overridden to add additional functionality.
 
         Returns
         =======
         QDialogButtonBox
@@ -712,17 +814,20 @@
         self.airfoil_names = [] if initial_mea is None else [a.name() for a in initial_mea.airfoils]
         self.widget_dict = {}
         self.grid_widgets = {}
         self.grid_widget = None
         self.grid_layout = None
         self.setValue()
 
-    def onMEAChanged(self, mea: MEA):
+    def onMEAChanged(self, mea: MEA or None):
         # Updated the widget based on a new MEA
-        self.airfoil_names = [airfoil.name() for airfoil in mea.airfoils]
+        if mea is None:
+            self.airfoil_names = []
+        else:
+            self.airfoil_names = [airfoil.name() for airfoil in mea.airfoils]
         self.setValue()
 
     def add_tab(self, name: str):
         self.grid_widget = QWidget()
         self.grid_layout = QGridLayout(self)
         self.grid_widget.setLayout(self.grid_layout)
         self.widget_dict[name] = {
@@ -797,17 +902,20 @@
         self.airfoil_names = [] if initial_mea is None else [a.name() for a in initial_mea.airfoils]
         self.widget_dict = {}
         self.grid_widgets = {}
         self.grid_widget = None
         self.grid_layout = None
         self.setValue()
 
-    def onMEAChanged(self, mea: MEA):
+    def onMEAChanged(self, mea: MEA or None):
         # Updated the widget based on a new MEA
-        self.airfoil_names = [airfoil.name() for airfoil in mea.airfoils]
+        if mea:
+            self.airfoil_names = [airfoil.name() for airfoil in mea.airfoils]
+        else:
+            self.airfoil_names = []
         self.setValue()
 
     def add_tab(self, name: str):
         self.grid_widget = QWidget()
         self.grid_layout = QGridLayout(self)
         self.grid_widget.setLayout(self.grid_layout)
         self.widget_dict[name] = {
@@ -1310,69 +1418,65 @@
                 airfoil_names = [a.name() for a in self.geo_col.container()["mea"][
                     self.widget_dict["mea"]["widget"].currentText()].airfoils]
             else:
                 airfoil_names = []
             self.widget_dict["multi_airfoil_grid"]["widget"].onAirfoilListChanged(airfoil_names)
 
     def saveas_mset_mses_mplot_settings(self):
-        all_inputs = get_parent(self, 2).valuesFromWidgets()
+        all_inputs = get_parent(self, 2).value()
         mses_inputs = {k: v for k, v in all_inputs.items() if k in ["MSET", "MSES", "MPLOT"]}
         json_dialog = select_json_file(parent=self)
         if json_dialog.exec_():
             input_filename = json_dialog.selectedFiles()[0]
             if not os.path.splitext(input_filename)[-1] == '.json':
                 input_filename = input_filename + '.json'
             save_data(mses_inputs, input_filename)
             # if get_parent(self, 4):
             #     get_parent(self, 4).current_settings_save_file = input_filename
             # else:
             #     self.current_save_file = input_filename
             get_parent(self, 3).setStatusTip(f"Saved MSES settings to {input_filename}")
 
     def load_mset_mses_mplot_settings(self):
-        override_inputs = get_parent(self, 2).valuesFromWidgets()
+        override_inputs = get_parent(self, 2).value()
         load_dialog = select_existing_json_file(parent=self)
         if load_dialog.exec_():
             load_file = load_dialog.selectedFiles()[0]
             new_inputs = load_data(load_file)
             for k, v in new_inputs.items():
                 override_inputs[k] = v
             # great_great_grandparent = get_parent(self, depth=4)
             # if great_great_grandparent:
             #     great_great_grandparent.current_settings_save_file = load_file
             # else:
             #     self.current_save_file = load_file
             get_parent(self, 3).setWindowTitle(f"Optimization Setup - {os.path.split(load_file)[-1]}")
-            get_parent(self, 2).setWidgetValuesFromDict(override_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
+            get_parent(self, 2).setValue(override_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
             get_parent(self, 2).setStatusTip(f"Loaded {load_file}")
 
     def show_airfoil_coordinates_preview(self, _):
-        override_inputs = get_parent(self, 2).valuesFromWidgets()
+        override_inputs = get_parent(self, 2).value()
         use_downsampling = bool(override_inputs["MSET"]["use_downsampling"])
         downsampling_max_pts = override_inputs["MSET"]["downsampling_max_pts"]
         downsampling_curve_exp = override_inputs["MSET"]["downsampling_curve_exp"]
         preview_dialog = DownsamplingPreviewDialog(use_downsampling=use_downsampling,
                                                    downsampling_max_pts=downsampling_max_pts,
                                                    downsampling_curve_exp=downsampling_curve_exp,
                                                    parent=self)
         preview_dialog.exec_()
 
 
 class MSETDialogWidget2(PymeadDialogWidget2):
 
-    sigMEAChanged = pyqtSignal(MEA)
+    sigMEAChanged = pyqtSignal(object)
 
     def __init__(self, geo_col: GeometryCollection, theme: dict, parent=None):
-        super().__init__(parent=parent)
         self.geo_col = geo_col
         self.theme = theme
-        self.widget_dict = None
-        self.lay = QGridLayout()
-        self.setLayout(self.lay)
-        self.initializeWidgets(label_column_split="timeout")
+        super().__init__(parent=parent, label_column_split="timeout")
 
     def initializeWidgets(self, label_column_split: str):
         initial_mea_names = [k for k in self.geo_col.container()["mea"].keys()]
         initial_mea = None if len(initial_mea_names) == 0 else self.geo_col.container()["mea"][initial_mea_names[0]]
         self.widget_dict = {
             "mea": PymeadLabeledComboBox(label="MEA", items=initial_mea_names),
             "grid_bounds": GridBounds(self),
@@ -1415,19 +1519,20 @@
             "downsampling_curve_exp": PymeadLabeledDoubleSpinBox(
                 label="Downsammpling curvature exponent", minimum=0.0001, maximum=9999., value=2.0,
                 tool_tip="Importance of curvature in the downsampling scheme.\nValues close to 0 place high emphasis "
                          "on curvature,\nwhile values close to positive infinity place no emphasis\non curvature and "
                          "leave the parameter\nvector effectively uniformly spaced")
         }
 
+    def addWidgets(self, **kwargs):
         # Add all the widgets
         row_count = 0
         column = 0
         for widget_name, widget in self.widget_dict.items():
-            if widget_name == label_column_split:
+            if widget_name == kwargs["label_column_split"]:
                 column = 4
                 row_count = 0
             if widget_name == "multi_airfoil_grid":
                 row_span = 7
                 col_span = 3
             elif widget_name == "grid_bounds":
                 row_span = 3
@@ -1443,181 +1548,96 @@
                 self.lay.addWidget(widget.widget, row_count, column + 1, row_span, col_span)
 
                 if widget.push is not None:
                     self.lay.addWidget(widget.push, row_count, column + 2, row_span, col_span)
 
             row_count += row_span
 
+    def establishWidgetConnections(self):
         # Connect the MEA combobox to the "MEA changed" signal
         self.widget_dict["mea"].widget.currentTextChanged.connect(self.onMEAChanged)
         self.sigMEAChanged.connect(self.widget_dict["multi_airfoil_grid"].onMEAChanged)
         # Show a preview of the downsampling when the button is pushed
         self.widget_dict["use_downsampling"].push.clicked.connect(self.showAirfoilCoordinatesPreview)
         # Connect the airfoil analysis directory button to the choose directory function
         self.widget_dict["airfoil_analysis_dir"].push.clicked.connect(
             partial(select_directory, self, line_edit=self.widget_dict["airfoil_analysis_dir"].widget))
         # Connect the load and save settings buttons
         self.widget_dict["load_mses_settings"].widget.clicked.connect(self.loadMSESSuiteSettings)
         self.widget_dict["save_as_mses_settings"].widget.clicked.connect(self.saveasMSESSuiteSettings)
 
     def onMEAChanged(self, mea_name: str):
-        self.sigMEAChanged.emit(self.geo_col.container()["mea"][mea_name])
+        if mea_name:
+            self.sigMEAChanged.emit(self.geo_col.container()["mea"][mea_name])
+        else:
+            self.sigMEAChanged.emit(None)
 
-    def setWidgetValuesFromDict(self, d: dict):
+    def setValue(self, d: dict):
         for d_name, d_value in d.items():
             try:
                 self.widget_dict[d_name].setValue(d_value)
             except KeyError:
                 pass
 
-    def valuesFromWidgets(self) -> dict:
+    def value(self) -> dict:
         return {k: v.value() for k, v in self.widget_dict.items()}
 
     def saveasMSESSuiteSettings(self):
-        all_inputs = get_parent(self, 2).valuesFromWidgets()
+        all_inputs = get_parent(self, 2).value()
         mses_inputs = {k: v for k, v in all_inputs.items() if k in ["MSET", "MSES", "MPLOT"]}
         json_dialog = select_json_file(parent=self)
         if json_dialog.exec_():
             input_filename = json_dialog.selectedFiles()[0]
             if not os.path.splitext(input_filename)[-1] == '.json':
                 input_filename = input_filename + '.json'
             save_data(mses_inputs, input_filename)
             get_parent(self, 3).setStatusTip(f"Saved MSES settings to {input_filename}")
 
     def loadMSESSuiteSettings(self):
-        override_inputs = get_parent(self, 2).valuesFromWidgets()
+        override_inputs = get_parent(self, 2).value()
         load_dialog = select_existing_json_file(parent=self)
         if load_dialog.exec_():
             load_file = load_dialog.selectedFiles()[0]
             new_inputs = load_data(load_file)
             for k, v in new_inputs.items():
                 override_inputs[k] = v
             get_parent(self, 3).setWindowTitle(f"Optimization Setup - {os.path.split(load_file)[-1]}")
-            get_parent(self, 2).setWidgetValuesFromDict(override_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
+            get_parent(self, 2).setValue(override_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
             get_parent(self, 2).setStatusTip(f"Loaded {load_file}")
 
     def showAirfoilCoordinatesPreview(self):
-        mset_settings = self.valuesFromWidgets()
+        mset_settings = self.value()
         preview_dialog = DownsamplingPreviewDialog(
             theme=self.theme, mea_name=self.widget_dict["mea"].widget.currentText(),
             max_airfoil_points=mset_settings["downsampling_max_pts"] if bool(mset_settings["use_downsampling"]) else None,
             curvature_exp=mset_settings["downsampling_curve_exp"],
             parent=self)
         preview_dialog.exec_()
 
 
-class MSESDialogWidget(PymeadDialogWidget):
-    def __init__(self, geo_col: GeometryCollection):
-        initial_mea_names = [k for k in geo_col.container()["mea"].keys()]
-        initial_mea = None if len(initial_mea_names) == 0 else geo_col.container()["mea"][initial_mea_names[0]]
-
-        param_list = [param for param in geo_col.container()["params"]]
-        dv_list = [dv + " (DV)" for dv in geo_col.container()["desvar"]]
-        super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'mses_settings.json'),
-                         initial_mea=initial_mea, param_list=param_list + dv_list, geo_col=geo_col)
-        self.geo_col = geo_col
-
-    def deactivate_AD(self, read_only: bool):
-        self.widget_dict['AD']['widget'].setReadOnly(read_only)
-        self.widget_dict['AD_number']['widget'].setReadOnly(read_only)
-        if not read_only:
-            self.widget_dict['AD']['widget'].setToolTip("")
-            self.widget_dict['AD_number']['widget'].setToolTip("")
-        else:
-            self.widget_dict['AD']['widget'].setToolTip(self.settings['AD']['setToolTip'])
-            self.widget_dict['AD_number']['widget'].setToolTip(self.settings['AD_number']['setToolTip'])
-
-    def calculate_and_set_Reynolds_number(self, new_inputs: dict):
-        Re_widget = self.widget_dict['REYNIN']['widget']
-        nu = viscosity_calculator(new_inputs['T'], rho=new_inputs['rho'])
-        a = np.sqrt(new_inputs['gam'] * new_inputs['R'] * new_inputs['T'])
-        V = new_inputs['MACHIN'] * a
-        Re_widget.setValue(V * new_inputs['L'] / nu)
-
-    def change_prescribed_aero_parameter(self, current_text: str):
-        w1 = self.widget_dict['ALFAIN']['widget']
-        w2 = self.widget_dict['CLIFIN']['widget']
-        if current_text == 'Specify Angle of Attack':
-            bools = (False, True)
-        elif current_text == 'Specify Lift Coefficient':
-            bools = (True, False)
-        else:
-            raise ValueError('Invalid value of currentText for QComboBox (alfa/Cl')
-        w1.setReadOnly(bools[0])
-        w2.setReadOnly(bools[1])
-
-    def change_prescribed_flow_variables(self, current_text: str):
-        w1 = self.widget_dict['P']['widget']
-        w2 = self.widget_dict['T']['widget']
-        w3 = self.widget_dict['rho']['widget']
-        if current_text == 'Specify Pressure, Temperature':
-            bools = (False, False, True)
-        elif current_text == 'Specify Pressure, Density':
-            bools = (False, True, False)
-        elif current_text == 'Specify Temperature, Density':
-            bools = (True, False, False)
-        else:
-            raise ValueError('Invalid value of currentText for QComboBox (P/T/rho)')
-        w1.setReadOnly(bools[0])
-        w2.setReadOnly(bools[1])
-        w3.setReadOnly(bools[2])
-
-    def change_Re_active_state(self, new_inputs: dict):
-        active = new_inputs['spec_Re']
-        widget_names = ['P', 'T', 'rho', 'L', 'R', 'gam']
-        skip_P, skip_T, skip_rho = False, False, False
-        if new_inputs['spec_P_T_rho'] == 'Specify Pressure, Temperature' and self.widget_dict['rho'][
-            'widget'].isReadOnly():
-            skip_rho = True
-        if new_inputs['spec_P_T_rho'] == 'Specify Pressure, Density' and self.widget_dict['T']['widget'].isReadOnly():
-            skip_T = True
-        if new_inputs['spec_P_T_rho'] == 'Specify Temperature, Density' and self.widget_dict['P'][
-            'widget'].isReadOnly():
-            skip_P = True
-        for widget_name in widget_names:
-            if not (skip_rho and widget_name == 'rho') and not (skip_P and widget_name == 'P') and not (
-                    skip_T and widget_name == 'T'):
-                self.widget_dict[widget_name]['widget'].setReadOnly(active)
-        self.widget_dict['REYNIN']['widget'].setReadOnly(not active)
-        self.widget_dict['spec_P_T_rho']['widget'].setEnabled(not active)
-        if not active:
-            self.calculate_and_set_Reynolds_number(new_inputs)
+class PanelDialogWidget(PymeadDialogWidget2):
+    def __init__(self, settings_override: dict, parent=None):
+        super().__init__(parent=parent)
+        if settings_override:
+            self.setValue(settings_override)
+        self.setMinimumWidth(250)
 
-    def updateDialog(self, new_inputs: dict, w_name: str):
-        if w_name == 'AD_number':
-            self.widget_dict['AD']['widget'].onADListChanged([str(j + 1) for j in range(new_inputs['AD_number'])])
-        if w_name == 'AD_active':
-            self.deactivate_AD(not new_inputs['AD_active'])
-        if w_name == 'spec_Re':
-            self.change_Re_active_state(new_inputs)
-        if w_name == 'spec_P_T_rho':
-            self.change_prescribed_flow_variables(new_inputs['spec_P_T_rho'])
-        if w_name == 'spec_alfa_Cl':
-            self.change_prescribed_aero_parameter(new_inputs['spec_alfa_Cl'])
-        if w_name in ['P', 'T', 'rho', 'R', 'gam', 'L', 'MACHIN'] and not self.widget_dict[w_name][
-            'widget'].isReadOnly():
-            if self.widget_dict['P']['widget'].isReadOnly():
-                self.widget_dict['P']['widget'].setValue(new_inputs['rho'] * new_inputs['R'] * new_inputs['T'])
-            elif self.widget_dict['T']['widget'].isReadOnly():
-                self.widget_dict['T']['widget'].setValue(new_inputs['P'] / new_inputs['R'] / new_inputs['rho'])
-            elif self.widget_dict['rho']['widget'].isReadOnly():
-                self.widget_dict['rho']['widget'].setValue(new_inputs['P'] / new_inputs['R'] / new_inputs['T'])
-            new_inputs = self.valuesFromWidgets()
-            if not (w_name == 'MACHIN' and new_inputs['spec_Re']):
-                self.calculate_and_set_Reynolds_number(new_inputs)
+    def initializeWidgets(self, *args, **kwargs):
+        self.widget_dict = {
+            "alfa": PymeadLabeledDoubleSpinBox(label="\u03b1 (\u00b0)", minimum=-np.inf, maximum=np.inf,
+                                               value=0.0, decimals=8, single_step=1.0,
+                                               tool_tip="Angle of attack (if the geometry is already at an angle"
+                                                        "of attack, this value will be added on)")
+        }
 
 
 class MSESDialogWidget2(PymeadDialogWidget2):
     def __init__(self, geo_col: GeometryCollection, parent=None):
-        super().__init__(parent=parent)
         self.geo_col = geo_col
-        self.widget_dict = None
-        self.lay = QGridLayout()
-        self.setLayout(self.lay)
-        self.initializeWidgets(label_column_split="timeout")
+        super().__init__(parent=parent, label_column_split="timeout")
 
     def initializeWidgets(self, label_column_split: str):
 
         initial_mea_names = [k for k in self.geo_col.container()["mea"].keys()]
         initial_mea = None if len(initial_mea_names) == 0 else self.geo_col.container()["mea"][initial_mea_names[0]]
 
         param_list = [param for param in self.geo_col.container()["params"]]
@@ -1693,19 +1713,20 @@
                                                initial_state=0),
             "AD_number": PymeadLabeledSpinBox(label="Num. Actuator Disks", minimum=0, maximum=5, value=0,
                                               read_only=True, tool_tip="'Actuator disks active' must be checked "
                                                                        "to enable modification of the number of AD's"),
             "AD": ADWidget(parent=self, param_list=param_list + dv_list, geo_col=self.geo_col, number_AD=0)
         }
 
+    def addWidgets(self, *args, **kwargs):
         # Add all the widgets
         row_count = 0
         column = 0
         for widget_name, widget in self.widget_dict.items():
-            if widget_name == label_column_split:
+            if widget_name == kwargs["label_column_split"]:
                 column = 4
                 row_count = 0
             if widget_name == "AD":
                 row_span = 5
                 col_span = 4
             elif widget_name == "xtrs":
                 row_span = 3
@@ -1721,14 +1742,15 @@
                 self.lay.addWidget(widget.widget, row_count, column + 1, row_span, col_span)
 
                 if widget.push is not None:
                     self.lay.addWidget(widget.push, row_count, column + 2, row_span, col_span)
 
             row_count += row_span
 
+    def establishWidgetConnections(self):
         # Create the required connections
         self.widget_dict["AD_active"].sigValueChanged.connect(self.widget_dict["AD_number"].setActive)
         self.widget_dict["AD_active"].sigValueChanged.connect(self.widget_dict["AD"].setAllActive)
         self.widget_dict["AD_number"].sigValueChanged.connect(self.widget_dict["AD"].numberADChanged)
         self.widget_dict["spec_P_T_rho"].sigValueChanged.connect(self.spec_P_T_rho_changed)
         for thermo_var in ("P", "T", "rho", "gam", "R", "MACHIN", "L"):
             self.widget_dict[thermo_var].sigValueChanged.connect(self.recalculateThermoState)
@@ -1747,55 +1769,57 @@
         if "Density" in spec_P_T_rho:
             self.widget_dict["rho"].setReadOnly(False)
         else:
             self.widget_dict["rho"].setReadOnly(True)
 
     def spec_Re_changed(self, state: int):
         if state:
-            for thermo_var in ("P", "T", "rho", "gam", "R", "MACHIN", "L", "spec_P_T_rho"):
+            for thermo_var in ("P", "T", "rho", "gam", "R", "L", "spec_P_T_rho"):
                 self.widget_dict[thermo_var].setReadOnly(True)
             self.widget_dict["REYNIN"].setReadOnly(False)
         else:
-            for thermo_var in ("P", "T", "rho", "gam", "R", "MACHIN", "L", "spec_P_T_rho"):
+            for thermo_var in ("P", "T", "rho", "gam", "R", "L", "spec_P_T_rho"):
                 self.widget_dict[thermo_var].setReadOnly(False)
             self.widget_dict["REYNIN"].setReadOnly(True)
             self.spec_P_T_rho_changed(self.widget_dict["spec_P_T_rho"].value())
             self.recalculateThermoState(None)
 
     def spec_alfa_Cl_changed(self, alfa_Cl: str):
         if "Angle" in alfa_Cl:
             self.widget_dict["ALFAIN"].setReadOnly(False)
             self.widget_dict["CLIFIN"].setReadOnly(True)
         else:
             self.widget_dict["ALFAIN"].setReadOnly(True)
             self.widget_dict["CLIFIN"].setReadOnly(False)
 
     def recalculateThermoState(self, _):
+        if self.widget_dict["spec_Re"].value():
+            return
         spec_P_T_rho = self.widget_dict["spec_P_T_rho"].value()
         R = self.widget_dict["R"].value()
         gam = self.widget_dict["gam"].value()
         if "Pressure" in spec_P_T_rho and "Temperature" in spec_P_T_rho:
             self.widget_dict["rho"].setValue(self.widget_dict["P"].value() / (R * self.widget_dict["T"].value()))
         elif "Pressure" in spec_P_T_rho and "Density" in spec_P_T_rho:
             self.widget_dict["T"].setValue(self.widget_dict["P"].value() / (R * self.widget_dict["rho"].value()))
         else:
             self.widget_dict["P"].setValue(self.widget_dict["rho"].value() * R * self.widget_dict["T"].value())
         nu = viscosity_calculator(self.widget_dict["T"].value(), rho=self.widget_dict["rho"].value())
         a = np.sqrt(gam * R * self.widget_dict["T"].value())
         V = self.widget_dict["MACHIN"].value() * a
         self.widget_dict['REYNIN'].setValue(V * self.widget_dict["L"].value() / nu)
 
-    def setWidgetValuesFromDict(self, d: dict):
+    def setValue(self, d: dict):
         for d_name, d_value in d.items():
             try:
                 self.widget_dict[d_name].setValue(d_value)
             except KeyError:
                 pass
 
-    def valuesFromWidgets(self) -> dict:
+    def value(self) -> dict:
         return {k: v.value() for k, v in self.widget_dict.items()}
 
 
 class MPLOTDialogWidget(PymeadDialogWidget):
     def __init__(self):
         super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, "mplot_settings.json"))
 
@@ -1818,18 +1842,23 @@
 
     OptConstraintsChanged = pyqtSignal()
 
     def __init__(self, parent, geo_col: GeometryCollection, mset_dialog_widget: MSETDialogWidget = None):
         super().__init__(parent=parent,
                          widgets={k: OptConstraintsDialogWidget() for k in geo_col.container()["airfoils"]})
         # mset_dialog_widget.airfoilsChanged.connect(self.onAirfoilListChanged)
+        self.label = QLabel("Optimization Constraints")
+        self.widget = self
+        self.push = None
 
     def reorderRegenerateWidgets(self, new_airfoil_name_list: list):
         temp_dict = {}
         for airfoil_name in new_airfoil_name_list:
+            if airfoil_name not in self.w_dict:
+                self.w_dict[airfoil_name] = OptConstraintsDialogWidget()
             temp_dict[airfoil_name] = self.w_dict[airfoil_name]
         self.w_dict = temp_dict
         self.regenerateWidgets()
 
     # def onAirfoilAdded(self, new_airfoil_name_list: list):
     #     for airfoil_name in new_airfoil_name_list:
     #         if airfoil_name not in self.w_dict.keys():
@@ -1852,28 +1881,30 @@
     #     elif len(new_airfoil_name_list) < len([k for k in self.w_dict.keys()]):
     #         self.onAirfoilRemoved(new_airfoil_name_list)
     #     else:
     #         self.reorderRegenerateWidgets(new_airfoil_name_list=new_airfoil_name_list)
 
     def setValues(self, values: dict):
         # self.onAirfoilListChanged(new_airfoil_name_list_str=','.join([k for k in values.keys()]))
-        self.setWidgetValuesFromDict(new_values=values)
+        self.setValue(new_values=values)
 
     def values(self):
-        return self.valuesFromWidgets()
+        return self.value()
 
     def valueChanged(self, k1, k2, v2):
         self.OptConstraintsChanged.emit()
 
 
 class XFOILDialogWidget(PymeadDialogWidget):
-    def __init__(self, current_airfoils: typing.List[str]):
+    def __init__(self, current_airfoils: typing.List[str], settings_override: dict = None):
         super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'xfoil_settings.json'))
         self.widget_dict['airfoil_analysis_dir']['widget'].setText(tempfile.gettempdir())
         self.widget_dict["airfoil"]["widget"].addItems(current_airfoils)
+        if settings_override:
+            self.setValue(new_values=settings_override)
 
     def calculate_and_set_Reynolds_number(self, new_inputs: dict):
         Re_widget = self.widget_dict['Re']['widget']
         nu = viscosity_calculator(new_inputs['T'], rho=new_inputs['rho'])
         a = np.sqrt(new_inputs['gam'] * new_inputs['R'] * new_inputs['T'])
         V = new_inputs['Ma'] * a
         Re_widget.setValue(V * new_inputs['L'] / nu)
@@ -1941,44 +1972,94 @@
         if w_name in ['P', 'T', 'rho', 'R', 'gam', 'L', 'Ma'] and not self.widget_dict[w_name]['widget'].isReadOnly():
             if self.widget_dict['P']['widget'].isReadOnly():
                 self.widget_dict['P']['widget'].setValue(new_inputs['rho'] * new_inputs['R'] * new_inputs['T'])
             elif self.widget_dict['T']['widget'].isReadOnly():
                 self.widget_dict['T']['widget'].setValue(new_inputs['P'] / new_inputs['R'] / new_inputs['rho'])
             elif self.widget_dict['rho']['widget'].isReadOnly():
                 self.widget_dict['rho']['widget'].setValue(new_inputs['P'] / new_inputs['R'] / new_inputs['T'])
-            new_inputs = self.valuesFromWidgets()
+            new_inputs = self.value()
             if not (w_name == 'Ma' and new_inputs['spec_Re']):
                 self.calculate_and_set_Reynolds_number(new_inputs)
 
     def select_directory(self, line_edit: QLineEdit):
         select_directory(parent=self.parent(), line_edit=line_edit, starting_dir=tempfile.gettempdir())
 
 
-class GAGeneralSettingsDialogWidget(PymeadDialogWidget):
-    def __init__(self):
-        super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'ga_general_settings.json'))
+class GAGeneralSettingsDialogWidget(PymeadDialogWidget2):
+
+    sigMEAFileChanged = pyqtSignal(list, list, object, object)
+
+    def __init__(self, parent=None):
         self.current_save_file = None
+        super().__init__(parent=parent)
+
+    def initializeWidgets(self, *args, **kwargs):
+        self.widget_dict = {
+            "save": PymeadLabeledPushButton(label="Save", text="Save Settings"),
+            "save_as": PymeadLabeledPushButton(label="Save As", text="Save Settings As..."),
+            "load": PymeadLabeledPushButton(label="Load", text="Load Settings File"),
+            "warm_start_active": PymeadLabeledCheckbox(label="Warm Start Active?", initial_state=0),
+            "warm_start_generation": PymeadLabeledSpinBox(label="Warm Start Generation", value=-1, minimum=-2147483647,
+                                                          maximum=2147483647, read_only=True),
+            "warm_start_dir": PymeadLabeledLineEdit(label="Warm Start Directory", push_label="Choose folder",
+                                                    read_only=True,
+                                                    tool_tip="Choose '-1' to start from the most recent generation"),
+            "use_initial_settings": PymeadLabeledCheckbox(label="Use Initial Settings?", initial_state=2),
+            "mea_file": PymeadLabeledLineEdit(label="MEA File", push_label="Choose file", read_only=True),
+            "batch_mode_active": PymeadLabeledCheckbox(
+                label="Batch Mode Active?", initial_state=0,
+                tool_tip="If this box is checked, all settings in this dialog will be\noverridden by the settings "
+                         "in the selected JSON settings files."),
+            "batch_mode_files": PymeadLabeledPlainTextEdit(label="Batch Settings Files", push_label="Choose files",
+                                                           read_only=True)
+        }
+
+    def establishWidgetConnections(self):
+        self.widget_dict["save"].widget.clicked.connect(self.save_opt_settings)
+        self.widget_dict["save_as"].widget.clicked.connect(self.saveas_opt_settings)
+        self.widget_dict["load"].widget.clicked.connect(self.load_opt_settings)
+        self.widget_dict["warm_start_active"].sigValueChanged.connect(self.warm_start_active_state_changed)
+        self.widget_dict["warm_start_dir"].push.clicked.connect(partial(self.select_directory,
+                                                                        self.widget_dict["warm_start_dir"].widget))
+        self.widget_dict["mea_file"].push.clicked.connect(partial(self.select_existing_jmea_file,
+                                                                  self.widget_dict["mea_file"].widget))
+        self.widget_dict["batch_mode_active"].sigValueChanged.connect(self.batch_mode_active_state_changed)
+        self.widget_dict["batch_mode_files"].push.clicked.connect(partial(self.select_multiple_json_files,
+                                                                          self.widget_dict["batch_mode_files"].widget))
+
+    def warm_start_active_state_changed(self, state: int):
+        self.widget_dict["warm_start_generation"].widget.setReadOnly(not bool(state))
+        self.widget_dict["warm_start_dir"].widget.setReadOnly(not bool(state))
+
+    def batch_mode_active_state_changed(self, state: int):
+        self.widget_dict["batch_mode_files"].widget.setReadOnly(not bool(state))
 
     def select_directory(self, line_edit: QLineEdit):
         select_directory(parent=self.parent(), line_edit=line_edit)
 
     def select_existing_jmea_file(self, line_edit: QLineEdit):
-        select_existing_jmea_file(parent=self.parent(), line_edit=line_edit)
+        jmea_file = select_existing_jmea_file(parent=self.parent(), line_edit=line_edit)
+        if jmea_file is not None:
+            gui_obj = get_parent(self, 4)
+            gui_obj.load_geo_col(file_name=jmea_file)
+            self.sigMEAFileChanged.emit([airfoil for airfoil in gui_obj.geo_col.container()["airfoils"].values()],
+                                        [mea for mea in gui_obj.geo_col.container()["mea"].values()],
+                                        None, None)
 
     def select_multiple_json_files(self, text_edit: QPlainTextEdit):
         select_multiple_json_files(parent=self.parent(), text_edit=text_edit)
 
     def save_opt_settings(self):
         opt_file = None
         if self.current_save_file is not None:
             opt_file = self.current_save_file
         if get_parent(self, 4) and get_parent(self, 4).current_settings_save_file is not None:
             opt_file = get_parent(self, 4).current_settings_save_file
         if opt_file is not None:
-            new_inputs = get_parent(self, 2).valuesFromWidgets()  # Gets the inputs from the PymeadDialogVTabWidget
+            new_inputs = get_parent(self, 2).value()  # Gets the inputs from the PymeadDialogVTabWidget
             save_data(new_inputs, opt_file)
             get_parent(self, 2).setStatusTip(f"Settings saved ({opt_file})")
             # msg_box = PymeadMessageBox(parent=self, msg=f"Settings saved as {self.current_save_file}",
             #                            window_title='Save Notification', msg_mode='info')
             # msg_box.exec()
         else:
             self.saveas_opt_settings()
@@ -1990,20 +2071,32 @@
             q_settings.setValue("ga-settings-dir", os.path.split(load_file)[0])
             new_inputs = load_data(load_file)
             great_great_grandparent = get_parent(self, depth=4)
             if great_great_grandparent:
                 great_great_grandparent.current_settings_save_file = load_file
             else:
                 self.current_save_file = load_file
+
+            gui_obj = get_parent(self, 4)
+            gui_obj.load_geo_col(file_name=new_inputs["General Settings"]["mea_file"])
+
+            # Pass the new GeometryCollection reference to the actuator disk
+            get_parent(self, 3).mses_widget.widget_dict["AD"].geo_col = deepcopy(gui_obj.geo_col)
+
+            self.sigMEAFileChanged.emit([airfoil for airfoil in gui_obj.geo_col.container()["airfoils"].values()],
+                                        [mea for mea in gui_obj.geo_col.container()["mea"].values()],
+                                        new_inputs["XFOIL"]["airfoil"],
+                                        new_inputs["MSET"]["mea"])
+
             get_parent(self, 3).setWindowTitle(f"Optimization Setup - {os.path.split(load_file)[-1]}")
-            get_parent(self, 2).setWidgetValuesFromDict(new_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
+            get_parent(self, 2).setValue(new_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
             get_parent(self, 2).setStatusTip(f"Loaded {load_file}")
 
     def saveas_opt_settings(self):
-        inputs_to_save = get_parent(self, 2).valuesFromWidgets()
+        inputs_to_save = get_parent(self, 2).value()
         json_dialog = select_json_file(parent=self)
         if json_dialog.exec_():
             input_filename = json_dialog.selectedFiles()[0]
             if not os.path.splitext(input_filename)[-1] == '.json':
                 input_filename = input_filename + '.json'
             save_data(inputs_to_save, input_filename)
             if get_parent(self, 4):
@@ -2025,14 +2118,36 @@
     def select_data_file(self, line_edit: QLineEdit):
         select_data_file(parent=self.parent(), line_edit=line_edit)
 
     def updateDialog(self, new_inputs: dict, w_name: str):
         pass
 
 
+class GAConstraintsTerminationDialogWidget2(PymeadDialogWidget2):
+    def __init__(self, geo_col: GeometryCollection, parent=None):
+        self.geo_col = geo_col
+        super().__init__(parent=parent)
+
+    def initializeWidgets(self, *args, **kwargs):
+        self.widget_dict = {
+            "constraints": OptConstraintsHTabWidget(parent=None, geo_col=self.geo_col),
+            "f_tol": PymeadLabeledScientificDoubleSpinBox(label="Function Tolerance", value=0.0025, minimum=0.0,
+                                                          maximum=100000.0),
+            "cv_tol": PymeadLabeledScientificDoubleSpinBox(label="Constraint Violation Tol.", value=1.0e-6,
+                                                           minimum=0.0, maximum=100000.0),
+            "x_tol": PymeadLabeledScientificDoubleSpinBox(label="Parameter Tolerance", value=1.0e-8,
+                                                          minimum=0.0, maximum=100000.0),
+            "nth_gen": PymeadLabeledSpinBox(label="Termination Calc. Frequency", value=10, minimum=1, maximum=100000),
+            "n_last": PymeadLabeledSpinBox(label="Num. Prev. Gens. to Check", value=30, minimum=1, maximum=100000),
+            "n_max_gen": PymeadLabeledSpinBox(label="Maximum Generations", value=500, minimum=1, maximum=100000),
+            "n_max_evals": PymeadLabeledSpinBox(label="Maximum Function Calls", value=100000, minimum=1,
+                                                maximum=10000000)
+        }
+
+
 class GASaveLoadDialogWidget(PymeadDialogWidget):
     def __init__(self):
         super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'ga_save_load_settings.json'))
         self.current_save_file = None
 
     def select_json_file(self, line_edit: QLineEdit):
         select_json_file(parent=self.parent(), line_edit=line_edit)
@@ -2041,29 +2156,29 @@
         select_existing_json_file(parent=self.parent(), line_edit=line_edit)
 
     def select_directory(self, line_edit: QLineEdit):
         select_directory(parent=self.parent(), line_edit=line_edit)
 
     def save_opt_settings(self):
         if self.current_save_file is not None:
-            new_inputs = self.parent().valuesFromWidgets()  # Gets the inputs from the PymeadDialogVTabWidget
+            new_inputs = self.parent().value()  # Gets the inputs from the PymeadDialogVTabWidget
             save_data(new_inputs, self.current_save_file)
             msg_box = PymeadMessageBox(parent=self, msg=f"Settings saved as {self.current_save_file}",
                                        window_title='Save Notification', msg_mode='info')
             msg_box.exec()
         else:
             self.saveas_opt_settings()
 
     def load_opt_settings(self):
         new_inputs = load_data(self.widget_dict['settings_load_dir']['widget'].text())
         self.current_save_file = new_inputs['Save/Load']['settings_save_dir']
-        self.parent().setWidgetValuesFromDict(new_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
+        self.parent().setValue(new_inputs)  # Overrides the inputs for the whole PymeadDialogVTabWidget
 
     def saveas_opt_settings(self):
-        inputs_to_save = self.parent().valuesFromWidgets()
+        inputs_to_save = self.parent().value()
         input_filename = os.path.join(self.widget_dict['settings_saveas_dir']['widget'].text(),
                                       self.widget_dict['settings_saveas_filename']['widget'].text())
         save_data(inputs_to_save, input_filename)
         self.current_save_file = input_filename
         msg_box = PymeadMessageBox(parent=self, msg=f"Settings saved as {input_filename}",
                                    window_title='Save Notification', msg_mode='info')
         msg_box.exec()
@@ -2089,41 +2204,35 @@
         super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'genetic_algorithm_settings.json'))
         self.widget_dict['J']['widget'].textChanged.connect(partial(self.objectives_changed,
                                                                     self.widget_dict['J']['widget']))
         self.widget_dict['G']['widget'].textChanged.connect(partial(self.constraints_changed,
                                                                     self.widget_dict['G']['widget']))
         multi_point_active_widget = multi_point_dialog_widget.widget_dict['multi_point_active']['widget']
         self.multi_point = multi_point_active_widget.checkState()
-        tool = self.valuesFromWidgets()['tool']
+        tool = self.value()['tool']
         self.cfd_template = tool
         if self.multi_point:
             self.cfd_template += '_MULTIPOINT'
         multi_point_active_widget.stateChanged.connect(self.multi_point_changed)
 
-    def setWidgetValuesFromDict(self, new_values: dict):
-        super().setWidgetValuesFromDict(new_values)
+    def setValue(self, new_values: dict):
+        super().setValue(new_values)
         self.update_objectives_and_constraints()
 
     def update_objectives_and_constraints(self):
-        inputs = self.valuesFromWidgets()
+        inputs = self.value()
         self.objectives_changed(self.widget_dict['J']['widget'], inputs['J'])
         self.constraints_changed(self.widget_dict['G']['widget'], inputs['G'])
 
     def visualize_sampling(self, ws_widget, _):
-        general_settings = self.parent().findChild(GAGeneralSettingsDialogWidget).valuesFromWidgets()
         starting_value = ws_widget.value()
-        use_current_mea = bool(general_settings["use_current_mea"])
-        jmea_file = general_settings["mea_file"]
         gui_obj = get_parent(self, depth=4)
         background_color = gui_obj.themes[gui_obj.current_theme]["graph-background-color"]
         theme = gui_obj.themes[gui_obj.current_theme]
-        if use_current_mea or len(jmea_file) == 0 or not os.path.exists(jmea_file):
-            geo_col_dict = gui_obj.geo_col.get_dict_rep()
-        else:
-            geo_col_dict = load_data(jmea_file)
+        geo_col_dict = gui_obj.geo_col.get_dict_rep()
 
         dialog = SamplingVisualizationDialog(geo_col_dict=geo_col_dict, initial_sampling_width=starting_value,
                                              initial_n_samples=20, background_color=background_color, theme=theme,
                                              parent=self)
         dialog.exec_()
 
     def select_directory(self, line_edit: QLineEdit):
@@ -2137,15 +2246,15 @@
         self.objectives_changed(self.widget_dict['J']['widget'], self.widget_dict['J']['widget'].text())
         self.constraints_changed(self.widget_dict['G']['widget'], self.widget_dict['G']['widget'].text())
 
     def objectives_changed(self, widget, text: str):
         objective_container = get_parent(self, depth=4)
         if objective_container is None:
             objective_container = get_parent(self, depth=1)
-        inputs = self.valuesFromWidgets()
+        inputs = self.value()
         tool = inputs['tool']
         if self.multi_point:
             tool += '_MULTIPOINT'
         objective_container.objectives = []
         for obj_func_str in text.split(','):
             objective = Objective(obj_func_str)
             objective_container.objectives.append(objective)
@@ -2161,15 +2270,15 @@
                 widget.setStyleSheet("QLineEdit {background-color: rgba(176,25,25,50)}")
                 return
 
     def constraints_changed(self, widget, text: str):
         constraint_container = get_parent(self, depth=4)
         if constraint_container is None:
             constraint_container = get_parent(self, depth=1)
-        inputs = self.valuesFromWidgets()
+        inputs = self.value()
         tool = inputs['tool']
         if self.multi_point:
             tool += '_MULTIPOINT'
         constraint_container.constraints = []
         for constraint_func_str in text.split(','):
             if len(constraint_func_str) > 0:
                 constraint = Constraint(constraint_func_str)
@@ -2192,18 +2301,24 @@
             if len(text_split) > 1:
                 k = text_split[0]
                 v = float(text_split[1])
                 data_dict[k] = v
         return data_dict
 
 
+class PanelDialog(PymeadDialog):
+    def __init__(self, parent: QWidget, theme: dict, settings_override: dict = None):
+        self.w = PanelDialogWidget(settings_override)
+        super().__init__(parent=parent, window_title="Basic Panel Code Analysis", widget=self.w, theme=theme)
+
+
 class XFOILDialog(PymeadDialog):
     def __init__(self, parent: QWidget, current_airfoils: typing.List[str], theme: dict,
                  settings_override: dict = None):
-        self.w = XFOILDialogWidget(current_airfoils=current_airfoils)
+        self.w = XFOILDialogWidget(current_airfoils=current_airfoils, settings_override=settings_override)
         super().__init__(parent=parent, window_title="Single Airfoil Viscous Analysis", widget=self.w,
                          theme=theme)
 
 
 class MultiAirfoilDialog(PymeadDialog):
     def __init__(self, parent: QWidget, geo_col: GeometryCollection, theme: dict, settings_override: dict = None):
         mset_dialog_widget = MSETDialogWidget2(geo_col=geo_col, theme=theme)
@@ -2211,46 +2326,33 @@
         mset_dialog_widget.sigMEAChanged.connect(mses_dialog_widget.widget_dict["xtrs"].onMEAChanged)
         mplot_dialog_widget = MPLOTDialogWidget()
         tab_widgets = {"MSET": mset_dialog_widget, "MSES": mses_dialog_widget, "MPLOT": mplot_dialog_widget}
         widget = PymeadDialogVTabWidget(parent=None, widgets=tab_widgets, settings_override=settings_override)
         super().__init__(parent=parent, window_title="Multi-Element-Airfoil Analysis", widget=widget, theme=theme)
 
 
-class SettingsDialog(QDialog):
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-        buttonBox = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, self)
-        layout = QFormLayout(self)
-
-        self.tab_widget = QTabWidget()
-        layout.addWidget(self.tab_widget)
-
-        layout.addWidget(buttonBox)
-
-        buttonBox.accepted.connect(self.accept)
-        buttonBox.rejected.connect(self.reject)
-
-
 class InviscidCpCalcDialog(QDialog):
     def __init__(self, parent=None):
         super().__init__(parent)
         layout = QFormLayout(self)
 
 
 class ScreenshotDialog(PymeadDialog):
-    def __init__(self, parent: QWidget, theme: dict):
+    def __init__(self, parent: QWidget, theme: dict, windows: typing.List[str]):
 
         widget = QWidget()
         super().__init__(parent=parent, window_title="Screenshot", widget=widget, theme=theme)
         self.grid_widget = {}
         self.grid_layout = QGridLayout()
 
         self.setInputs()
+        self.grid_widget["window"]["combobox"].addItems(windows)
         widget.setLayout(self.grid_layout)
+        self.window_list = windows
+        self.setMinimumWidth(400)
 
     def setInputs(self):
         widget_dict = load_data(os.path.join(GUI_DIALOG_WIDGETS_DIR, "screenshot_dialog.json"))
         for row_name, row_dict in widget_dict.items():
             self.grid_widget[row_name] = {}
             for w_name, w_dict in row_dict.items():
                 widget = getattr(sys.modules[__name__], w_dict["w"])(self)
@@ -2267,21 +2369,27 @@
                     widget.setToolTip(w_dict["tool_tip"])
                 for attr_name, attr_value in w_dict.items():
                     if attr_name not in ["text", "func", "tool_tip", "grid", "w"]:
                         getattr(widget, attr_name)(attr_value)
                 self.grid_layout.addWidget(widget, w_dict["grid"][0], w_dict["grid"][1], w_dict["grid"][2],
                                            w_dict["grid"][3])
 
-    def valuesFromWidgets(self):
+    def value(self):
         inputs = {
             "image_file": self.grid_widget["choose_image_file"]["line"].text(),
             "window": self.grid_widget["window"]["combobox"].currentText()
         }
         return inputs
 
+    def setValue(self, new_inputs):
+        if new_inputs["window"] in self.window_list:
+            combo = self.grid_widget["window"]["combobox"]
+            combo.setCurrentIndex(combo.findText(new_inputs["window"]))
+        self.grid_widget["choose_image_file"]["line"].setText(new_inputs["image_file"])
+
     def select_jpg_file(self, line_edit: QLineEdit):
         select_jpg_file(parent=self.parent(), line_edit=line_edit)
 
 
 class BoundsDialog(QDialog):
     def __init__(self, bounds, parent=None, pos_param: bool = False):
         super().__init__(parent)
@@ -2587,32 +2695,75 @@
 
 
 class OptimizationSetupDialog(PymeadDialog):
     def __init__(self, parent, geo_col: GeometryCollection, theme: dict, settings_override: dict = None):
         w0 = GAGeneralSettingsDialogWidget()
         w3 = XFOILDialogWidget(current_airfoils=[k for k in geo_col.container()["airfoils"]])
         w4 = MSETDialogWidget2(geo_col=geo_col, theme=theme)
-        w2 = GAConstraintsTerminationDialogWidget(geo_col=geo_col, mset_dialog_widget=w4)
+        w2 = GAConstraintsTerminationDialogWidget2(geo_col=geo_col)
         w7 = MultiPointOptDialogWidget()
         w5 = MSESDialogWidget2(geo_col=geo_col)
-        # w4.sigMEAChanged.connect(w5.widget_dict["xtrs"].widget.onMEAChanged)
         w1 = GeneticAlgorithmDialogWidget(multi_point_dialog_widget=w7)
         w6 = PymeadDialogWidget(os.path.join(GUI_DEFAULTS_DIR, 'mplot_settings.json'))
         w = OptimizationDialogVTabWidget(parent=self, widgets={'General Settings': w0,
                                                         'Genetic Algorithm': w1,
                                                         'Constraints/Termination': w2,
                                                                'Multi-Point Optimization': w7,
                                                         'XFOIL': w3, 'MSET': w4, 'MSES': w5, 'MPLOT': w6},
                                          settings_override=settings_override)
         super().__init__(parent=parent, window_title='Optimization Setup', widget=w, theme=theme)
         w.objectives = self.parent().objectives
         w.constraints = self.parent().constraints
 
         w1.update_objectives_and_constraints()  # IMPORTANT: makes sure that the objectives/constraints get stored
 
+        self.geo_col = geo_col
+        self.mset_widget = w4
+        self.xfoil_widget = w3
+        self.mses_widget = w5
+        self.constraints_widget = w2
+        self.mset_widget.sigMEAChanged.connect(self.mses_widget.widget_dict["xtrs"].onMEAChanged)
+        w0.sigMEAFileChanged.connect(self.onMEAFileChanged)
+
+    def onMEAFileChanged(self, airfoil_objs: typing.List[Airfoil], mea_objs: typing.List[MEA],
+                         current_airfoil: str or None, current_mea: str or None):
+        self.geo_col = get_parent(self, 1).geo_col
+        self.mset_widget.geo_col = self.geo_col
+        self.mses_widget.geo_col = self.geo_col
+        self.constraints_widget.geo_col = self.geo_col
+        self.xfoil_widget.widget_dict["airfoil"]["widget"].clear()
+        self.mset_widget.widget_dict["mea"].widget.clear()
+
+        # Add the new list of parameters to the actuator disk MSES widget
+        param_list = [param for param in self.geo_col.container()["params"]]
+        dv_list = [dv + " (DV)" for dv in self.geo_col.container()["desvar"]]
+        AD_widget = self.mses_widget.widget_dict["AD"]
+        AD_widget.param_list = [""] + param_list + dv_list
+        for ad in AD_widget.widget_dict.values():
+            ad["XCDELH-Param"].widget.clear()
+            ad["XCDELH-Param"].widget.addItems(AD_widget.param_list)
+
+        airfoil_names = [airfoil.name() for airfoil in airfoil_objs]
+        mea_names = [mea.name() for mea in mea_objs]
+        self.xfoil_widget.widget_dict["airfoil"]["widget"].addItems(airfoil_names)
+        self.mset_widget.widget_dict["mea"].widget.addItems(mea_names)
+        self.constraints_widget.widget_dict["constraints"].reorderRegenerateWidgets(airfoil_names)
+
+        if current_airfoil is not None:
+            self.xfoil_widget.widget_dict["airfoil"]["widget"].setCurrentText(current_airfoil)
+        else:
+            if len(airfoil_names) > 0:
+                self.xfoil_widget.widget_dict["airfoil"]["widget"].setCurrentText(airfoil_names[0])
+
+        if current_mea is not None:
+            self.mset_widget.widget_dict["mea"].widget.setCurrentText(current_mea)
+        else:
+            if len(mea_names) > 0:
+                self.mset_widget.widget_dict["mea"].widget.setCurrentText(mea_names[0])
+
 
 class ExportCoordinatesDialog(PymeadDialog):
     def __init__(self, parent, theme: dict):
         w = QWidget()
         self.grid_widget = {}
         self.grid_layout = QGridLayout()
         self.setInputs()
@@ -2646,15 +2797,15 @@
                 if "upper_bound" in w_dict.keys() and (isinstance(widget, QSpinBox) or isinstance(widget, QDoubleSpinBox)):
                     widget.setMaximum(w_dict["upper_bound"])
                 if "value" in w_dict.keys() and (isinstance(widget, QSpinBox) or isinstance(widget, QDoubleSpinBox)):
                     widget.setValue(w_dict["value"])
                 self.grid_layout.addWidget(widget, w_dict["grid"][0], w_dict["grid"][1], w_dict["grid"][2],
                                            w_dict["grid"][3])
 
-    def valuesFromWidgets(self):
+    def value(self):
         inputs = {}
         for k, v in self.grid_widget.items():
             if "line" in v.keys():
                 inputs[k] = v["line"].text()
             elif "spinbox" in v.keys():
                 inputs[k] = v["spinbox"].value()
             elif "checkbox" in v.keys():
@@ -2710,15 +2861,15 @@
                     else:
                         widget.clicked.connect(getattr(self, w_dict["func"]))
                 if "tool_tip" in w_dict.keys():
                     widget.setToolTip(w_dict["tool_tip"])
                 self.grid_layout.addWidget(widget, w_dict["grid"][0], w_dict["grid"][1], w_dict["grid"][2],
                                            w_dict["grid"][3])
 
-    def valuesFromWidgets(self):
+    def value(self):
         inputs = {k: v["line"].text() if "line" in v.keys() else None for k, v in self.grid_widget.items()}
 
         # Make sure any newline characters are not double-escaped:
         for k, input_ in inputs.items():
             if isinstance(input_, str):
                 inputs[k] = input_.replace('\\n', '\n')
 
@@ -2765,15 +2916,15 @@
                         getattr(widget, attr_name)(attr_value)
                 if isinstance(widget, QDoubleSpinBox):
                     widget.setMinimum(-np.inf)
                     widget.setMaximum(np.inf)
                 self.grid_layout.addWidget(widget, w_dict["grid"][0], w_dict["grid"][1], w_dict["grid"][2],
                                            w_dict["grid"][3])
 
-    def valuesFromWidgets(self):
+    def value(self):
         inputs = {
             "dir": self.grid_widget["choose_dir"]["line"].text(),
             "file_name": self.grid_widget["file_name"]["line"].text(),
             "rotation": [self.grid_widget["rotation"][xyz].value() for xyz in ["x", "y", "z"]],
             "scaling": [self.grid_widget["scaling"][xyz].value() for xyz in ["x", "y", "z"]],
             "translation": [self.grid_widget["translation"][xyz].value() for xyz in ["x", "y", "z"]],
             "transformation_order": self.grid_widget["transform_order"]["line"].text()
@@ -2813,15 +2964,15 @@
     def setInputs(self):
         r0 = ["Tool Airfoil", QComboBox(self)]
         r0[1].addItems(self.airfoil_names)
         r1 = ["Target Airfoil", QLineEdit(self)]
         r1[1].setText('n0012-il')
         return [r0, r1]
 
-    def valuesFromWidgets(self):
+    def value(self):
         return {"tool_airfoil": self.inputs[0][1].currentText(), "target_airfoil": self.inputs[1][1].text()}
 
 
 class AirfoilPlotDialog(PymeadDialog):
     def __init__(self, parent, theme: dict):
         widget = QWidget()
         super().__init__(parent, window_title="Select Airfoil to Plot", widget=widget, theme=theme)
@@ -2835,38 +2986,98 @@
         self.setMinimumWidth(300)
 
     def setInputs(self):
         r0 = ["Airfoil to Plot", QLineEdit(self)]
         r0[1].setText('n0012-il')
         return [r0]
 
-    def valuesFromWidgets(self):
+    def value(self):
         return self.inputs[0][1].text()
 
 
+class LoadPointsDialog(PymeadDialog):
+    def __init__(self, parent, theme: dict):
+        self.grid_widget = QWidget()
+        super().__init__(parent, window_title="Load Points", widget=self.grid_widget, theme=theme)
+        self.lay = QGridLayout()
+        explanation = QPlainTextEdit("Load points from a .txt/.dat/.csv file in space- or comma-delimited format "
+                                     "with two columns: x and y")
+        explanation.setReadOnly(True)
+        self.lay.addWidget(explanation, 0, 0, 1, 3)
+        self.file_name_widget = QLineEdit()
+        self.lay.addWidget(QLabel("Data File"), 1, 0, 1, 1)
+        self.lay.addWidget(self.file_name_widget, 1, 1, 1, 1)
+        push = QPushButton("Choose File")
+        push.clicked.connect(self.select_data_file)
+        self.lay.addWidget(push, 1, 2, 1, 1)
+        self.grid_widget.setLayout(self.lay)
+        self.setMinimumWidth(450)
+
+    def select_data_file(self):
+        select_data_file(self, self.file_name_widget, starting_dir=get_setting("load_points_default_open_location"))
+        file_name = self.file_name_widget.text()
+        if file_name:
+            set_setting("load_points_default_open_location", file_name)
+
+    def value(self):
+        file_name = self.file_name_widget.text()
+        return file_name
+
+
 class WebAirfoilDialog(PymeadDialog):
     def __init__(self, parent, theme: dict):
         widget = QWidget()
-        super().__init__(parent, window_title="Select AirfoilTools airfoil", widget=widget, theme=theme)
-        self.lay = QFormLayout()
+        super().__init__(parent, window_title="Load Airfoil from Coordinates", widget=widget, theme=theme)
+        self.lay = QGridLayout()
         widget.setLayout(self.lay)
-        self.inputs = self.setInputs()
+        self.setInputs()
 
         for i in self.inputs:
-            self.lay.addRow(i[0], i[1])
+            row_count = self.lay.rowCount()
+            self.lay.addWidget(i.label, row_count, 0)
+            if i.push is None:
+                self.lay.addWidget(i.widget, row_count, 1, 1, 2)
+            else:
+                self.lay.addWidget(i.widget, row_count, 1, 1, 1)
+                self.lay.addWidget(i.push, row_count, 2, 1, 1)
 
         self.setMinimumWidth(300)
 
     def setInputs(self):
-        r0 = ["Web airfoil", QLineEdit(self)]
-        r0[1].setText("n0012-il")
-        return [r0]
+        self.inputs = [
+            PymeadLabeledComboBox(label="Airfoil type", tool_tip="Choose whether to use an AirfoilTools airfoil or a "
+                                                                 "coordinate-file airfoil",
+                                  items=["AirfoilTools", "Coordinate File"]),
+            PymeadLabeledLineEdit(label="Web Airfoil", tool_tip="URL-name of the AirfoilTools airfoil (name in the "
+                                                                "parentheses on airfoiltools.com)", text="n0012-il"),
+            PymeadLabeledLineEdit(label="Airfoil from File", tool_tip="Absolute file path of a Selig-format "
+                                                                      "(counter-clockwise starting with upper trailing "
+                                                                      "edge, space-delimited, airfoil coordinates file",
+                                  text="", push_label="Select Airfoil", read_only=True)
+        ]
+        self.inputs[0].sigValueChanged.connect(self.airfoilTypeChanged)
+        self.inputs[2].push.clicked.connect(self.selectDatFile)
+        return self.inputs
 
-    def valuesFromWidgets(self):
-        return self.inputs[0][1].text()
+    def airfoilTypeChanged(self, airfoil_type: str):
+        if airfoil_type == "AirfoilTools":
+            self.inputs[1].setReadOnly(False)
+            self.inputs[2].setReadOnly(True)
+        else:
+            self.inputs[1].setReadOnly(True)
+            self.inputs[2].setReadOnly(False)
+
+    def selectDatFile(self):
+        select_data_file(parent=self, line_edit=self.inputs[2].widget)
+
+    def value(self):
+        if self.inputs[0].value() == "AirfoilTools":
+            return self.inputs[1].value()
+        else:
+            return self.inputs[2].value()
 
 
 class MSESFieldPlotDialogWidget(PymeadDialogWidget):
     def __init__(self, default_field_dir: str = None):
         super().__init__(settings_file=os.path.join(GUI_DEFAULTS_DIR, 'mses_field_plot_settings.json'))
         if default_field_dir is not None:
             self.widget_dict['analysis_dir']['widget'].setText(default_field_dir)
@@ -2939,22 +3150,18 @@
 
     def valueChanged(self, _):
         self.boundsChanged.emit()
 
 
 class PlotExportDialogWidget(PymeadDialogWidget2):
     def __init__(self, gui_obj, current_min_level: float, current_max_level: float, parent=None):
-        super().__init__(parent=parent)
-        self.widget_dict = None
-        self.lay = QGridLayout()
-        self.setLayout(self.lay)
         self.gui_obj = gui_obj
         self.current_min_level = current_min_level
         self.current_max_level = current_max_level
-        self.initializeWidgets()
+        super().__init__(parent=parent)
 
     def initializeWidgets(self):
         available_fonts = ["DejaVu Sans Mono", "DejaVu Serif", "DejaVu Sans"]
         self.widget_dict = {
             "save_name": PymeadLabeledLineEdit(label="File Name", text="airfoil.png",
                                                tool_tip="Name of the image. If the '.png' extension is not included,"
                                                         " it will be appended automatically"),
@@ -2978,72 +3185,74 @@
             self.widget_dict["min_level"] = PymeadLabeledDoubleSpinBox(
                 label="Minimum Contour Level", minimum=-10000, maximum=10000, value=self.current_min_level,
                 decimals=4, single_step=0.1)
             self.widget_dict["max_level"] = PymeadLabeledDoubleSpinBox(
                 label="Maximum Contour Level", minimum=-10000, maximum=10000, value=self.current_max_level,
                 decimals=4, single_step=0.1)
 
+    def addWidgets(self, *args, **kwargs):
         # Add all the widgets
         for widget_name, widget in self.widget_dict.items():
             row_count = self.lay.rowCount()
             self.lay.addWidget(widget.label, row_count, 0)
             self.lay.addWidget(widget.widget, row_count, 1)
             if widget.push is not None:
                 self.lay.addWidget(widget.push, row_count, 2)
 
+    def establishWidgetConnections(self):
         self.widget_dict["save_dir"].push.clicked.connect(
             partial(select_directory, self, line_edit=self.widget_dict["save_dir"].widget))
 
         self.widget_dict["tick_font_family"].sigValueChanged.connect(self.tickFontChanged)
         self.widget_dict["tick_font_size"].sigValueChanged.connect(self.tickFontChanged)
         self.widget_dict["label_font_family"].sigValueChanged.connect(self.labelFontChanged)
         self.widget_dict["label_font_size"].sigValueChanged.connect(self.labelFontChanged)
         self.widget_dict["save_dir"].sigValueChanged.connect(partial(set_setting, "plot-field-export-dir"))
         if "min_level" in self.widget_dict and "max_level" in self.widget_dict:
             self.widget_dict["min_level"].sigValueChanged.connect(self.minLevelChanged)
             self.widget_dict["max_level"].sigValueChanged.connect(self.maxLevelChanged)
 
     def tickFontChanged(self, _):
-        widget_values = self.valuesFromWidgets()
+        widget_values = self.value()
         tick_font = QFont(widget_values["tick_font_family"], widget_values["tick_font_size"])
         set_setting("cbar-tick-font-family", widget_values["tick_font_family"])
         set_setting("cbar-tick-point-size", widget_values["tick_font_size"])
         set_setting("axis-tick-font-family", widget_values["tick_font_family"])
         set_setting("axis-tick-point-size", widget_values["tick_font_size"])
         if self.gui_obj.cbar is not None:
             self.gui_obj.cbar.axis.setStyle(tickFont=tick_font)
             self.gui_obj.cbar.getAxis("right").setWidth(20 + 2 * widget_values["label_font_size"] +
                                                         2 * widget_values["tick_font_size"])
         self.gui_obj.airfoil_canvas.plot.getAxis("bottom").setTickFont(tick_font)
         self.gui_obj.airfoil_canvas.plot.getAxis("left").setTickFont(tick_font)
 
     def labelFontChanged(self, _):
-        widget_values = self.valuesFromWidgets()
+        widget_values = self.value()
         theme_color = self.gui_obj.themes[self.gui_obj.current_theme]["main-color"]
         new_font = f"{widget_values['label_font_size']}pt {widget_values['label_font_family']}"
         set_setting("axis-label-font-family", widget_values["label_font_family"])
         set_setting("axis-label-point-size", widget_values["label_font_size"])
         for axis in ("left", "bottom"):
             label_text = self.gui_obj.airfoil_canvas.plot.getAxis(axis).label.toPlainText()
             self.gui_obj.airfoil_canvas.plot.setLabel(
                 axis=axis, text=label_text, color=theme_color, font=new_font)
         if self.gui_obj.cbar is not None:
             cbar_text = self.gui_obj.cbar.getAxis("right").label.toPlainText()
             self.gui_obj.cbar.setLabel(axis="right", text=cbar_text, color=theme_color, font=new_font)
             self.gui_obj.cbar.getAxis("right").setWidth(20 + 2 * widget_values["label_font_size"] +
                                                         2 * widget_values["tick_font_size"])
 
-    def setWidgetValuesFromDict(self, d: dict):
+    def setValue(self, d: dict):
         for d_name, d_value in d.items():
             try:
                 self.widget_dict[d_name].setValue(d_value)
             except KeyError:
                 pass
 
-    def valuesFromWidgets(self) -> dict:
+    def value(self) -> dict:
         return {k: v.value() for k, v in self.widget_dict.items()}
 
     def minLevelChanged(self, min_level: float):
         self.widget_dict["max_level"].widget.setMinimum(min_level + 0.0001)
         self.gui_obj.airfoil_canvas.setColorBarLevels(min_level, self.widget_dict["max_level"].widget.value())
 
     def maxLevelChanged(self, max_level: float):
@@ -3097,24 +3306,47 @@
         self.removeSplitPoint()
         super().reject()
 
     def close(self):
         self.removeSplitPoint()
         super().close()
 
-    def valuesFromWidgets(self):
+    def value(self):
         return self.spin.value()
 
 
-class SettingsDialogWidget(PymeadDialogWidget2):
-
-    def __init__(self, parent):
-        super().__init__(parent)
+class GeneralSettingsDialogWidget(PymeadDialogWidget2):
+    def __init__(self, geo_col: GeometryCollection, parent=None):
+        self.geo_col = geo_col
+        super().__init__(parent=parent)
 
     def initializeWidgets(self, *args, **kwargs):
-        pass
+        self.widget_dict = {
+            "length_unit": PymeadLabeledComboBox(label="Length Unit", items=["m", "mm", "in", "cm"],
+                                                 current_item=UNITS.current_length_unit()),
+            "angle_unit": PymeadLabeledComboBox(label="Angle Unit", items=["rad", "deg"],
+                                                current_item=UNITS.current_angle_unit())
+        }
 
-    def setWidgetValuesFromDict(self, *args, **kwargs):
-        pass
+    def establishWidgetConnections(self):
+        self.widget_dict["length_unit"].sigValueChanged.connect(self.onLengthUnitChanged)
+        self.widget_dict["angle_unit"].sigValueChanged.connect(self.onAngleUnitChanged)
+
+    def onLengthUnitChanged(self, new_unit: str):
+        self.geo_col.switch_units("length", old_unit=UNITS.current_length_unit(), new_unit=new_unit)
+        q_settings.setValue("length_unit", new_unit)
+        if self.geo_col.gui_obj.field_plot_variable is not None:
+            self.geo_col.gui_obj.plot_field(show_dialog=False)
+
+    def onAngleUnitChanged(self, new_unit: str):
+        self.geo_col.switch_units("angle", old_unit=UNITS.current_angle_unit(), new_unit=new_unit)
+        q_settings.setValue("angle_unit", new_unit)
 
-    def valuesFromWidgets(self) -> dict:
-        pass
+
+class SettingsDialog(PymeadDialog):
+
+    def __init__(self, parent, geo_col: GeometryCollection, theme: dict, settings_override: dict = None):
+        widgets = {
+            "General": GeneralSettingsDialogWidget(geo_col=geo_col)
+        }
+        w = PymeadDialogVTabWidget(parent=None, widgets=widgets, settings_override=settings_override)
+        super().__init__(parent=parent, window_title="Settings", widget=w, theme=theme)
```

### Comparing `pymead-2.0.0b3/pymead/gui/main_icon_toolbar.py` & `pymead-2.0.0b4/pymead/gui/main_icon_toolbar.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/message_box.py` & `pymead-2.0.0b4/pymead/gui/message_box.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt5.QtCore import Qt
 
-from pymead.gui.input_dialog import PymeadMessageBox
+from pymead.gui.dialogs import PymeadMessageBox
 
 
 def disp_message_box(message: str, parent, theme: dict, message_mode: str = 'error', rich_text: bool = False):
     window_title_keys = {"error": "Error", "info": "Information", "warn": "Warning"}
     msg_box = PymeadMessageBox(parent, msg=message, window_title=window_title_keys[message_mode], msg_mode=message_mode,
                                theme=theme)
     if rich_text:
```

### Comparing `pymead-2.0.0b3/pymead/gui/opt_airfoil_graph.py` & `pymead-2.0.0b4/pymead/gui/parallel_coords_graph.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pyqtgraph as pg
 
 
-class OptAirfoilGraph:
+class ParallelCoordsGraph:
     def __init__(self, pen=None, size: tuple = (1000, 300), background_color: str = 'w'):
         pg.setConfigOptions(antialias=True)
 
         if pen is None:
             pen = pg.mkPen(color='cornflowerblue', width=2)
 
         self.w = pg.GraphicsLayoutWidget(show=True, size=size)
         # self.w.setWindowTitle('Airfoil')
         self.w.setBackground(background_color)
         self.v = self.w.addPlot(pen=pen)
-        self.v.setAspectLocked()
-        self.v.setLabel(axis='bottom', text='x')
-        self.v.setLabel(axis='left', text='y')
-        self.legend = self.v.addLegend(offset=(300, 20))
-        # self.v.setAspectLocked()
+        self.v.setYRange(0, 1, padding=0)
+        self.v.setLabel(axis='bottom', text='parameter')
+        self.v.setLabel(axis='left', text='normalized value')
+        self.v.showGrid(x=True, y=True)
 
     def set_background(self, background_color: str):
         self.w.setBackground(background_color)
```

### Comparing `pymead-2.0.0b3/pymead/gui/parameter_tree.py` & `pymead-2.0.0b4/pymead/gui/parameter_tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
 from abc import abstractmethod
+from copy import deepcopy
 
-from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QRegularExpression
+from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QRegularExpression, QStringListModel
 from PyQt5.QtGui import QValidator, QBrush, QColor
 from PyQt5.QtWidgets import QTreeWidget, QTreeWidgetItem, QPushButton, QHBoxLayout, QHeaderView, QDialog, QGridLayout, \
-    QDoubleSpinBox, QLineEdit, QLabel, QMenu, QAbstractItemView, QTreeWidgetItemIterator, QWidget
+    QDoubleSpinBox, QLineEdit, QLabel, QMenu, QAbstractItemView, QTreeWidgetItemIterator, QWidget, QCompleter
 
 from pymead.core.airfoil import Airfoil
 from pymead.core.bezier import Bezier
 from pymead.core.constraints import *
 from pymead.core.geometry_collection import GeometryCollection
 from pymead.core.line import LineSegment, PolyLine
 from pymead.core.mea import MEA
-from pymead.core.param import Param, DesVar, LengthParam, AngleParam, LengthDesVar, AngleDesVar
+from pymead.core.param import Param, DesVar, LengthParam, AngleParam, LengthDesVar, AngleDesVar, EquationCompileError
 from pymead.core.point import Point
 from pymead.core.pymead_obj import PymeadObj
-from pymead.gui.input_dialog import PymeadDialog
+from pymead.gui.dialogs import PymeadDialog
 
 
 class HeaderButtonRow(QHeaderView):
     sigExpandPressed = pyqtSignal()
     sigCollapsePressed = pyqtSignal()
 
     def __init__(self, parent):
@@ -65,14 +66,15 @@
         else:
             # if isinstance(self.param, AngleParam):
             #     self.setMaximum(UNITS.convert_angle_to_base(2 * np.pi, self.param.unit()))
             # else:
             self.setMaximum(1.0e9)
         self.setValue(self.param.value())
         self.valueChanged.connect(self.onValueChanged)
+        self.setEnabled(self.param.enabled())
 
     # def setValue(self, val):
     #
     #     print(f"{val = }")
     #
     #     if isinstance(self.param, LengthParam) and self.param.point is None and val < 0.0:
     #         return
@@ -232,14 +234,75 @@
         return dialog
 
     @abstractmethod
     def modifyDialogInternals(self, dialog: QDialog, layout: QGridLayout) -> None:
         pass
 
 
+class Completer(QCompleter):
+    """
+    From https://gitter.im/baudren/NoteOrganiser?at=55afbefdcce129d570a3c188
+    """
+
+    def __init__(self, model=None, parent=None):
+        if model is None:
+            super().__init__(parent)
+        else:
+            super().__init__(model, parent)
+
+        self.setCaseSensitivity(Qt.CaseInsensitive)
+        self.setCompletionMode(QCompleter.PopupCompletion)
+        self.setWrapAround(False)
+
+    # Add texts instead of replace
+    def pathFromIndex(self, index):
+        path = QCompleter.pathFromIndex(self, index)
+
+        print(f"At the start, {path = }")
+
+        lst = str(self.widget().text()).split('$')
+
+        if len(lst) > 1:
+            # path = "$".join(lst[:-1]) + path
+            path = "$" + path
+
+        print(f"{lst = }, {path = }, {self.widget().text() = }")
+
+        return path
+
+    # Add operator to separate between texts
+    def splitPath(self, path):
+        for ch in [" ", "+", " - ", "*", "/", "(", "$"]:
+            path = str(path.split(ch)[-1])
+            print(f"{path = }")
+        return [path]
+
+
+class ParamEquationEdit(QLineEdit):
+    def __init__(self, param: Param, parent=None):
+        super().__init__(parent=parent)
+        self.param = param
+        # completer = Completer([p.name() for p in self.param.param_graph.param_list], self)
+        # self.setCompleter(completer)  # TODO: fix autocomplete (removed for now)
+        self.editingFinished.connect(self.updateEquation)
+        self.setPlaceholderText("$")
+        if self.param.equation_str is not None:
+            self.setText(self.param.equation_str)
+
+    def updateEquation(self):
+        try:
+            self.param.update_equation(self.text())
+        except EquationCompileError as e:
+            if self.param.geo_col and self.param.geo_col.gui_obj:
+                self.param.geo_col.gui_obj.disp_message_box(str(e))
+                return
+            else:
+                raise e
+
+
 class ParamButton(TreeButton):
     sigValueChanged = pyqtSignal(float)  # value
 
     def __init__(self, param: Param, tree, name_editable: bool = True, top_level: bool = False):
         super().__init__(pymead_obj=param, tree=tree, top_level=top_level)
         self.name_editable = name_editable
         self.param = param
@@ -265,14 +328,17 @@
             layout.addWidget(lower_spin, row_count, 1)
         if self.param.upper() is not None:
             upper_label = QLabel("Upper Bound", self)
             upper_spin = UpperSpin(self, self.param)
             row_count = layout.rowCount()
             layout.addWidget(upper_label, row_count, 0)
             layout.addWidget(upper_spin, row_count, 1)
+        row_count = layout.rowCount()
+        layout.addWidget(QLabel("Equation"), row_count, 0)
+        layout.addWidget(ParamEquationEdit(param=self.param, parent=self), row_count, 1)
 
     def onValueChange(self, value: float):
         self.sigValueChanged.emit(value)
 
 
 class LengthParamButton(ParamButton):
     pass
@@ -309,14 +375,17 @@
         layout.addWidget(lower_label, row_count, 0)
         layout.addWidget(lower_spin, row_count, 1)
         upper_label = QLabel("Upper Bound", self)
         upper_spin = UpperSpin(self, self.desvar)
         row_count = layout.rowCount()
         layout.addWidget(upper_label, row_count, 0)
         layout.addWidget(upper_spin, row_count, 1)
+        row_count = layout.rowCount()
+        layout.addWidget(QLabel("Equation"), row_count, 0)
+        layout.addWidget(ParamEquationEdit(param=self.desvar, parent=self), row_count, 1)
 
     def onValueChange(self, value: float):
         self.sigValueChanged.emit(value)
 
 
 class LengthDesVarButton(DesVarButton):
     pass
@@ -374,32 +443,72 @@
         if self.pymead_obj.tree_item.hoverable:
             self.tree.geo_col.hover_leave_obj(self.pymead_obj)
 
 
 class BezierButton(TreeButton):
 
     def __init__(self, bezier: Bezier, tree, top_level: bool = False):
-        super().__init__(pymead_obj=bezier, tree=tree, top_level=top_level)
         self.bezier = bezier
+        super().__init__(pymead_obj=bezier, tree=tree, top_level=top_level)
 
     def modifyDialogInternals(self, dialog: QDialog, layout: QGridLayout) -> None:
         name_label = QLabel("Name", self)
         name_edit = NameEdit(self, self.bezier, self.tree)
         name_edit.textChanged.connect(self.onNameChange)
         layout.addWidget(name_label, 1, 0)
         layout.addWidget(name_edit, 1, 1)
         for point in self.bezier.point_sequence().points():
             point_button = PointButton(point, self.tree)
             point_button.sigNameChanged.connect(self.onPointNameChange)
             layout.addWidget(point_button, layout.rowCount(), 0)
 
+        # Add t start widget
+        row_count = layout.rowCount()
+        layout.addWidget(QLabel("t start", self), row_count, 0)
+        t_start_widget = QDoubleSpinBox(self)
+        t_start_widget.setMinimum(-np.inf)
+        t_start_widget.setMaximum(np.inf)
+        t_start_widget.setSingleStep(0.01)
+        t_start_widget.setDecimals(8)
+        if self.bezier.t_start is not None:
+            t_start_widget.setValue(self.bezier.t_start)
+        else:
+            t_start_widget.setValue(0.0)
+        t_start_widget.valueChanged.connect(self.onTStartChange)
+        layout.addWidget(t_start_widget, row_count, 1)
+
+        # Add t end widget
+        row_count = layout.rowCount()
+        layout.addWidget(QLabel("t end", self), row_count, 0)
+        t_end_widget = QDoubleSpinBox(self)
+        t_end_widget.setMinimum(-np.inf)
+        t_end_widget.setMaximum(np.inf)
+        t_end_widget.setSingleStep(0.01)
+        t_end_widget.setDecimals(8)
+        if self.bezier.t_end is not None:
+            t_end_widget.setValue(self.bezier.t_end)
+        else:
+            t_end_widget.setValue(1.0)
+        t_end_widget.valueChanged.connect(self.onTEndChange)
+        layout.addWidget(t_end_widget, row_count, 1)
+
+        dialog.setMinimumWidth(250)
+
     def onPointNameChange(self, name: str, point: Point):
         if point.tree_item is not None:
             self.tree.itemWidget(point.tree_item, 0).setText(name)
 
+    def onTStartChange(self, t_start: float):
+        self.bezier.t_start = t_start
+        self.bezier.canvas_item.updateCurveItem(self.bezier.evaluate())
+
+    def onTEndChange(self, t_end: float):
+        self.bezier.t_end = t_end
+        self.bezier.canvas_item.updateCurveItem(self.bezier.evaluate())
+
     def enterEvent(self, a0):
         self.bezier.canvas_item.setCurveStyle("hovered")
 
     def leaveEvent(self, a0):
         self.bezier.canvas_item.setCurveStyle("default")
 
 
@@ -849,16 +958,14 @@
         top_level_item = self.items[self.topLevelDict[pymead_obj.sub_container]]
         child_item = PymeadTreeWidgetItem([pymead_obj.name()])
         top_level_item.addChild(child_item)
         pymead_obj.tree_item = child_item
 
         if isinstance(pymead_obj, Param):
             right_column_widget = ValueSpin(self, pymead_obj)
-            if not pymead_obj.enabled:
-                right_column_widget.setEnabled(False)
             self.setItemWidget(child_item, 1, right_column_widget)
 
     def removePymeadTreeItem(self, pymead_obj: PymeadObj):
         top_level_item = self.items[self.topLevelDict[pymead_obj.sub_container]]
         top_level_item.removeChild(pymead_obj.tree_item)
         pymead_obj.tree_item = None
 
@@ -890,14 +997,53 @@
 
     def setForegroundColorAllItems(self, color: str):
         it = QTreeWidgetItemIterator(self)
         while it.value():
             it.value().setForeground(0, QBrush(QColor(color)))
             it += 1
 
+    @staticmethod
+    def undoRedoAction(action: typing.Callable):
+        def wrapped(self, *args, **kwargs):
+            self.gui_obj.undo_stack.append(deepcopy(self.geo_col.get_dict_rep()))
+            action(self, *args, **kwargs)
+
+        return wrapped
+
+    @undoRedoAction
+    def removeObjects(self, pymead_objs: typing.List[PymeadObj]):
+        for pymead_obj in pymead_objs:
+            self.geo_col.remove_pymead_obj(pymead_obj)
+
+    @undoRedoAction
+    def promoteParamsToDesvar(self, pymead_objs: typing.List[Param]):
+        for pymead_obj in pymead_objs:
+            self.geo_col.promote_param_to_desvar(pymead_obj)
+
+    @undoRedoAction
+    def demoteDesvarsToParam(self, pymead_objs: typing.List[DesVar]):
+        for pymead_obj in pymead_objs:
+            self.geo_col.demote_desvar_to_param(pymead_obj)
+
+    @undoRedoAction
+    def exposePointXY(self, pymead_objs: typing.List[Point]):
+        for pymead_obj in pymead_objs:
+            self.geo_col.expose_point_xy(pymead_obj)
+
+    @undoRedoAction
+    def coverPointXY(self, pymead_objs: typing.List[Param]):
+        points_to_cover = list(set([pymead_obj.point for pymead_obj in pymead_objs]))
+        for point_to_cover in points_to_cover:
+            self.geo_col.cover_point_xy(point_to_cover)
+
+    @undoRedoAction
+    def equateConstraints(self, pymead_objs: typing.List[GeoCon]):
+        for pymead_obj in pymead_objs[1:]:
+            self.geo_col.equate_constraints(pymead_objs[0], pymead_obj)
+
     def contextMenuEvent(self, a0):
         # item = self.itemAt(a0.x(), a0.y())
         # if item is None:
         #     return
 
         items = self.selectedItems()
         if len(items) == 0:
@@ -932,14 +1078,15 @@
             pymead_objs = [pymead_obj for pymead_obj in pymead_objs if pymead_obj is not None]
 
             promoteAction = None
             demoteAction = None
             exposeAction = None
             coverAction = None
             addBezierPointAction = None
+            equateConstraintsAction = None
 
             pymead_obj_type = type(pymead_objs[0])
 
             menu = QMenu(self)
             if pymead_obj_type in [Param, LengthParam, AngleParam]:
                 promoteAction = menu.addAction("Promote to Design Variable")
                 if all([pymead_obj.point for pymead_obj in pymead_objs]):
@@ -948,37 +1095,32 @@
                 demoteAction = menu.addAction("Demote to Parameter")
                 if all([pymead_obj.point for pymead_obj in pymead_objs]):
                     coverAction = menu.addAction("Cover x and y Parameters")
             elif pymead_obj_type is Point:
                 exposeAction = menu.addAction("Expose x and y Parameters")
             elif pymead_obj_type is Bezier:
                 addBezierPointAction = menu.addAction("Insert Control Point")
+            elif pymead_obj_type in [DistanceConstraint, RelAngle3Constraint]:
+                equateConstraintsAction = menu.addAction("Equate Constraints")
             removeObjectAction = menu.addAction("Delete")
 
             res = menu.exec_(a0.globalPos())
 
             if res is None:
                 return
 
             if res is removeObjectAction:
-                for pymead_obj in pymead_objs:
-                    # If the object is a Point, set the style to default first so that the text item gets removed
-                    # if isinstance(pymead_obj, Point):
-                    #     self.geo_col.canvas.setItemStyle(pymead_obj.canvas_item, "default")
-                    self.geo_col.remove_pymead_obj(pymead_obj)
+                self.removeObjects(pymead_objs)
             elif res is promoteAction:
-                for pymead_obj in pymead_objs:
-                    self.geo_col.promote_param_to_desvar(pymead_obj)
+                self.promoteParamsToDesvar(pymead_objs)
             elif res is demoteAction:
-                for pymead_obj in pymead_objs:
-                    self.geo_col.demote_desvar_to_param(pymead_obj)
+                self.demoteDesvarsToParam(pymead_objs)
             elif res is exposeAction:
-                for pymead_obj in pymead_objs:
-                    self.geo_col.expose_point_xy(pymead_obj)
+                self.exposePointXY(pymead_objs)
             elif res is coverAction:
-                points_to_cover = list(set([pymead_obj.point for pymead_obj in pymead_objs]))
-                for point_to_cover in points_to_cover:
-                    self.geo_col.cover_point_xy(point_to_cover)
+                self.coverPointXY(pymead_objs)
             elif res is addBezierPointAction:
                 self.gui_obj.airfoil_canvas.addPointToCurve(pymead_objs[0].canvas_item)
+            elif res is equateConstraintsAction:
+                self.equateConstraints(pymead_objs)
 
             self.geo_col.clear_selected_objects()
```

### Comparing `pymead-2.0.0b3/pymead/gui/permanent_widget.py` & `pymead-2.0.0b4/pymead/gui/permanent_widget.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/polygon_item.py` & `pymead-2.0.0b4/pymead/gui/polygon_item.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/pymeadPColorMeshItem.py` & `pymead-2.0.0b4/pymead/gui/pymeadPColorMeshItem.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/verticalTabWidget.py` & `pymead-2.0.0b4/pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget/verticalTabWidget.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/rename_popup.py` & `pymead-2.0.0b4/pymead/gui/rename_popup.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/sampling_visualization.py` & `pymead-2.0.0b4/pymead/gui/sampling_visualization.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/scientificspinbox_master/ScientificDoubleSpinBox.py` & `pymead-2.0.0b4/pymead/gui/scientificspinbox_master/ScientificDoubleSpinBox.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/scientificspinbox_master/ScientificSpinBox.py` & `pymead-2.0.0b4/pymead/gui/scientificspinbox_master/ScientificSpinBox.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/selectable_header.py` & `pymead-2.0.0b4/pymead/gui/selectable_header.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/separation_lines.py` & `pymead-2.0.0b4/pymead/gui/separation_lines.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/show_hide.py` & `pymead-2.0.0b4/pymead/gui/show_hide.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QGridLayout, QCheckBox, QLabel, QWidget
 
-from pymead.gui.input_dialog import PymeadDialog
+from pymead.gui.dialogs import PymeadDialog
 
 
 class ShowHideDialog(PymeadDialog):
     def __init__(self, parent, state: dict, theme: dict):
         widget = QWidget()
         super().__init__(parent=parent, window_title="Show/Hide", widget=widget, theme=theme)
         self.lay = QGridLayout()
```

### Comparing `pymead-2.0.0b3/pymead/gui/side_grip.py` & `pymead-2.0.0b4/pymead/gui/side_grip.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/text_area.py` & `pymead-2.0.0b4/pymead/gui/text_area.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/title_bar.py` & `pymead-2.0.0b4/pymead/gui/title_bar.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/gui/worker.py` & `pymead-2.0.0b4/pymead/gui/worker.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/Add-Icon3.png` & `pymead-2.0.0b4/pymead/icons/Add-Icon3.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/Moon-Icon.png` & `pymead-2.0.0b4/pymead/icons/Moon-Icon.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/add_icon.png` & `pymead-2.0.0b4/pymead/icons/add_icon.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/airfoil_dark.svg` & `pymead-2.0.0b4/pymead/icons/airfoil_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/airfoil_light.svg` & `pymead-2.0.0b4/pymead/icons/airfoil_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/airfoil_slat.png` & `pymead-2.0.0b4/pymead/icons/airfoil_slat.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/anti_parallel_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/anti_parallel_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/anti_parallel_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/anti_parallel_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/back.png` & `pymead-2.0.0b4/pymead/icons/back.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/bezier_dark.svg` & `pymead-2.0.0b4/pymead/icons/bezier_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/bezier_light.svg` & `pymead-2.0.0b4/pymead/icons/bezier_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/close-dark-mode.svg` & `pymead-2.0.0b4/pymead/icons/close-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/close-light-mode.svg` & `pymead-2.0.0b4/pymead/icons/close-light-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/closed-arrow-dark.png` & `pymead-2.0.0b4/pymead/icons/closed-arrow-dark.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/closed-arrow-light.png` & `pymead-2.0.0b4/pymead/icons/closed-arrow-light.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/distance_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/distance_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/distance_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/distance_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/forward.png` & `pymead-2.0.0b4/pymead/icons/forward.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/grid_icon.png` & `pymead-2.0.0b4/pymead/icons/grid_icon.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/help.png` & `pymead-2.0.0b4/pymead/icons/help.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/home.png` & `pymead-2.0.0b4/pymead/icons/home.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/line_dark.svg` & `pymead-2.0.0b4/pymead/icons/line_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/line_light.svg` & `pymead-2.0.0b4/pymead/icons/line_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/maximize-dark-mode.svg` & `pymead-2.0.0b4/pymead/icons/maximize-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/maximize-light-mode.svg` & `pymead-2.0.0b4/pymead/icons/maximize-light-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/mea_dark.svg` & `pymead-2.0.0b4/pymead/icons/mea_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/mea_light.svg` & `pymead-2.0.0b4/pymead/icons/mea_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/minimize-dark-mode.svg` & `pymead-2.0.0b4/pymead/icons/minimize-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/minimize-light-mode.svg` & `pymead-2.0.0b4/pymead/icons/minimize-light-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/normal-dark-mode.svg` & `pymead-2.0.0b4/pymead/icons/normal-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/normal-light-mode.svg` & `pymead-2.0.0b4/pymead/icons/normal-light-mode.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/opened-arrow-dark.png` & `pymead-2.0.0b4/pymead/icons/opened-arrow-dark.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/opened-arrow-light.png` & `pymead-2.0.0b4/pymead/icons/opened-arrow-light.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/perp3_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/perp3_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/perp3_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/perp3_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/point_dark.svg` & `pymead-2.0.0b4/pymead/icons/point_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/point_light.svg` & `pymead-2.0.0b4/pymead/icons/point_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/pymead-logo.png` & `pymead-2.0.0b4/pymead/icons/pymead-logo.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/pymead-logo_old.png` & `pymead-2.0.0b4/pymead/icons/pymead-logo_old.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/rel_angle_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/rel_angle_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/rel_angle_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/rel_angle_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/reload.png` & `pymead-2.0.0b4/pymead/icons/reload.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/roc_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/roc_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/roc_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/roc_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/stop.png` & `pymead-2.0.0b4/pymead/icons/stop.png`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/symmetry_constraint_dark.svg` & `pymead-2.0.0b4/pymead/icons/symmetry_constraint_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/symmetry_constraint_light.svg` & `pymead-2.0.0b4/pymead/icons/symmetry_constraint_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/web_airfoil_dark.svg` & `pymead-2.0.0b4/pymead/icons/web_airfoil_dark.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/icons/web_airfoil_light.svg` & `pymead-2.0.0b4/pymead/icons/web_airfoil_light.svg`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/optimization/conn_test.py` & `pymead-2.0.0b4/pymead/optimization/conn_test.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/optimization/objectives_and_constraints.py` & `pymead-2.0.0b4/pymead/optimization/objectives_and_constraints.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/optimization/opt_callback.py` & `pymead-2.0.0b4/pymead/optimization/opt_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,17 @@
             # self.parent.output_area_text(f"<head><style>body {{font-family: DejaVu Sans Mono;}}</style></head><body><p><font size='4'>&#8203;</font></p></body>", mode="html")
             # self.parent.output_area_text("\n")
             for header_line in self.generate_header():
                 self.parent.output_area_text(header_line, line_break=True)
             # self.parent.output_area_text("\n")
         t = f"{self.stringify_text_list()}"
         self.parent.output_area_text(t, line_break=True)
-        # self.parent.output_area_text("\n")
         self.parent.closer = self.generate_closer(len(t))
         if self.completed:
             self.parent.output_area_text(f"{self.generate_closer(len(t))}", line_break=True)
-            self.parent.stop_optimization(completed=True)
-            # self.parent.output_area_text("\n")
 
 
 class PlotAirfoilCallback(OptCallback):
     def __init__(self, parent, coords: list, background_color: str = 'w'):
         super().__init__(parent=parent)
         self.coords = coords
         self.parent = parent
```

### Comparing `pymead-2.0.0b3/pymead/optimization/opt_setup.py` & `pymead-2.0.0b4/pymead/optimization/opt_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from pymoo.core.problem import Problem
 from pymoo.factory import get_decomposition
 from pymoo.util.display import Display
 from pymoo.util.termination.default import MultiObjectiveDefaultTermination
 from pymoo.util.termination.f_tol import MultiObjectiveSpaceToleranceTermination
 
-from pymead.gui.input_dialog import convert_dialog_to_mset_settings, convert_dialog_to_mses_settings, \
+from pymead.gui.dialogs import convert_dialog_to_mset_settings, convert_dialog_to_mses_settings, \
     convert_dialog_to_mplot_settings
 
 multi_point_keys_mses = {
     0: 'MACHIN',
     1: 'REYNIN',
     2: 'ALFAIN',
     3: 'CLIFIN',
```

### Comparing `pymead-2.0.0b3/pymead/optimization/pop_chrom.py` & `pymead-2.0.0b4/pymead/optimization/pop_chrom.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,28 +68,29 @@
             self.mea_airfoil_names = [airfoil.name() for airfoil in self.mea.airfoils]
         # self.mea_object = MEA.generate_from_param_dict(self.mea)
         # if deactivate_airfoil_graphs:
         #     self.mea_object.remove_airfoil_graphs()
         if self.verbose:
             print(f'Generating chromosome idx = {self.population_idx}, gen = {self.generation}')
         self.generate_airfoil_sys_from_genes()
-        line_strings = self.get_airfoil_line_strings()
+        line_strings = self.get_airfoil_line_strings(airfoil_frame_relative=False)
+        relative_line_strings = self.get_airfoil_line_strings(airfoil_frame_relative=True)
         airfoil_polygons = self.get_airfoil_polygons(line_strings)
         self.chk_self_intersection(line_strings)
         for airfoil in self.airfoil_list:
             airfoil_name = airfoil.name()
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['min_radius_curvature'][1]:
                     self.chk_min_radius(airfoil_name=airfoil_name)
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['min_val_of_max_thickness'][1]:
-                    self.chk_max_thickness(line_strings[airfoil_name], airfoil_name=airfoil_name)
+                    self.chk_max_thickness(relative_line_strings[airfoil_name], airfoil_name=airfoil_name)
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['thickness_at_points'] is not None:
-                    self.check_thickness_at_points(line_strings[airfoil_name], airfoil_name=airfoil_name)
+                    self.check_thickness_at_points(relative_line_strings[airfoil_name], airfoil_name=airfoil_name)
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['min_area'][1]:
                     self.check_min_area(airfoil_polygons[airfoil_name], airfoil_name=airfoil_name)
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['internal_geometry'] is not None:
                     if self.param_dict['constraints'][airfoil_name]['internal_geometry_timing'] == 'Before Aerodynamic Evaluation':
                         self.check_contains_points(airfoil_polygons[airfoil_name], airfoil_name=airfoil_name)
@@ -97,24 +98,26 @@
                         raise ValueError('Internal geometry timing after aerodynamic evaluation not yet implemented')
             if self.valid_geometry:
                 if self.param_dict['constraints'][airfoil_name]['external_geometry'] is not None:
                     if self.param_dict['constraints'][airfoil_name]['external_geometry_timing'] == 'Before Aerodynamic Evaluation':
                         self.check_if_inside_points(airfoil_name=airfoil_name)
                     else:
                         raise ValueError('External geometry timing after aerodynamic evaluation not yet implemented')
-        # self.control_points = [[c.P.tolist() for c in self.mea_object.airfoils[k].curve_list]
-        #                        for k in self.mea_object.airfoils.keys()]
-        # self.airfoil_state = {k: {p: getattr(a, p).value for p in ['c', 'alf', 'dx', 'dy']} for k, a in self.mea_object.airfoils.items()}
-        # self.mea_object = None
+
+        # Set the equation_dict to None because it contains the unpicklable __builtins__ module
+        for param in self.geo_col.container()["params"].values():
+            param.equation_dict = None
+        for desvar in self.geo_col.container()["desvar"].values():
+            desvar.equation_dict = None
 
     def get_coords(self):
         if self.airfoil is not None:
-            coords = self.airfoil.get_coords_selig_format()
+            coords = self.airfoil.get_scaled_coords()
         else:
-            coords = self.mea.get_coords_list(
+            coords, transformation_kwargs = self.mea.get_coords_list_chord_relative(
                 max_airfoil_points=self.param_dict['mset_settings']["downsampling_max_pts"] if bool(
                     self.param_dict['mset_settings']["use_downsampling"]) else None,
                 curvature_exp=self.param_dict['mset_settings']["downsampling_curve_exp"]
             )
         return coords
 
     def generate_airfoil_sys_from_genes(self) -> dict:
@@ -128,24 +131,32 @@
         self.coords = self.get_coords()
         self.airfoil_sys_generated = True
         return self.param_dict
 
     def update_param_dict(self):
         if self.param_dict["tool"] != "MSES":
             return
-        # dben = benedict(self.param_dict)
-        # for idx, from_geometry in enumerate(self.param_dict['mses_settings']['from_geometry']):
-        #     for k, v in from_geometry.items():
-        #         self.param_dict['mses_settings'][k][idx] = dben[v.replace('$', '')].value
+        xcdelh_params = self.param_dict["mses_settings"]["XCDELH-Param"]
+        for idx, xcdelh_param in enumerate(xcdelh_params):
+            if xcdelh_param:
+                if xcdelh_param in self.geo_col.container()["params"]:
+                    self.param_dict["mses_settings"]["XCDELH"][idx] = self.geo_col.container()["params"][xcdelh_param].value()
+                elif xcdelh_param in self.geo_col.container()["desvar"]:
+                    self.param_dict["mses_settings"]["XCDELH"][idx] = self.geo_col.container()["desvar"][xcdelh_param].value()
+                else:
+                    raise ValueError(f"Could not find XCDELH parameter {xcdelh_param}")
 
-    def get_airfoil_line_strings(self):
+    def get_airfoil_line_strings(self, airfoil_frame_relative: bool):
         line_strings = {}
         for airfoil in self.airfoil_list:
-            line_strings[airfoil.name()] = Airfoil.create_line_string(
-                Airfoil.convert_coords_to_shapely_format(airfoil.coords))
+            if airfoil_frame_relative:
+                coords = airfoil.get_chord_relative_coords(airfoil.coords)
+            else:
+                coords = airfoil.coords
+            line_strings[airfoil.name()] = Airfoil.create_line_string(Airfoil.convert_coords_to_shapely_format(coords))
         return line_strings
 
     @staticmethod
     def get_airfoil_polygons(line_strings: dict):
         return {k: Airfoil.create_shapely_polygon(v) for k, v in line_strings.items()}
 
     def chk_self_intersection(self, line_strings: dict) -> bool:
@@ -211,16 +222,16 @@
             raise Exception('Airfoil system has not yet been generated. Aborting self-intersection check.')
 
     def check_thickness_at_points(self, line_string, airfoil_name: str):
         if self.airfoil_sys_generated:
             thickness_array = np.array(self.param_dict['constraints'][airfoil_name]['thickness_at_points'])
             x_over_c_array = thickness_array[:, 0]
             t_over_c_array = thickness_array[:, 1]
-            thickness = self.geo_col.container()["airfoils"][airfoil_name].compute_thickness_at_points(
-                line_string, x_over_c_array)
+            airfoil = self.geo_col.container()["airfoils"][airfoil_name]
+            thickness = airfoil.compute_thickness_at_points(x_over_c_array, line_string)
             if np.any(thickness < t_over_c_array):
                 if self.verbose:
                     print(f"Minimum required thickness condition not met at some point. Trying again")
                 self.valid_geometry = False
             else:
                 if self.verbose:
                     print(f"Minimum required thickness condition met everywhere [success]")
@@ -318,25 +329,14 @@
                                                        mea_airfoil_names=chromosome.mea_airfoil_names,
                                                        xfoil_settings=xfoil_settings,
                                                        mset_settings=mset_settings,
                                                        mses_settings=mses_settings,
                                                        mplot_settings=mplot_settings,
                                                        export_Cp=True)
 
-            # Here, we remove the data attribute from the chromosome, since "data" includes a non-serializable
-            # JIT-compiled equation set. Without these two lines, an error is raised when trying to send data across
-            # the pipe
-            # chromosome.geo_col = None
-            # if chromosome.mea is not None:
-            #     chromosome.mea.geo_col = None
-            #     for airfoil in chromosome.mea.airfoils:
-            #         airfoil.geo_col = None
-            for cnstr in chromosome.geo_col.container()["geocon"].values():
-                cnstr.data = None
-
             if (xfoil_settings is not None and xfoil_settings["multi_point_stencil"] is None) or (
                     mses_settings is not None and mses_settings['multi_point_stencil'] is None):
                 if chromosome.forces['converged'] and not chromosome.forces['errored_out'] \
                         and not chromosome.forces['timed_out']:
                     chromosome.fitness = 1  # Set to any value that is not False and not None
             else:
                 if all(chromosome.forces['converged']) and not any(chromosome.forces['errored_out']) and not any(chromosome.forces['timed_out']):
```

### Comparing `pymead-2.0.0b3/pymead/optimization/sampling.py` & `pymead-2.0.0b4/pymead/optimization/sampling.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/optimization/shape_optimization.py` & `pymead-2.0.0b4/pymead/optimization/shape_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     if param_dict["tool"] == "XFOIL":
         airfoil_name = opt_settings["XFOIL"]["airfoil"]
     elif param_dict["tool"] == "MSES":
         mea_name = opt_settings["MSET"]["mea"]
     parameter_list = geo_col.extract_design_variable_values(bounds_normalized=True)
     num_parameters = len(parameter_list)
 
-    send_over_pipe(("text", f"Number of active and unlinked design variables: {num_parameters}"))
+    send_over_pipe(("text", f"Number of design variables: {num_parameters}"))
 
     problem = TPAIOPT(n_var=param_dict['n_var'], n_obj=param_dict['n_obj'], n_constr=param_dict['n_constr'],
                       xl=param_dict['xl'], xu=param_dict['xu'], param_dict=param_dict)
 
     if not opt_settings['General Settings']['warm_start_active']:
         if param_dict['seed'] is not None:
             np.random.seed(param_dict['seed'])
@@ -407,12 +407,11 @@
         if n_generation % param_dict['algorithm_save_frequency'] == 0:
             save_data(algorithm, os.path.join(param_dict['opt_dir'], f'algorithm_gen_{n_generation}.pkl'))
 
     # obtain the result objective from the algorithm
     res = algorithm.result()
     save_data(res, os.path.join(param_dict['opt_dir'], 'res.pkl'))
     write_force_dict_to_file(forces_dict, os.path.join(param_dict["opt_dir"], "force_history.json"))
-    if len(objectives) == 1:
-        np.savetxt(os.path.join(param_dict['opt_dir'], 'opt_X.dat'), res.X)
+    np.savetxt(os.path.join(param_dict['opt_dir'], 'opt_X.dat'), res.X)
 
     send_over_pipe(("finished", None))
     # self.save_opt_plots(param_dict['opt_dir'])  # not working at the moment
```

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/curves.py` & `pymead-2.0.0b4/pymead/plugins/IGES/curves.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/entity.py` & `pymead-2.0.0b4/pymead/plugins/IGES/entity.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/global_params.py` & `pymead-2.0.0b4/pymead/plugins/IGES/global_params.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/iges_generator.py` & `pymead-2.0.0b4/pymead/plugins/IGES/iges_generator.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/iges_param.py` & `pymead-2.0.0b4/pymead/plugins/IGES/iges_param.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/IGES/start_end_section.py` & `pymead-2.0.0b4/pymead/plugins/IGES/start_end_section.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/NX/journal_functions.py` & `pymead-2.0.0b4/pymead/plugins/NX/journal_functions.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/plugins/NX/write_journal_function.py` & `pymead-2.0.0b4/pymead/plugins/NX/write_journal_function.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/post/mses_field.py` & `pymead-2.0.0b4/pymead/post/mses_field.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/post/plot_formatters.py` & `pymead-2.0.0b4/pymead/post/plot_formatters.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/post/post_process.py` & `pymead-2.0.0b4/pymead/post/post_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.colors as mpl_colors
 import numpy
 from matplotlib import animation
 from matplotlib.lines import Line2D
 from matplotlib import ticker as mticker
-import scienceplots
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-from matplotlib.ticker import MultipleLocator
 from cycler import cycler
-from matplotlib.patches import Polygon, Patch, Arrow
+from matplotlib.patches import Polygon, Patch
 import numpy as np
 from copy import deepcopy
 import PIL
 from pymoo.decomposition.asf import ASF
 
 from pymead.optimization.objectives_and_constraints import Objective
 from pymead.utils.read_write_files import load_data, save_data
 from pymead.optimization.pop_chrom import Chromosome, Population
-from pymead.post.mses_field import generate_field_matplotlib, flow_var_label
+from pymead.post.mses_field import generate_field_matplotlib
 from pymead.analysis.read_aero_data import read_bl_data_from_mses
-from functools import partial
-from pymead.core.bezier import Bezier
-from pymead.core.mea import MEA
-from pymead.core.transformation import Transformation2D
+from pymead.core.geometry_collection import GeometryCollection
 from pymead.utils.transformations import rotate_matrix
 from pymead.post.fonts_and_colors import ILLINI_ORANGE, ILLINI_BLUE, font
 from pymead.post.plot_formatters import format_axis_scientific, show_save_fig, legend_entry_flip
 from pymead import DATA_DIR
 
 
 ylabel = {
@@ -98,16 +92,16 @@
         self.solid_handles = []
         self.analysis_dir = analysis_dir
         self.image_dir = image_dir
         if not os.path.exists(self.image_dir):
             os.mkdir(self.image_dir)
         self.post_process_force_file = post_process_force_file
         self.jmea_file = jmea_file
-        self.mea = load_data(jmea_file)
-        self.mea['airfoil_graphs_active'] = False
+        self.geo_col_dict = load_data(jmea_file)
+        self.geo_col_dict['airfoil_graphs_active'] = False
         self.underwing = underwing
         self.param_dict = load_data(os.path.join(self.analysis_dir, 'param_dict.json'))
         self.pop_size = deepcopy(self.param_dict["population_size"])
         print(f"{self.pop_size = }")
         self.param_dict_original = deepcopy(self.param_dict)
         self.modify_param_dict_func = modify_param_dict_func
         if self.modify_param_dict_func is not None:
@@ -215,15 +209,15 @@
 
     def get_mea(self, index: int, weight_idx: int = 0):
         if index != 0:
             X = self.get_X(os.path.join(self.analysis_dir, f"algorithm_gen_{index}.pkl"), weight_idx=weight_idx)
         else:
             X = None
 
-        mea_object = MEA.generate_from_param_dict(self.mea)
+        mea_object = GeometryCollection.set_from_dict_rep(self.geo_col_dict)
 
         if X is not None:
             mea_object.update_parameters(X)
 
         return mea_object
 
     def set_index(self, index: int or typing.Iterable = None):
@@ -252,19 +246,25 @@
         param_set['mses_settings']['timeout'] += 10.0
         param_set['mset_settings']['airfoil_analysis_dir'] = os.path.join(
             self.analysis_dir, 'analysis', f'analysis_0')
         param_set['mset_settings']['airfoil_coord_file_name'] = f'analysis_0'
         param_set['base_folder'] = os.path.join(self.analysis_dir, 'analysis')
         param_set['name'] = [f"analysis_0"]
 
-        chromosome = Chromosome(param_dict=param_set, population_idx=0, mea=self.mea, genes=None,
-                                generation=0)
+        airfoil_name, mea_name = None, None
+        if param_set["tool"] == "XFOIL":
+            airfoil_name = param_set["xfoil_settings"]["airfoil"]
+        elif param_set["tool"] == "MSES":
+            mea_name = param_set["mset_settings"]["mea"]
+
+        chromosome = Chromosome(param_dict=param_set, population_idx=0, geo_col_dict=deepcopy(self.geo_col_dict),
+                                genes=None, generation=0, mea_name=mea_name, airfoil_name=airfoil_name)
 
         population = Population(param_dict=param_set, generation=0, parents=[chromosome],
-                                mea=self.mea, verbose=True, skip_parent_assignment=False)
+                                verbose=True, skip_parent_assignment=False)
 
         population.eval_pop_fitness()
         population_forces = population.population[0].forces
         obj_fun_strings = self.settings["Genetic Algorithm"]["J"].split(",")
         J_baseline = []
         for J in obj_fun_strings:
             objective = Objective("")
@@ -294,46 +294,57 @@
                 param_set = deepcopy(self.param_dict)
                 param_set['mset_settings']['airfoil_analysis_dir'] = os.path.join(
                     self.analysis_dir, 'analysis', f'analysis_{i}' + weight_str)
                 param_set['mset_settings']['airfoil_coord_file_name'] = f'analysis_{i}' + weight_str
                 param_set['base_folder'] = os.path.join(self.analysis_dir, 'analysis')
                 param_set['name'] = [f"analysis_{j}" + weight_str for j in index]
 
+                airfoil_name, mea_name = None, None
+                if param_set["tool"] == "XFOIL":
+                    airfoil_name = param_set["xfoil_settings"]["airfoil"]
+                elif param_set["tool"] == "MSES":
+                    mea_name = param_set["mset_settings"]["mea"]
+
                 # parent_chromosomes.append(Chromosome(param_set=param_set, population_idx=s, mea=mea, X=X))
                 X = X_list[idx]
-                self.chromosomes.append(Chromosome(param_dict=param_set, population_idx=i, mea=self.mea, genes=X,
-                                                   generation=0))
+                self.chromosomes.append(Chromosome(param_dict=param_set, population_idx=i,
+                                                   geo_col_dict=deepcopy(self.geo_col_dict), genes=X,
+                                                   generation=0, mea_name=mea_name, airfoil_name=airfoil_name))
 
             population = Population(param_dict=self.param_dict, generation=0, parents=self.chromosomes,
-                                    mea=self.mea, verbose=True, skip_parent_assignment=False)
-            population.generate_chromosomes_parallel()
+                                    verbose=True, skip_parent_assignment=False)
+
+            if evaluate:
+                population.eval_pop_fitness()
+                population_forces = {k: [c.forces[k] if c.forces is not None else None for c in population.population]
+                                     for k in population.population[0].forces.keys()}
+                post_process_file_split = os.path.splitext(self.post_process_force_file)
+                save_data(population_forces, post_process_file_split[0] + weight_str + post_process_file_split[1])
+            else:
+                population.generate_chromosomes_parallel()
+
             if save_coords:
                 if not os.path.exists(os.path.join(self.analysis_dir, f'coords{weight_str}')):
                     os.mkdir(os.path.join(self.analysis_dir, f'coords{weight_str}'))
                 for idx, c in enumerate(population.population):
-                    save_data(c.coords, os.path.join(self.analysis_dir, f'coords{weight_str}', f'coords_{index[idx]}.json'))
+                    save_data([a.tolist() for a in c.coords], os.path.join(self.analysis_dir, f'coords{weight_str}', f'coords_{index[idx]}.json'))
             if save_control_points:
                 if not os.path.exists(os.path.join(self.analysis_dir, f'control_points{weight_str}')):
                     os.mkdir(os.path.join(self.analysis_dir, f'control_points{weight_str}'))
                 for idx, c in enumerate(population.population):
-                    save_data(c.control_points, os.path.join(self.analysis_dir,
+                    control_points = [[curve.point_sequence().as_array().tolist() for curve in a.curves] for a in c.mea.airfoils]
+                    save_data(control_points, os.path.join(self.analysis_dir,
                                                              f'control_points{weight_str}', f'control_points_{index[idx]}.json'))
             if save_airfoil_state:
-                if not os.path.exists(os.path.join(self.analysis_dir, f'airfoil_state{weight_str}')):
-                    os.mkdir(os.path.join(self.analysis_dir, f'airfoil_state{weight_str}'))
-                for idx, c in enumerate(population.population):
-                    save_data(c.airfoil_state, os.path.join(self.analysis_dir,
-                                                            f'airfoil_state{weight_str}', f'airfoil_state_{index[idx]}.json'))
-
-            if evaluate:
-                population.eval_pop_fitness()
-                population_forces = {k: [c.forces[k] for c in population.population]
-                                     for k in population.population[0].forces.keys()}
-                post_process_file_split = os.path.splitext(self.post_process_force_file)
-                save_data(population_forces, post_process_file_split[0] + weight_str + post_process_file_split[1])
+                # if not os.path.exists(os.path.join(self.analysis_dir, f'airfoil_state{weight_str}')):
+                #     os.mkdir(os.path.join(self.analysis_dir, f'airfoil_state{weight_str}'))
+                # for idx, c in enumerate(population.population):
+                #     save_data(c.airfoil_state, os.path.join(self.analysis_dir,
+                #                                             f'airfoil_state{weight_str}', f'airfoil_state_{index[idx]}.json'))
+                pass
 
     def generate_objective_function_plot(self, index: int or typing.Iterable = None):
         obj_fun_label_dict = {
             0: r"$J_P$",
             1: r"$J_F$"
         }
         save_name_dict = {
@@ -362,22 +373,25 @@
                     "w0-100": f"POP{self.pop_size}L",
                     "w50-50": f"POP{self.pop_size}M",
                     "w100-0": f"POP{self.pop_size}R"
                 }
                 label = label_dict[label]
 
                 # Determine what ydata to plot
+                xdata = np.arange(F.shape[0])
                 ydata = F[:, obj_fun_idx]
+                xdata = np.delete(xdata, np.argwhere(ydata == 1.0e9))
+                ydata = np.delete(ydata, np.argwhere(ydata == 1.0e9))
 
-                # Plot the ydata
-                axs.plot(ydata, label=label)
+                # Plot the data
+                axs.plot(xdata, ydata, label=label)
 
             fig.set_tight_layout('tight')
-            if obj_fun_idx == 0 and self.pop_size == 150:
-                axs.set_ylim([0.165, 0.235])
+            # if obj_fun_idx == 0 and self.pop_size == 150:
+            #     axs.set_ylim([0.165, 0.235])
             axs.set_xlabel("Generation", fontdict=font)
             axs.set_ylabel(obj_fun_label_dict[obj_fun_idx], fontdict=font)
             axs.grid("on", ls=":")
             if self.weights.shape[0] > 1:
                 legend_font_dict = {k: v for k, v in font.items() if k != "color"}
                 axs.legend(prop=legend_font_dict)
             format_axis_scientific(axs)
@@ -465,15 +479,16 @@
             axs.grid("on", ls=":")
             if self.weights.shape[0] > 1:
                 legend_font_dict = {k: v for k, v in font.items() if k != "color"}
                 axs.legend(prop=legend_font_dict)
             format_axis_scientific(axs)
             show_save_fig(fig, save_base_dir=self.image_dir, file_name_stub=f'design_{v}')
 
-    def pareto_front(self, opt_start: int = 5, opt_end: int = None, opt_num: int = 10):
+    def pareto_front(self, main_axes_xy_lim: typing.List, inset_axes_xy_lim: typing.List, axes_location: typing.List,
+                     opt_start: int = 5, opt_end: int = None, opt_num: int = 10):
 
         fig, axs = plt.subplots(figsize=(8, 4.8))
 
         def generate_plots(ax: plt.Axes, opt_end_):
             index = self.set_index(None)
             if opt_end_ is None:
                 opt_end_ = index[-1]
@@ -516,36 +531,38 @@
                     else:
                         extra_kwargs = {}
                         if not opt_labeled:
                             extra_kwargs["label"] = "Optimal"
                             opt_labeled = True
                         ax.plot(F[:, 0], F[:, 1], **gray_circle_kwargs, **extra_kwargs)
             # ax.set_xlim([0.058, 0.19])  # FOR POP50 input ga_opt_70
-            ax.set_xlim([0.17, 0.26])  # FOR POP50 consumption ga_opt_93
+            ax.set_xlim(main_axes_xy_lim[:2])  # FOR POP50 consumption ga_opt_93
+            ax.set_ylim(main_axes_xy_lim[2:])
             # ax.set_xlim([0.17, 0.26])  # FOR POP150 consumption ga_opt_92
             ax.set_xlabel(r"$J_P$", fontdict=font)
             ax.set_ylabel(r"$J_F$", fontdict=font)
             format_axis_scientific(ax)
 
         generate_plots(axs, opt_end)
         legend_font_dict = {k: v for k, v in font.items() if k != "color"}
         legend_font_dict["size"] = 12
         axs.legend(prop=legend_font_dict, loc="upper right", ncol=1)
 
-        axs_inset = axs.inset_axes([0.17, 0.53, 0.35, 0.4])
+        axs_inset = axs.inset_axes(axes_location)
         generate_plots(axs_inset, opt_end)
-        x1, x2, y1, y2 = 0.17, 0.20, 0.012, 0.014
+        x1, x2, y1, y2 = inset_axes_xy_lim[0], inset_axes_xy_lim[1], inset_axes_xy_lim[2], inset_axes_xy_lim[3]
         axs_inset.set_xlim(x1, x2)
         axs_inset.set_ylim(y1, y2)
         # x_labels = [item if idx % 2 else "" for idx, item in enumerate(axs_inset.get_xticklabels())]
         # y_labels = [item if not idx % 2 else "" for idx, item in enumerate(axs_inset.get_yticklabels())]
         # axs_inset.set_xticklabels(x_labels)
         # axs_inset.set_yticklabels(y_labels)
         axs_inset.xaxis.set_major_locator(mticker.MaxNLocator(2))
         axs_inset.yaxis.set_major_locator(mticker.MaxNLocator(2, prune="lower"))
+        axs_inset.set_zorder(100)
 
         show_save_fig(fig, save_base_dir=self.image_dir, file_name_stub="pareto_front")
 
     def compare_geometries(self, index: list, plot_actuator_disk: bool = True,
                            rotate_x_axis_wind_direction: bool = False, rotate_zero_alf: bool = False):
         for weight_idx, weights in enumerate(self.weights):
             weight_str = self.get_weight_str(weight_idx)
@@ -726,17 +743,17 @@
             show_save_fig(fig, save_base_dir=self.image_dir, file_name_stub=f_name[i])
 
     def generate_BL_plot(self, var: str or typing.Iterable = None, index: int or typing.Iterable = None,
                          mode: str = 'standalone', legend_strs: tuple = ('upper', 'lower')):
 
         save_filetypes = ['.svg', '.pdf']
         pai_props = {
-            0: dict(title='Main', xlim=[-0.1, 1.1], xlabel=r'$x/c_{main}$', ylabel=bl_matplotlib_labels[var]),
-            1: dict(title='Hub', xlim=[0.75, 1.4], xlabel=r'$x/c_{main}$', ylabel=''),
-            2: dict(title='Nacelle', xlim=[0.65, 1.1], xlabel=r'$x/c_{main}$', ylabel='')
+            0: dict(title='Main', xlim=[-0.1, 1.1], ylim=[2.2, -1.6], xlabel=r'$x/c_{main}$', ylabel=bl_matplotlib_labels[var]),
+            1: dict(title='Hub', xlim=[0.75, 1.4], ylim=[2.2, -1.6], xlabel=r'$x/c_{main}$', ylabel=''),
+            2: dict(title='Nacelle', xlim=[0.55, 1.1], ylim=[2.2, -1.6], xlabel=r'$x/c_{main}$', ylabel='')
         }
 
         valid_modes = ['compare', 'standalone']
         if mode not in valid_modes:
             raise ValueError(f"mode must be one of {valid_modes}")
         index = self.set_index(index)
         if isinstance(index, int):
@@ -770,14 +787,15 @@
                             target_axs = int(side / 2)
                         else:
                             target_axs = 2 - int(side / 2)
                         axs[target_axs].plot(BL_data[i][side]['x'], BL_data[i][side][v], color=color,
                                              ls=line_styles[side % 2])
                     for k, v_ in pai_props.items():
                         axs[k].set_xlim(v_["xlim"])
+                        axs[k].set_ylim(v_["ylim"])
                         axs[k].set_title(v_["title"], fontdict=font)
                         axs[k].set_xlabel(v_["xlabel"], fontdict=font)
                         axs[k].set_ylabel(v_["ylabel"], fontdict=font)
                         if v == "Cp":
                             axs[k].set_yticks([-1, 0, 1])
                         axs[k].grid('on', ls=':')
                     for k in range(3):
```

### Comparing `pymead-2.0.0b3/pymead/resources/cmcrameri/LICENSE.txt` & `pymead-2.0.0b4/pymead/resources/cmcrameri/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/cmcrameri/berlin.txt` & `pymead-2.0.0b4/pymead/resources/cmcrameri/berlin.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/cmcrameri/vik.txt` & `pymead-2.0.0b4/pymead/resources/cmcrameri/vik.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/AUTHORS` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/AUTHORS`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/LICENSE` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/LICENSE`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/NEWS` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/NEWS`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/README.md` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/README.md`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans-mono.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans-mono.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-sans.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-serif.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/20-unhint-small-dejavu-serif.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans-mono.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans-mono.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-sans.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-serif.conf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/fontconfig/57-dejavu-serif.conf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/langcover.txt` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/langcover.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/status.txt` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/status.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuMathTeXGyre.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuMathTeXGyre.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Bold.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-BoldOblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-ExtraLight.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Oblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Bold.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-BoldOblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Oblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Bold.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-BoldOblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Oblique.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Bold.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-BoldItalic.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Italic.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Bold.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-BoldItalic.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Italic.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed.ttf` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed.ttf`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/dejavu-fonts-ttf-2.37/unicover.txt` & `pymead-2.0.0b4/pymead/resources/dejavu-fonts-ttf-2.37/unicover.txt`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/resources/grid_test.pdf` & `pymead-2.0.0b4/pymead/resources/grid_test.pdf`

 * *Files 14% similar despite different names*

#### Comparing `pymead-2.0.0b3/pymead/resources/grid_test.pdf` & `pymead-2.0.0b4/pymead/resources/grid_test.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240222174352-06'00'"
-ModDate: "D:20240222174352-06'00'"
+CreationDate: "D:20240424110637-05'00'"
+ModDate: "D:20240424110637-05'00'"
 Producer: 'GPL Ghostscript 9.56.1'
```

### Comparing `pymead-2.0.0b3/pymead/tests/run_all_tests.py` & `pymead-2.0.0b4/pymead/tests/run_all_tests.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/airfoil_matching.py` & `pymead-2.0.0b4/pymead/utils/airfoil_matching.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/dict_recursion.py` & `pymead-2.0.0b4/pymead/utils/dict_recursion.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/downsampling_schemes.py` & `pymead-2.0.0b4/pymead/utils/downsampling_schemes.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/file_conversion.py` & `pymead-2.0.0b4/pymead/utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/geometry.py` & `pymead-2.0.0b4/pymead/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/get_airfoil.py` & `pymead-2.0.0b4/pymead/utils/get_airfoil.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,33 @@
     ### Returns:
 
     The set of xy-coordinates of type `numpy.ndarray` with `shape=(N,2)`, where `N` is the number of airfoil coordinates
     and the columns represent `x` and `y`
     """
     url = f'http://airfoiltools.com/airfoil/seligdatfile?airfoil={name}'
     data = requests.get(url)
+    if data.status_code == 404:
+        raise AirfoilNotFoundError(f"Airfoil {name} not found at http://airfoiltools.com/")
     text = deepcopy(data.text)
     coords_str = text.split('\n')
     xy_str_list = [coord_str.split() for coord_str in coords_str]
     xy_list = []
     for xy_str in xy_str_list[1:-1]:
         xy = [float(xy_str[0]), float(xy_str[1])]
         xy_list.append(xy)
     xy = np.array(xy_list)
     if repair is not None:
         xy = repair(xy)
     return xy
 
 
+class AirfoilNotFoundError(Exception):
+    pass
+
+
 def main():
     """
     ### Description:
 
     Example usage of `extract_data_from_airfoiltools`: download the `NACA 0012` airfoil and
     plot
     """
```

### Comparing `pymead-2.0.0b3/pymead/utils/increment_string_index.py` & `pymead-2.0.0b4/pymead/utils/increment_string_index.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/misc.py` & `pymead-2.0.0b4/pymead/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/pymead_mp.py` & `pymead-2.0.0b4/pymead/utils/pymead_mp.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import psutil
 
 
 def kill_child_processes(parent_pid: int, sig: int = signal.SIGTERM):
     """
     Kills all child processes (using ``SIGTERM``) of a process with a given PID.
-    All code in the function body is directly pulled from
-    `this StackOverflow answer <https://stackoverflow.com/a/17112379>`_
+    Most code is from `this StackOverflow answer <https://stackoverflow.com/a/17112379>`_.
 
     Parameters
     ----------
     parent_pid: int
         Process ID of the parent
 
     sig: int
@@ -27,7 +26,16 @@
         return
     children = parent.children(recursive=True)
     for process in children:
         try:
             process.send_signal(sig)
         except psutil.NoSuchProcess:
             continue
+
+    # In the rare case that an instance of XFOIL or MSES does not get shut down, force-close any processes with those
+    # names
+    for proc in psutil.process_iter():
+        if proc.name() in ["xfoil.exe", "mses.exe", "xfoil", "mses"]:
+            try:
+                proc.send_signal(sig)
+            except psutil.NoSuchProcess:
+                continue
```

### Comparing `pymead-2.0.0b3/pymead/utils/read_write_files.py` & `pymead-2.0.0b4/pymead/utils/read_write_files.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/transformations.py` & `pymead-2.0.0b4/pymead/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead/utils/version_check.py` & `pymead-2.0.0b4/pymead/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `pymead-2.0.0b3/pymead.egg-info/PKG-INFO` & `pymead-2.0.0b4/pymead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymead
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Python library for generation, aerodynamic analysis, and aerodynamic shape optimization of parametric airfoils and airfoil systems
 Home-page: https://github.com/mlau154/pymead
 Author: Matthew G Lauer
 Author-email: mlauer2015@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymead-2.0.0b3/pymead.egg-info/SOURCES.txt` & `pymead-2.0.0b4/pymead.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 pymead/core/constraint_equations.py
 pymead/core/constraints.py
 pymead/core/gcs.py
 pymead/core/geometry_collection.py
 pymead/core/line.py
 pymead/core/mea.py
 pymead/core/param.py
+pymead/core/param_graph.py
 pymead/core/parametric_curve.py
 pymead/core/point.py
 pymead/core/pymead_obj.py
 pymead/core/spline.py
 pymead/core/transformation.py
 pymead/core/units.py
 pymead/data/__init__.py
@@ -49,22 +50,22 @@
 pymead/gui/autocomplete.py
 pymead/gui/bounds_values_table.py
 pymead/gui/concurrency.py
 pymead/gui/constraint_items.py
 pymead/gui/custom_context_menu_event.py
 pymead/gui/custom_graphics_view.py
 pymead/gui/default_settings.py
+pymead/gui/dialogs.py
 pymead/gui/dockable_tab_widget.py
 pymead/gui/draggable_point.py
 pymead/gui/file_selection.py
 pymead/gui/gui.py
 pymead/gui/help_browser.py
 pymead/gui/hoverable_curve.py
 pymead/gui/infty_doublespinbox.py
-pymead/gui/input_dialog.py
 pymead/gui/main_icon_toolbar.py
 pymead/gui/message_box.py
 pymead/gui/opt_airfoil_graph.py
 pymead/gui/parallel_coords_graph.py
 pymead/gui/parameter_tree.py
 pymead/gui/permanent_widget.py
 pymead/gui/polygon_item.py
@@ -108,15 +109,14 @@
 pymead/post/plot_formatters.py
 pymead/post/post_process.py
 pymead/resources/__init__.py
 pymead/resources/cmcrameri/__init__.py
 pymead/resources/cmcrameri/cmaps.py
 pymead/tests/__init__.py
 pymead/tests/run_all_tests.py
-pymead/tests/update_MEA.py
 pymead/utils/__init__.py
 pymead/utils/airfoil_matching.py
 pymead/utils/dict_recursion.py
 pymead/utils/downsampling_schemes.py
 pymead/utils/file_conversion.py
 pymead/utils/geometry.py
 pymead/utils/get_airfoil.py
@@ -141,14 +141,15 @@
 pymead/core/constraint_equations.py
 pymead/core/constraints.py
 pymead/core/gcs.py
 pymead/core/geometry_collection.py
 pymead/core/line.py
 pymead/core/mea.py
 pymead/core/param.py
+pymead/core/param_graph.py
 pymead/core/parametric_curve.py
 pymead/core/point.py
 pymead/core/pymead_obj.py
 pymead/core/spline.py
 pymead/core/transformation.py
 pymead/core/units.py
 pymead/data/__init__.py
@@ -169,22 +170,22 @@
 pymead/gui/autocomplete.py
 pymead/gui/bounds_values_table.py
 pymead/gui/concurrency.py
 pymead/gui/constraint_items.py
 pymead/gui/custom_context_menu_event.py
 pymead/gui/custom_graphics_view.py
 pymead/gui/default_settings.py
+pymead/gui/dialogs.py
 pymead/gui/dockable_tab_widget.py
 pymead/gui/draggable_point.py
 pymead/gui/file_selection.py
 pymead/gui/gui.py
 pymead/gui/help_browser.py
 pymead/gui/hoverable_curve.py
 pymead/gui/infty_doublespinbox.py
-pymead/gui/input_dialog.py
 pymead/gui/main_icon_toolbar.py
 pymead/gui/message_box.py
 pymead/gui/opt_airfoil_graph.py
 pymead/gui/parallel_coords_graph.py
 pymead/gui/parameter_tree.py
 pymead/gui/permanent_widget.py
 pymead/gui/polygon_item.py
@@ -260,14 +261,15 @@
 pymead/icons/opened-arrow-light.png
 pymead/icons/perp3_constraint_dark.svg
 pymead/icons/perp3_constraint_light.svg
 pymead/icons/point_dark.svg
 pymead/icons/point_light.svg
 pymead/icons/pymead-logo.png
 pymead/icons/pymead-logo_old.png
+pymead/icons/pymead-splash.png
 pymead/icons/rel_angle_constraint_dark.svg
 pymead/icons/rel_angle_constraint_light.svg
 pymead/icons/reload.png
 pymead/icons/roc_constraint_dark.svg
 pymead/icons/roc_constraint_light.svg
 pymead/icons/stop.png
 pymead/icons/symmetry_constraint_dark.svg
@@ -342,15 +344,18 @@
 pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerif.ttf
 pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Bold.ttf
 pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-BoldItalic.ttf
 pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed-Italic.ttf
 pymead/resources/dejavu-fonts-ttf-2.37/ttf/DejaVuSerifCondensed.ttf
 pymead/tests/__init__.py
 pymead/tests/run_all_tests.py
-pymead/tests/update_MEA.py
+pymead/tests/core_tests/baseline_joa_complete.jmea
+pymead/tests/core_tests/connected_angles.jmea
+pymead/tests/core_tests/double_angle.jmea
+pymead/tests/core_tests/mirror_ap3_constraint.jmea
 pymead/utils/__init__.py
 pymead/utils/airfoil_matching.py
 pymead/utils/dict_recursion.py
 pymead/utils/downsampling_schemes.py
 pymead/utils/file_conversion.py
 pymead/utils/geometry.py
 pymead/utils/get_airfoil.py
```

### Comparing `pymead-2.0.0b3/setup.py` & `pymead-2.0.0b4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,27 +26,61 @@
     author="Matthew G Lauer",
     author_email="mlauer2015@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
-    package_data={"pymead": ["gui/gui_settings/defaults/*.json", "icons/*.png", "icons/*.svg",
-                             "resources/*", "resources/dejavu-fonts-ttf-2.37/*",
-                             "resources/dejavu-fonts-ttf-2.37/fontconfig/*", "resources/dejavu-fonts-ttf-2.37/ttf/*",
-                             "resources/cmcrameri/*",
-                             "gui/*.json", "gui/gui_settings/themes/*.json", "gui/gui_settings/*.json",
-                             "gui/dialog_widgets/*.json"]},
+    package_data={"pymead": [
+        "gui/gui_settings/defaults/*.json",
+        "icons/*.png",
+        "icons/*.svg",
+        "resources/*",
+        "resources/dejavu-fonts-ttf-2.37/*",
+        "resources/dejavu-fonts-ttf-2.37/fontconfig/*",
+        "resources/dejavu-fonts-ttf-2.37/ttf/*",
+        "resources/cmcrameri/*",
+        "gui/*.json",
+        "gui/gui_settings/themes/*.json",
+        "gui/gui_settings/*.json",
+        "gui/dialog_widgets/*.json",
+        "tests/core_tests/*.jmea"
+    ]},
     python_requires=">=3.10",
-    packages=["pymead", "pymead/core", "pymead/examples", "pymead/utils", "pymead/gui",
-              "pymead/tests", "pymead/resources", "pymead/resources/cmcrameri", "pymead/analysis", "pymead/data",
-              "pymead/icons",
-              "pymead/optimization", "pymead/plugins", "pymead/plugins/IGES", "pymead/plugins/NX",
-              "pymead/post", "pymead/gui/scientificspinbox_master",
-              "pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget"],
+    packages=[
+        "pymead",
+        "pymead/core",
+        "pymead/examples",
+        "pymead/utils",
+        "pymead/gui",
+        "pymead/tests",
+        "pymead/resources",
+        "pymead/resources/cmcrameri",
+        "pymead/analysis",
+        "pymead/data",
+        "pymead/icons",
+        "pymead/optimization",
+        "pymead/plugins",
+        "pymead/plugins/IGES",
+        "pymead/plugins/NX",
+        "pymead/post",
+        "pymead/gui/scientificspinbox_master",
+        "pymead/gui/pyqt_vertical_tab_widget/pyqt_vertical_tab_widget"
+    ],
     include_package_data=True,
-    install_requires=["scipy", "numpy", "shapely", "matplotlib", "requests>=2.31", "PyQt5==5.15.7",
-                      "pyqtgraph==0.13.1", "python-benedict", "pandas", "pymoo==0.5.0", "numba", "PyQtWebEngine",
-                      "networkx", "psutil"],
+    install_requires=[
+        "scipy",
+        "numpy",
+        "shapely",
+        "matplotlib",
+        "requests>=2.31",
+        "PyQt5==5.15.7",
+        "pyqtgraph==0.13.1",
+        "python-benedict",
+        "pandas",
+        "pymoo==0.5.0",
+        "numba",
+        "PyQtWebEngine",
+        "networkx",
+        "psutil"
+    ],
 )
-
-# TODO: fix relative file-pathing (like "menu.json") when calling the GUI main directly from a Python interpreter after
```

