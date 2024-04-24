# Comparing `tmp/robotpy-rev-2024.2.3.tar.gz` & `tmp/robotpy-rev-2024.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotpy-rev-2024.2.3.tar", last modified: Thu Mar 14 18:52:22 2024, max compression
+gzip compressed data, was "robotpy-rev-2024.2.4.tar", last modified: Wed Apr 24 14:19:30 2024, max compression
```

## Comparing `robotpy-rev-2024.2.3.tar` & `robotpy-rev-2024.2.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.829464 robotpy-rev-2024.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.829464 robotpy-rev-2024.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/.github/workflows/scan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.829464 robotpy-rev-2024.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/can-arcade-drive/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/can-arcade-drive/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/can-tank-drive/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/can-tank-drive/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/color_match/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/color_match/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/get-set-params/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/get-set-params/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/getting-started/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/getting-started/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/limit-switch/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/limit-switch/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/limit-switch/shuffleboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/maxswerve/
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/robotcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/maxswerve/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/subsystems/drivesubsystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/subsystems/maxswervemodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/maxswerve/swerveutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/position-pid-control/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/position-pid-control/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/position-pid-control/shuffleboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/read-encoder-values/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/read-encoder-values/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/read_rgb_values/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3055 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/read_rgb_values/robot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/smart-motion/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8341 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/smart-motion/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/smart-motion/shuffleboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.833464 robotpy-rev-2024.2.3/examples/velocity-pid-control/
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/velocity-pid-control/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/examples/velocity-pid-control/shuffleboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/gen/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/AbsoluteEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/AnalogInput.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANAnalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANError.yml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANSensor.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANSparkBase.yml
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANSparkFlex.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANSparkLowLevel.yml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CANSparkMax.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/CIEColor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/ColorMatch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/ColorSensorV3.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/ControlType.yml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/MotorFeedbackSensor.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/REVLibError.yml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/RelativeEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkAbsoluteEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkAnalogSensor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkFlexExternalEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkLimitSwitch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxAbsoluteEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxAlternateEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxAnalogSensor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxLimitSwitch.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxPIDController.yml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkMaxRelativeEncoder.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkPIDController.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/SparkRelativeEncoder.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/gen/driver/
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/gen/driver/CANSparkMaxFrames.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/rev/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/rev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/rev/rev.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/rev/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/robotpy_rev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-14 18:52:22.000000 robotpy-rev-2024.2.3/robotpy_rev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:52:22.841464 robotpy-rev-2024.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/tests/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      246 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-14 18:52:06.000000 robotpy-rev-2024.2.3/tests/test_cansparkmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.012002 robotpy-rev-2024.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.016002 robotpy-rev-2024.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/.github/workflows/scan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.016002 robotpy-rev-2024.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/can-arcade-drive/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/can-arcade-drive/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/can-tank-drive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/can-tank-drive/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/color_match/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/color_match/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/get-set-params/
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/get-set-params/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/getting-started/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/getting-started/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/limit-switch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/limit-switch/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/limit-switch/shuffleboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/maxswerve/
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/robotcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/maxswerve/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/subsystems/drivesubsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/subsystems/maxswervemodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/maxswerve/swerveutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/position-pid-control/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/position-pid-control/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/position-pid-control/shuffleboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/read-encoder-values/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/read-encoder-values/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/read_rgb_values/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3055 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/read_rgb_values/robot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/smart-motion/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8341 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/smart-motion/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/smart-motion/shuffleboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.020002 robotpy-rev-2024.2.4/examples/velocity-pid-control/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/velocity-pid-control/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/examples/velocity-pid-control/shuffleboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.024002 robotpy-rev-2024.2.4/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/AbsoluteEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/AnalogInput.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANAnalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANError.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANSensor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANSparkBase.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANSparkFlex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANSparkLowLevel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CANSparkMax.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/CIEColor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/ColorMatch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/ColorSensorV3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/ControlType.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/MotorFeedbackSensor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/REVLibError.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/RelativeEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkAbsoluteEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkAnalogSensor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkFlexExternalEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkLimitSwitch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxAbsoluteEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxAlternateEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxAnalogSensor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxLimitSwitch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxPIDController.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkMaxRelativeEncoder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkPIDController.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/SparkRelativeEncoder.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.024002 robotpy-rev-2024.2.4/gen/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/gen/driver/CANSparkMaxFrames.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/rev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/rev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/rev/rev.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/rev/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/robotpy_rev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-24 14:19:30.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-24 14:19:29.000000 robotpy-rev-2024.2.4/robotpy_rev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:19:30.028002 robotpy-rev-2024.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      246 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 14:19:20.000000 robotpy-rev-2024.2.4/tests/test_cansparkmax.py
```

### Comparing `robotpy-rev-2024.2.3/.github/workflows/dist.yml` & `robotpy-rev-2024.2.4/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/LICENSE` & `robotpy-rev-2024.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/PKG-INFO` & `robotpy-rev-2024.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-rev
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: REVLib for RobotPy
 Home-page: https://github.com/robotpy/robotpy-rev
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: BSD-3-Clause
 Description: robotpy-rev
         ===========
```

### Comparing `robotpy-rev-2024.2.3/README.rst` & `robotpy-rev-2024.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/docs/Makefile` & `robotpy-rev-2024.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/docs/api.rst` & `robotpy-rev-2024.2.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/docs/conf.py` & `robotpy-rev-2024.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/docs/make.bat` & `robotpy-rev-2024.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/can-arcade-drive/robot.py` & `robotpy-rev-2024.2.4/examples/can-arcade-drive/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/can-tank-drive/robot.py` & `robotpy-rev-2024.2.4/examples/can-tank-drive/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/color_match/robot.py` & `robotpy-rev-2024.2.4/examples/color_match/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/get-set-params/robot.py` & `robotpy-rev-2024.2.4/examples/get-set-params/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/getting-started/robot.py` & `robotpy-rev-2024.2.4/examples/getting-started/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/limit-switch/robot.py` & `robotpy-rev-2024.2.4/examples/limit-switch/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/limit-switch/shuffleboard.json` & `robotpy-rev-2024.2.4/examples/limit-switch/shuffleboard.json`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/constants.py` & `robotpy-rev-2024.2.4/examples/maxswerve/constants.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/robot.py` & `robotpy-rev-2024.2.4/examples/maxswerve/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/robotcontainer.py` & `robotpy-rev-2024.2.4/examples/maxswerve/robotcontainer.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/subsystems/drivesubsystem.py` & `robotpy-rev-2024.2.4/examples/maxswerve/subsystems/drivesubsystem.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/subsystems/maxswervemodule.py` & `robotpy-rev-2024.2.4/examples/maxswerve/subsystems/maxswervemodule.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/maxswerve/swerveutils.py` & `robotpy-rev-2024.2.4/examples/maxswerve/swerveutils.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/position-pid-control/robot.py` & `robotpy-rev-2024.2.4/examples/position-pid-control/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/position-pid-control/shuffleboard.json` & `robotpy-rev-2024.2.4/examples/position-pid-control/shuffleboard.json`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/read-encoder-values/robot.py` & `robotpy-rev-2024.2.4/examples/read-encoder-values/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/read_rgb_values/robot.py` & `robotpy-rev-2024.2.4/examples/read_rgb_values/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/smart-motion/robot.py` & `robotpy-rev-2024.2.4/examples/smart-motion/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/smart-motion/shuffleboard.json` & `robotpy-rev-2024.2.4/examples/smart-motion/shuffleboard.json`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/velocity-pid-control/robot.py` & `robotpy-rev-2024.2.4/examples/velocity-pid-control/robot.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/examples/velocity-pid-control/shuffleboard.json` & `robotpy-rev-2024.2.4/examples/velocity-pid-control/shuffleboard.json`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/CANSparkBase.yml` & `robotpy-rev-2024.2.4/gen/CANSparkBase.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/CANSparkLowLevel.yml` & `robotpy-rev-2024.2.4/gen/CANSparkLowLevel.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/CANSparkMax.yml` & `robotpy-rev-2024.2.4/gen/CANSparkMax.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/ColorSensorV3.yml` & `robotpy-rev-2024.2.4/gen/ColorSensorV3.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/RelativeEncoder.yml` & `robotpy-rev-2024.2.4/gen/RelativeEncoder.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/SparkMaxPIDController.yml` & `robotpy-rev-2024.2.4/gen/SparkMaxPIDController.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/gen/driver/CANSparkMaxFrames.yml` & `robotpy-rev-2024.2.4/gen/driver/CANSparkMaxFrames.yml`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/pyproject.toml` & `robotpy-rev-2024.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 [tool.robotpy-build]
 base_package = "rev"
 
 [tool.robotpy-build.static_libs."revlib_driver".maven_lib_download]
 artifact_id = "REVLib-driver"
 group_id = "com.revrobotics.frc"
 repo_url = "https://maven.revrobotics.com"
-version = "2024.2.3"
+version = "2024.2.4"
 libs = ["REVLibDriver"]
 
 [tool.robotpy-build.static_libs."revlib".maven_lib_download]
 artifact_id = "REVLib-cpp"
 group_id = "com.revrobotics.frc"
 repo_url = "https://maven.revrobotics.com"
-version = "2024.2.3"
+version = "2024.2.4"
 libs = ["REVLib"]
 
 [tool.robotpy-build.wrappers."rev"]
 name = "rev"
 sources = [
     "rev/rev.cpp"
 ]
```

### Comparing `robotpy-rev-2024.2.3/rev/__init__.py` & `robotpy-rev-2024.2.4/rev/__init__.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/robotpy_rev.egg-info/PKG-INFO` & `robotpy-rev-2024.2.4/robotpy_rev.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotpy-rev
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: REVLib for RobotPy
 Home-page: https://github.com/robotpy/robotpy-rev
 Author: RobotPy Development Team
 Author-email: robotpy@googlegroups.com
 License: BSD-3-Clause
 Description: robotpy-rev
         ===========
```

### Comparing `robotpy-rev-2024.2.3/robotpy_rev.egg-info/SOURCES.txt` & `robotpy-rev-2024.2.4/robotpy_rev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/tests/conftest.py` & `robotpy-rev-2024.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `robotpy-rev-2024.2.3/tests/test_cansparkmax.py` & `robotpy-rev-2024.2.4/tests/test_cansparkmax.py`

 * *Files identical despite different names*

