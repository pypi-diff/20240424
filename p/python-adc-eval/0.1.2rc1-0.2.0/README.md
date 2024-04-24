# Comparing `tmp/python-adc-eval-0.1.2rc1.tar.gz` & `tmp/python-adc-eval-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adc-eval-0.1.2rc1.tar", last modified: Fri Jul 14 20:14:30 2023, max compression
+gzip compressed data, was "python-adc-eval-0.2.0.tar", last modified: Wed Apr 24 19:56:54 2024, max compression
```

## Comparing `python-adc-eval-0.1.2rc1.tar` & `python-adc-eval-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/adc_eval/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:56:54.780737 python-adc-eval-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 19:56:54.780737 python-adc-eval-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:56:54.780737 python-adc-eval-0.2.0/adc_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/adc_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/adc_eval/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/adc_eval/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/adc_eval/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:56:54.780737 python-adc-eval-0.2.0/python_adc_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 19:56:54.000000 python-adc-eval-0.2.0/python_adc_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 19:56:54.000000 python-adc-eval-0.2.0/python_adc_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:56:54.000000 python-adc-eval-0.2.0/python_adc_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:56:54.000000 python-adc-eval-0.2.0/python_adc_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:56:54.000000 python-adc-eval-0.2.0/python_adc_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:56:45.000000 python-adc-eval-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:56:54.780737 python-adc-eval-0.2.0/setup.cfg
```

### Comparing `python-adc-eval-0.1.2rc1/LICENSE` & `python-adc-eval-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.2rc1/PKG-INFO` & `python-adc-eval-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.2rc1
+Version: 0.2.0
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
@@ -14,50 +14,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: matplotlib==3.8.4
 
 python-adc-eval |Lint| |PyPi Version| |Codestyle|
 ===================================================
 
 A python-based ADC evaluation tool, suitable for standalone or library-based usage
 
 Details
 --------
 
-Package based on
+Inspired by
 `esynr3z/adc-eval <https://github.com/esynr3z/adc-eval>`__
 
-Tiny tools collection (Python
-`NumPy <https://numpy.org/>`__\ +\ `Matplotlib <https://matplotlib.org/>`__
-based) to do spectral analysis and calculate the key performance
-parameters of an ADC. Just collect some data from the ADC, specify basic
-ADC parameters and run analysis. See `example.ipynb <example.ipynb>`__
-(you will need `Jupyter Notebook <https://jupyter.org/>`__ to be
-installed).
+Performs spectral analysis of a dataset utilizing the Bartlett method. Calculates SFDR, SNDR, as well as harmonics.
 
 .. figure:: analyser.png
    :alt: analyser
 
    analyser
 
-References: - `Analog Devices MT-003 TUTORIAL “Understand SINAD, ENOB,
-SNR, THD, THD + N, and SFDR so You Don’t Get Lost in the Noise
-Floor” <https://www.analog.com/media/en/training-seminars/tutorials/MT-003.pdf>`__
-- `National Instruments Application Note 041 “The Fundamentals of
-FFT-Based Signal Analysis and
-Measurement” <http://www.sjsu.edu/people/burford.furman/docs/me120/FFT_tutorial_NI.pdf>`__
-
-Inspired by Linear Technology (now Analog Devices)
-`PScope <https://www.analog.com/en/technical-articles/pscope-basics.html>`__
-tool.
-
 
 USAGE
 =======
 
 To load the library in a module:
 
 .. code-block:: python
@@ -67,20 +51,26 @@
 
 Given an array of values representing the output of an ADC, the spectrum can be analyzed with the following:
 
 .. code-block:: python
 
     import adc_eval
 
-    adc_eval.spectrum.analyze(<adc list>, <adc_bits>, <adc vref>, <adc fsamp>, window='hanning', no_plot=<True/False>)
-
+    adc_eval.spectrum.analyze(
+        <data>,
+        <fft bins>,
+        fs=<sample frequency>,
+        dr=<dynamicrange/vref>,
+        harmonics=<num of harmonics to find>,
+        leak=<adjacent bins to filter>,
+        window=<window type (rectangular/hanning)>,
+        no_plot=<True/False>,
+        yaxis=<"power"/"fullscale">
+    )
 
-|pscope| Image source: `Creating an ADC Using FPGA Resources WP -
-Lattice <https://www.latticesemi.com/-/media/LatticeSemi/Documents/WhitePapers/AG/CreatingAnADCUsingFPGAResources.ashx?document_id=36525>`__
 
-.. |pscope| image:: pscope.png
 .. |Lint| image:: https://github.com/fronzbot/python-adc-eval/workflows/Lint/badge.svg
    :target: https://github.com/fronzbot/python-adc-eval/actions?query=workflow%3ALint
 .. |PyPi Version| image:: https://img.shields.io/pypi/v/spithon.svg
    :target: https://pypi.org/project/python-adc-eval
 .. |Codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-adc-eval-0.1.2rc1/adc_eval/converters.py` & `python-adc-eval-0.2.0/adc_eval/converters.py`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.2rc1/pyproject.toml` & `python-adc-eval-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-adc-eval"
-version = "0.1.2rc1"
+version = "0.2.0"
 license = {text = "MIT"}
 description = "ADC Evaluation Library"
 readme = "README.rst"
 authors = [{name = "Kevin Fronczak", email = "kfronczak@gmail.com"}]
 keywords = ["adc", "analog-to-digital", "evaluation", "eval", "spectrum"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -17,29 +17,29 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8.0"
 dependencies = [
-    "matplotlib==3.7.2",
+    "matplotlib==3.8.4",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/fronzbot/python-adc-eval"
 "Bug Reports" = "https://github.com/fronzbot/python-adc-eval/issues"
 
 [tool.setuptools]
 platforms = ["any"]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["adc_eval*"]
 
-[tool.ruff]
+[lint]
 select = [
     "C",  # complexity
     "D",  # docstrings
     "E",  # pydocstyle
     "F",  # pyflakes/autoflake
     "G",  # flake8-logging-format
     "I",  # isort
@@ -61,30 +61,34 @@
     "D202",  # No blank lines allowed after function docstring
     "D203",  # 1 blank line required before class docstring
     "D213",  # Multi-line docstring summary should start at the second line
     "D406",  # Section name should end with a newline
     "D407",  # Section name underlining
     "E501",  # line too long
     "E731",  # do not assign a lambda expression, use a def
+    "I001",  #Unformatted/unsorted imports...who cares?
     "PLC1901", # Lots of false positives
     # False positives https://github.com/astral-sh/ruff/issues/5386
     "PLC0208", # Use a sequence type instead of a `set` when iterating over values
     "PLR0911", # Too many return statements ({returns} > {max_returns})
     "PLR0912", # Too many branches ({branches} > {max_branches})
     "PLR0913", # Too many arguments to function call ({c_args} > {max_args})
     "PLR0915", # Too many statements ({statements} > {max_statements})
     "PLR2004",  # Magic value used in comparison, consider replacing {value} with a constant variable
     "PLW2901", # Outer {outer_kind} variable {name} overwritten by inner {inner_kind} target
+    "T201", # Allow print statements
     "UP006", # keep type annotation style as is
     "UP007", # keep type annotation style as is
     # Ignored due to performance: https://github.com/charliermarsh/ruff/issues/2923
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
 ]
+
+[tool.ruff]
 exclude = [
     "__init__.py",
 ]
 line-length = 88
 
-target-version = "py39"
+target-version = "py311"
 
-[tool.ruff.mccabe]
+[lint.mccabe]
 max-complexity = 10
```

### Comparing `python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/PKG-INFO` & `python-adc-eval-0.2.0/python_adc_eval.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.2rc1
+Version: 0.2.0
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
@@ -14,50 +14,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: matplotlib==3.8.4
 
 python-adc-eval |Lint| |PyPi Version| |Codestyle|
 ===================================================
 
 A python-based ADC evaluation tool, suitable for standalone or library-based usage
 
 Details
 --------
 
-Package based on
+Inspired by
 `esynr3z/adc-eval <https://github.com/esynr3z/adc-eval>`__
 
-Tiny tools collection (Python
-`NumPy <https://numpy.org/>`__\ +\ `Matplotlib <https://matplotlib.org/>`__
-based) to do spectral analysis and calculate the key performance
-parameters of an ADC. Just collect some data from the ADC, specify basic
-ADC parameters and run analysis. See `example.ipynb <example.ipynb>`__
-(you will need `Jupyter Notebook <https://jupyter.org/>`__ to be
-installed).
+Performs spectral analysis of a dataset utilizing the Bartlett method. Calculates SFDR, SNDR, as well as harmonics.
 
 .. figure:: analyser.png
    :alt: analyser
 
    analyser
 
-References: - `Analog Devices MT-003 TUTORIAL “Understand SINAD, ENOB,
-SNR, THD, THD + N, and SFDR so You Don’t Get Lost in the Noise
-Floor” <https://www.analog.com/media/en/training-seminars/tutorials/MT-003.pdf>`__
-- `National Instruments Application Note 041 “The Fundamentals of
-FFT-Based Signal Analysis and
-Measurement” <http://www.sjsu.edu/people/burford.furman/docs/me120/FFT_tutorial_NI.pdf>`__
-
-Inspired by Linear Technology (now Analog Devices)
-`PScope <https://www.analog.com/en/technical-articles/pscope-basics.html>`__
-tool.
-
 
 USAGE
 =======
 
 To load the library in a module:
 
 .. code-block:: python
@@ -67,20 +51,26 @@
 
 Given an array of values representing the output of an ADC, the spectrum can be analyzed with the following:
 
 .. code-block:: python
 
     import adc_eval
 
-    adc_eval.spectrum.analyze(<adc list>, <adc_bits>, <adc vref>, <adc fsamp>, window='hanning', no_plot=<True/False>)
-
+    adc_eval.spectrum.analyze(
+        <data>,
+        <fft bins>,
+        fs=<sample frequency>,
+        dr=<dynamicrange/vref>,
+        harmonics=<num of harmonics to find>,
+        leak=<adjacent bins to filter>,
+        window=<window type (rectangular/hanning)>,
+        no_plot=<True/False>,
+        yaxis=<"power"/"fullscale">
+    )
 
-|pscope| Image source: `Creating an ADC Using FPGA Resources WP -
-Lattice <https://www.latticesemi.com/-/media/LatticeSemi/Documents/WhitePapers/AG/CreatingAnADCUsingFPGAResources.ashx?document_id=36525>`__
 
-.. |pscope| image:: pscope.png
 .. |Lint| image:: https://github.com/fronzbot/python-adc-eval/workflows/Lint/badge.svg
    :target: https://github.com/fronzbot/python-adc-eval/actions?query=workflow%3ALint
 .. |PyPi Version| image:: https://img.shields.io/pypi/v/spithon.svg
    :target: https://pypi.org/project/python-adc-eval
 .. |Codestyle| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

