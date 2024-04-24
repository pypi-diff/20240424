# Comparing `tmp/control-lab-ly-1.3.1.tar.gz` & `tmp/control_lab_ly-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.3.1.tar", last modified: Thu Apr 11 09:12:18 2024, max compression
+gzip compressed data, was "control_lab_ly-1.3.2.tar", last modified: Wed Apr 24 03:54:35 2024, max compression
```

## Comparing `control-lab-ly-1.3.1.tar` & `control_lab_ly-1.3.2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.646182 control-lab-ly-1.3.1/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.1/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    26329 2024-04-11 09:12:18.645682 control-lab-ly-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.300680 control-lab-ly-1.3.1/docs/
--rw-rw-rw-   0        0        0    11700 2024-04-11 09:06:45.000000 control-lab-ly-1.3.1/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.3.1/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.3.1/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13173 2024-02-16 02:53:34.000000 control-lab-ly-1.3.1/docs/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.302433 control-lab-ly-1.3.1/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.3.1/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1499 2024-04-11 09:12:18.651222 control-lab-ly-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.158280 control-lab-ly-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.642682 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    26329 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7183 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 09:12:18.000000 control-lab-ly-1.3.1/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.319774 control-lab-ly-1.3.1/src/controllably/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.323275 control-lab-ly-1.3.1/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.326854 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/
--rw-rw-rw-   0        0        0      261 2023-07-31 07:45:25.000000 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/__init__.py
--rw-rw-rw-   0        0        0     6299 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/forceclamper_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.333628 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.337128 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    18427 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control-lab-ly-1.3.1/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.338628 control-lab-ly-1.3.1/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.349834 control-lab-ly-1.3.1/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.359846 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-10-29 17:05:20.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16511 2023-08-08 14:17:29.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     4019 2024-02-07 03:02:59.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.373850 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14719 2023-09-05 05:32:23.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.3.1/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.377350 control-lab-ly-1.3.1/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.383371 control-lab-ly-1.3.1/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11341 2024-04-09 07:38:31.000000 control-lab-ly-1.3.1/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.387888 control-lab-ly-1.3.1/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9920 2023-07-25 02:35:05.000000 control-lab-ly-1.3.1/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.389387 control-lab-ly-1.3.1/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.393415 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.402341 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.405441 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-07-12 03:09:07.000000 control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4136 2024-01-10 14:43:02.000000 control-lab-ly-1.3.1/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.414122 control-lab-ly-1.3.1/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.417882 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.421215 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/
--rw-rw-rw-   0        0        0      259 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/__init__.py
--rw-rw-rw-   0        0        0     7175 2024-02-16 02:09:56.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py
--rw-rw-rw-   0        0        0        0 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Chemical/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.425408 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.436102 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      377 2023-11-21 07:02:23.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    23227 2024-04-05 09:10:59.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2175 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.439660 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      302 2023-11-22 02:06:57.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    17922 2024-04-11 05:01:17.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.445196 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.454651 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10789 2023-08-29 02:36:35.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.458678 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3549 2023-10-12 08:34:58.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0      247 2023-08-10 08:59:40.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0     8576 2023-08-29 02:54:55.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/load_cell_utils.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.467193 control-lab-ly-1.3.1/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      258 2023-08-11 05:01:25.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     9941 2023-08-11 05:02:02.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8206 2023-07-31 02:56:41.000000 control-lab-ly-1.3.1/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14577 2023-08-14 02:29:33.000000 control-lab-ly-1.3.1/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.470192 control-lab-ly-1.3.1/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.479062 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      360 2024-01-03 07:23:50.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0    14600 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0    11446 2024-04-11 06:29:22.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     9678 2024-01-03 09:37:19.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/grbl_lib.py
--rw-rw-rw-   0        0        0     9224 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.486156 control-lab-ly-1.3.1/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.494191 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.500265 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24212 2023-08-08 13:17:57.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    18542 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0    10073 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     6199 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    12736 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    37565 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.503765 control-lab-ly-1.3.1/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.510950 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.519380 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.524337 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    30840 2024-02-20 08:20:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.530024 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    32219 2023-11-08 05:13:56.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3457 2023-08-03 05:19:47.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.534395 control-lab-ly-1.3.1/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.537394 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.541395 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8815 2024-02-07 03:03:00.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.3.1/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.552235 control-lab-ly-1.3.1/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.557030 control-lab-ly-1.3.1/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.560561 control-lab-ly-1.3.1/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2024-01-29 16:02:35.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.566583 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.572714 control-lab-ly-1.3.1/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.584412 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0      224 2023-07-28 03:13:38.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-08-10 02:38:36.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_lib.py
--rw-rw-rw-   0        0        0    17276 2024-01-29 16:02:57.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_utils.py
--rw-rw-rw-   0        0        0      225 2023-08-08 11:08:14.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.591730 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     3128 2023-08-08 11:07:54.000000 control-lab-ly-1.3.1/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2024-01-29 15:34:00.000000 control-lab-ly-1.3.1/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    17271 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.613029 control-lab-ly-1.3.1/src/controllably/misc/
--rw-rw-rw-   0        0        0      661 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9550 2024-01-04 15:54:27.000000 control-lab-ly-1.3.1/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     8551 2024-01-12 10:16:16.000000 control-lab-ly-1.3.1/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    24907 2024-02-20 10:17:37.000000 control-lab-ly-1.3.1/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.3.1/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     5480 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.619494 control-lab-ly-1.3.1/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.621494 control-lab-ly-1.3.1/src/controllably/misc/templates/library/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.625055 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/my_plugin.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.631471 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.638640 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/
--rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/__init__.py
--rw-rw-rw-   0        0        0      439 2024-02-16 02:09:43.000000 control-lab-ly-1.3.1/src/controllably/misc/templates/tools/registry.yaml
-drwxrwxrwx   0        0        0        0 2024-04-11 09:12:18.640647 control-lab-ly-1.3.1/tests/
--rw-rw-rw-   0        0        0      363 2023-07-20 03:51:29.000000 control-lab-ly-1.3.1/tests/test_init.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.571101 control_lab_ly-1.3.2/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control_lab_ly-1.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    26637 2024-04-24 03:54:35.570601 control_lab_ly-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.189234 control_lab_ly-1.3.2/docs/
+-rw-rw-rw-   0        0        0    12008 2024-04-24 03:52:50.000000 control_lab_ly-1.3.2/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control_lab_ly-1.3.2/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control_lab_ly-1.3.2/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13173 2024-02-16 02:53:34.000000 control_lab_ly-1.3.2/docs/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.190772 control_lab_ly-1.3.2/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control_lab_ly-1.3.2/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1499 2024-04-24 03:54:35.573159 control_lab_ly-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control_lab_ly-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.123779 control_lab_ly-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.567186 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    26637 2024-04-24 03:54:34.000000 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7183 2024-04-24 03:54:35.000000 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:54:34.000000 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-24 03:54:34.000000 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 03:54:34.000000 control_lab_ly-1.3.2/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.204961 control_lab_ly-1.3.2/src/controllably/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.208413 control_lab_ly-1.3.2/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.210913 control_lab_ly-1.3.2/src/controllably/Compound/ForceClamper/
+-rw-rw-rw-   0        0        0      261 2023-07-31 07:45:25.000000 control_lab_ly-1.3.2/src/controllably/Compound/ForceClamper/__init__.py
+-rw-rw-rw-   0        0        0     6299 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Compound/ForceClamper/forceclamper_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.214558 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.219239 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    18427 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8214 2023-07-03 06:35:57.000000 control_lab_ly-1.3.2/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.221128 control_lab_ly-1.3.2/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.228149 control_lab_ly-1.3.2/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.252964 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-10-29 17:05:20.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16511 2023-08-08 14:17:29.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     4019 2024-02-07 03:02:59.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.261042 control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14719 2023-09-05 05:32:23.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control_lab_ly-1.3.2/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.264151 control_lab_ly-1.3.2/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.268602 control_lab_ly-1.3.2/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11309 2024-04-12 07:42:12.000000 control_lab_ly-1.3.2/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.273011 control_lab_ly-1.3.2/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9920 2023-07-25 02:35:05.000000 control_lab_ly-1.3.2/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.274688 control_lab_ly-1.3.2/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.277839 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.284302 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.289944 control_lab_ly-1.3.2/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    11489 2023-07-12 03:09:07.000000 control_lab_ly-1.3.2/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4136 2024-01-10 14:43:02.000000 control_lab_ly-1.3.2/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.302462 control_lab_ly-1.3.2/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.306779 control_lab_ly-1.3.2/src/controllably/Measure/Chemical/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.310555 control_lab_ly-1.3.2/src/controllably/Measure/Chemical/Sentron/
+-rw-rw-rw-   0        0        0      259 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/Chemical/Sentron/__init__.py
+-rw-rw-rw-   0        0        0     7175 2024-02-16 02:09:56.000000 control_lab_ly-1.3.2/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/Chemical/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.315554 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.326544 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      377 2023-11-21 07:02:23.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    23328 2024-04-24 02:29:29.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7458 2024-04-24 02:40:51.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2175 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.329620 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      302 2023-11-22 02:06:57.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    18066 2024-04-24 02:40:37.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.337225 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.342844 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10789 2023-08-29 02:36:35.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.347910 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3549 2023-10-12 08:34:58.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0      247 2023-08-10 08:59:40.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0     8576 2023-08-29 02:54:55.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/load_cell_utils.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.357909 control_lab_ly-1.3.2/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      303 2024-04-12 07:51:23.000000 control_lab_ly-1.3.2/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     9941 2023-08-11 05:02:02.000000 control_lab_ly-1.3.2/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8210 2024-04-12 08:12:34.000000 control_lab_ly-1.3.2/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2024-04-24 02:44:49.000000 control_lab_ly-1.3.2/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14577 2023-08-14 02:29:33.000000 control_lab_ly-1.3.2/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.361909 control_lab_ly-1.3.2/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.380668 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      360 2024-01-03 07:23:50.000000 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0    14600 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0    11446 2024-04-11 06:29:22.000000 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     9678 2024-01-03 09:37:19.000000 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/grbl_lib.py
+-rw-rw-rw-   0        0        0     9224 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.383379 control_lab_ly-1.3.2/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.392231 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.395733 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24212 2023-08-08 13:17:57.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    18542 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0    10073 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     6199 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    12736 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    37565 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.406407 control_lab_ly-1.3.2/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.412682 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.417180 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.427580 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    30840 2024-02-20 08:20:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.432257 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    32219 2023-11-08 05:13:56.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3457 2023-08-03 05:19:47.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.436907 control_lab_ly-1.3.2/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.455231 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.458843 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8815 2024-02-07 03:03:00.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control_lab_ly-1.3.2/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.467208 control_lab_ly-1.3.2/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.473087 control_lab_ly-1.3.2/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.475687 control_lab_ly-1.3.2/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2024-01-29 16:02:35.000000 control_lab_ly-1.3.2/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.478529 control_lab_ly-1.3.2/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control_lab_ly-1.3.2/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.502470 control_lab_ly-1.3.2/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.511515 control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0      224 2023-07-28 03:13:38.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-08-10 02:38:36.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/ax8_lib.py
+-rw-rw-rw-   0        0        0    17276 2024-01-29 16:02:57.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/ax8_utils.py
+-rw-rw-rw-   0        0        0      225 2023-08-08 11:08:14.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.514234 control_lab_ly-1.3.2/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     3128 2023-08-08 11:07:54.000000 control_lab_ly-1.3.2/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2024-01-29 15:34:00.000000 control_lab_ly-1.3.2/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    17271 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.541509 control_lab_ly-1.3.2/src/controllably/misc/
+-rw-rw-rw-   0        0        0      661 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9550 2024-01-04 15:54:27.000000 control_lab_ly-1.3.2/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     8551 2024-01-12 10:16:16.000000 control_lab_ly-1.3.2/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    24907 2024-02-20 10:17:37.000000 control_lab_ly-1.3.2/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control_lab_ly-1.3.2/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     5480 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.543008 control_lab_ly-1.3.2/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.544213 control_lab_ly-1.3.2/src/controllably/misc/templates/library/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.548550 control_lab_ly-1.3.2/src/controllably/misc/templates/library/plugins/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/library/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/library/plugins/my_plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.558643 control_lab_ly-1.3.2/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.562893 control_lab_ly-1.3.2/src/controllably/misc/templates/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/tools/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-02-16 02:09:43.000000 control_lab_ly-1.3.2/src/controllably/misc/templates/tools/registry.yaml
+drwxrwxrwx   0        0        0        0 2024-04-24 03:54:35.564629 control_lab_ly-1.3.2/tests/
+-rw-rw-rw-   0        0        0      363 2023-07-20 03:51:29.000000 control_lab_ly-1.3.2/tests/test_init.py
```

### Comparing `control-lab-ly-1.3.1/LICENSE.md` & `control_lab_ly-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/PKG-INFO` & `control_lab_ly-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.3.1
+Version: 1.3.2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -369,20 +369,28 @@
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
+## Version 1.3.2
+Feature enhancements, bug fixes and patches. First released 24 Apr 2024.
+### Added
+- add new `delay` parameter in `Keithley.programs.IV_Scan`
+### Changed
+- fix critical bug in setting sense/source limits for `KeithleyDevice`
+- fix bugs in `KeithleyDevice`, `Peltier`, `ForceSensor`
+
+
 ## Version 1.3.1
-Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+Feature enhancements, bug fixes and patches. First released 11 Apr 2024.
 ### Added
 - implementation of `TriContinent.pullback()`
 - new `Well` properties and option in return list of wells by rows instead of columns
-
 ### Changed
 - fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
 - fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
 - fix bug in `Keithley.setFunction()`
 - generalise `IV_Scan` to take either currents or voltages
```

### Comparing `control-lab-ly-1.3.1/docs/CHANGELOG.md` & `control_lab_ly-1.3.2/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # Change Log
 
+## Version 1.3.2
+Feature enhancements, bug fixes and patches. First released 24 Apr 2024.
+### Added
+- add new `delay` parameter in `Keithley.programs.IV_Scan`
+### Changed
+- fix critical bug in setting sense/source limits for `KeithleyDevice`
+- fix bugs in `KeithleyDevice`, `Peltier`, `ForceSensor`
+
+
 ## Version 1.3.1
-Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+Feature enhancements, bug fixes and patches. First released 11 Apr 2024.
 ### Added
 - implementation of `TriContinent.pullback()`
 - new `Well` properties and option in return list of wells by rows instead of columns
-
 ### Changed
 - fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
 - fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
 - fix bug in `Keithley.setFunction()`
 - generalise `IV_Scan` to take either currents or voltages
```

### Comparing `control-lab-ly-1.3.1/docs/CODE_OF_CONDUCT.md` & `control_lab_ly-1.3.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/docs/LICENSE.md` & `control_lab_ly-1.3.2/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/docs/README.md` & `control_lab_ly-1.3.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/docs/assets/Documentation guide.png` & `control_lab_ly-1.3.2/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/setup.cfg` & `control_lab_ly-1.3.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e33  y..version = 1.3
-00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
+00000030: 2e32 0d0a 6465 7363 7269 7074 696f 6e20  .2..description 
 00000040: 3d20 4c61 6220 4571 7569 706d 656e 7420  = Lab Equipment 
 00000050: 4175 746f 6d61 7469 6f6e 2050 6163 6b61  Automation Packa
 00000060: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2064 6f63  tion = file: doc
 00000080: 732f 5245 4144 4d45 2e6d 642c 2064 6f63  s/README.md, doc
 00000090: 732f 4348 414e 4745 4c4f 472e 6d64 0d0a  s/CHANGELOG.md..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `control-lab-ly-1.3.1/src/control_lab_ly.egg-info/PKG-INFO` & `control_lab_ly-1.3.2/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.3.1
+Version: 1.3.2
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -369,20 +369,28 @@
 
 ## License
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
+## Version 1.3.2
+Feature enhancements, bug fixes and patches. First released 24 Apr 2024.
+### Added
+- add new `delay` parameter in `Keithley.programs.IV_Scan`
+### Changed
+- fix critical bug in setting sense/source limits for `KeithleyDevice`
+- fix bugs in `KeithleyDevice`, `Peltier`, `ForceSensor`
+
+
 ## Version 1.3.1
-Feature enhancements, bug fixes and patches. First released 19 Feb 2024.
+Feature enhancements, bug fixes and patches. First released 11 Apr 2024.
 ### Added
 - implementation of `TriContinent.pullback()`
 - new `Well` properties and option in return list of wells by rows instead of columns
-
 ### Changed
 - fix bugs in `Peltier` (`setTemperature()` and `getTemperature()`)
 - fix bugs in `Ender` (`setTemperature()` and `getTemperature()`)
 - fix bug in `Keithley.setFunction()`
 - generalise `IV_Scan` to take either currents or voltages
```

### Comparing `control-lab-ly-1.3.1/src/control_lab_ly.egg-info/SOURCES.txt` & `control_lab_ly-1.3.2/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Compound/ForceClamper/forceclamper_utils.py` & `control_lab_ly-1.3.2/src/controllably/Compound/ForceClamper/forceclamper_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control_lab_ly-1.3.2/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Compound/compound_utils.py` & `control_lab_ly-1.3.2/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/__init__.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/maker_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/mover_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/loader_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/pop_ups.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/Elements/templates.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/__init__.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/compound_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/gui_utils.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/guide_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Control/GUI/multichannel_panel.py` & `control_lab_ly-1.3.2/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/Heat/peltier_utils.py` & `control_lab_ly-1.3.2/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,14 @@
         else:
             self.device = device
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
             time.sleep(1)
             self.getTemperature()
             print(self.temperature)
-        # self.device = device
         return
     
     def _loop_feedback(self):
         """Loop to constantly read from device"""
         print('Listening...')
         while self.flags['get_feedback']:
             if self.flags['pause_feedback']:
```

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/Light/led_utils.py` & `control_lab_ly-1.3.2/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control_lab_ly-1.3.2/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/ThinFilm/spinner_utils.py` & `control_lab_ly-1.3.2/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Make/make_utils.py` & `control_lab_ly-1.3.2/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Chemical/Sentron/phmeter_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,14 +599,16 @@
         if self.verbose:
             print(command)
         try:
             self.device.write(command)
         except visa.VisaIOError:
             self.getErrors()
             return False
+        except AttributeError:
+            print(f'Not connected to Keithley ({self.ip_address})')
         if self.verbose and "*WAI" not in command:
             # self.getErrors()
             ...
         return True
 
 
 class DAQ6510(KeithleyDevice):
```

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     if type(limit) is str:
         limit = limit.lower()
         choices = ('DEFault', 'MAXimum', 'MINimum')
         for choice in choices:
             if limit in choice.lower():
                 return choice
         raise ValueError(f"Select a valid option from: {', '.join([c.lower() for c in choices])}")
-    unit = 'A' if is_current == 'CURRent' else 'V'
-    options = np.array(CURRENT_LIMITS) if is_current == 'CURRent' else np.array(VOLTAGE_LIMITS)
+    unit = 'A' if is_current else 'V'
+    options = np.array(CURRENT_LIMITS) if is_current else np.array(VOLTAGE_LIMITS)
     shortlist = options[options >= abs(limit)]
     if len(shortlist):
         return shortlist[0]
     print(f'Input limit beyond -{limit} and {limit} {unit}')
     print(f'Defaulting to {options[-1]} {unit}')
     return options[-1]
```

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     
     ### Parameters:
         sense_limit (float, optional): measurement limit. Defaults to 1A or 200V.
         currents (iterable, optional): current values to measure. Defaults to (0,).
         voltages (iterable, optional): voltage values to measure. Defaults to (0,).
         count (int, optional): number of readings to take and average over. Defaults to 1.
         four_point (bool, optional): whether to use four point probe. Defaults to True.
+        delay(float, optional): the time delay between each measurement. Defaults to 0.1.
     """
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
         verbose: bool = False, 
         **kwargs
@@ -92,14 +93,15 @@
         return
     
     def run(self):
         """Run the measurement program"""
         device = self.device
         count = self.parameters.get('count', 1)
         four_point = self.parameters.get('four_point', True)
+        delay = self.parameters.get('delay', 0.1)
         
         if 'voltages' in self.parameters:
             _source = 'voltage'
             _sense = 'current'
             values = self.parameters.get('voltages', (0,))
             limits = VOLTAGE_LIMITS
             sense_limit = CURRENT_LIMITS[-1]
@@ -122,15 +124,15 @@
         device.makeBuffer()
         device.beep()
         
         for value in values:
             device.setSource(value=value)
             device.toggleOutput(on=True)
             device.run()
-            time.sleep(0.1*count)
+            time.sleep(delay*count)
         time.sleep(1)
         self.data_df = device.readAll()
         device.beep()
         device.getErrors()
         return
```

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Mechanical/load_cell_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Mechanical/load_cell_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Physical/balance_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/Physical/force_sensor_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,19 +221,19 @@
         try:
             device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
+            self.device = device
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
             time.sleep(1)
             self.zero()
-        self.device = device
         return
     
     def _loop_feedback(self):
         """Loop to constantly read from device"""
         print('Listening...')
         while self.flags['get_feedback']:
             if self.flags['pause_feedback']:
```

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/__init__.py` & `control_lab_ly-1.3.2/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/instrument_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/measure_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Measure/program_utils.py` & `control_lab_ly-1.3.2/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/cartesian_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/ender_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/grbl_lib.py` & `control_lab_ly-1.3.2/src/controllably/Move/Cartesian/grbl_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Cartesian/primitiv_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/Jointed/jointed_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Move/move_utils.py` & `control_lab_ly-1.3.2/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/liquid_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_lib.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Liquid/syringe_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/Transfer/Substrate/substrate_utils.py` & `control_lab_ly-1.3.2/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Classifiers/classifier_utils.py` & `control_lab_ly-1.3.2/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Optical/optical_utils.py` & `control_lab_ly-1.3.2/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Optical/placeholders/optical_camera.png` & `control_lab_ly-1.3.2/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_lib.py` & `control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/ax8_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Thermal/Flir/ax8_utils.py` & `control_lab_ly-1.3.2/src/controllably/View/Thermal/Flir/ax8_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control_lab_ly-1.3.2/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/Thermal/thermal_utils.py` & `control_lab_ly-1.3.2/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/image.py` & `control_lab_ly-1.3.2/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/View/view_utils.py` & `control_lab_ly-1.3.2/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/__init__.py` & `control_lab_ly-1.3.2/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/decorators.py` & `control_lab_ly-1.3.2/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/factory.py` & `control_lab_ly-1.3.2/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/helper.py` & `control_lab_ly-1.3.2/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/layout.py` & `control_lab_ly-1.3.2/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/logger.py` & `control_lab_ly-1.3.2/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/misc_utils.py` & `control_lab_ly-1.3.2/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/templates/library/plugins/my_plugin.py` & `control_lab_ly-1.3.2/src/controllably/misc/templates/library/plugins/my_plugin.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/__init__.py` & `control_lab_ly-1.3.2/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/config.yaml` & `control_lab_ly-1.3.2/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.3.1/src/controllably/misc/templates/setup/layout.json` & `control_lab_ly-1.3.2/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

