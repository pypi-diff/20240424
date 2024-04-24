# Comparing `tmp/rfb-battery-cycler-0.0.1.tar.gz` & `tmp/rfb_battery_cycler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb-battery-cycler-0.0.1.tar", last modified: Thu Mar 14 07:58:22 2024, max compression
+gzip compressed data, was "rfb_battery_cycler-0.0.2.tar", last modified: Wed Apr 24 06:52:46 2024, max compression
```

## Comparing `rfb-battery-cycler-0.0.1.tar` & `rfb_battery_cycler-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-14 07:58:20.000000 rfb-battery-cycler-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43021 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.753743 rfb-battery-cycler-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.757743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/___version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.753743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.757743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/app_man_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/app_man_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.753743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.757743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    22710 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/mid_dabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.757743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/mid_meas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_pwr/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_pwr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_pwr/mid_pwr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19571 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-03-14 07:57:48.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:58:22.761743 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43021 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 07:58:22.000000 rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.577130 rfb_battery_cycler-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-24 06:52:44.000000 rfb_battery_cycler-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43021 2024-04-24 06:52:46.577130 rfb_battery_cycler-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 06:52:46.577130 rfb_battery_cycler-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.569130 rfb_battery_cycler-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.569130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/___version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.569130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.573130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/app_man_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/app_man_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.569130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.573130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22708 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/mid_dabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.573130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/mid_meas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.573130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_pwr/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_pwr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_pwr/mid_pwr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.573130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19856 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-24 06:52:11.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:52:46.577130 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43021 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 06:52:46.000000 rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/top_level.txt
```

### Comparing `rfb-battery-cycler-0.0.1/LICENSE.txt` & `rfb_battery_cycler-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/PKG-INFO` & `rfb_battery_cycler-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-battery-cycler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Battery cycler control used to execute custom profile on multiple battery technologies.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb-battery-cycler-0.0.1/pyproject.toml` & `rfb_battery_cycler-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/app_man_core.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/app_man_core.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/app_man_node.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/app_man_node.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/app/app_man/context.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/app/app_man/context.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/context.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/context.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_dabs/mid_dabs.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_dabs/mid_dabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
                                             dev_db_id= self._dev_db_id[0])
             res_load: DrvRsDataC = self.load.get_data()
             status.load = CyclerDataDeviceStatusC(error= res_load.status.error_code,
                                             dev_db_id= self._dev_db_id[1])
             log.debug(f"Source mode: {res_source.mode.name}, {res_source.mode.value}")
             log.debug(f"Load mode: {res_load.mode.name}, {res_load.mode.value}")
             if res_source.power >= res_load.power:
-                gen_meas.voltage = res_source.voltage
+                gen_meas.voltage = res_load.voltage
                 gen_meas.current = res_source.current
                 gen_meas.power   = res_source.power
                 status.pwr_mode = CyclerDataPwrModeE(res_source.mode.value)
             else:
                 gen_meas.voltage = res_load.voltage
                 # The current is negative because the load is consuming power
                 gen_meas.current = res_load.current*-1
```

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/context.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/context.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_meas/mid_meas.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_meas/mid_meas.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_pwr/mid_pwr.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_pwr/mid_pwr.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             instructions (List[CyclerDataInstructionC]): [description]
             bat_pwr_range (CyclerDataPwrRangeC): [description]
         """
         self.all_instructions = instructions
         self.actual_inst.instr_id = None
         self.pwr_limits = bat_pwr_range
 
-    def process_iteration(self) -> Tuple[CyclerDataExpStatusE, int]: #pylint: disable= too-many-branches
+    def process_iteration(self) -> Tuple[CyclerDataExpStatusE, int]: #pylint: disable= too-many-branches, too-many-statements
         """Processes a single instruction .
 
         Returns:
             Tuple[CyclerDataExpStatusE, int]: [description]
         """
         status = CyclerDataExpStatusE.QUEUED
         # Check if the security limits are correct
@@ -238,14 +238,15 @@
                             if len(self.all_instructions) > 0:
                                 self.actual_inst = self.all_instructions.pop(0)
                                 self.__apply_instruction()
                                 self.__last_mode = self.actual_inst.mode
                                 status = CyclerDataExpStatusE.RUNNING
                             else:
                                 self.actual_inst.instr_id = None
+                                self.pwr_dev.disable()
                                 self.__last_mode = CyclerDataPwrModeE.DISABLE
                                 status = CyclerDataExpStatusE.FINISHED
                 else:
                     #Check if there are more instructions to read
                     if len(self.all_instructions) > 0:
                         self.actual_inst = self.all_instructions.pop(0)
                         self.__apply_instruction()
@@ -254,14 +255,15 @@
                     else:
                         self.actual_inst.instr_id = None
                         self.pwr_dev.disable()
                         self.__last_mode = CyclerDataPwrModeE.DISABLE
                         status = CyclerDataExpStatusE.FINISHED
         else:
             status = CyclerDataExpStatusE.ERROR
+            self.pwr_dev.disable()
             # TODO: Add alarms callback #pylint: disable= fixme
             self.__alarm_callback(CyclerDataAlarmC(code= 0, value=0))
         return status, self.actual_inst.instr_id
 
     def __instruction_limit(self) -> bool: #pylint: disable=too-many-branches
         """Function to activate the time instruction limits
         """
```

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/context.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/context.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_cmd.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_cmd.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_facade.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,22 @@
         self.all_status: CyclerDataAllStatusC = CyclerDataAllStatusC()
         self.gen_meas: CyclerDataGenMeasC = CyclerDataGenMeasC()
         self.ext_meas: CyclerDataExtMeasC = CyclerDataExtMeasC()
         self.meas_id: int = 0
         self.status_id: int = 0
         self.alarm_id: int = 0
 
+    def check_connection(self) -> None:
+        """Check if the connection to the database is working.
+        Returns:
+            [bool]: [description]
+        """
+        self.__master_db.check_connection()
+        self.__cache_db.check_connection()
+
     def get_start_queued_exp(self) -> Tuple[CyclerDataExperimentC|None, CyclerDataBatteryC|None,
                                             CyclerDataProfileC|None]:
         '''
         Get the oldest queued experiment, assigned to the cycler station where this
         cycler would be running, and change its status to RUNNING in database.
         '''
         self.meas_id = 0
@@ -96,15 +104,15 @@
             battery = self.__get_exp_battery_data(exp_result.BatID)
             # Get profile info
             profile = self.__get_exp_profile_data(exp_result.ProfID)
             # Change experiment status to running and update begin datetime
             exp_db = DrvDbCacheExperimentC()
             transform_experiment_db(source= exp_result, target = exp_db)
             exp_db.Status = DrvDbExpStatusE.RUNNING.value
-            exp_db.DateBegin = datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
+            exp_db.DateBegin = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             self.__cache_db.session.add(exp_db)
             log.debug(f"Experiment fetched: {exp.__dict__}, {battery.__dict__}, {profile.__dict__}")
         else:
             log.debug("No experiment found")
         return exp, battery, profile
 
     ## All methods that get information will gather the info from the master db
@@ -190,15 +198,15 @@
             [bool]: [description]
         """
         ## Get cycler station info
         stmt = select(DrvDbCyclerStationC.Deprecated).where(DrvDbCyclerStationC.CSID == self.cs_id)
         result = self.__master_db.session.execute(stmt).one()[0]
         return result
 
-    def get_cycler_station_info(self) -> CyclerDataCyclerStationC|None: #pylint: disable= too-many-locals
+    def get_cycler_station_info(self) -> CyclerDataCyclerStationC|None: #pylint: disable= too-many-locals, too-many-branches, too-many-statements
         """Returns the name and name of the cycle station for the experiment .
         Returns:
             [CyclerDataCyclerStationC]: [description]
         """
         ## Get cycler station info
         stmt = select(DrvDbCyclerStationC).where(DrvDbCyclerStationC.CSID == self.cs_id)
         result = self.__master_db.session.execute(stmt).one()[0]
@@ -360,16 +368,16 @@
         result = self.__master_db.session.execute(stmt).all()
 
         for exp_result in result:
             exp_result: DrvDbMasterExperimentC = exp_result[0]
             exp_db = DrvDbCacheExperimentC()
             transform_experiment_db(source= exp_result, target = exp_db)
             exp_db.Status = DrvDbExpStatusE.ERROR.value
-            exp_db.DateBegin = datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
-            exp_db.DateFinish = datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
+            exp_db.DateBegin = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            exp_db.DateFinish = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             self.__cache_db.session.add(exp_db)
 
     def commit_changes(self):
         """Commit changes made to the cache database.
         """
         self.__cache_db.commit_changes()
```

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_mapping.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_mapping.py`

 * *Files identical despite different names*

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler/mid/mid_str/mid_str_node.py` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler/mid/mid_str/mid_str_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #######################         GENERIC IMPORTS          #######################
 from threading import Event, current_thread
 from typing import List
 
 #######################       THIRD PARTY IMPORTS        #######################
 from func_timeout import func_timeout, FunctionTimedOut
-
+from sqlalchemy.exc import DatabaseError
 #######################      SYSTEM ABSTRACTION IMPORTS  #######################
 from rfb_logger_tool import sys_log_logger_get_module_logger
 log = sys_log_logger_get_module_logger(__name__)
 
 #######################          PROJECT IMPORTS         #######################
 from rfb_shared_tool import (SysShdSharedObjC, SysShdNodeC, SysShdNodeParamsC, SysShdChanC,
                         SysShdNodeStatusE)
@@ -145,14 +145,16 @@
         self.status = SysShdNodeStatusE.STOP
         log.critical(f"Stopping {current_thread().name} node")
 
     def process_iteration(self) -> None:
         """AI is creating summary for process_iteration
         """
         try:
+            # Check if the db are connected
+            self.db_iface.check_connection()
             # Syncronising shared data
             self.sync_shd_data()
             # Receive and write alarms
             self.__receive_alarms()
 
             if len(self.__new_raised_alarms)>0:
                 self.db_iface.write_new_alarm(alarms= self.__new_raised_alarms,
@@ -175,14 +177,18 @@
             # TIMEOUT added to detect if database connection was ended
             func_timeout(DEFAULT_TIMEOUT_CONNECTION, self.db_iface.commit_changes)
         except FunctionTimedOut as exc:
             log.warning(("Timeout during commit changes to local database."
                          f"Database connection will be restarted. {exc}"))
             self.status = SysShdNodeStatusE.COMM_ERROR
             self.db_iface.reset_db_connection()
+        except DatabaseError as exc:
+            self.status = SysShdNodeStatusE.COMM_ERROR
+            log.critical(f"Database error in str node {exc}")
+            self.db_iface.reset_db_connection()
         except ConnectionError as exc:
             self.status = SysShdNodeStatusE.COMM_ERROR
             log.critical(f"Communication error in str node {exc}")
         except Exception as exc:
             self.status = SysShdNodeStatusE.INTERNAL_ERROR
             log.critical(f"Unexpected error in MID_STR_Node_c thread.\n{exc}")
             self.working_flag.clear()
```

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/PKG-INFO` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-battery-cycler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Battery cycler control used to execute custom profile on multiple battery technologies.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb-battery-cycler-0.0.1/src/rfb_battery_cycler.egg-info/SOURCES.txt` & `rfb_battery_cycler-0.0.2/src/rfb_battery_cycler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

