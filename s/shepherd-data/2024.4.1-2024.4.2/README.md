# Comparing `tmp/shepherd_data-2024.4.1.tar.gz` & `tmp/shepherd_data-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2024.4.1.tar", last modified: Thu Apr 18 13:25:13 2024, max compression
+gzip compressed data, was "shepherd_data-2024.4.2.tar", last modified: Wed Apr 24 19:39:07 2024, max compression
```

## Comparing `shepherd_data-2024.4.1.tar` & `shepherd_data-2024.4.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.164982 shepherd_data-2024.4.1/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/debug_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:12.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.164982 shepherd_data-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:39:06.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_reader.py
```

### Comparing `shepherd_data-2024.4.1/PKG-INFO` & `shepherd_data-2024.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://pypi.org/project/shepherd-data/issues
 Project-URL: Source, https://pypi.org/project/shepherd-data/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -31,15 +31,15 @@
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pyYAML
 Requires-Dist: scipy
-Requires-Dist: shepherd-core[inventory]>=2024.04.1
+Requires-Dist: shepherd-core[inventory]>=2024.4.2
 Requires-Dist: tqdm
 Provides-Extra: elf
 Requires-Dist: shepherd-core[elf]; extra == "elf"
 Provides-Extra: dev
 Requires-Dist: shepherd-core[dev]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
```

### Comparing `shepherd_data-2024.4.1/README.md` & `shepherd_data-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/pyproject.toml` & `shepherd_data-2024.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "click",
     "h5py",
     "matplotlib",  # full-version
     "numpy",
     "pandas>=2.0.0",  # full-version, v2 is OK
     "pyYAML",
     "scipy",   # full-version
-    "shepherd-core[inventory]>=2024.04.1",
+    "shepherd-core[inventory]>=2024.4.2",
     "tqdm",    # full-version
 ]
 
 [project.optional-dependencies]
 elf = [
     "shepherd-core[elf]"
 ]
```

### Comparing `shepherd_data-2024.4.1/shepherd_data/cli.py` & `shepherd_data-2024.4.2/shepherd_data/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Command definitions for CLI"""
+"""Command definitions for CLI."""
 
 import logging
 import os
 import sys
 from contextlib import suppress
 from datetime import datetime
 from pathlib import Path
@@ -12,23 +12,25 @@
 import click
 
 from shepherd_core import get_verbose_level
 from shepherd_core import increase_verbose_level
 from shepherd_core import local_tz
 from shepherd_core.commons import samplerate_sps_default
 
-from . import Reader
 from . import Writer
 from . import __version__
+from .reader import Reader
 
 logger = logging.getLogger("SHPData.cli")
 
 
 def path_to_flist(data_path: Path) -> List[Path]:
-    """Every path gets transformed to a list of paths
+    """Every path gets transformed to a list of paths.
+
+    Transformations:
     - if directory: list of files inside
     - if existing file: list with 1 element
     - or else: empty list
     """
     data_path = Path(data_path).resolve()
     h5files = []
     if data_path.is_file() and data_path.suffix.lower() == ".h5":
@@ -53,44 +55,44 @@
 @click.option(
     "--version",
     is_flag=True,
     help="Prints version-info at start (combinable with -v)",
 )
 @click.pass_context  # TODO: is the ctx-type correct?
 def cli(ctx: click.Context, verbose: bool, version: bool) -> None:  # noqa: FBT001
-    """Shepherd: Synchronized Energy Harvesting Emulator and Recorder"""
+    """Shepherd: Synchronized Energy Harvesting Emulator and Recorder."""
     if verbose:
         increase_verbose_level(3)
     if version:
         logger.info("Shepherd-Data v%s", __version__)
         logger.debug("Python v%s", sys.version)
         logger.debug("Click v%s", click.__version__)
     if not ctx.invoked_subcommand:
         click.echo("Please specify a valid command")
 
 
 @cli.command(short_help="Validates a file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 def validate(in_data: Path) -> None:
-    """Validates a file or directory containing shepherd-recordings"""
+    """Validate a file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()  # TODO: should be stored and passed in ctx
     valid_dir = True
     for file in files:
         logger.info("Validating '%s' ...", file.name)
         valid_file = True
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 valid_file &= shpr.is_valid()
                 valid_file &= shpr.check_timediffs()
                 valid_dir &= valid_file
                 if not valid_file:
                     logger.error(" -> File '%s' was NOT valid", file.name)
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
     sys.exit(int(not valid_dir))
 
 
 @cli.command(short_help="Extracts recorded IVSamples and stores it to csv")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--ds-factor",
@@ -103,15 +105,15 @@
     "--separator",
     "-s",
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract(in_data: Path, ds_factor: float, separator: str) -> None:
-    """Extracts recorded IVSamples and stores it to csv"""
+    """Extract recorded IVSamples and store them to csv."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     if not isinstance(ds_factor, (float, int)) or ds_factor < 1:
         ds_factor = 1000
         logger.info("DS-Factor was invalid was reset to 1'000")
     for file in files:
         logger.info("Extracting IV-Samples from '%s' ...", file.name)
@@ -139,62 +141,62 @@
                             is_time=True,
                         )
                         shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=ds_factor)
                         shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=ds_factor)
 
                 with Reader(ds_file, verbose=verbose_level > 2) as shpd:
                     shpd.save_csv(shpd["data"], separator)
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
 
 
 @cli.command(
     short_help="Extracts metadata and logs from file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--separator",
     "-s",
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract_meta(in_data: Path, separator: str) -> None:
-    """Extracts metadata and logs from file or directory containing shepherd-recordings"""
+    """Extract metadata and logs from file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting metadata & logs from '%s' ...", file.name)
         # TODO: add default exports (user-centric) and allow specifying --all or specific ones
         # TODO: could also be combined with other extractors (just have one)
-        # TODO remove deprecated: timesync; "shepherd-log", "dmesg", "exceptions"
+        # TODO: remove deprecated timesync; "shepherd-log", "dmesg", "exceptions"
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 shpr.save_metadata()
                 for element in ["ptp", "sysutil", "timesync"]:
                     if element in shpr.h5file:
                         shpr.save_csv(shpr[element], separator)
                 logs_depr = ["shepherd-log", "dmesg", "exceptions"]
                 logs = ["sheep", "kernel", "phc2sys", "uart"]
                 for element in logs + logs_depr:
                     if element in shpr.h5file:
                         shpr.save_log(shpr[element])
                         # TODO: allow omitting timestamp,
                         #       also test if segmented uart is correctly written
                         shpr.warn_logs(element, show=True)
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
 
 
 @cli.command(
     short_help="Extracts uart from gpio-trace in file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 def extract_uart(in_data: Path) -> None:
-    """Extracts uart from gpio-trace in file or directory containing shepherd-recordings"""
+    """Extract UART from GPIO-trace in file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting uart from gpio-trace from from '%s' ...", file.name)
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 # TODO: move into separate fn OR add to h5-file and use .save_log(), ALSO TEST
@@ -209,40 +211,40 @@
                     for line in lines:
                         with suppress(TypeError):
                             timestamp = datetime.fromtimestamp(float(line[0]), tz=local_tz())
                             log_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f") + ":")
                             # TODO: allow to skip Timestamp and export raw text
                             log_file.write(f"\t{str.encode(line[1])}")
                             log_file.write("\n")
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
 
 
 @cli.command(short_help="Extracts gpio-trace from file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--separator",
     "-s",
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract_gpio(in_data: Path, separator: str) -> None:
-    """Extracts uart from gpio-trace in file or directory containing shepherd-recordings"""
+    """Extract UART from gpio-trace in file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting gpio-trace from from '%s' ...", file.name)
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 wfs = shpr.gpio_to_waveforms()
                 for name, wf in wfs.items():
                     shpr.waveform_to_csv(name, wf, separator)
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
 
 
 @cli.command(
     short_help="Creates an array of downsampling-files from "
     "file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
@@ -257,17 +259,15 @@
 @click.option(
     "--sample-rate",
     "-r",
     type=click.INT,
     help="Alternative Input to determine a downsample-factor (Choose One)",
 )
 def downsample(in_data: Path, ds_factor: Optional[float], sample_rate: Optional[int]) -> None:
-    """Creates an array of downsampling-files from file
-    or directory containing shepherd-recordings
-    """
+    """Create an array of down-sampled files from file or dir containing shepherd-recordings."""
     if ds_factor is None and sample_rate is not None and sample_rate >= 1:
         ds_factor = int(samplerate_sps_default / sample_rate)
         # TODO: shouldn't current sps be based on file rather than default?
     if isinstance(ds_factor, (float, int)) and ds_factor >= 1:
         ds_list = [ds_factor]
     else:
         ds_list = [5, 25, 100, 500, 2_500, 10_000, 50_000, 250_000, 1_000_000]
@@ -299,16 +299,16 @@
                     ) as shpw:
                         shpw["ds_factor"] = _factor
                         shpw.store_hostname(shpr.get_hostname())
                         shpw.store_config(shpr.get_config())
                         shpr.downsample(shpr.ds_time, shpw.ds_time, ds_factor=_factor, is_time=True)
                         shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=_factor)
                         shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=_factor)
-        except TypeError as _xpc:
-            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
 
 
 @cli.command(short_help="Plots IV-trace from file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--start",
     "-s",
@@ -347,29 +347,29 @@
     in_data: Path,
     start: Optional[float],
     end: Optional[float],
     width: int,
     height: int,
     multiplot: bool,  # noqa: FBT001
 ) -> None:
-    """Plots IV-trace from file or directory containing shepherd-recordings"""
+    """Plot IV-trace from file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     multiplot = multiplot and len(files) > 1
     data = []
     for file in files:
         logger.info("Generating plot for '%s' ...", file.name)
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 if multiplot:
                     data.append(shpr.generate_plot_data(start, end, relative_timestamp=True))
                 else:
                     shpr.plot_to_file(start, end, width, height)
-        except TypeError as _xpc:
-            logger.exception("ERROR: will skip file, caught exception: %s", _xpc)
+        except TypeError:
+            logger.exception("ERROR: Will skip file. It caused an exception.")
     if multiplot:
         logger.info("Got %d datasets to plot", len(data))
         mpl_path = Reader.multiplot_to_file(data, in_data, width, height)
         if mpl_path:
             logger.info("Plot generated and saved to '%s'", mpl_path.name)
         else:
             logger.info("Plot not generated, path was already in use.")
```

### Comparing `shepherd_data-2024.4.1/shepherd_data/ivonne.py` & `shepherd_data-2024.4.2/shepherd_data/ivonne.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""prototype of a file-reader with various converters
-to generate valid shepherd-data for emulation
-
-"""
+"""file-reader with various converters to generate valid shepherd-data for emulation."""
 
 import errno
 import logging
 import math
 import os
 import pickle
 from pathlib import Path
```

### Comparing `shepherd_data-2024.4.1/shepherd_data/mppt.py` & `shepherd_data-2024.4.2/shepherd_data/mppt.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/shepherd_data/reader.py` & `shepherd_data-2024.4.2/shepherd_data/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/shepherd_data.egg-info/PKG-INFO` & `shepherd_data-2024.4.2/shepherd_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://pypi.org/project/shepherd-data/issues
 Project-URL: Source, https://pypi.org/project/shepherd-data/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -31,15 +31,15 @@
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pyYAML
 Requires-Dist: scipy
-Requires-Dist: shepherd-core[inventory]>=2024.04.1
+Requires-Dist: shepherd-core[inventory]>=2024.4.2
 Requires-Dist: tqdm
 Provides-Extra: elf
 Requires-Dist: shepherd-core[elf]; extra == "elf"
 Provides-Extra: dev
 Requires-Dist: shepherd-core[dev]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
```

### Comparing `shepherd_data-2024.4.1/shepherd_data.egg-info/SOURCES.txt` & `shepherd_data-2024.4.2/shepherd_data.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 README.md
 pyproject.toml
 shepherd_data/__init__.py
 shepherd_data/cli.py
-shepherd_data/debug_resampler.py
 shepherd_data/ivonne.py
 shepherd_data/mppt.py
 shepherd_data/reader.py
 shepherd_data.egg-info/PKG-INFO
 shepherd_data.egg-info/SOURCES.txt
 shepherd_data.egg-info/dependency_links.txt
 shepherd_data.egg-info/entry_points.txt
```

### Comparing `shepherd_data-2024.4.1/tests/test_cli_downsample.py` & `shepherd_data-2024.4.2/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/tests/test_cli_extract.py` & `shepherd_data-2024.4.2/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/tests/test_cli_plot.py` & `shepherd_data-2024.4.2/tests/test_cli_plot.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/tests/test_examples.py` & `shepherd_data-2024.4.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.1/tests/test_ivonne.py` & `shepherd_data-2024.4.2/tests/test_ivonne.py`

 * *Files identical despite different names*

