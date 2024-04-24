# Comparing `tmp/sigpro-0.2.0.tar.gz` & `tmp/sigpro-0.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigpro-0.2.0.tar", last modified: Fri Feb  2 22:06:34 2024, max compression
+gzip compressed data, was "sigpro-0.2.1.dev0.tar", last modified: Wed Apr 24 16:42:50 2024, max compression
```

## Comparing `sigpro-0.2.0.tar` & `sigpro-0.2.1.dev0.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.572766 sigpro-0.2.0/
--rw-r--r--   0 andy       (501) staff       (20)      151 2024-02-02 21:59:04.000000 sigpro-0.2.0/AUTHORS.rst
--rw-r--r--   0 andy       (501) staff       (20)     3989 2024-02-02 21:59:04.000000 sigpro-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 andy       (501) staff       (20)     3466 2024-02-02 22:06:32.000000 sigpro-0.2.0/HISTORY.md
--rw-r--r--   0 andy       (501) staff       (20)     1077 2024-02-02 21:59:04.000000 sigpro-0.2.0/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)      336 2024-02-02 21:59:04.000000 sigpro-0.2.0/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)     8485 2024-02-02 22:06:34.572647 sigpro-0.2.0/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     2475 2024-02-02 22:06:32.000000 sigpro-0.2.0/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.553621 sigpro-0.2.0/docs/
--rw-r--r--   0 andy       (501) staff       (20)      607 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/Makefile
--rw-r--r--   0 andy       (501) staff       (20)       28 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/authors.rst
--rw-r--r--   0 andy       (501) staff       (20)     5794 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/conf.py
--rw-r--r--   0 andy       (501) staff       (20)       34 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/contributing.rst
--rw-r--r--   0 andy       (501) staff       (20)       29 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/history.rst
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.553768 sigpro-0.2.0/docs/images/
--rw-r--r--   0 andy       (501) staff       (20)    33432 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/images/dai-logo-white-200.png
--rw-r--r--   0 andy       (501) staff       (20)      306 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/index.rst
--rw-r--r--   0 andy       (501) staff       (20)      768 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/make.bat
--rw-r--r--   0 andy       (501) staff       (20)       28 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/readme.rst
--rw-r--r--   0 andy       (501) staff       (20)       27 2024-02-02 21:59:04.000000 sigpro-0.2.0/docs/usage.rst
--rw-r--r--   0 andy       (501) staff       (20)     1268 2024-02-02 22:06:34.573285 sigpro-0.2.0/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     2707 2024-02-02 22:06:32.000000 sigpro-0.2.0/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.555016 sigpro-0.2.0/sigpro/
--rw-r--r--   0 andy       (501) staff       (20)     1400 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.555980 sigpro-0.2.0/sigpro/aggregations/
--rw-r--r--   0 andy       (501) staff       (20)       34 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.556268 sigpro-0.2.0/sigpro/aggregations/amplitude/
--rw-r--r--   0 andy       (501) staff       (20)       44 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/amplitude/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     2915 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/amplitude/statistical.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.556584 sigpro-0.2.0/sigpro/aggregations/frequency/
--rw-r--r--   0 andy       (501) staff       (20)       41 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/frequency/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      952 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/frequency/band.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.556730 sigpro-0.2.0/sigpro/aggregations/frequency_time/
--rw-r--r--   0 andy       (501) staff       (20)       48 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/aggregations/frequency_time/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     6333 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/basic_primitives.py
--rw-r--r--   0 andy       (501) staff       (20)    17975 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/contributing.py
--rw-r--r--   0 andy       (501) staff       (20)     6769 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/contributing_primitive.py
--rw-r--r--   0 andy       (501) staff       (20)     9810 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/core.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.556881 sigpro-0.2.0/sigpro/data/
--rw-r--r--   0 andy       (501) staff       (20)  6296970 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/data/demo_timeseries.csv
--rw-r--r--   0 andy       (501) staff       (20)     5444 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/demo.py
--rw-r--r--   0 andy       (501) staff       (20)    27372 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/pipeline.py
--rw-r--r--   0 andy       (501) staff       (20)     8408 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/primitive.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.548649 sigpro-0.2.0/sigpro/primitives/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.561936 sigpro-0.2.0/sigpro/primitives/sigpro/
--rw-r--r--   0 andy       (501) staff       (20)      861 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/SigPro.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.548976 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.548879 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.564216 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/
--rw-r--r--   0 andy       (501) staff       (20)      521 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/crest_factor.json
--rw-r--r--   0 andy       (501) staff       (20)      791 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/kurtosis.json
--rw-r--r--   0 andy       (501) staff       (20)      515 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/mean.json
--rw-r--r--   0 andy       (501) staff       (20)      512 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/rms.json
--rw-r--r--   0 andy       (501) staff       (20)      515 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/skew.json
--rw-r--r--   0 andy       (501) staff       (20)      512 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/std.json
--rw-r--r--   0 andy       (501) staff       (20)      512 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/var.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.549024 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/frequency/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.564379 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/frequency/band/
--rw-r--r--   0 andy       (501) staff       (20)      857 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/frequency/band/band_mean.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.549502 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.549264 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.564537 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/identity/
--rw-r--r--   0 andy       (501) staff       (20)      540 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/identity/identity.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.564684 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/
--rw-r--r--   0 andy       (501) staff       (20)      772 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/power_spectrum.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.549437 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.564838 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/band/
--rw-r--r--   0 andy       (501) staff       (20)      986 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/band/frequency_band.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.565224 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/fft/
--rw-r--r--   0 andy       (501) staff       (20)      740 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/fft/fft.json
--rw-r--r--   0 andy       (501) staff       (20)      750 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/fft/fft_real.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.549553 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.565557 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/stft/
--rw-r--r--   0 andy       (501) staff       (20)      867 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft.json
--rw-r--r--   0 andy       (501) staff       (20)      882 2024-02-02 22:06:32.000000 sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft_real.json
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.565677 sigpro-0.2.0/sigpro/transformations/
--rw-r--r--   0 andy       (501) staff       (20)       37 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.566135 sigpro-0.2.0/sigpro/transformations/amplitude/
--rw-r--r--   0 andy       (501) staff       (20)       47 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/amplitude/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      166 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/amplitude/identity.py
--rw-r--r--   0 andy       (501) staff       (20)      920 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/amplitude/spectrum.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.566609 sigpro-0.2.0/sigpro/transformations/frequency/
--rw-r--r--   0 andy       (501) staff       (20)       47 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/frequency/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      773 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/frequency/band.py
--rw-r--r--   0 andy       (501) staff       (20)     1817 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/frequency/fft.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.566896 sigpro-0.2.0/sigpro/transformations/frequency_time/
--rw-r--r--   0 andy       (501) staff       (20)       52 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/frequency_time/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1481 2024-02-02 21:59:04.000000 sigpro-0.2.0/sigpro/transformations/frequency_time/stft.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.555865 sigpro-0.2.0/sigpro.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     8485 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     3333 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       51 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)      648 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        7 2024-02-02 22:06:34.000000 sigpro-0.2.0/sigpro.egg-info/top_level.txt
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.567041 sigpro-0.2.0/tests/
--rw-r--r--   0 andy       (501) staff       (20)      522 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.567998 sigpro-0.2.0/tests/integration/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/integration/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3701 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/integration/test_contributing.py
--rw-r--r--   0 andy       (501) staff       (20)     2820 2024-02-02 22:06:32.000000 sigpro-0.2.0/tests/integration/test_contributing_primitive.py
--rw-r--r--   0 andy       (501) staff       (20)     5392 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/integration/test_core.py
--rw-r--r--   0 andy       (501) staff       (20)     2661 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/integration/test_demo.py
--rw-r--r--   0 andy       (501) staff       (20)     7695 2024-02-02 22:06:32.000000 sigpro-0.2.0/tests/integration/test_pipeline.py
--rw-r--r--   0 andy       (501) staff       (20)     3812 2024-02-02 22:06:32.000000 sigpro-0.2.0/tests/integration/test_primitive.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.568120 sigpro-0.2.0/tests/requirement_files/
--rw-r--r--   0 andy       (501) staff       (20)       58 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/requirement_files/latest_requirements.txt
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.568362 sigpro-0.2.0/tests/unit/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.568538 sigpro-0.2.0/tests/unit/aggregations/
--rw-r--r--   0 andy       (501) staff       (20)       32 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/aggregations/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.568838 sigpro-0.2.0/tests/unit/aggregations/amplitude/
--rw-r--r--   0 andy       (501) staff       (20)       45 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/aggregations/amplitude/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1197 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/aggregations/amplitude/test_statistical.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.569101 sigpro-0.2.0/tests/unit/aggregations/frequency/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/aggregations/frequency/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      462 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/aggregations/frequency/test_band.py
--rw-r--r--   0 andy       (501) staff       (20)       21 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/test___init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.550619 sigpro-0.2.0/tests/unit/transformations/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.569414 sigpro-0.2.0/tests/unit/transformations/amplitude/
--rw-r--r--   0 andy       (501) staff       (20)       52 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/amplitude/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      209 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/amplitude/identity.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.569748 sigpro-0.2.0/tests/unit/transformations/frequency/
--rw-r--r--   0 andy       (501) staff       (20)       52 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/frequency/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1055 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/frequency/test_fft.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-02-02 22:06:34.570091 sigpro-0.2.0/tests/unit/transformations/frequency_time/
--rw-r--r--   0 andy       (501) staff       (20)       57 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/frequency_time/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1286 2024-02-02 21:59:04.000000 sigpro-0.2.0/tests/unit/transformations/frequency_time/test_stft.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.689046 sigpro-0.2.1.dev0/
+-rw-r--r--   0 sarah      (501) staff       (20)      151 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3989 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/CONTRIBUTING.md
+-rw-r--r--   0 sarah      (501) staff       (20)     3466 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1077 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      336 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)     8490 2024-04-24 16:42:50.688948 sigpro-0.2.1.dev0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     2475 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.666087 sigpro-0.2.1.dev0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      607 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/Makefile
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/authors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5794 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       34 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.666214 sigpro-0.2.1.dev0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)    33432 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/images/dai-logo-white-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)      306 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      768 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/make.bat
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/readme.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       27 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/docs/usage.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1273 2024-04-24 16:42:50.689318 sigpro-0.2.1.dev0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2712 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.669054 sigpro-0.2.1.dev0/sigpro/
+-rw-r--r--   0 sarah      (501) staff       (20)     1405 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.670308 sigpro-0.2.1.dev0/sigpro/aggregations/
+-rw-r--r--   0 sarah      (501) staff       (20)       34 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.670684 sigpro-0.2.1.dev0/sigpro/aggregations/amplitude/
+-rw-r--r--   0 sarah      (501) staff       (20)       44 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/amplitude/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2915 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/amplitude/statistical.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.670940 sigpro-0.2.1.dev0/sigpro/aggregations/frequency/
+-rw-r--r--   0 sarah      (501) staff       (20)       41 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/frequency/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      952 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/frequency/band.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.671066 sigpro-0.2.1.dev0/sigpro/aggregations/frequency_time/
+-rw-r--r--   0 sarah      (501) staff       (20)       48 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/aggregations/frequency_time/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     6524 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/basic_primitives.py
+-rw-r--r--   0 sarah      (501) staff       (20)    17975 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/contributing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     6769 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/contributing_primitive.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9810 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/core.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.671200 sigpro-0.2.1.dev0/sigpro/data/
+-rw-r--r--   0 sarah      (501) staff       (20)  6296970 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/data/demo_timeseries.csv
+-rw-r--r--   0 sarah      (501) staff       (20)     5444 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/demo.py
+-rw-r--r--   0 sarah      (501) staff       (20)    27372 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/pipeline.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8408 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitive.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.661442 sigpro-0.2.1.dev0/sigpro/primitives/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.675536 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/
+-rw-r--r--   0 sarah      (501) staff       (20)      861 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/SigPro.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.661666 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.661601 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.678745 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/
+-rw-r--r--   0 sarah      (501) staff       (20)      521 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/crest_factor.json
+-rw-r--r--   0 sarah      (501) staff       (20)      791 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/kurtosis.json
+-rw-r--r--   0 sarah      (501) staff       (20)      515 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/mean.json
+-rw-r--r--   0 sarah      (501) staff       (20)      512 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/rms.json
+-rw-r--r--   0 sarah      (501) staff       (20)      515 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/skew.json
+-rw-r--r--   0 sarah      (501) staff       (20)      512 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/std.json
+-rw-r--r--   0 sarah      (501) staff       (20)      512 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/var.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.661713 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/frequency/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.680242 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/frequency/band/
+-rw-r--r--   0 sarah      (501) staff       (20)      857 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/frequency/band/band_mean.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.662294 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.661935 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.680410 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/identity/
+-rw-r--r--   0 sarah      (501) staff       (20)      540 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/identity/identity.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.680571 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/
+-rw-r--r--   0 sarah      (501) staff       (20)      772 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/power_spectrum.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.662207 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.680733 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/band/
+-rw-r--r--   0 sarah      (501) staff       (20)      986 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/band/frequency_band.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.681006 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fft/
+-rw-r--r--   0 sarah      (501) staff       (20)      740 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fft/fft.json
+-rw-r--r--   0 sarah      (501) staff       (20)      750 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fft/fft_real.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.681136 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fftfreq/
+-rw-r--r--   0 sarah      (501) staff       (20)      758 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fftfreq/fft_freq.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.662353 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.681536 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/stft/
+-rw-r--r--   0 sarah      (501) staff       (20)      867 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft.json
+-rw-r--r--   0 sarah      (501) staff       (20)      882 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft_real.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.681662 sigpro-0.2.1.dev0/sigpro/transformations/
+-rw-r--r--   0 sarah      (501) staff       (20)       37 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.682374 sigpro-0.2.1.dev0/sigpro/transformations/amplitude/
+-rw-r--r--   0 sarah      (501) staff       (20)       47 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/amplitude/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      166 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/amplitude/identity.py
+-rw-r--r--   0 sarah      (501) staff       (20)      920 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/amplitude/spectrum.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.683542 sigpro-0.2.1.dev0/sigpro/transformations/frequency/
+-rw-r--r--   0 sarah      (501) staff       (20)       47 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      773 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency/band.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1817 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency/fft.py
+-rw-r--r--   0 sarah      (501) staff       (20)      646 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency/fftfreq.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.683790 sigpro-0.2.1.dev0/sigpro/transformations/frequency_time/
+-rw-r--r--   0 sarah      (501) staff       (20)       52 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency_time/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1481 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/sigpro/transformations/frequency_time/stft.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.670194 sigpro-0.2.1.dev0/sigpro.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)     8490 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     3450 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       51 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      648 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        7 2024-04-24 16:42:50.000000 sigpro-0.2.1.dev0/sigpro.egg-info/top_level.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.683920 sigpro-0.2.1.dev0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)      522 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685066 sigpro-0.2.1.dev0/tests/integration/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3701 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_contributing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2820 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_contributing_primitive.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5392 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_core.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2661 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_demo.py
+-rw-r--r--   0 sarah      (501) staff       (20)     7695 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_pipeline.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3812 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/integration/test_primitive.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685185 sigpro-0.2.1.dev0/tests/requirement_files/
+-rw-r--r--   0 sarah      (501) staff       (20)       58 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/requirement_files/latest_requirements.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685388 sigpro-0.2.1.dev0/tests/unit/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685526 sigpro-0.2.1.dev0/tests/unit/aggregations/
+-rw-r--r--   0 sarah      (501) staff       (20)       32 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/aggregations/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685779 sigpro-0.2.1.dev0/tests/unit/aggregations/amplitude/
+-rw-r--r--   0 sarah      (501) staff       (20)       45 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/aggregations/amplitude/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1197 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/aggregations/amplitude/test_statistical.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.685991 sigpro-0.2.1.dev0/tests/unit/aggregations/frequency/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/aggregations/frequency/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      462 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/aggregations/frequency/test_band.py
+-rw-r--r--   0 sarah      (501) staff       (20)       21 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/test___init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.663377 sigpro-0.2.1.dev0/tests/unit/transformations/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.686241 sigpro-0.2.1.dev0/tests/unit/transformations/amplitude/
+-rw-r--r--   0 sarah      (501) staff       (20)       52 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/amplitude/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      209 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/amplitude/identity.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.686507 sigpro-0.2.1.dev0/tests/unit/transformations/frequency/
+-rw-r--r--   0 sarah      (501) staff       (20)       52 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/frequency/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1055 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/frequency/test_fft.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2024-04-24 16:42:50.686748 sigpro-0.2.1.dev0/tests/unit/transformations/frequency_time/
+-rw-r--r--   0 sarah      (501) staff       (20)       57 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/frequency_time/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1294 2024-04-24 16:41:31.000000 sigpro-0.2.1.dev0/tests/unit/transformations/frequency_time/test_stft.py
```

### Comparing `sigpro-0.2.0/CONTRIBUTING.md` & `sigpro-0.2.1.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/HISTORY.md` & `sigpro-0.2.1.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/LICENSE` & `sigpro-0.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/PKG-INFO` & `sigpro-0.2.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigpro
-Version: 0.2.0
+Version: 0.2.1.dev0
 Summary: Signal Processing Tools for Machine Mearning
 Home-page: https://github.com/sintel-dev/SigPro
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sigpro signal processing tools machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `sigpro-0.2.0/README.md` & `sigpro-0.2.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/docs/Makefile` & `sigpro-0.2.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/docs/conf.py` & `sigpro-0.2.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/docs/images/dai-logo-white-200.png` & `sigpro-0.2.1.dev0/docs/images/dai-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/docs/make.bat` & `sigpro-0.2.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/setup.cfg` & `sigpro-0.2.1.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sigpro-0.2.0/setup.py` & `sigpro-0.2.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,10 +99,10 @@
     name='sigpro',
     packages=find_packages(include=['sigpro', 'sigpro.*']),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/SigPro',
-    version='0.2.0',
+    version='0.2.1.dev0',
     zip_safe=False,
 )
```

### Comparing `sigpro-0.2.0/sigpro/__init__.py` & `sigpro-0.2.1.dev0/sigpro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for SigPro."""
 
 __author__ = """MIT Data To AI Lab"""
 __email__ = 'dailabmit@gmail.com'
-__version__ = '0.2.0'
+__version__ = '0.2.1.dev0'
 
 import os
 
 from mlblocks import discovery
 
 from sigpro.core import SigPro
```

### Comparing `sigpro-0.2.0/sigpro/aggregations/amplitude/statistical.py` & `sigpro-0.2.1.dev0/sigpro/aggregations/amplitude/statistical.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/aggregations/frequency/band.py` & `sigpro-0.2.1.dev0/sigpro/aggregations/frequency/band.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/basic_primitives.py` & `sigpro-0.2.1.dev0/sigpro/basic_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 class FFT(primitive.FrequencyTransformation):
     """FFT primitive class."""
 
     def __init__(self):
         super().__init__("sigpro.transformations.frequency.fft.fft")
 
 
+class FFTFreq(primitive.FrequencyTransformation):
+    """FFT Freq primitive class."""
+
+    def __init__(self):
+        super().__init__("sigpro.transformations.frequency.fftfreq.fft_freq")
+
+
 class FFTReal(primitive.FrequencyTransformation):
     """FFTReal primitive class."""
 
     def __init__(self):
         super().__init__("sigpro.transformations.frequency.fft.fft_real")
```

### Comparing `sigpro-0.2.0/sigpro/contributing.py` & `sigpro-0.2.1.dev0/sigpro/contributing.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/contributing_primitive.py` & `sigpro-0.2.1.dev0/sigpro/contributing_primitive.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/core.py` & `sigpro-0.2.1.dev0/sigpro/core.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/data/demo_timeseries.csv` & `sigpro-0.2.1.dev0/sigpro/data/demo_timeseries.csv`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/demo.py` & `sigpro-0.2.1.dev0/sigpro/demo.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/pipeline.py` & `sigpro-0.2.1.dev0/sigpro/pipeline.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitive.py` & `sigpro-0.2.1.dev0/sigpro/primitive.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/SigPro.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/SigPro.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/crest_factor.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/crest_factor.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/kurtosis.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/kurtosis.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/mean.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/mean.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/rms.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/rms.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/skew.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/skew.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/std.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/std.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/var.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/amplitude/statistical/var.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/aggregations/frequency/band/band_mean.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/aggregations/frequency/band/band_mean.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/identity/identity.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/identity/identity.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/power_spectrum.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/amplitude/spectrum/power_spectrum.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/band/frequency_band.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/band/frequency_band.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/fft/fft.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fft/fft.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency/fft/fft_real.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency/fft/fft_real.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft_real.json` & `sigpro-0.2.1.dev0/sigpro/primitives/sigpro/transformations/frequency_time/stft/stft_real.json`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/transformations/amplitude/spectrum.py` & `sigpro-0.2.1.dev0/sigpro/transformations/amplitude/spectrum.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/transformations/frequency/band.py` & `sigpro-0.2.1.dev0/sigpro/transformations/frequency/band.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/transformations/frequency/fft.py` & `sigpro-0.2.1.dev0/sigpro/transformations/frequency/fft.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro/transformations/frequency_time/stft.py` & `sigpro-0.2.1.dev0/sigpro/transformations/frequency_time/stft.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/sigpro.egg-info/PKG-INFO` & `sigpro-0.2.1.dev0/sigpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigpro
-Version: 0.2.0
+Version: 0.2.1.dev0
 Summary: Signal Processing Tools for Machine Mearning
 Home-page: https://github.com/sintel-dev/SigPro
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sigpro signal processing tools machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `sigpro-0.2.0/sigpro.egg-info/SOURCES.txt` & `sigpro-0.2.1.dev0/sigpro.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,25 @@
 sigpro/primitives/sigpro/aggregations/amplitude/statistical/var.json
 sigpro/primitives/sigpro/aggregations/frequency/band/band_mean.json
 sigpro/primitives/sigpro/transformations/amplitude/identity/identity.json
 sigpro/primitives/sigpro/transformations/amplitude/spectrum/power_spectrum.json
 sigpro/primitives/sigpro/transformations/frequency/band/frequency_band.json
 sigpro/primitives/sigpro/transformations/frequency/fft/fft.json
 sigpro/primitives/sigpro/transformations/frequency/fft/fft_real.json
+sigpro/primitives/sigpro/transformations/frequency/fftfreq/fft_freq.json
 sigpro/primitives/sigpro/transformations/frequency_time/stft/stft.json
 sigpro/primitives/sigpro/transformations/frequency_time/stft/stft_real.json
 sigpro/transformations/__init__.py
 sigpro/transformations/amplitude/__init__.py
 sigpro/transformations/amplitude/identity.py
 sigpro/transformations/amplitude/spectrum.py
 sigpro/transformations/frequency/__init__.py
 sigpro/transformations/frequency/band.py
 sigpro/transformations/frequency/fft.py
+sigpro/transformations/frequency/fftfreq.py
 sigpro/transformations/frequency_time/__init__.py
 sigpro/transformations/frequency_time/stft.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/test_contributing.py
 tests/integration/test_contributing_primitive.py
 tests/integration/test_core.py
```

### Comparing `sigpro-0.2.0/sigpro.egg-info/requires.txt` & `sigpro-0.2.1.dev0/sigpro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/__init__.py` & `sigpro-0.2.1.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_contributing.py` & `sigpro-0.2.1.dev0/tests/integration/test_contributing.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_contributing_primitive.py` & `sigpro-0.2.1.dev0/tests/integration/test_contributing_primitive.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_core.py` & `sigpro-0.2.1.dev0/tests/integration/test_core.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_demo.py` & `sigpro-0.2.1.dev0/tests/integration/test_demo.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_pipeline.py` & `sigpro-0.2.1.dev0/tests/integration/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/integration/test_primitive.py` & `sigpro-0.2.1.dev0/tests/integration/test_primitive.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/unit/aggregations/amplitude/test_statistical.py` & `sigpro-0.2.1.dev0/tests/unit/aggregations/amplitude/test_statistical.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/unit/transformations/frequency/test_fft.py` & `sigpro-0.2.1.dev0/tests/unit/transformations/frequency/test_fft.py`

 * *Files identical despite different names*

### Comparing `sigpro-0.2.0/tests/unit/transformations/frequency_time/test_stft.py` & `sigpro-0.2.1.dev0/tests/unit/transformations/frequency_time/test_stft.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # assert
     expected_amplitude_values_len = 129
     expected_frequency_values_len = 129
     expected_time_values_len = 3
     value = amplitude_values[0][0]
 
-    assert type(value) == np.complex128
+    assert isinstance(value, np.complex128)
     assert len(amplitude_values) == expected_amplitude_values_len
     assert len(frequency_values) == expected_frequency_values_len
     assert len(time_values) == expected_time_values_len
 
 
 def test_stft_real():
     # setup
@@ -35,11 +35,11 @@
 
     # assert
     expected_amplitude_values_len = 129
     expected_frequency_values_len = 129
     expected_time_values_len = 3
     value = amplitude_values[0][0]
 
-    assert type(value) == np.float64
+    assert isinstance(value, np.float64)
     assert len(amplitude_values) == expected_amplitude_values_len
     assert len(frequency_values) == expected_frequency_values_len
     assert len(time_values) == expected_time_values_len
```

