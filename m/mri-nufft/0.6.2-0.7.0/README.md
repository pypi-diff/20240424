# Comparing `tmp/mri_nufft-0.6.2.tar.gz` & `tmp/mri_nufft-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri_nufft-0.6.2.tar", last modified: Mon Apr 15 13:26:44 2024, max compression
+gzip compressed data, was "mri_nufft-0.7.0.tar", last modified: Wed Apr 24 13:22:02 2024, max compression
```

## Comparing `mri_nufft-0.6.2.tar` & `mri_nufft-0.7.0.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.343490 mri_nufft-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_static/logos/mri-nufft-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_static/logos/mri-nufft.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/related.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/nufft.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/trajectory_gradspec.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_2D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_3D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_trajectory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/src/mri_nufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/src/mrinufft/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mrinufft/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/src/mrinufft/density/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/geometry_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/nufft_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/io/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/cfl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/nsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/_cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/finufft.py
--rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/gpunufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nfft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nudft_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/pynufft_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/sigpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/tfnufft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/css_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/off_resonnance.py
--rw-r--r--   0 runner    (1001) docker     (127)    27992 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/stacked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/src/mrinufft/trajectories/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/case_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_gpunufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_stacked_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_ndft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.948195 mri_nufft-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_static/logos/mri-nufft-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_static/logos/mri-nufft.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/related.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/nufft.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/trajectory_gradspec.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_2D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_3D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_gif_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_gif_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26645 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_trajectory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.948195 mri_nufft-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/src/mri_nufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mrinufft/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/density/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/geometry_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/nufft_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/cfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/nsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/_cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/finufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nudft_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/pynufft_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/sigpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/tfnufft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/css_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/off_resonnance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30205 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/stacked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23461 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/case_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_stacked_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_ndft.py
```

### Comparing `mri_nufft-0.6.2/.github/workflows/master-cd.yml` & `mri_nufft-0.7.0/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/.github/workflows/style.yml` & `mri_nufft-0.7.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/.github/workflows/tags-release.yml` & `mri_nufft-0.7.0/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/.github/workflows/test-ci.yml` & `mri_nufft-0.7.0/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/LICENSE.txt` & `mri_nufft-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/PKG-INFO` & `mri_nufft-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.6.2
+Version: 0.7.0
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `mri_nufft-0.6.2/README.rst` & `mri_nufft-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/Makefile` & `mri_nufft-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/_static/logos/mri-nufft-icon.png` & `mri_nufft-0.7.0/docs/_static/logos/mri-nufft-icon.png`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/_static/logos/mri-nufft.png` & `mri_nufft-0.7.0/docs/_static/logos/mri-nufft.png`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/_templates/autosummary/class.rst` & `mri_nufft-0.7.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/_templates/autosummary/module.rst` & `mri_nufft-0.7.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/conf.py` & `mri_nufft-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/getting_started.rst` & `mri_nufft-0.7.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/index.rst` & `mri_nufft-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/misc/code_of_conduct.rst` & `mri_nufft-0.7.0/docs/misc/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/misc/development.rst` & `mri_nufft-0.7.0/docs/misc/development.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/nufft.rst` & `mri_nufft-0.7.0/docs/nufft.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/docs/trajectory_gradspec.rst` & `mri_nufft-0.7.0/docs/trajectory_gradspec.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/examples/conftest.py` & `mri_nufft-0.7.0/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/examples/example_2D_trajectories.py` & `mri_nufft-0.7.0/examples/example_2D_trajectories.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 # ``spiral (str, float)``
 # ~~~~~~~~~~~~~~~~~~~~~~~
 #
 #
 # The shape of the spiral defined through :math:`n` in the
 # :math:`r = a \theta^{1/n}` equality, with :math:`r` the radius and
 # :math:`\theta` the polar angle. Both ``"archimedes"`` and ``"fermat"``
-# are available as string options for simplicity.
+# are available as string options for convenience.
 #
 
 arguments = ["archimedes", "fermat", 0.5, 1.5]
 function = lambda x: mn.initialize_2D_spiral(Nc, Ns, tilt=tilt, spiral=x, in_out=in_out)
 show_argument(function, arguments, one_shot=one_shot, subfigure_size=subfigure_size)
```

### Comparing `mri_nufft-0.6.2/examples/example_3D_trajectories.py` & `mri_nufft-0.7.0/examples/example_3D_trajectories.py`

 * *Files 7% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 # - ``Ns (int)``: number of samples per shot
 # - ``tilt (str, float)``: angle between each consecutive shot (in radians).
 #   ``(default "uniform")``
 # - ``in_out (bool)``: define whether the shots should travel toward
 #   the center then outside (in-out) or not (center-out). ``(default False)``
 # - ``nb_zigzags (float)``: number of revolutions over a center-out shot.
 #   ``(default 5)``
+# - ``spiral (str, float)``: type of spiral defined through the general
+#   archimedean equation. ``(default "archimedes")``. See 2D spiral
 # - ``width (float)``: cone width factor, normalized to densely cover the k-space
 #   by default. ``(default 1)``
 #
 
 trajectory = mn.initialize_3D_cones(Nc, Ns, in_out=in_out)
 show_trajectory(trajectory, figure_size=figure_size, one_shot=one_shot)
 
@@ -199,14 +201,29 @@
 
 arguments = [0.5, 2, 5, 10]
 function = lambda x: mn.initialize_3D_cones(Nc, Ns, in_out=in_out, nb_zigzags=x)
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
 
 # %%
+# ``spiral (str, float)``
+# ~~~~~~~~~~~~~~~~~~~~~~~
+#
+#
+# The shape of the spiral defined and documented in
+# ``initialize_2D_spiral``. Both ``"archimedes"`` and ``"fermat"``
+# spirals are available as string options for convenience.
+#
+
+arguments = ["archimedes", "fermat", 0.5, 1.5]
+function = lambda x: mn.initialize_3D_cones(Nc, Ns, in_out=in_out, spiral=x)
+show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
+
+
+# %%
 # ``width (float)``
 # ~~~~~~~~~~~~~~~~~
 #
 # The cone width normalized such that ``width = 1`` corresponds to
 # non-overlapping cones covering the whole k-space sphere, and
 # therefore ``width > 1`` creates overlap between cone regions and
 # ``width < 1`` tends to more radial patterns.
@@ -231,34 +248,29 @@
 # - ``Nc (int)``: number of individual shots. See 3D cones
 # - ``Ns (int)``: number of samples per shot. See 3D cones
 # - ``in_out (bool)``: define whether the shots should travel toward
 #   the center then outside (in-out) or not (center-out).
 #   ``(default False)``. See 3D cones or 2D spiral
 # - ``nb_revolutions (float)``: number of revolutions performed from the
 #   center. ``(default 1)``. See 2D spiral
-# - ``spiral_tilt (str, float)``: angle between each spiral within a plane
-#   (in radians). ``(default "uniform")``. See 2D spiral
 # - ``spiral (str, float)``: type of spiral defined through the general
 #   archimedean equation. ``(default "fermat")``. See 2D spiral
-# - ``nb_cones (int)``: number of cones around the :math:`k_z`-axis.
-#   See ``tools.conify``
 # - ``cone_tilt (float)``: angle tilt between consecutive cones
 #   around the :math:`k_z`-axis. ``(default "golden")``. See ``tools.conify``
 # - ``max_angle (float)``: maximum angle of the cones. ``(default pi / 2)``.
 #   See ``tools.conify``
 # - ``axes (tuple)``: axes over which cones are created, by default (2,)
 #
 
 trajectory = mn.initialize_3D_floret(
-    Nc,
+    Nc * nb_repetitions,
     Ns,
     in_out=in_out,
     nb_revolutions=nb_revolutions,
-    nb_cones=nb_repetitions,
-    max_angle=np.pi / 2,
+    max_angle=np.pi / 3,
 )[::-1]
 show_trajectory(trajectory, figure_size=figure_size, one_shot=one_shot)
 
 # %%
 #
 # ``axes (tuple)``
 # ~~~~~~~~~~~~~~~~
@@ -270,26 +282,31 @@
 #
 # The point is to provide an efficient coverage by reducing ``max_angle``
 # to avoid redundancy around one axis, but still cover the whole
 # k-space sphere by duplicating cones along several axes, as initially
 # proposed by [Pip+11]_.
 #
 
-arguments = [(2,), (0,), (0, 2), (0, 1, 2)]
+arguments = [(0,), (1,), (0, 1), (0, 1, 2)]
 function = lambda x: mn.initialize_3D_floret(
-    Nc,
+    Nc * nb_repetitions,
     Ns,
     in_out=in_out,
     nb_revolutions=nb_revolutions,
-    nb_cones=nb_repetitions,
     max_angle=np.pi / 4,
     axes=x,
 )[::-1]
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
+# %%
+
+show_argument(
+    function, arguments, one_shot=one_shot, subfig_size=subfigure_size, dim="2D"
+)
+
 
 # %%
 # Wave-CAIPI
 # ----------
 #
 # A pattern introduced in [Bil+15]_ composed of helices evolving
 # in the same direction and packed together,
@@ -344,25 +361,27 @@
 
 # %%
 # ``packing (str)``
 # ~~~~~~~~~~~~~~~~~
 #
 # The method used to pack circles of same size within an arbitrary ``shape``.
 # The available methods are ``"triangular"`` and ``"square"`` for regular tiling
-# over dense grids, and ``"circular"`` and ``"random"`` for irregular packing.
+# over dense grids, and ``"circular"``, ``fibonacci`` and ``"random"`` for
+# irregular packing.
 # Different aliases are available, such as ``"triangle"``, ``"hexagon"`` instead
 # of ``"triangular"``.
 #
-# Note that ``"triangular"`` packing has slightly overlapping helices,
-# as it corresponds to a triangular/hexagonal grid.
+# Note that ``"triangular"`` and ``fibonacci`` packings have slightly overlapping
+# helices, as their widths correspond to that of an optimaly packed
+# triangular/hexagonal grid.
 # The ``"random"`` packing also naturally overlaps as the positions are determined
 # following a uniform distribution over :math:`k_x` and :math:`k_y` dimensions.
 #
 
-arguments = ["triangular", "square", "circular", "random"]
+arguments = ["triangular", "square", "circular", "fibonacci", "random"]
 function = lambda x: mn.initialize_3D_wave_caipi(Nc, Ns, packing=x)
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
 # %%
 
 show_argument(
     function, arguments, one_shot=one_shot, subfig_size=subfigure_size, dim="2D"
@@ -436,16 +455,18 @@
 #
 # - ``Nc (int)``: number of individual shots. See 3D cones
 # - ``Ns (int)``: number of samples per shot. See 3D cones
 # - ``curve_index (float)``: Index controlling curvature from 0 (flat) to 1 (curvy).
 #   ``(default 0.3)``
 # - ``nb_revolutions (float)``: number of revolutions or elliptic periods.
 #   ``(default 1)``
-# - ``tilt (str, float)``: angle between each consecutive shot (in radians).
-#   ``(default "uniform")``. See 3D cones
+# - ``axis_tilt (str, float)``: angle between each consecutive shot (in radians)
+#   while descending over the :math:`k_z`-axis ``(default "golden")``. See 3D cones
+# - ``spiral_tilt (str, float)``: angle of the spiral within its own axis,
+#   defined from center to its outermost point ``(default "golden")``.
 # - ``in_out (bool)``: define whether the shots should travel toward the center
 #   then outside (in-out) or not (center-out). ``(default False)``. See 3D cones
 #
 
 trajectory = mn.initialize_3D_seiffert_spiral(Nc, Ns, in_out=in_out)
 show_trajectory(trajectory, figure_size=figure_size, one_shot=one_shot)
 
@@ -472,17 +493,70 @@
 #
 # Number of revolutions, or simply the number of times a curve reaches its
 # original orientation. For regular Seiffert spirals, it corresponds to the
 # number of times the shot reaches the starting pole of the sphere. It
 # subsequently defines the length of the curve.
 #
 
-arguments = [0.5, 1, 1.5, 2]
+arguments = [0, 0.5, 1, 2]
+function = lambda x: mn.initialize_3D_seiffert_spiral(
+    Nc,
+    Ns,
+    in_out=in_out,
+    nb_revolutions=x,
+)
+show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
+
+
+# %%
+# ``axis_tilt (str, float)``
+# ~~~~~~~~~~~~~~~~~~~~~~~~~~
+#
+# Angle between consecutive shots while descending along the :math:`k_z`-axis.
+# The ``"golden"`` value chosen as default provides an almost even distribution
+# over the k-space sphere by relying on Fibonacci lattice, and therefore it should
+# be changed carefully when relevant.
+#
+# Note that in the examples below, the ``spiral_tilt`` argument is set to 0
+# for clarity.
+#
+
+arguments = [0, "uniform", "golden", 20 * 2 * np.pi / Nc]
 function = lambda x: mn.initialize_3D_seiffert_spiral(
-    Nc, Ns, in_out=in_out, nb_revolutions=x
+    Nc,
+    Ns,
+    in_out=in_out,
+    axis_tilt=x,
+    spiral_tilt=0,
+)
+show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
+
+
+# %%
+# ``spiral_tilt (str, float)``
+# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+#
+# Define the angle of the spiral within its own axis after precession of the spiral
+# along the :math:`k_z`-axis. Since the precession is applied through Rodrigues'
+# coefficients and Seiffert spirals are asymetric, their orientation right after
+# the precession can be quite biased and yield unbalanced densities.
+#
+# The method proposed in [SMR18]_ to handle that issue is to rotate the spirals
+# along their own axes, but the exact way to choose the rotation is not specified.
+# Rather than picking random angles, we decided to provide the conventional "tilt"
+# argument.
+#
+
+arguments = [0, "uniform", "golden", 20 * 2 * np.pi / Nc]
+function = lambda x: mn.initialize_3D_seiffert_spiral(
+    Nc,
+    Ns,
+    in_out=in_out,
+    axis_tilt="golden",
+    spiral_tilt=x,
 )
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
 
 # %%
 # Shell trajectories
 # ==================
```

### Comparing `mri_nufft-0.6.2/examples/example_density.py` & `mri_nufft-0.7.0/examples/example_density.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/examples/example_display_config.py` & `mri_nufft-0.7.0/examples/example_display_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # %%
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
 from mrinufft import displayConfig, display_2D_trajectory, display_3D_trajectory
 from mrinufft.trajectories import (
-    initialize_2D_radial,
-    initialize_3D_cones,
-    initialize_3D_floret,
+    initialize_2D_spiral,
+    conify,
 )
 
 # Trajectory parameters
 Nc = 120  # Number of shots
 Ns = 500  # Number of samples per shot
 
 # Display parameters
@@ -50,15 +49,15 @@
 # %%
 #
 # Trajectory displays
 # ====================
 # To show case the display parameters of trajectories, we will use the following trajectory
 # The effect of trajectory parameter are explained in the :ref:`sphx_glr_generated_autoexamples_example_3D_trajectories.py` Example.
 
-traj = initialize_3D_floret(Nc, Ns, nb_cones=6)[::-1]
+traj = conify(initialize_2D_spiral(Nc // 6, Ns), nb_cones=6)[::-1]
 
 # %%
 # ``linewidth``
 # -------------
 # The linewidth of the shot can be updated to have more or less empty space in the plot.
 show_traj(traj, "linewidth", [0.5, 2, 4])
```

### Comparing `mri_nufft-0.6.2/examples/example_readme.py` & `mri_nufft-0.7.0/examples/example_readme.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/examples/example_stacked.py` & `mri_nufft-0.7.0/examples/example_stacked.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/examples/example_trajectory_tools.py` & `mri_nufft-0.7.0/examples/example_trajectory_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -125,19 +125,14 @@
         Nc // nb_repetitions, Ns, in_out=in_out, nb_zigzags=nb_zigzags
     )[:1],
     "3D Cones": mn.initialize_3D_cones(Nc, Ns, in_out=in_out, nb_zigzags=nb_zigzags)[
         :1
     ],
 }
 
-# Adjust the trajectory direction
-single_trajectories["3D Cones"] = np.roll(
-    single_trajectories["3D Cones"], axis=-1, shift=1
-)
-
 # %%
 
 arguments = ["Radial", "Spiral", "2D Cones", "3D Cones"]
 function = lambda x: single_trajectories[x]
 show_argument(function, arguments, one_shot=bool(one_shot), subfig_size=subfigure_size)
 
 
@@ -301,15 +296,17 @@
 # been used in the literature to rotate planes around one axis to
 # create 3D trajectories, but the density (and redundancy) along that
 # axis is then much greater than anywhere else.
 #
 
 arguments = ["Radial", "Spiral", "2D Cones", "3D Cones"]
 function = lambda x: tools.rotate(
-    planar_trajectories[x], nb_rotations=nb_repetitions, x_tilt="uniform"
+    planar_trajectories[x],
+    nb_rotations=nb_repetitions,
+    x_tilt="uniform",
 )
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 # %%
 show_argument(
     function,
     arguments,
     one_shot=one_shot,
@@ -320,66 +317,253 @@
 
 
 # %%
 # Precess
 # -------
 #
 # A method to duplicate a trajectory while applying a
-# precession-like rotation around the :math:`k_x`-axis.
+# precession-like rotation around a provided axis.
 #
 # Arguments:
 #
 # - ``trajectory (array)``: array of k-space coordinates of
 #   size :math:`(N_c, N_s, N_d)`
 # - ``nb_rotations (int)``: number of rotations repeating ``trajectory``
 #   over the :math:`k_z`-axis.
-# - ``z_tilt (float)``: angle tilt between consecutive stacks
-#   over the :math:`k_z`-axis. ``(default "golden")``
+# - ``tilt (float)``: angle tilt between consecutive rotations
+#   around the :math:`k_z`-axis. ``(default "golden")``
 # - ``half_sphere (bool)``: whether the precession should be limited
 #   to the upper half of the k-space sphere, typically for in-out
 #   trajectories or planes. ``(default False)``
+# - ``partition (str)``: partition type between an "axial" or "polar"
+#   split of the :math:`k_z`-axis, designating whether the axis should
+#   be fragmented by radius or angle respectively. ``(default "axial")``
+# - ``axis (int, array)``: axis selected for alignment reference
+#   when rotating the trajectory around the :math:`k_z`-axis,
+#   generally corresponding to the shot direction for
+#   single shot ``trajectory`` inputs. It can either be an integer for
+#   one of the three k-space axes, or directly a 3D array.
+#   The default behavior when ``None`` is to select the last coordinate
+#   of the first shot as the axis. ``(default None)``
 #
 
 trajectory = tools.precess(
-    planar_trajectories["Radial"], nb_rotations=nb_repetitions, z_tilt="golden"
+    planar_trajectories["Radial"],
+    nb_rotations=nb_repetitions,
+    tilt="golden",
+    half_sphere=in_out,
+    axis=2,
 )
 show_trajectory(trajectory, figure_size=figure_size, one_shot=one_shot)
 
 # %%
 # ``trajectory (array)``
 # ~~~~~~~~~~~~~~~~~~~~~~
 #
 # This method provides a way to distribute duplicated trajectories
-# (planes or anything else) to cover evenly polar angles, while
-# tilting the azimuthal orientation.
+# (single shots, planes or anything else) to cover evenly a provided
+# axis tilting the azimuthal orientation.
 #
 
 arguments = ["Radial", "Spiral", "2D Cones", "3D Cones"]
 function = lambda x: tools.precess(
-    planar_trajectories[x], nb_rotations=nb_repetitions, z_tilt="golden"
+    planar_trajectories[x],
+    nb_rotations=nb_repetitions,
+    tilt="golden",
+    half_sphere=in_out,
+    axis=2,
 )
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
 # %%
 #
 # It is however most often used with single shots to
 # cover more evenly the k-space sphere, such as with 3D cones
 # or Seiffert spirals. Indeed, applying a precession with
 # the golden angle is known to approximate an even distribution
 # of points over a sphere surface.
 #
 
 arguments = ["Radial", "Spiral", "2D Cones", "3D Cones"]
 function = lambda x: tools.precess(
-    single_trajectories[x], nb_rotations=Nc, z_tilt="golden"
+    single_trajectories[x],
+    nb_rotations=Nc,
+    tilt="golden",
+    half_sphere=in_out,
+    axis=0,
 )
 show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
 
 
 # %%
+# ``half_sphere (bool)``
+# ~~~~~~~~~~~~~~~~~~~~~~
+#
+# Whether the precession should be limited to the upper half
+# of the k-space sphere (with respect to the provided axis).
+# It is typically used for in-out trajectories or planes, as
+# otherwise shots would likely be stacked in a redundant way.
+#
+# In the example hereafter, center-out shots are shown for clarity.
+#
+
+
+arguments = [True, False]
+function = lambda x: tools.precess(
+    single_trajectories["Radial"][:, Ns // (1 + in_out) :],
+    nb_rotations=Nc,
+    tilt="golden",
+    half_sphere=x,
+    axis=0,
+)
+show_argument(
+    function,
+    arguments,
+    one_shot=one_shot,
+    subfig_size=subfigure_size,
+    dim="2D",
+    axes=(0, 2),
+)
+
+
+# %%
+# ``partition (str)``
+# ~~~~~~~~~~~~~~~~~~~
+#
+# Partition type between an "axial" or "polar"
+# split of the :math:`k_z`-axis, designating whether the axis should
+# be fragmented by radius or angle respectively.
+#
+
+arguments = ["axial", "polar"]
+function = lambda x: tools.precess(
+    single_trajectories["Radial"],
+    nb_rotations=Nc,
+    tilt=None,
+    partition=x,
+    axis=0,
+)
+show_argument(
+    function,
+    arguments,
+    one_shot=one_shot,
+    subfig_size=subfigure_size,
+    dim="2D",
+    axes=(0, 2),
+)
+
+# %%
+#
+# While "polar" looks more natural in the absence of rotation (``tilt=None``),
+# it results in too many shots close to the rotation axis, and therefore
+# a non-uniform density. The best approximation of a uniform distribution
+# is obtained with an "axial" partition and "golden" tilt along
+# the provided axis.
+#
+
+arguments = ["axial", "polar"]
+function = lambda x: tools.precess(
+    single_trajectories["Radial"],
+    nb_rotations=Nc,
+    tilt="golden",
+    partition=x,
+    axis=0,
+)
+show_argument(
+    function,
+    arguments,
+    one_shot=one_shot,
+    subfig_size=subfigure_size,
+    dim="2D",
+    axes=(0, 2),
+)
+
+# %%
+#
+# The distribution over the k-space sphere surface can be shown by
+# displaying only the tip of the shots.
+#
+
+arguments = ["axial", "polar"]
+function = lambda x: tools.precess(
+    single_trajectories["Radial"][:, -5:],
+    nb_rotations=Nc,
+    tilt="golden",
+    partition=x,
+    axis=0,
+)
+show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
+
+# %%
+# ``axis (int, array)``
+# ~~~~~~~~~~~~~~~~~~~~~
+#
+# Axis selected for alignment reference when rotating the trajectory
+# around the :math:`k_z`-axis, generally corresponding to the
+# shot direction for single shot ``trajectory`` inputs.
+# It can either be an integer for one of the three k-space axes,
+# or directly a 3D array. The default behavior when `None`
+# is to select the last coordinate of the first shot as the axis.
+#
+# This argument is simple to select but still important, as the
+# precession relies on Rodrigues' rotation coefficients that enable
+# a rotation from one vector to another to align the trajectory
+# through the provided axis with the precession vectors all over
+# the k-space sphere. However, misalignement between shots and the
+# provided axis will result in a non-uniform distribution, as the
+# rotation around the axis is unfavorably deterministic.
+#
+# The first case is single shots, where the provided axis should
+# simply correspond to the shot axis.
+#
+
+arguments = [None, 0, 1, 2]
+function = lambda x: tools.precess(
+    single_trajectories["Radial"],
+    nb_rotations=Nc,
+    tilt="golden",
+    half_sphere=in_out,
+    axis=x,
+)
+show_argument(
+    function,
+    arguments,
+    one_shot=one_shot,
+    subfig_size=subfigure_size,
+    dim="2D",
+    axes=(1, 2),
+)
+
+# %%
+#
+# The second case is planar trajectories, where the axis orthogonal
+# to the shots plane is preferred.
+#
+
+arguments = [None, 0, 1, 2]
+function = lambda x: tools.precess(
+    planar_trajectories["Radial"],
+    nb_rotations=nb_repetitions,
+    tilt="golden",
+    half_sphere=in_out,
+    axis=x,
+)
+show_argument(function, arguments, one_shot=one_shot, subfig_size=subfigure_size)
+
+# %%
+#
+# Some trickier cases exist in the literature, with the example of Seiffert spirals.
+# Those 3D spirals neither correspond to a single-axis shot or a plane, so the authors
+# chose to use the center-out axis of each shot as a reference axis for the rotation.
+# In order to handle the redundant distribution, they added a pseudo-random rotation
+# within the shot axes.
+#
+
+
+# %%
 # Conify
 # ------
 #
 # A tool to distort trajectories into multiple cones
 # positioned to cover the k-space sphere.
 #
 # Arguments:
@@ -390,14 +574,16 @@
 #   with conical distortion over the :math:`k_z`-axis.
 # - ``z_tilt (float)``: angle tilt between consecutive cones
 #   around the :math:`k_z`-axis. ``(default "golden")``
 # - ``in_out (bool)``: whether to account for the in-out
 #   nature of some trajectories to avoid hard angles
 #   around the center, ``(default False)``
 # - ``max_angle (float)``: maximum angle of the cones. ``(default pi / 2)``
+# - ``borderless (bool)``: Whether the cones should reach `max_angle` or not,
+#   mostly to avoid 1D cones if ``max_angle`` is equal to pi / 2, by default True.
 #
 
 trajectory = tools.conify(
     planar_trajectories["Radial"], nb_cones=nb_repetitions, in_out=in_out
 )
 show_trajectory(trajectory, figure_size=figure_size, one_shot=one_shot)
 
@@ -469,14 +655,41 @@
 )
 show_argument(
     function,
     arguments,
     one_shot=one_shot,
     subfig_size=subfigure_size,
     dim="2D",
+    axes=(0, 2),
+)
+
+
+# %%
+# ``borderless (bool)``
+# ~~~~~~~~~~~~~~~~~~~~~
+#
+# Define whether or not the edge cones should reach ``max_angle``
+# when equal to ``False``, or instead simply partition the
+# sphere over a polar split.
+#
+
+arguments = [True, False]
+function = lambda x: tools.conify(
+    planar_trajectories["Radial"],
+    nb_cones=nb_repetitions,
+    in_out=in_out,
+    max_angle=np.pi / 2,
+    borderless=x,
+)
+show_argument(
+    function,
+    arguments,
+    one_shot=one_shot,
+    subfig_size=subfigure_size,
+    dim="2D",
     axes=(0, 2),
 )
 
 
 # %%
 # Functional tools
 # ================
```

### Comparing `mri_nufft-0.6.2/pyproject.toml` & `mri_nufft-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mri_nufft.egg-info/PKG-INFO` & `mri_nufft-0.7.0/src/mri_nufft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.6.2
+Version: 0.7.0
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `mri_nufft-0.6.2/src/mri_nufft.egg-info/SOURCES.txt` & `mri_nufft-0.7.0/src/mri_nufft.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 examples/README.rst
 examples/__init__.py
 examples/conftest.py
 examples/example_2D_trajectories.py
 examples/example_3D_trajectories.py
 examples/example_density.py
 examples/example_display_config.py
+examples/example_gif_2D.py
+examples/example_gif_3D.py
 examples/example_readme.py
 examples/example_stacked.py
 examples/example_trajectory_tools.py
 src/mri_nufft.egg-info/PKG-INFO
 src/mri_nufft.egg-info/SOURCES.txt
 src/mri_nufft.egg-info/dependency_links.txt
 src/mri_nufft.egg-info/requires.txt
@@ -66,14 +68,15 @@
 src/mrinufft/operators/interfaces/tfnufft.py
 src/mrinufft/operators/interfaces/utils/__init__.py
 src/mrinufft/operators/interfaces/utils/css_color.txt
 src/mrinufft/operators/interfaces/utils/gpu_utils.py
 src/mrinufft/operators/interfaces/utils/utils.py
 src/mrinufft/trajectories/__init__.py
 src/mrinufft/trajectories/display.py
+src/mrinufft/trajectories/maths.py
 src/mrinufft/trajectories/tools.py
 src/mrinufft/trajectories/trajectory2D.py
 src/mrinufft/trajectories/trajectory3D.py
 src/mrinufft/trajectories/utils.py
 tests/case_trajectories.py
 tests/conftest.py
 tests/test_density.py
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/__init__.py` & `mri_nufft-0.7.0/src/mrinufft/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,22 @@
     initialize_3D_cones,
     initialize_3D_floret,
     initialize_3D_wave_caipi,
     initialize_3D_seiffert_spiral,
     initialize_3D_helical_shells,
     initialize_3D_annular_shells,
     initialize_3D_seiffert_shells,
+    stack,
+    rotate,
+    precess,
+    conify,
+    stack_spherically,
+    shellify,
+    duplicate_along_axes,
+    radialize_center,
     displayConfig,
     display_2D_trajectory,
     display_3D_trajectory,
 )
 
 from .density import voronoi, cell_count, pipe, get_density
 
@@ -55,14 +63,22 @@
     "initialize_3D_cones",
     "initialize_3D_floret",
     "initialize_3D_wave_caipi",
     "initialize_3D_seiffert_spiral",
     "initialize_3D_helical_shells",
     "initialize_3D_annular_shells",
     "initialize_3D_seiffert_shells",
+    "stack",
+    "rotate",
+    "precess",
+    "conify",
+    "stack_spherically",
+    "shellify",
+    "duplicate_along_axes",
+    "radialize_center",
     "displayConfig",
     "display_2D_trajectory",
     "display_3D_trajectory",
     "voronoi",
     "cell_count",
     "pipe",
     "get_density",
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/_utils.py` & `mri_nufft-0.7.0/src/mrinufft/_utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/density/geometry_based.py` & `mri_nufft-0.7.0/src/mrinufft/density/geometry_based.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/density/nufft_based.py` & `mri_nufft-0.7.0/src/mrinufft/density/nufft_based.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/density/utils.py` & `mri_nufft-0.7.0/src/mrinufft/density/utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/io/cfl.py` & `mri_nufft-0.7.0/src/mrinufft/io/cfl.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/io/nsp.py` & `mri_nufft-0.7.0/src/mrinufft/io/nsp.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/__init__.py` & `mri_nufft-0.7.0/src/mrinufft/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/base.py` & `mri_nufft-0.7.0/src/mrinufft/operators/base.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/_cupy_kernels.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/_cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/bart.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/bart.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/cufinufft.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/finufft.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/finufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/gpunufft.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/gpunufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nfft.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nfft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nudft_numpy.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nudft_numpy.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/pynufft_cpu.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/pynufft_cpu.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/sigpy.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/sigpy.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/tfnufft.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/tfnufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/css_color.txt` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/css_color.txt`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/gpu_utils.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/utils.py` & `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/off_resonnance.py` & `mri_nufft-0.7.0/src/mrinufft/operators/off_resonnance.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/operators/stacked.py` & `mri_nufft-0.7.0/src/mrinufft/operators/stacked.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 import warnings
 
 import numpy as np
 import scipy as sp
 
 from mrinufft._utils import proper_trajectory, power_method, get_array_module, auto_cast
-from mrinufft.operators.base import FourierOperatorBase, check_backend, get_operator
+from mrinufft.operators.base import (
+    FourierOperatorBase,
+    check_backend,
+    get_operator,
+    with_numpy_cupy,
+)
 from mrinufft.operators.interfaces.utils import (
     is_cuda_array,
     is_host_array,
     pin_memory,
     sizeof_fmt,
 )
 
@@ -32,16 +37,21 @@
     ----------
     samples : array-like
         Sample locations in a 2D kspace
     shape: tuple
         Shape of the image.
     z_index: array-like
         Cartesian z index of masked plan.
-    backend: str
+    backend: str or FourierOperatorBase
         Backend to use.
+        If str, a NUFFT operator is initialized with str being a registered backend.
+        If FourierOperatorBase, operator is checked for compatibility and used as is
+        notably one should have:
+        ``n_coils = self.n_coils*len(z_index), squeeze_dims=True, smaps=None``
+
     smaps: array-like
         Sensitivity maps.
     n_coils: int
         Number of coils.
     n_batchs: int
         Number of batchs.
     **kwargs: dict
@@ -69,30 +79,56 @@
         smaps,
         n_coils=1,
         n_batchs=1,
         squeeze_dims=False,
         **kwargs,
     ):
         super().__init__()
-        samples2d, z_index_ = self._init_samples(samples, z_index, shape)
         self.shape = shape
-        self.samples = samples2d.reshape(-1, 2)
-        self.z_index = z_index_
         self.n_coils = n_coils
         self.n_batchs = n_batchs
         self.squeeze_dims = squeeze_dims
         self.smaps = smaps
-        self.operator = get_operator(backend)(
-            self.samples,
-            shape[:-1],
-            n_coils=self.n_coils * len(self.z_index),
-            smaps=None,
-            squeeze_dims=True,
-            **kwargs,
-        )
+        if isinstance(backend, str):
+            samples2d, z_index_ = self._init_samples(samples, z_index, shape)
+            self.samples = samples2d.reshape(-1, 2)
+            self.z_index = z_index_
+            self.operator = get_operator(backend)(
+                self.samples,
+                shape[:-1],
+                n_coils=self.n_coils * len(self.z_index),
+                smaps=None,
+                squeeze_dims=True,
+                **kwargs,
+            )
+        elif isinstance(backend, FourierOperatorBase):
+            # get all the interesting values from the operator
+            if backend.shape != shape[:-1]:
+                raise ValueError("Backend operator should have compatible shape")
+
+            samples2d, z_index_ = self._init_samples(backend.samples, z_index, shape)
+            self.samples = samples2d.reshape(-1, 2)
+            self.z_index = z_index_
+
+            if backend.n_coils != self.n_coils * (len(z_index_)):
+                raise ValueError(
+                    "The backend operator should have ``n_coils * len(z_index)``"
+                    " specified for its coil dimension."
+                )
+            if backend.uses_sense:
+                raise ValueError("Backend operator should not uses smaps.")
+            if not backend.squeeze_dims:
+                raise ValueError("Backend operator should have ``squeeze_dims=True``")
+            self.operator = backend
+
+        else:
+            raise ValueError(
+                "backend should either be a 2D nufft operator,"
+                " or a str specifying which nufft library to use."
+            )
 
     @staticmethod
     def _init_samples(samples, z_index, shape):
         samples_dim = samples.shape[-1]
         auto_z = isinstance(z_index, str) and z_index == "auto"
         if samples_dim == len(shape) and auto_z:
             # samples describes a 3D trajectory,
@@ -141,14 +177,15 @@
     def _ifftz(data):
         """Apply IFFT on z-axis."""
         # sqrt(2) required for normalization
         return sp.fft.fftshift(
             sp.fft.ifft(sp.fft.ifftshift(data, axes=-1), axis=-1, norm="ortho"), axes=-1
         ) / np.sqrt(2)
 
+    @with_numpy_cupy
     def op(self, data, ksp=None):
         """Forward operator."""
         if self.uses_sense:
             return self._safe_squeeze(self._op_sense(data, ksp))
         return self._safe_squeeze(self._op_calibless(data, ksp))
 
     def _op_sense(self, data, ksp=None):
@@ -185,14 +222,15 @@
             tmp = np.moveaxis(tmp, -1, 1)
             tmp = tmp.reshape(C * NZ, *XYZ[:2])
             ksp[b, ...] = self.operator.op(np.ascontiguousarray(tmp))
         ksp = ksp.reshape((B, C, NZ, NS))
         ksp = ksp.reshape((B, C, NZ * NS))
         return ksp
 
+    @with_numpy_cupy
     def adj_op(self, coeffs, img=None):
         """Adjoint operator."""
         if self.uses_sense:
             return self._safe_squeeze(self._adj_op_sense(coeffs, img))
         return self._safe_squeeze(self._adj_op_calibless(coeffs, img))
 
     def _adj_op_sense(self, coeffs, img):
@@ -281,50 +319,74 @@
         smaps,
         n_coils=1,
         n_batchs=1,
         n_trans=1,
         squeeze_dims=False,
         smaps_cached=False,
         density=False,
+        backend="cufinufft",
         **kwargs,
     ):
         if not (CUPY_AVAILABLE and check_backend("cufinufft")):
             raise RuntimeError("Cupy and cufinufft are required for this backend.")
 
         if (n_batchs * n_coils) % n_trans != 0:
             raise ValueError("n_batchs * n_coils should be a multiple of n_transf")
 
-        samples2d, z_index_ = self._init_samples(samples, z_index, shape)
         self.shape = shape
-        self.samples = samples2d.reshape(-1, 2)
-        self.z_index = z_index_
         self.n_coils = n_coils
         self.n_batchs = n_batchs
         self.n_trans = n_trans
         self.squeeze_dims = squeeze_dims
+        if isinstance(backend, str):
+            samples2d, z_index_ = self._init_samples(samples, z_index, shape)
+            self.samples = samples2d.reshape(-1, 2)
+            self.z_index = z_index_
+            self.operator = get_operator(backend)(
+                self.samples,
+                shape[:-1],
+                n_coils=self.n_trans * len(self.z_index),
+                n_trans=len(self.z_index),
+                smaps=None,
+                squeeze_dims=True,
+                **kwargs,
+            )
+        elif isinstance(backend, FourierOperatorBase):
+            # get all the interesting values from the operator
+            if backend.shape != shape[:-1]:
+                raise ValueError("Backend operator should have compatible shape")
+
+            samples2d, z_index_ = self._init_samples(backend.samples, z_index, shape)
+            self.samples = samples2d.reshape(-1, 2)
+            self.z_index = z_index_
+
+            if backend.n_coils != self.n_trans * len(z_index_):
+                raise ValueError(
+                    "The backend operator should have ``n_coils * len(z_index)``"
+                    " specified for its coil dimension."
+                )
+            if backend.uses_sense:
+                raise ValueError("Backend operator should not uses smaps.")
+            if not backend.squeeze_dims:
+                raise ValueError("Backend operator should have ``squeeze_dims=True``")
+            self.operator = backend
+        else:
+            raise ValueError(
+                "backend should either be a 2D nufft operator,"
+                " or a str specifying which nufft library to use."
+            )
 
-        self.operator = get_operator("cufinufft")(
-            self.samples,
-            shape[:-1],
-            n_coils=n_trans * len(self.z_index),
-            n_trans=len(self.z_index),
-            smaps=None,
-            squeeze_dims=True,
-            density=density,
-            **kwargs,
-        )
         # Smaps support
         self.smaps = smaps
         self.smaps_cached = False
         if smaps is not None:
             if not (is_host_array(smaps) or is_cuda_array(smaps)):
                 raise ValueError(
                     "Smaps should be either a C-ordered ndarray, " "or a GPUArray."
                 )
-            self.smaps_cached = False
             if smaps_cached:
                 warnings.warn(
                     f"{sizeof_fmt(smaps.size * np.dtype(self.cpx_dtype).itemsize)}"
                     "used on gpu for smaps."
                 )
                 self.smaps = cp.array(
                     smaps, order="C", copy=False, dtype=self.cpx_dtype
@@ -363,36 +425,30 @@
                 axis=-1,
                 norm="ortho",
                 overwrite_x=False,
             ),
             axes=-1,
         )
 
+    @with_numpy_cupy
     def op(self, data, ksp=None):
         """Forward operator."""
         # Dispatch to special case.
-        xp = get_array_module(data)
-        if xp.__name__ == "torch" and data.is_cpu:
-            data = data.numpy()
         data = auto_cast(data, self.cpx_dtype)
 
         if self.uses_sense and is_cuda_array(data):
             op_func = self._op_sense_device
         elif self.uses_sense:
             op_func = self._op_sense_host
         elif is_cuda_array(data):
             op_func = self._op_calibless_device
         else:
             op_func = self._op_calibless_host
         ret = op_func(data, ksp)
 
-        if xp.__name__ == "torch" and is_cuda_array(ret):
-            ret = xp.as_tensor(ret, device=data.device)
-        elif xp.__name__ == "torch":
-            ret = xp.from_numpy(ret)
         return self._safe_squeeze(ret)
 
     def _op_sense_host(self, data, ksp=None):
         B, C, T, XYZ = self.n_batchs, self.n_coils, self.n_trans, self.shape
         NS, NZ = len(self.samples), len(self.z_index)
 
         dataf = data.reshape((B, *XYZ))
@@ -523,38 +579,31 @@
             ksp_batched = ksp_batched.reshape(T, NZ, NS)
             ksp_batched = ksp_batched.reshape(T, NZ * NS)
             ksp[i * T : (i + 1) * T] = ksp_batched
 
         ksp = ksp.reshape((B, C, NZ * NS))
         return ksp
 
+    @with_numpy_cupy
     def adj_op(self, coeffs, img=None):
         """Adjoint operator."""
         # Dispatch to special case.
-        xp = get_array_module(coeffs)
-        if xp.__name__ == "torch" and coeffs.is_cpu:
-            coeffs = coeffs.numpy()
         coeffs = auto_cast(coeffs, self.cpx_dtype)
 
         if self.uses_sense and is_cuda_array(coeffs):
             adj_op_func = self._adj_op_sense_device
         elif self.uses_sense:
             adj_op_func = self._adj_op_sense_host
         elif is_cuda_array(coeffs):
             adj_op_func = self._adj_op_calibless_device
         else:
             adj_op_func = self._adj_op_calibless_host
 
         ret = adj_op_func(coeffs, img)
 
-        if xp.__name__ == "torch" and is_cuda_array(ret):
-            ret = xp.as_tensor(ret, device=coeffs.device)
-        elif xp.__name__ == "torch":
-            ret = xp.from_numpy(ret)
-
         return self._safe_squeeze(ret)
 
     def _adj_op_sense_host(self, coeffs, img_d=None):
         B, C, T, XYZ = self.n_batchs, self.n_coils, self.n_trans, self.shape
         NS, NZ = len(self.samples), len(self.z_index)
 
         coeffs_f = coeffs.reshape(B * C, NZ * NS)
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/__init__.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,25 @@
     initialize_3D_wave_caipi,
     initialize_3D_seiffert_spiral,
     initialize_3D_helical_shells,
     initialize_3D_annular_shells,
     initialize_3D_seiffert_shells,
 )
 
+from .tools import (
+    stack,
+    rotate,
+    precess,
+    conify,
+    stack_spherically,
+    shellify,
+    duplicate_along_axes,
+    radialize_center,
+)
+
 from .display import (
     displayConfig,
     display_2D_trajectory,
     display_3D_trajectory,
 )
 
 __all__ = [
@@ -44,11 +55,19 @@
     "initialize_3D_cones",
     "initialize_3D_floret",
     "initialize_3D_wave_caipi",
     "initialize_3D_seiffert_spiral",
     "initialize_3D_helical_shells",
     "initialize_3D_annular_shells",
     "initialize_3D_seiffert_shells",
+    "stack",
+    "rotate",
+    "precess",
+    "conify",
+    "stack_spherically",
+    "shellify",
+    "duplicate_along_axes",
+    "radialize_center",
     "displayConfig",
     "display_2D_trajectory",
     "display_3D_trajectory",
 ]
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/display.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/display.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/tools.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Functions to manipulate trajectories."""
 
 import numpy as np
 
+from .maths import Rv, Rx, Ry, Rz
 from .utils import (
     KMAX,
-    Rv,
-    Rx,
-    Ry,
-    Rz,
     initialize_tilt,
 )
 
 ################
 # DIRECT TOOLS #
 ################
 
@@ -96,58 +93,101 @@
     for i in range(1, nb_rotations):
         rotation = (Rx(i * x_angle) @ Ry(i * y_angle) @ Rz(i * z_angle)).T
         new_trajectory[i] = new_trajectory[0] @ rotation
 
     return new_trajectory.reshape(nb_rotations * Nc, Ns, 3)
 
 
-def precess(trajectory, nb_rotations, z_tilt="golden", half_sphere=False):
-    """Rotate 2D or 3D trajectories as a precession around :math:`k_z`.
+def precess(
+    trajectory,
+    nb_rotations,
+    tilt="golden",
+    half_sphere=False,
+    partition="axial",
+    axis=None,
+):
+    """Rotate trajectories as a precession around the :math:`k_z`-axis.
 
     Parameters
     ----------
     trajectory : array_like
         Trajectory in 2D or 3D to rotate.
     nb_rotations : int
-        Number of rotations repeating the provided trajectory.
-    z_tilt : str, optional
-        Tilt of the trajectory over the :math:`k_z`-axis, by default "golden".
+        Number of rotations repeating the provided trajectory while precessing.
+    tilt : str, optional
+        Angle tilt between consecutive rotations around the :math:`k_z`-axis,
+        by default "golden".
     half_sphere : bool, optional
         Whether the precession should be limited to the upper half
-        of the k-space sphere, typically for in-out trajectories or planes.
+        of the k-space sphere.
+        It is typically used for in-out trajectories or planes.
+    partition : str, optional
+        Partition type between an "axial" or "polar" split of the
+        :math:`k_z`-axis, designating whether the axis should be fragmented
+        by radius or angle respectively, by default "axial".
+    axis : int, array_like, optional
+        Axis selected for alignment reference when rotating the trajectory
+        around the :math:`k_z`-axis, generally corresponding to the shot
+        direction for single shot ``trajectory`` inputs. It can either
+        be an integer for one of the three k-space axes, or directly a 3D
+        array. The default behavior when `None` is to select the last
+        coordinate of the first shot as the axis, by default `None`.
 
     Returns
     -------
     array_like
         Precessed trajectory.
     """
+    # Check for partition option error
+    if partition not in ["polar", "axial"]:
+        raise NotImplementedError(f"Unknown partition type: {partition}")
+
     # Check dimensionality and initialize output
     Nc, Ns = trajectory.shape[:2]
     if trajectory.shape[-1] == 2:
         trajectory = np.concatenate([trajectory, np.zeros((Nc, Ns, 1))], axis=-1)
     trajectory = trajectory.reshape((Nc * Ns, 3))
     new_trajectory = np.zeros((nb_rotations, Nc * Ns, 3))
 
     # Determine direction vectors on a sphere
     vectors = np.zeros((nb_rotations, 3))
-    phi = initialize_tilt(z_tilt, nb_rotations) * np.arange(nb_rotations)
-    vectors[:, 2] = np.sin(np.pi / 2 * np.linspace(-1 + half_sphere, 1, nb_rotations))
+    phi = initialize_tilt(tilt, nb_rotations) * np.arange(nb_rotations)
+    vectors[:, 2] = np.linspace(-1 + half_sphere, 1, nb_rotations)
+    if partition == "polar":
+        vectors[:, 2] = np.sin(np.pi / 2 * vectors[:, 2])
     radius = np.sqrt(1 - vectors[:, 2] ** 2)
     vectors[:, 0] = np.cos(phi) * radius
     vectors[:, 1] = np.sin(phi) * radius
 
+    # Select rotation axis when axis is not already a vector
+    if axis is None:
+        axis_vector = np.copy(trajectory[Ns - 1])
+        axis_vector /= np.linalg.norm(axis_vector)
+    elif isinstance(axis, int):
+        axis_vector = np.zeros(3)
+        axis_vector[axis] = 1
+    else:
+        axis_vector = axis
+
     # Rotate initial trajectory
     for i in np.arange(nb_rotations):
-        rotation = Rv(np.array((1, 0, 0)), vectors[i], normalize=False).T
+        rotation = Rv(axis_vector, vectors[i], normalize=False).T
         new_trajectory[i] = trajectory @ rotation
 
     return new_trajectory.reshape((nb_rotations * Nc, Ns, 3))
 
 
-def conify(trajectory, nb_cones, z_tilt=None, in_out=False, max_angle=np.pi / 2):
+def conify(
+    trajectory,
+    nb_cones,
+    z_tilt=None,
+    in_out=False,
+    max_angle=np.pi / 2,
+    borderless=True,
+):
     """Distort 2D or 3D trajectories into cones along the :math:`k_z`-axis.
 
     Parameters
     ----------
     trajectory : array_like
         Trajectory to conify.
     nb_cones : int
@@ -155,14 +195,17 @@
     z_tilt : str, optional
         Tilt of the trajectory over the :math:`k_z`-axis, by default `None`.
     in_out : bool, optional
         Whether to account for the in-out nature of some trajectories
         to avoid hard angles around the center, by default False.
     max_angle : float, optional
         Maximum angle of the cones, by default pi / 2.
+    borderless : bool, optional
+        Whether the cones should reach `max_angle` or not,
+        and avoid 1D cones if equal to pi / 2, by default True.
 
     Returns
     -------
     array_like
         Conified trajectory.
     """
     # Check dimensionality and initialize output
@@ -170,17 +213,17 @@
     if trajectory.shape[-1] == 2:
         trajectory = np.concatenate([trajectory, np.zeros((Nc, Ns, 1))], axis=-1)
     trajectory = trajectory.reshape((Nc * Ns, 3))
     new_trajectory = np.zeros((nb_cones, Nc * Ns, 3))
 
     # Initialize angles
     z_angle = initialize_tilt(z_tilt, nb_cones)
-    alphas = np.linspace(-max_angle, +max_angle, nb_cones + 2)[
-        1:-1
-    ]  # Borderless partition
+    alphas = np.linspace(-max_angle, +max_angle, nb_cones + 2 * borderless)
+    if borderless:
+        alphas = alphas[1:-1]  # Remove partition borders
 
     # Start processing the trajectory
     new_trajectory[:] = trajectory
     for i, alpha in enumerate(alphas):
         # Apply tilt
         rotation = Rz(np.abs(i - nb_cones // 2) * z_angle).T  # Symmetrical for in-out
         new_trajectory[i] = new_trajectory[i] @ rotation
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory2D.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """2D trajectory initializations."""
 
 import numpy as np
 
+from .maths import (
+    R2D,
+    compute_coprime_factors,
+)
 from .utils import (
     KMAX,
-    R2D,
     initialize_tilt,
     initialize_spiral,
-    compute_coprime_factors,
 )
 from .tools import rotate
 
 
 #####################
 # CIRCULAR PATTERNS #
 #####################
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory3D.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,104 +2,129 @@
 
 import numpy as np
 import numpy.linalg as nl
 
 from functools import partial
 from scipy.special import ellipj, ellipk
 
+from .maths import Ry, Rz, Ra, generate_fibonacci_circle, CIRCLE_PACKING_DENSITY
 from .tools import precess, conify, duplicate_along_axes
 from .trajectory2D import initialize_2D_spiral
-from .utils import Ry, Rz, initialize_tilt, initialize_shape_norm, KMAX, Packings
+from .utils import initialize_tilt, initialize_shape_norm, KMAX, Packings
 
 
 ############################
 # FREEFORM 3D TRAJECTORIES #
 ############################
 
 
-def initialize_3D_cones(Nc, Ns, tilt="golden", in_out=False, nb_zigzags=5, width=1):
+def initialize_3D_cones(
+    Nc, Ns, tilt="golden", in_out=False, nb_zigzags=5, spiral="archimedes", width=1
+):
     """Initialize 3D trajectories with cones.
 
+    Initialize a trajectory consisting of 3D cones duplicated
+    in each direction and almost evenly distributed using a Fibonacci
+    lattice spherical projection when the tilt is set to "golden".
+
+    The cone width is automatically determined based on the optimal
+    circle packing of a sphere surface, as discussed in [CK90]_.
+
     Parameters
     ----------
     Nc : int
         Number of shots
     Ns : int
         Number of samples per shot
     tilt : str, float, optional
         Tilt of the cones, by default "golden"
     in_out : bool, optional
         Whether the curves are going in-and-out or start from the center,
         by default False
     nb_zigzags : float, optional
         Number of zigzags of the cones, by default 5
+    spiral : str, float, optional
+        Spiral type, by default "archimedes"
     width : float, optional
-        Width of a cone such that 1 has no redundacy and full coverage, by default 1
+        Cone width normalized such that `width=1` avoids cone overlaps, by default 1
 
     Returns
     -------
     array_like
         3D cones trajectory
+
+    References
+    ----------
+    .. [CK90] Clare, B. W., and D. L. Kepert.
+       "The optimal packing of circles on a sphere."
+       Journal of mathematical chemistry 6, no. 1 (1991): 325-349.
     """
-    # Initialize first cone
-    radius = np.linspace(-KMAX if (in_out) else 0, KMAX, Ns)
-    angles = np.linspace(
-        -2 * np.pi * nb_zigzags if (in_out) else 0, 2 * np.pi * nb_zigzags, Ns
-    )
-    cone = np.zeros((1, Ns, 3))
-    cone[:, :, 0] = radius
-    cone[:, :, 1] = (
-        radius * np.cos(angles) * width * 2 * np.pi / Nc ** (2 / 3) / (1 + in_out)
+    # Initialize first spiral
+    spiral = initialize_2D_spiral(
+        Nc=1,
+        Ns=Ns,
+        spiral=spiral,
+        in_out=in_out,
+        nb_revolutions=nb_zigzags,
     )
-    cone[:, :, 2] = (
-        radius * np.sin(angles) * width * 2 * np.pi / Nc ** (2 / 3) / (1 + in_out)
+
+    # Estimate best cone angle based on the ratio between
+    # sphere volume divided by Nc and spherical sector packing optimaly a sphere
+    max_angle = np.pi / 2 - width * np.arccos(
+        1 - CIRCLE_PACKING_DENSITY * 2 / Nc / (1 + in_out)
     )
 
+    # Initialize first cone
+    ## Create three cones for proper partitioning, but only one is needed
+    cone = conify(
+        spiral,
+        nb_cones=3,
+        z_tilt=None,
+        in_out=in_out,
+        max_angle=max_angle,
+        borderless=False,
+    )[-1:]
+
     # Apply precession to the first cone
-    trajectory = precess(cone, nb_rotations=Nc, z_tilt=tilt)
+    trajectory = precess(
+        cone, tilt=tilt, nb_rotations=Nc, half_sphere=in_out, partition="axial", axis=2
+    )
 
     return trajectory
 
 
 def initialize_3D_floret(
     Nc,
     Ns,
     in_out=False,
     nb_revolutions=1,
-    spiral_tilt="uniform",
     spiral="fermat",
-    nb_cones=None,
     cone_tilt="golden",
     max_angle=np.pi / 2,
     axes=(2,),
 ):
     """Initialize 3D trajectories with FLORET.
 
     This implementation is based on the work from [Pip+11]_.
     The acronym FLORET stands for Fermat Looped, Orthogonally
     Encoded Trajectories. It consists of Fermat spirals
-    folded into 3D cones along the :math:`k_z`-axis.
+    folded into 3D cones along one or several axes.
 
     Parameters
     ----------
     Nc : int
         Number of shots
     Ns : int
         Number of samples per shot
     in_out : bool, optional
         Whether to start from the center or not, by default False
     nb_revolutions : float, optional
         Number of revolutions of the spirals, by default 1
-    spiral_tilt : str, float, optional
-        Tilt of the spirals around the :math:`k_z`-axis, by default "uniform"
     spiral : str, float, optional
         Spiral type, by default "fermat"
-    nb_cones : int, optional
-        Number of cones used to partition the k-space sphere,
-        with `None` making one cone per shot, by default `None`.
     cone_tilt : str, float, optional
         Tilt of the cones around the :math:`k_z`-axis, by default "golden"
     max_angle : float, optional
         Maximum polar angle starting from the :math:`k_x-k_y` plane,
         by default pi / 2
     axes : tuple, optional
         Axes over which cones are created, by default (2,)
@@ -113,40 +138,32 @@
     ----------
     .. [Pip+11] Pipe, James G., Nicholas R. Zwart, Eric A. Aboussouan,
        Ryan K. Robison, Ajit Devaraj, and Kenneth O. Johnson.
        "A new design and rationale for 3D orthogonally
        oversampled k‐space trajectories."
        Magnetic resonance in medicine 66, no. 5 (2011): 1303-1311.
     """
-    # Define variables for convenience
-    nb_cones = Nc if (nb_cones is None) else nb_cones
-    Nd = len(axes)
-    Nc_per_spiral = Nc // nb_cones
-    nb_cones_per_axis = nb_cones // Nd
-
-    # Check argument errors
-    if Nc % nb_cones != 0:
-        raise ValueError("Nc should be divisible by nb_cones.")
-    if nb_cones % Nd != 0:
-        raise ValueError("nb_cones should be divisible by len(axes).")
+    # Define convenience variables and check argument errors
+    Nc_per_axis = Nc // len(axes)
+    if Nc % len(axes) != 0:
+        raise ValueError("Nc should be divisible by len(axes).")
 
     # Initialize first spiral
     spiral = initialize_2D_spiral(
-        Nc=Nc_per_spiral,
+        Nc=1,
         Ns=Ns,
         spiral=spiral,
         in_out=in_out,
-        tilt=spiral_tilt,
         nb_revolutions=nb_revolutions,
     )
 
     # Initialize first cone
     cone = conify(
         spiral,
-        nb_cones=nb_cones_per_axis,
+        nb_cones=Nc_per_axis,
         z_tilt=cone_tilt,
         in_out=in_out,
         max_angle=max_angle,
     )
 
     # Duplicate cone along axes
     axes = [2 - ax for ax in axes]  # Default axis is kz, not kx
@@ -211,16 +228,16 @@
 
     # Initialize first shot
     angles = nb_revolutions * 2 * np.pi * np.arange(0, Ns) / Ns
     trajectory[0, :, 0] = width * np.cos(angles)
     trajectory[0, :, 1] = width * np.sin(angles)
     trajectory[0, :, 2] = np.linspace(-1, 1, Ns)
 
+    # Choose the helix positions according to packing
     packing = Packings[packing]
-    # Packing
     side = 2 * int(np.ceil(np.sqrt(Nc))) * np.max(spacing)
     if packing == Packings.RANDOM:
         positions = 2 * side * (np.random.random((side * side, 2)) - 0.5)
     elif packing == Packings.CIRCLE:
         positions = [[0, 0]]
         counter = 0
         while len(positions) < side**2:
@@ -244,14 +261,21 @@
     if packing in [Packings.HEXAGON, Packings.TRIANGLE]:
         # Hexagonal/triangular packing based on square packing
         positions[::2, 1] += 1 / 2
         positions[1::2, 1] -= 1 / 2
         ratio = nl.norm(np.diff(positions[:2], axis=-1))
         positions[:, 0] /= ratio / 2
 
+    if packing == Packings.FIBONACCI:
+        # Estimate helix width based on the k-space 2D surface
+        # and an optimal circle packing
+        positions = np.sqrt(
+            Nc * 2 / CIRCLE_PACKING_DENSITY
+        ) * generate_fibonacci_circle(Nc * 2)
+
     # Remove points by distance to fit both shape and Nc
     main_order = initialize_shape_norm(shape)
     tie_order = 2 if (main_order != 2) else np.inf  # breaking ties
     positions = np.array(positions) * spacing
     positions = sorted(positions, key=partial(nl.norm, ord=tie_order))
     positions = sorted(positions, key=partial(nl.norm, ord=main_order))
     positions = positions[:Nc]
@@ -263,15 +287,21 @@
         trajectory[i] = initial_shot + positions[i]
 
     trajectory[..., :2] /= np.max(np.abs(trajectory))
     return KMAX * trajectory
 
 
 def initialize_3D_seiffert_spiral(
-    Nc, Ns, curve_index=0.2, nb_revolutions=1, tilt="golden", in_out=False
+    Nc,
+    Ns,
+    curve_index=0.2,
+    nb_revolutions=1,
+    axis_tilt="golden",
+    spiral_tilt="golden",
+    in_out=False,
 ):
     """Initialize 3D trajectories with modulated Seiffert spirals.
 
     Initially introduced in [SMR18]_, but also proposed later as "Yarnball"
     in [SB21]_ as a nod to [IN95]_. The implementation is based on work
     from [Er00]_ and [Br09]_, using Jacobi elliptic functions rather than
     auxiliary theta functions.
@@ -283,16 +313,19 @@
     Ns : int
         Number of samples per shot
     curve_index : float
         Index controlling curve from 0 (flat) to 1 (curvy), by default 0.3
     nb_revolutions : float
         Number of revolutions, i.e. times the polar angle of the curves
         passes through 0, by default 1
-    tilt : str, float, optional
-        Angle between shots around z-axis over precession, by default "golden"
+    axis_tilt : str, float, optional
+        Angle between shots over a precession around the z-axis, by default "golden"
+    spiral_tilt : str, float, optional
+        Angle of the spiral within its own axis defined from center to its outermost
+        point, by default "golden"
     in_out : bool
         Whether the curves are going in-and-out or start from the center,
         by default False
 
     Returns
     -------
     array_like
@@ -330,15 +363,28 @@
     spiral[0, :, 2] = jacobi[1]
 
     # Make it volumetric instead of just a sphere surface
     magnitudes = np.sqrt(np.linspace(0, 1, Ns // (1 + in_out)))
     spiral = magnitudes.reshape((1, -1, 1)) * spiral
 
     # Apply precession to the first spiral
-    trajectory = precess(spiral, nb_rotations=Nc, z_tilt=tilt)
+    trajectory = precess(
+        spiral,
+        tilt=axis_tilt,
+        nb_rotations=Nc,
+        half_sphere=in_out,
+        partition="axial",
+        axis=None,
+    )
+
+    # Tilt the spiral along its own axis
+    for i in range(Nc):
+        angle = i * initialize_tilt(spiral_tilt)
+        rotation = Ra(trajectory[i, -1], angle).T
+        trajectory[i] = trajectory[i] @ rotation
 
     # Handle in_out case
     if in_out:
         first_half_traj = np.copy(trajectory)
         first_half_traj = -first_half_traj[:, ::-1]
         trajectory = np.concatenate([first_half_traj, trajectory], axis=1)
     return KMAX * trajectory
```

### Comparing `mri_nufft-0.6.2/src/mrinufft/trajectories/utils.py` & `mri_nufft-0.7.0/src/mrinufft/trajectories/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utility functions for the trajectory design."""
 
-import numpy as np
-
 from enum import Enum, EnumMeta
+from numbers import Real
 
+import numpy as np
 
 #############
 # CONSTANTS #
 #############
 
 KMAX = 0.5
 
@@ -128,20 +128,22 @@
     """
 
     RANDOM = "random"
     CIRCLE = "circle"
     TRIANGLE = "triangle"
     HEXAGON = "hexagon"
     SQUARE = "square"
+    FIBONACCI = "fibonacci"
 
     # Aliases
     CIRCULAR = CIRCLE
     TRIANGULAR = TRIANGLE
     HEXAGONAL = HEXAGON
     UNIFORM = RANDOM
+    SPIRAL = FIBONACCI
 
 
 ###############
 # CONSTRAINTS #
 ###############
 
 
@@ -276,15 +278,15 @@
     """
     # Handle no initial positions
     if initial_positions is None:
         initial_positions = np.zeros((gradients.shape[0], 1, gradients.shape[-1]))
 
     # Prepare and integrate gradients
     trajectory = gradients * gamma * raster_time
-    trajectory = np.concatenate([initial_positions, trajectory])
+    trajectory = np.concatenate([initial_positions[:, None, :], trajectory], axis=1)
     trajectory = np.cumsum(trajectory, axis=1)
 
     # Normalize the trajectory for NUFFT usage
     trajectory = normalize_trajectory(trajectory, norm_factor, resolution)
     return trajectory
 
 
@@ -342,15 +344,15 @@
     """
     # Handle no initial gradients
     if initial_gradients is None:
         initial_gradients = np.zeros((slewrates.shape[0], 1, slewrates.shape[-1]))
 
     # Prepare and integrate slew rates
     gradients = slewrates * raster_time
-    gradients = np.concatenate([initial_gradients, gradients])
+    gradients = np.concatenate([initial_gradients[:, None, :], gradients], axis=1)
     gradients = np.cumsum(gradients, axis=1)
     return gradients
 
 
 def compute_gradients_and_slew_rates(
     trajectory,
     norm_factor=KMAX,
@@ -431,179 +433,14 @@
         Maximum slew rate in T/m/ms.
     """
     max_grad = np.max(np.linalg.norm(gradients, axis=-1, ord=order))
     max_slew = np.max(np.linalg.norm(slewrates, axis=-1, ord=order))
     return (max_grad < gmax) and (max_slew < smax), max_grad, max_slew
 
 
-###############
-# MATHEMATICS #
-###############
-
-
-def compute_greatest_common_divider(p, q):
-    """Compute the greatest common divider of two integers p and q.
-
-    Parameters
-    ----------
-    p : int
-        First integer.
-    q : int
-        Second integer.
-
-    Returns
-    -------
-    int
-        The greatest common divider of p and q.
-    """
-    while q != 0:
-        p, q = q, p % q
-    return p
-
-
-def compute_coprime_factors(Nc, length, start=1, update=1):
-    """Compute a list of coprime factors of Nc.
-
-    Parameters
-    ----------
-    Nc : int
-        Number to factorize.
-    length : int
-        Number of coprime factors to compute.
-    start : int, optional
-        First number to check. The default is 1.
-    update : int, optional
-        Increment between two numbers to check. The default is 1.
-
-    Returns
-    -------
-    list
-        List of coprime factors of Nc.
-    """
-    count = start
-    coprimes = []
-    while len(coprimes) < length:
-        if compute_greatest_common_divider(Nc, count) == 1:
-            coprimes.append(count)
-        count += update
-    return coprimes
-
-
-#############
-# ROTATIONS #
-#############
-
-
-def R2D(theta):
-    """Initialize 2D rotation matrix.
-
-    Parameters
-    ----------
-    theta : float
-        Rotation angle in rad.
-
-    Returns
-    -------
-    np.ndarray
-        2D rotation matrix.
-    """
-    return np.array([[np.cos(theta), -np.sin(theta)], [np.sin(theta), np.cos(theta)]])
-
-
-def Rx(theta):
-    """Initialize 3D rotation matrix around x axis.
-
-    Parameters
-    ----------
-    theta : float
-        Rotation angle in rad.
-
-    Returns
-    -------
-    np.ndarray
-        2D rotation matrix.
-    """
-    return np.array(
-        [
-            [1, 0, 0],
-            [0, np.cos(theta), -np.sin(theta)],
-            [0, np.sin(theta), np.cos(theta)],
-        ]
-    )
-
-
-def Ry(theta):
-    """Initialize 3D rotation matrix around y axis.
-
-    Parameters
-    ----------
-    theta : float
-        Rotation angle in rad.
-
-    Returns
-    -------
-    np.ndarray
-        2D rotation matrix.
-    """
-    return np.array(
-        [
-            [np.cos(theta), 0, np.sin(theta)],
-            [0, 1, 0],
-            [-np.sin(theta), 0, np.cos(theta)],
-        ]
-    )
-
-
-def Rz(theta):
-    """Initialize 3D rotation matrix around z axis.
-
-    Parameters
-    ----------
-    theta : float
-        Rotation angle in rad.
-
-    Returns
-    -------
-    np.ndarray
-        2D rotation matrix.
-    """
-    return np.array(
-        [
-            [np.cos(theta), -np.sin(theta), 0],
-            [np.sin(theta), np.cos(theta), 0],
-            [0, 0, 1],
-        ]
-    )
-
-
-def Rv(v1, v2, normalize=True):
-    """Initialize 3D rotation matrix from two vectors.
-
-    Parameters
-    ----------
-    v1 : np.ndarray
-        First vector.
-    v2 : np.ndarray
-        Second vector.
-    normalize : bool, optional
-        Normalize the vectors. The default is True.
-
-    Returns
-    -------
-    np.ndarray
-        3D rotation matrix.
-    """
-    if normalize:
-        v1, v2 = v1 / np.linalg.norm(v1), v2 / np.linalg.norm(v2)
-    cos_theta = np.dot(v1, v2)
-    v3 = np.cross(v1, v2)
-    cross_matrix = np.cross(v3, np.identity(v3.shape[0]) * -1)
-    return np.identity(3) + cross_matrix + cross_matrix @ cross_matrix / (1 + cos_theta)
-
-
 ###########
 # OPTIONS #
 ###########
 
 
 def initialize_tilt(tilt, nb_partitions=1):
     r"""Initialize the tilt angle.
@@ -626,15 +463,15 @@
         If the tilt name is unknown.
 
     See Also
     --------
     Tilts
 
     """
-    if not (isinstance(tilt, str) or tilt is None):
+    if isinstance(tilt, Real):
         return tilt
     elif tilt is None or tilt == Tilts.NONE:
         return 0
     elif tilt == Tilts.UNIFORM:
         return 2 * np.pi / nb_partitions
     elif tilt == Tilts.INTERGAPS:
         return np.pi / nb_partitions / 2
@@ -657,15 +494,15 @@
         Spiral type or spiral power value.
 
     Returns
     -------
     float
         Spiral power value.
     """
-    if isinstance(spiral, float):
+    if isinstance(spiral, Real):
         return spiral
     return Spirals[spiral]
 
 
 def initialize_shape_norm(shape):
     """Initialize the norm for a given shape.
 
@@ -675,10 +512,10 @@
         Shape name or p-norm value.
 
     Returns
     -------
     float
         Shape p-norm value.
     """
-    if isinstance(shape, float):
+    if isinstance(shape, Real):
         return shape
     return NormShapes[shape]
```

### Comparing `mri_nufft-0.6.2/tests/case_trajectories.py` & `mri_nufft-0.7.0/tests/case_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/conftest.py` & `mri_nufft-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/helpers/__init__.py` & `mri_nufft-0.7.0/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/helpers/asserts.py` & `mri_nufft-0.7.0/tests/helpers/asserts.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/helpers/factories.py` & `mri_nufft-0.7.0/tests/helpers/factories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/operators/test_batch.py` & `mri_nufft-0.7.0/tests/operators/test_batch.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/operators/test_bindings.py` & `mri_nufft-0.7.0/tests/operators/test_bindings.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/operators/test_gpunufft.py` & `mri_nufft-0.7.0/tests/operators/test_gpunufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/operators/test_interfaces.py` & `mri_nufft-0.7.0/tests/operators/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/operators/test_stacked.py` & `mri_nufft-0.7.0/tests/operators/test_stacked.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,7 +130,23 @@
 
     traj3d = stacked2traj3d(traj2d, z_index, dimz)
 
     traj2d, z_index2 = traj3d2stacked(traj3d, dimz)
 
     npt.assert_allclose(traj2d, traj2d)
     npt.assert_allclose(z_index, z_index2)
+
+
+def test_stack_reuse(operator, stacked_op):
+    """Test the reuse of the stacked operator."""
+    nufft_2d = stacked_op.operator
+
+    reuse_op = MRIStackedNUFFT(
+        backend=nufft_2d,
+        shape=stacked_op.shape,
+        samples=stacked_op.samples,
+        z_index=stacked_op.z_index,
+        n_coils=stacked_op.n_coils,
+        n_batchs=stacked_op.n_batchs,
+        smaps=stacked_op.smaps,
+    )
+    assert reuse_op.operator is nufft_2d
```

### Comparing `mri_nufft-0.6.2/tests/operators/test_stacked_gpu.py` & `mri_nufft-0.7.0/tests/operators/test_stacked_gpu.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/test_density.py` & `mri_nufft-0.7.0/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/test_io.py` & `mri_nufft-0.7.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.6.2/tests/test_ndft.py` & `mri_nufft-0.7.0/tests/test_ndft.py`

 * *Files identical despite different names*

