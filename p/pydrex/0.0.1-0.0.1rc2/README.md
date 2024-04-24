# Comparing `tmp/pydrex-0.0.1.tar.gz` & `tmp/pydrex-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrex-0.0.1.tar", last modified: Wed Apr 24 07:38:46 2024, max compression
+gzip compressed data, was "pydrex-0.0.1rc2.tar", last modified: Wed Apr  3 09:34:07 2024, max compression
```

## Comparing `pydrex-0.0.1.tar` & `pydrex-0.0.1rc2.tar`

### file list

```diff
@@ -1,133 +1,127 @@
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.051064 pydrex-0.0.1/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.012064 pydrex-0.0.1/.github/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.038064 pydrex-0.0.1/.github/workflows/
--rw-r--r--   0 leon      (1001) leon      (1001)     1916 2024-04-24 07:20:50.000000 pydrex-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 leon      (1001) leon      (1001)     1203 2024-04-24 07:20:50.000000 pydrex-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 leon      (1001) leon      (1001)     1166 2024-02-26 22:21:28.000000 pydrex-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 leon      (1001) leon      (1001)      293 2024-04-24 07:34:56.000000 pydrex-0.0.1/CHANGELOG.md
--rw-r--r--   0 leon      (1001) leon      (1001)    35149 2022-10-30 09:44:13.000000 pydrex-0.0.1/LICENSE
--rw-r--r--   0 leon      (1001) leon      (1001)    44499 2024-04-24 07:38:46.051064 pydrex-0.0.1/PKG-INFO
--rw-r--r--   0 leon      (1001) leon      (1001)     2177 2024-04-24 07:33:55.000000 pydrex-0.0.1/README.md
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.012064 pydrex-0.0.1/docs/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.038064 pydrex-0.0.1/docs/assets/
--rw-r--r--   0 leon      (1001) leon      (1001)    80910 2023-08-26 02:58:48.000000 pydrex-0.0.1/docs/assets/pydrex.png
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.039064 pydrex-0.0.1/docs/template/
--rw-r--r--   0 leon      (1001) leon      (1001)     1022 2023-08-26 02:58:48.000000 pydrex-0.0.1/docs/template/index.html.jinja2
--rw-r--r--   0 leon      (1001) leon      (1001)     1955 2023-06-23 00:10:13.000000 pydrex-0.0.1/docs/template/math.html.jinja2
--rw-r--r--   0 leon      (1001) leon      (1001)       98 2023-06-23 00:10:14.000000 pydrex-0.0.1/docs/template/module.html.jinja2
--rw-r--r--   0 leon      (1001) leon      (1001)     9390 2023-06-23 00:10:14.000000 pydrex-0.0.1/docs/template/syntax-highlighting.css
--rw-r--r--   0 leon      (1001) leon      (1001)     1330 2023-08-26 02:58:48.000000 pydrex-0.0.1/docs/template/theme.css
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.013064 pydrex-0.0.1/examples/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.039064 pydrex-0.0.1/examples/fluidity/
--rw-r--r--   0 leon      (1001) leon      (1001)      769 2024-03-28 10:06:39.000000 pydrex-0.0.1/examples/fluidity/README.md
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.040064 pydrex-0.0.1/examples/fluidity/advection2d/
--rw-r--r--   0 leon      (1001) leon      (1001)     2078 2024-03-27 11:33:35.000000 pydrex-0.0.1/examples/fluidity/advection2d/Makefile
--rw-r--r--   0 leon      (1001) leon      (1001)    12703 2024-03-28 10:06:39.000000 pydrex-0.0.1/examples/fluidity/advection2d/advection2d.flml
--rw-r--r--   0 leon      (1001) leon      (1001)     2032 2024-03-28 10:06:39.000000 pydrex-0.0.1/examples/fluidity/advection2d/advection2d.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.040064 pydrex-0.0.1/examples/fluidity/corner2d/
--rw-r--r--   0 leon      (1001) leon      (1001)     2326 2024-03-28 10:06:39.000000 pydrex-0.0.1/examples/fluidity/corner2d/Makefile
--rw-r--r--   0 leon      (1001) leon      (1001)    13076 2024-04-24 07:20:50.000000 pydrex-0.0.1/examples/fluidity/corner2d/corner2d.flml
--rw-r--r--   0 leon      (1001) leon      (1001)     2052 2024-03-28 10:06:39.000000 pydrex-0.0.1/examples/fluidity/corner2d/corner2d.py
--rwxr-xr-x   0 leon      (1001) leon      (1001)     1716 2024-03-25 14:42:57.000000 pydrex-0.0.1/examples/fluidity/envcheck.sh
--rwxr-xr-x   0 leon      (1001) leon      (1001)     1033 2024-03-25 14:42:57.000000 pydrex-0.0.1/examples/fluidity/load_modules.sh
--rw-r--r--   0 leon      (1001) leon      (1001)      264 2024-03-25 14:42:57.000000 pydrex-0.0.1/examples/fluidity/pbsrun_advection2d.sh
--rw-r--r--   0 leon      (1001) leon      (1001)     4219 2024-04-24 07:34:37.000000 pydrex-0.0.1/pyproject.toml
--rw-r--r--   0 leon      (1001) leon      (1001)       38 2024-04-24 07:38:46.051064 pydrex-0.0.1/setup.cfg
--rw-r--r--   0 leon      (1001) leon      (1001)      181 2024-02-26 22:21:28.000000 pydrex-0.0.1/setup.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.013064 pydrex-0.0.1/src/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.041064 pydrex-0.0.1/src/initial_implementation/
--rw-r--r--   0 leon      (1001) leon      (1001)    26810 2022-10-30 09:44:13.000000 pydrex-0.0.1/src/initial_implementation/AlternativeFunctions.py
--rw-r--r--   0 leon      (1001) leon      (1001)     2488 2022-10-30 09:44:13.000000 pydrex-0.0.1/src/initial_implementation/DRexParam.py
--rw-r--r--   0 leon      (1001) leon      (1001)    40980 2022-10-30 09:44:13.000000 pydrex-0.0.1/src/initial_implementation/PyDRex.py
--rwxr-xr-x   0 leon      (1001) leon      (1001)    41738 2022-10-30 09:44:13.000000 pydrex-0.0.1/src/initial_implementation/PyDRexFullIVP.py
--rw-r--r--   0 leon      (1001) leon      (1001)     3265 2023-06-23 00:10:14.000000 pydrex-0.0.1/src/initial_implementation/README.md
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.041064 pydrex-0.0.1/src/initial_implementation/pbs_cluster_instructions/
--rw-r--r--   0 leon      (1001) leon      (1001)     1049 2023-06-23 00:10:14.000000 pydrex-0.0.1/src/initial_implementation/pbs_cluster_instructions/job.sh
--rw-r--r--   0 leon      (1001) leon      (1001)      172 2023-06-23 00:10:14.000000 pydrex-0.0.1/src/initial_implementation/pbs_cluster_instructions/startWorkerNode.sh
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.041064 pydrex-0.0.1/src/initial_implementation/visualisation/
--rw-r--r--   0 leon      (1001) leon      (1001)     3012 2023-06-23 00:10:14.000000 pydrex-0.0.1/src/initial_implementation/visualisation/PlotDRex.py
--rw-r--r--   0 leon      (1001) leon      (1001)     8604 2023-06-23 00:10:14.000000 pydrex-0.0.1/src/initial_implementation/visualisation/pathlineIVP.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.043064 pydrex-0.0.1/src/pydrex/
--rw-r--r--   0 leon      (1001) leon      (1001)     7512 2024-04-24 07:34:56.000000 pydrex-0.0.1/src/pydrex/__init__.py
--rw-r--r--   0 leon      (1001) leon      (1001)     3729 2024-02-26 22:21:28.000000 pydrex-0.0.1/src/pydrex/axes.py
--rw-r--r--   0 leon      (1001) leon      (1001)    12247 2024-03-27 11:33:35.000000 pydrex-0.0.1/src/pydrex/cli.py
--rw-r--r--   0 leon      (1001) leon      (1001)    16448 2024-03-20 06:40:33.000000 pydrex-0.0.1/src/pydrex/core.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.014064 pydrex-0.0.1/src/pydrex/data/
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.044064 pydrex-0.0.1/src/pydrex/data/drexF90/
--rw-r--r--   0 leon      (1001) leon      (1001)    15909 2024-02-26 22:21:28.000000 pydrex-0.0.1/src/pydrex/data/drexF90/olA_D1E4_dt50_X0_L5.scsv
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.045064 pydrex-0.0.1/src/pydrex/data/outputs/
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001xy.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001xz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001yz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010xy.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010xz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010yz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100xy.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100xz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100yz.npz
--rw-r--r--   0 leon      (1001) leon      (1001)    80528 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_resampled.npz
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.045064 pydrex-0.0.1/src/pydrex/data/rng/
--rw-r--r--   0 leon      (1001) leon      (1001)      406 2023-08-01 12:47:38.000000 pydrex-0.0.1/src/pydrex/data/rng/hexaxis_nearX45_seeds.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)     6995 2023-07-24 10:21:37.000000 pydrex-0.0.1/src/pydrex/data/rng/seeds.scsv
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.046064 pydrex-0.0.1/src/pydrex/data/specs/
--rw-r--r--   0 leon      (1001) leon      (1001)     2396 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/specs/spec.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)     4721 2023-08-01 12:47:38.000000 pydrex-0.0.1/src/pydrex/data/specs/spec.toml
--rw-r--r--   0 leon      (1001) leon      (1001)      339 2023-08-01 12:47:38.000000 pydrex-0.0.1/src/pydrex/data/specs/start.scsv
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.046064 pydrex-0.0.1/src/pydrex/data/steadyflow/
--rw-r--r--   0 leon      (1001) leon      (1001)   120791 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/steadyflow/corner2d_2cmyr_5e5x1e5.vtu
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.047064 pydrex-0.0.1/src/pydrex/data/thirdparty/
--rw-r--r--   0 leon      (1001) leon      (1001)    12382 2023-07-20 15:33:42.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2001_GBMshear.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)      728 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2002_ISAtime.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)     2311 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2004_AaxisDynamicShear.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)     4485 2023-07-20 20:59:24.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2004_GBSshear.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)     5237 2023-06-26 20:28:43.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/Skemer2016_ShearStrainAngles.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)    15111 2023-09-05 09:36:45.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/a_axis_GBS_fortran.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)    36713 2023-09-05 09:36:45.000000 pydrex-0.0.1/src/pydrex/data/thirdparty/a_axis_GBS_long_fortran.scsv
--rw-r--r--   0 leon      (1001) leon      (1001)    17989 2024-04-24 07:20:50.000000 pydrex-0.0.1/src/pydrex/diagnostics.py
--rw-r--r--   0 leon      (1001) leon      (1001)      374 2024-04-24 07:20:50.000000 pydrex-0.0.1/src/pydrex/distributed.py
--rw-r--r--   0 leon      (1001) leon      (1001)     1875 2024-03-25 14:42:57.000000 pydrex-0.0.1/src/pydrex/exceptions.py
--rw-r--r--   0 leon      (1001) leon      (1001)    14062 2024-03-28 10:06:39.000000 pydrex-0.0.1/src/pydrex/geometry.py
--rw-r--r--   0 leon      (1001) leon      (1001)    22652 2024-04-24 07:20:50.000000 pydrex-0.0.1/src/pydrex/io.py
--rw-r--r--   0 leon      (1001) leon      (1001)     6459 2024-02-26 22:21:28.000000 pydrex-0.0.1/src/pydrex/logger.py
--rw-r--r--   0 leon      (1001) leon      (1001)     8484 2024-03-28 10:06:39.000000 pydrex-0.0.1/src/pydrex/mesh.py
--rw-r--r--   0 leon      (1001) leon      (1001)    26814 2024-04-05 10:09:03.000000 pydrex-0.0.1/src/pydrex/minerals.py
--rw-r--r--   0 leon      (1001) leon      (1001)     3620 2024-04-08 17:41:34.000000 pydrex-0.0.1/src/pydrex/mock.py
--rw-r--r--   0 leon      (1001) leon      (1001)     5354 2024-03-28 10:06:39.000000 pydrex-0.0.1/src/pydrex/pathlines.py
--rw-r--r--   0 leon      (1001) leon      (1001)    14167 2024-04-24 07:20:50.000000 pydrex-0.0.1/src/pydrex/stats.py
--rw-r--r--   0 leon      (1001) leon      (1001)     9094 2024-03-28 10:06:39.000000 pydrex-0.0.1/src/pydrex/tensors.py
--rw-r--r--   0 leon      (1001) leon      (1001)    10854 2024-04-24 07:33:55.000000 pydrex-0.0.1/src/pydrex/utils.py
--rw-r--r--   0 leon      (1001) leon      (1001)    12088 2024-03-28 10:06:39.000000 pydrex-0.0.1/src/pydrex/velocity.py
--rw-r--r--   0 leon      (1001) leon      (1001)    23391 2024-04-24 07:33:55.000000 pydrex-0.0.1/src/pydrex/visualisation.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.049064 pydrex-0.0.1/src/pydrex.egg-info/
--rw-r--r--   0 leon      (1001) leon      (1001)    44499 2024-04-24 07:38:45.000000 pydrex-0.0.1/src/pydrex.egg-info/PKG-INFO
--rw-r--r--   0 leon      (1001) leon      (1001)     3531 2024-04-24 07:38:46.000000 pydrex-0.0.1/src/pydrex.egg-info/SOURCES.txt
--rw-r--r--   0 leon      (1001) leon      (1001)        1 2024-04-24 07:38:45.000000 pydrex-0.0.1/src/pydrex.egg-info/dependency_links.txt
--rw-r--r--   0 leon      (1001) leon      (1001)      250 2024-04-24 07:38:45.000000 pydrex-0.0.1/src/pydrex.egg-info/entry_points.txt
--rw-r--r--   0 leon      (1001) leon      (1001)      300 2024-04-24 07:38:45.000000 pydrex-0.0.1/src/pydrex.egg-info/requires.txt
--rw-r--r--   0 leon      (1001) leon      (1001)       30 2024-04-24 07:38:45.000000 pydrex-0.0.1/src/pydrex.egg-info/top_level.txt
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.048064 pydrex-0.0.1/tests/
--rw-r--r--   0 leon      (1001) leon      (1001)     3537 2024-04-16 14:50:51.000000 pydrex-0.0.1/tests/README.md
--rw-r--r--   0 leon      (1001) leon      (1001)       32 2023-06-23 00:10:14.000000 pydrex-0.0.1/tests/__init__.py
--rw-r--r--   0 leon      (1001) leon      (1001)     7681 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/conftest.py
--rw-r--r--   0 leon      (1001) leon      (1001)     1817 2024-02-26 22:21:28.000000 pydrex-0.0.1/tests/test_config.py
--rw-r--r--   0 leon      (1001) leon      (1001)    31341 2024-04-03 11:24:15.000000 pydrex-0.0.1/tests/test_core.py
--rw-r--r--   0 leon      (1001) leon      (1001)     9795 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/test_corner_flow_2d.py
--rw-r--r--   0 leon      (1001) leon      (1001)    12924 2024-04-09 09:23:45.000000 pydrex-0.0.1/tests/test_diagnostics.py
--rw-r--r--   0 leon      (1001) leon      (1001)     2118 2024-04-24 07:34:56.000000 pydrex-0.0.1/tests/test_doctests.py
--rw-r--r--   0 leon      (1001) leon      (1001)     1767 2024-02-26 22:21:28.000000 pydrex-0.0.1/tests/test_geometry.py
--rw-r--r--   0 leon      (1001) leon      (1001)    14782 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/test_scsv.py
--rw-r--r--   0 leon      (1001) leon      (1001)    36542 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/test_simple_shear_2d.py
--rw-r--r--   0 leon      (1001) leon      (1001)    10709 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/test_simple_shear_3d.py
--rw-r--r--   0 leon      (1001) leon      (1001)     3892 2024-02-26 22:21:28.000000 pydrex-0.0.1/tests/test_tensors.py
--rw-r--r--   0 leon      (1001) leon      (1001)    10934 2024-04-24 07:20:50.000000 pydrex-0.0.1/tests/test_vortex_2d.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.049064 pydrex-0.0.1/tools/
--rw-r--r--   0 leon      (1001) leon      (1001)    30103 2023-09-07 08:35:56.000000 pydrex-0.0.1/tools/drex_forward_simpleshear.f90
--rwxr-xr-x   0 leon      (1001) leon      (1001)      705 2024-03-28 10:06:39.000000 pydrex-0.0.1/tools/find_45_seeds.py
-drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-24 07:38:46.049064 pydrex-0.0.1/tools/pbs_scripts/
--rwxr-xr-x   0 leon      (1001) leon      (1001)      596 2024-04-24 07:20:50.000000 pydrex-0.0.1/tools/pbs_scripts/run_test_ray_cluster_setup.sh
--rwxr-xr-x   0 leon      (1001) leon      (1001)     4259 2024-04-24 07:20:50.000000 pydrex-0.0.1/tools/pbs_start_ray_cluster.sh
--rwxr-xr-x   0 leon      (1001) leon      (1001)      876 2024-04-24 07:20:50.000000 pydrex-0.0.1/tools/pbs_start_ray_worker.sh
--rwxr-xr-x   0 leon      (1001) leon      (1001)     4226 2024-02-26 22:21:28.000000 pydrex-0.0.1/tools/perf_compare.sh
--rwxr-xr-x   0 leon      (1001) leon      (1001)     1836 2024-02-26 22:21:28.000000 pydrex-0.0.1/tools/run_fortran_ensemble.sh
--rw-r--r--   0 leon      (1001) leon      (1001)     1847 2024-02-26 22:21:28.000000 pydrex-0.0.1/tools/simple_shear_2d.py
--rwxr-xr-x   0 leon      (1001) leon      (1001)     1942 2024-02-26 22:21:28.000000 pydrex-0.0.1/tools/venv_install.sh
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.945153 pydrex-0.0.1rc2/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.930153 pydrex-0.0.1rc2/.github/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.933153 pydrex-0.0.1rc2/.github/workflows/
+-rw-r--r--   0 leon      (1001) leon      (1001)     1631 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/.github/workflows/ci.yml
+-rw-r--r--   0 leon      (1001) leon      (1001)     1183 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/.github/workflows/docs.yml
+-rw-r--r--   0 leon      (1001) leon      (1001)     1166 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/.pre-commit-config.yaml
+-rw-r--r--   0 leon      (1001) leon      (1001)    35149 2022-10-30 09:44:13.000000 pydrex-0.0.1rc2/LICENSE
+-rw-r--r--   0 leon      (1001) leon      (1001)    44461 2024-04-03 09:34:07.945153 pydrex-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 leon      (1001) leon      (1001)     2177 2024-04-03 07:31:02.000000 pydrex-0.0.1rc2/README.md
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.931152 pydrex-0.0.1rc2/docs/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.933153 pydrex-0.0.1rc2/docs/assets/
+-rw-r--r--   0 leon      (1001) leon      (1001)    80910 2023-08-26 02:58:48.000000 pydrex-0.0.1rc2/docs/assets/pydrex.png
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.933153 pydrex-0.0.1rc2/docs/template/
+-rw-r--r--   0 leon      (1001) leon      (1001)     1022 2023-08-26 02:58:48.000000 pydrex-0.0.1rc2/docs/template/index.html.jinja2
+-rw-r--r--   0 leon      (1001) leon      (1001)     1955 2023-06-23 00:10:13.000000 pydrex-0.0.1rc2/docs/template/math.html.jinja2
+-rw-r--r--   0 leon      (1001) leon      (1001)       98 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/docs/template/module.html.jinja2
+-rw-r--r--   0 leon      (1001) leon      (1001)     9390 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/docs/template/syntax-highlighting.css
+-rw-r--r--   0 leon      (1001) leon      (1001)     1330 2023-08-26 02:58:48.000000 pydrex-0.0.1rc2/docs/template/theme.css
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.931152 pydrex-0.0.1rc2/examples/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.934152 pydrex-0.0.1rc2/examples/fluidity/
+-rw-r--r--   0 leon      (1001) leon      (1001)      769 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/README.md
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.934152 pydrex-0.0.1rc2/examples/fluidity/advection2d/
+-rw-r--r--   0 leon      (1001) leon      (1001)     2078 2024-03-27 11:33:35.000000 pydrex-0.0.1rc2/examples/fluidity/advection2d/Makefile
+-rw-r--r--   0 leon      (1001) leon      (1001)    12703 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/advection2d/advection2d.flml
+-rw-r--r--   0 leon      (1001) leon      (1001)     2032 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/advection2d/advection2d.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.934152 pydrex-0.0.1rc2/examples/fluidity/corner2d/
+-rw-r--r--   0 leon      (1001) leon      (1001)     2326 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/corner2d/Makefile
+-rw-r--r--   0 leon      (1001) leon      (1001)    12695 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/corner2d/corner2d.flml
+-rw-r--r--   0 leon      (1001) leon      (1001)     2052 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/examples/fluidity/corner2d/corner2d.py
+-rwxr-xr-x   0 leon      (1001) leon      (1001)     1716 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/examples/fluidity/envcheck.sh
+-rwxr-xr-x   0 leon      (1001) leon      (1001)     1033 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/examples/fluidity/load_modules.sh
+-rw-r--r--   0 leon      (1001) leon      (1001)      264 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/examples/fluidity/pbsrun_advection2d.sh
+-rw-r--r--   0 leon      (1001) leon      (1001)     4180 2024-04-03 09:28:07.000000 pydrex-0.0.1rc2/pyproject.toml
+-rw-r--r--   0 leon      (1001) leon      (1001)       38 2024-04-03 09:34:07.945153 pydrex-0.0.1rc2/setup.cfg
+-rw-r--r--   0 leon      (1001) leon      (1001)      181 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/setup.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.931152 pydrex-0.0.1rc2/src/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.935153 pydrex-0.0.1rc2/src/initial_implementation/
+-rw-r--r--   0 leon      (1001) leon      (1001)    26810 2022-10-30 09:44:13.000000 pydrex-0.0.1rc2/src/initial_implementation/AlternativeFunctions.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     2488 2022-10-30 09:44:13.000000 pydrex-0.0.1rc2/src/initial_implementation/DRexParam.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    40980 2022-10-30 09:44:13.000000 pydrex-0.0.1rc2/src/initial_implementation/PyDRex.py
+-rwxr-xr-x   0 leon      (1001) leon      (1001)    41738 2022-10-30 09:44:13.000000 pydrex-0.0.1rc2/src/initial_implementation/PyDRexFullIVP.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     3265 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/src/initial_implementation/README.md
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.935153 pydrex-0.0.1rc2/src/initial_implementation/pbs_cluster_instructions/
+-rw-r--r--   0 leon      (1001) leon      (1001)     1049 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/src/initial_implementation/pbs_cluster_instructions/job.sh
+-rw-r--r--   0 leon      (1001) leon      (1001)      172 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/src/initial_implementation/pbs_cluster_instructions/startWorkerNode.sh
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.935153 pydrex-0.0.1rc2/src/initial_implementation/visualisation/
+-rw-r--r--   0 leon      (1001) leon      (1001)     3012 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/src/initial_implementation/visualisation/PlotDRex.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     8604 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/src/initial_implementation/visualisation/pathlineIVP.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.937152 pydrex-0.0.1rc2/src/pydrex/
+-rw-r--r--   0 leon      (1001) leon      (1001)     7516 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/src/pydrex/__init__.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     3729 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/src/pydrex/axes.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    12247 2024-03-27 11:33:35.000000 pydrex-0.0.1rc2/src/pydrex/cli.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    16448 2024-03-20 06:40:33.000000 pydrex-0.0.1rc2/src/pydrex/core.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.932153 pydrex-0.0.1rc2/src/pydrex/data/
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.938152 pydrex-0.0.1rc2/src/pydrex/data/drexF90/
+-rw-r--r--   0 leon      (1001) leon      (1001)    15909 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/src/pydrex/data/drexF90/olA_D1E4_dt50_X0_L5.scsv
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.940153 pydrex-0.0.1rc2/src/pydrex/data/outputs/
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001xy.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001xz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001yz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010xy.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010xz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010yz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100xy.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100xz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    24748 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100yz.npz
+-rw-r--r--   0 leon      (1001) leon      (1001)    80528 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_resampled.npz
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.940153 pydrex-0.0.1rc2/src/pydrex/data/rng/
+-rw-r--r--   0 leon      (1001) leon      (1001)      406 2023-08-01 12:47:38.000000 pydrex-0.0.1rc2/src/pydrex/data/rng/hexaxis_nearX45_seeds.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)     6995 2023-07-24 10:21:37.000000 pydrex-0.0.1rc2/src/pydrex/data/rng/seeds.scsv
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.940153 pydrex-0.0.1rc2/src/pydrex/data/specs/
+-rw-r--r--   0 leon      (1001) leon      (1001)     2396 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/specs/spec.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)     4721 2023-08-01 12:47:38.000000 pydrex-0.0.1rc2/src/pydrex/data/specs/spec.toml
+-rw-r--r--   0 leon      (1001) leon      (1001)      339 2023-08-01 12:47:38.000000 pydrex-0.0.1rc2/src/pydrex/data/specs/start.scsv
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.940153 pydrex-0.0.1rc2/src/pydrex/data/steadyflow/
+-rw-r--r--   0 leon      (1001) leon      (1001)   120791 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/steadyflow/corner2d_2cmyr_5e5x1e5.vtu
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.941152 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/
+-rw-r--r--   0 leon      (1001) leon      (1001)    12382 2023-07-20 15:33:42.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2001_GBMshear.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)      728 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2002_ISAtime.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)     2311 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2004_AaxisDynamicShear.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)     4485 2023-07-20 20:59:24.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2004_GBSshear.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)     5237 2023-06-26 20:28:43.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Skemer2016_ShearStrainAngles.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)    15111 2023-09-05 09:36:45.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/a_axis_GBS_fortran.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)    36713 2023-09-05 09:36:45.000000 pydrex-0.0.1rc2/src/pydrex/data/thirdparty/a_axis_GBS_long_fortran.scsv
+-rw-r--r--   0 leon      (1001) leon      (1001)    17218 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/diagnostics.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     1875 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/src/pydrex/exceptions.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    14062 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/geometry.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    22552 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/io.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     6459 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/src/pydrex/logger.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     8484 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/mesh.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    26814 2024-04-03 09:15:59.000000 pydrex-0.0.1rc2/src/pydrex/minerals.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     3620 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/src/pydrex/mock.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     5354 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/pathlines.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    14133 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/stats.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     9094 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/tensors.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    10006 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/src/pydrex/utils.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    12088 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/velocity.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    22697 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/src/pydrex/visualisation.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.943153 pydrex-0.0.1rc2/src/pydrex.egg-info/
+-rw-r--r--   0 leon      (1001) leon      (1001)    44461 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/PKG-INFO
+-rw-r--r--   0 leon      (1001) leon      (1001)     3383 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/SOURCES.txt
+-rw-r--r--   0 leon      (1001) leon      (1001)        1 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/dependency_links.txt
+-rw-r--r--   0 leon      (1001) leon      (1001)      250 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/entry_points.txt
+-rw-r--r--   0 leon      (1001) leon      (1001)      253 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/requires.txt
+-rw-r--r--   0 leon      (1001) leon      (1001)       30 2024-04-03 09:34:07.000000 pydrex-0.0.1rc2/src/pydrex.egg-info/top_level.txt
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.943153 pydrex-0.0.1rc2/tests/
+-rw-r--r--   0 leon      (1001) leon      (1001)     3537 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tests/README.md
+-rw-r--r--   0 leon      (1001) leon      (1001)       32 2023-06-23 00:10:14.000000 pydrex-0.0.1rc2/tests/__init__.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     7045 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/conftest.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     1817 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/test_config.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    30988 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/test_core.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     9785 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tests/test_corner_flow_2d.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    12924 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/test_diagnostics.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     2059 2024-04-03 09:29:57.000000 pydrex-0.0.1rc2/tests/test_doctests.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     1767 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/test_geometry.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    14419 2024-03-25 14:42:57.000000 pydrex-0.0.1rc2/tests/test_scsv.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    36351 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tests/test_simple_shear_2d.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    10192 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tests/test_simple_shear_3d.py
+-rw-r--r--   0 leon      (1001) leon      (1001)     3892 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tests/test_tensors.py
+-rw-r--r--   0 leon      (1001) leon      (1001)    10771 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tests/test_vortex_2d.py
+drwxr-xr-x   0 leon      (1001) leon      (1001)        0 2024-04-03 09:34:07.943153 pydrex-0.0.1rc2/tools/
+-rw-r--r--   0 leon      (1001) leon      (1001)    30103 2023-09-07 08:35:56.000000 pydrex-0.0.1rc2/tools/drex_forward_simpleshear.f90
+-rwxr-xr-x   0 leon      (1001) leon      (1001)      705 2024-03-28 10:06:39.000000 pydrex-0.0.1rc2/tools/find_45_seeds.py
+-rwxr-xr-x   0 leon      (1001) leon      (1001)     4226 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tools/perf_compare.sh
+-rwxr-xr-x   0 leon      (1001) leon      (1001)     1836 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tools/run_fortran_ensemble.sh
+-rw-r--r--   0 leon      (1001) leon      (1001)     1847 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tools/simple_shear_2d.py
+-rwxr-xr-x   0 leon      (1001) leon      (1001)     1942 2024-02-26 22:21:28.000000 pydrex-0.0.1rc2/tools/venv_install.sh
```

### Comparing `pydrex-0.0.1/.github/workflows/ci.yml` & `pydrex-0.0.1rc2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,72 +8,64 @@
     branches:
       - main
 
 jobs:
   install-linux:
     name: (Linux) Install package and run tests
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ['3.10', '3.11', '3.12']
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v4
+        uses: actions/checkout@v3
 
       - name: Setup Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: '3.12'
 
       - name: Install and test
         run: |
           sudo apt-get update
           sudo apt-get install -y libglu1-mesa
           sudo apt-get install -y python3-pip
           python3 -m pip install --upgrade pip
           python3 -m pip install "$PWD[test]"
           python3 -m pytest -rN
 
   install-macos:
     name: (MacOS) Install package and run tests
     runs-on: macos-latest
-    strategy:
-      matrix:
-        python-version: ['3.10', '3.11', '3.12']
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v4
+        uses: actions/checkout@v3
 
       - name: Setup Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: '3.12'
 
       - name: Install and test
         run: |
           python3 -m pip install --upgrade pip
           python3 -m pip install "$PWD[test]"
           python3 -m pytest -rN
 
   install-windows:
     name: (Windows) Install package and run tests
-    runs-on: windows-latest
-    strategy:
-      matrix:
-        python-version: ['3.10', '3.11', '3.12']
+    runs-on: windows-2019
+    if: false
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v4
+        uses: actions/checkout@v3
 
       - name: Setup Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: '3.12'
 
       - name: Install and test
         run: |
           python3 -m pip install --upgrade pip
           python3 -m pip install "$PWD[test]"
           python3 -m pytest -rN
```

### Comparing `pydrex-0.0.1/.github/workflows/docs.yml` & `pydrex-0.0.1rc2/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,30 @@
     runs-on: ubuntu-latest
     permissions:
       contents: write
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v4
+        uses: actions/checkout@v3
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.12'
 
       - name: Build
         run: |
           sudo apt-get update
           sudo apt-get install -y python3-pip
           python3 -m pip install --upgrade pip
           python3 -m venv .venv-gh-pages
           source .venv-gh-pages/bin/activate
           python3 -m pip install "$PWD"[doc,test]
-          pdoc -t docs/template -o html --math pydrex !pydrex.mesh !pydrex.distributed tests
+          pdoc -t docs/template -o html --math pydrex !pydrex.mesh tests
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         # If you're changing the branch from main,
         # also change the `main` in `refs/heads/main`
         # below accordingly.
         if: ${{ github.ref == 'refs/heads/main' }}
         with:
```

### Comparing `pydrex-0.0.1/.pre-commit-config.yaml` & `pydrex-0.0.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/LICENSE` & `pydrex-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/PKG-INFO` & `pydrex-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrex
-Version: 0.0.1
+Version: 0.0.1rc2
 Summary: Dynamic CPO calculations for olivine-enstatite polycrystal aggregates
 Author: Chris Mathews
 Author-email: Thomas Duvernay <td75013@hotmail.fr>, Leon Bilton <adigitoleo@posteo.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,18 +683,17 @@
 Project-URL: documentation, https://seismic-anisotropy.github.io/PyDRex/
 Keywords: CPO,LPO,olivine,deformation,anisotropy,crystallography
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: numpy>=1.8
 Requires-Dist: numba>=0.57
 Requires-Dist: scipy>=1.2
 Requires-Dist: pyyaml
 Requires-Dist: meshio
 Requires-Dist: matplotlib
 Requires-Dist: cmcrameri
@@ -702,24 +701,24 @@
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: pdoc; extra == "doc"
 Provides-Extra: mesh
 Requires-Dist: gmsh; extra == "mesh"
-Provides-Extra: ray
-Requires-Dist: ray>=2.0.0; extra == "ray"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: uniplot; extra == "dev"
 Requires-Dist: pdoc; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: ptpython; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Provides-Extra: lsp
 Requires-Dist: python-lsp-server; extra == "lsp"
 Requires-Dist: pyls-isort; extra == "lsp"
 Requires-Dist: python-lsp-black; extra == "lsp"
 Requires-Dist: python-lsp-ruff; extra == "lsp"
 
 # PyDRex
```

### Comparing `pydrex-0.0.1/README.md` & `pydrex-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/docs/assets/pydrex.png` & `pydrex-0.0.1rc2/docs/assets/pydrex.png`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/docs/template/index.html.jinja2` & `pydrex-0.0.1rc2/docs/template/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/docs/template/math.html.jinja2` & `pydrex-0.0.1rc2/docs/template/math.html.jinja2`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/docs/template/syntax-highlighting.css` & `pydrex-0.0.1rc2/docs/template/syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/docs/template/theme.css` & `pydrex-0.0.1rc2/docs/template/theme.css`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/README.md` & `pydrex-0.0.1rc2/examples/fluidity/README.md`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/advection2d/Makefile` & `pydrex-0.0.1rc2/examples/fluidity/advection2d/Makefile`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/advection2d/advection2d.flml` & `pydrex-0.0.1rc2/examples/fluidity/advection2d/advection2d.flml`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/advection2d/advection2d.py` & `pydrex-0.0.1rc2/examples/fluidity/advection2d/advection2d.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/corner2d/Makefile` & `pydrex-0.0.1rc2/examples/fluidity/corner2d/Makefile`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/corner2d/corner2d.flml` & `pydrex-0.0.1rc2/examples/fluidity/corner2d/corner2d.flml`

 * *Files 2% similar despite different names*

#### Comparing `pydrex-0.0.1/examples/fluidity/corner2d/corner2d.flml` & `pydrex-0.0.1rc2/examples/fluidity/corner2d/corner2d.flml`

```diff
@@ -79,25 +79,14 @@
           <python>
             <string_value type="code" language="python" lines="20">def val(t):
     from corner2d import INITIAL_POSITIONS
 
     return INITIAL_POSITIONS</string_value>
           </python>
         </initial_position>
-        <initialise_during_simulation>
-          <python>
-            <string_value type="code" language="python" lines="20">def val(t):
-    from corner2d import INITIAL_POSITIONS
-
-    if 8.7e13 &lt; t &lt; 8.75e13 or 4.3e14 &lt; t &lt; 4.4e14:
-        return INITIAL_POSITIONS
-    else:
-        return []</string_value>
-          </python>
-        </initialise_during_simulation>
         <attributes>
           <scalar_attribute_array name="CPO_">
             <dimension>
               <integer_value rank="0">50022</integer_value>
               <comment>= n_grains (PyDRex) * 10 + 22</comment>
             </dimension>
             <initial_attribute_value>
```

### Comparing `pydrex-0.0.1/examples/fluidity/corner2d/corner2d.py` & `pydrex-0.0.1rc2/examples/fluidity/corner2d/corner2d.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/envcheck.sh` & `pydrex-0.0.1rc2/examples/fluidity/envcheck.sh`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/examples/fluidity/load_modules.sh` & `pydrex-0.0.1rc2/examples/fluidity/load_modules.sh`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/pyproject.toml` & `pydrex-0.0.1rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Use modern (PEP621, PEP660) setuptools build system.
-# PEP 660 editable installs: <https://github.com/pypa/setuptools/blob/main/NEWS.rst#v6400>.
-# Python 3.11 support: <https://github.com/pypa/setuptools_scm/blob/main/CHANGELOG.md#v710>.
+# PEP 660 editable installs: <https://github.com/pypa/setuptools/blob/main/CHANGES.rst#v6400>.
+# Python 3.11 support: <https://github.com/pypa/setuptools_scm/blob/main/CHANGELOG.rst#v710>.
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
 
 # Automatically use the version number from vcs (e.g. git) tags,
 # <https://github.com/pypa/setuptools_scm>.
 [tool.setuptools_scm]
 
-# Docs: <https://packaging.python.org/en/latest/specifications/pyproject-toml/>.
+# Docs: <https://packaging.python.org/en/latest/specifications/declaring-project-metadata/>.
+# Example: <https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#example>.
 [project]
 name = "pydrex"
 dynamic = ["version"]  # Managed by setuptools_scm.
 description = "Dynamic CPO calculations for olivine-enstatite polycrystal aggregates"
 readme = "README.md"
-requires-python = ">=3.10"  # We use tomllib on 3.11: <https://docs.python.org/3/library/tomllib.html>.
+requires-python = ">=3.11"  # We use tomllib: <https://docs.python.org/3/library/tomllib.html>.
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas Duvernay", email = "td75013@hotmail.fr"},
     {name = "Leon Bilton", email = "adigitoleo@posteo.net"},
     {name = "Chris Mathews"},
 ]
 keywords = ["CPO", "LPO", "olivine", "deformation", "anisotropy", "crystallography"]
@@ -28,15 +29,14 @@
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
 ]
 
 dependencies = [
-    "tomli >= 1.1.0 ; python_version < '3.11'",  # https://github.com/hukkin/tomli?tab=readme-ov-file#building-a-tomlitomllib-compatibility-layer
     "numpy >= 1.8",  # <https://numpy.org/doc/stable/reference/generated/numpy.linalg.eigvalsh.html>
     "numba >= 0.57",  # <https://numba.readthedocs.io/en/stable/release-notes.html#version-0-57-0-1-may-2023>
     "scipy >= 1.2",  # <https://github.com/scipy/scipy/pull/9176>
     "pyyaml",  # For YAML headers of plaintext datafiles.
     "meshio",  # For reading VTK and other meshes.
     "matplotlib",  # Plotting library, The.
     "cmcrameri",  # Matplotlib colormaps using the palettes designed by Fabio Crameri.
@@ -44,16 +44,15 @@
     "tqdm",  # For progress bars (for long-running CLI scripts)
 ]
 
 [project.optional-dependencies]
 test = ["pytest"]
 doc = ["pdoc"]
 mesh = ["gmsh"]  # NOTE: Saying `import gmsh` is like saying "I don't want my CI to work".
-ray = ["ray >= 2.0.0"]
-dev = ["pytest", "uniplot", "pdoc", "ruff", "black", "isort", "ptpython"]
+dev = ["pytest", "uniplot", "pdoc", "ruff", "black", "isort", "ptpython", "build", "twine"]
 lsp = ["python-lsp-server", "pyls-isort", "python-lsp-black", "python-lsp-ruff"]
 
 [project.urls]
 repository = "https://github.com/seismic-anisotropy/PyDRex"
 documentation = "https://seismic-anisotropy.github.io/PyDRex/"
 
 [project.scripts]
```

### Comparing `pydrex-0.0.1/src/initial_implementation/AlternativeFunctions.py` & `pydrex-0.0.1rc2/src/initial_implementation/AlternativeFunctions.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/DRexParam.py` & `pydrex-0.0.1rc2/src/initial_implementation/DRexParam.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/PyDRex.py` & `pydrex-0.0.1rc2/src/initial_implementation/PyDRex.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/PyDRexFullIVP.py` & `pydrex-0.0.1rc2/src/initial_implementation/PyDRexFullIVP.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/README.md` & `pydrex-0.0.1rc2/src/initial_implementation/README.md`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/pbs_cluster_instructions/job.sh` & `pydrex-0.0.1rc2/src/initial_implementation/pbs_cluster_instructions/job.sh`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/visualisation/PlotDRex.py` & `pydrex-0.0.1rc2/src/initial_implementation/visualisation/PlotDRex.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/initial_implementation/visualisation/pathlineIVP.py` & `pydrex-0.0.1rc2/src/initial_implementation/visualisation/pathlineIVP.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/__init__.py` & `pydrex-0.0.1rc2/src/pydrex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 #### Simulate crystallographic preferred orientation evolution in polycrystals
 
 ---
 
 .. warning::
-    **This software is currently in early development (alpha)
+    **This software is currently in early development (pre-alpha)
     and therefore subject to breaking changes without notice.**
 
 ## About
 
 Viscoplastic deformation of minerals, e.g. in Earth's mantle, leads to distinct
 signatures in the mineral texture. Many minerals naturally occur in
 polycrystalline form, which means that they are composed of many grains with
```

### Comparing `pydrex-0.0.1/src/pydrex/axes.py` & `pydrex-0.0.1rc2/src/pydrex/axes.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/cli.py` & `pydrex-0.0.1rc2/src/pydrex/cli.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/core.py` & `pydrex-0.0.1rc2/src/pydrex/core.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/drexF90/olA_D1E4_dt50_X0_L5.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/drexF90/olA_D1E4_dt50_X0_L5.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001xy.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001xy.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001xz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001xz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_001yz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_001yz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010xy.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010xy.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010xz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010xz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_010yz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_010yz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100xy.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100xy.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100xz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100xz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_poles_100yz.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_poles_100yz.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/outputs/example_CPO_resampled.npz` & `pydrex-0.0.1rc2/src/pydrex/data/outputs/example_CPO_resampled.npz`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/rng/seeds.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/rng/seeds.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/specs/spec.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/specs/spec.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/specs/spec.toml` & `pydrex-0.0.1rc2/src/pydrex/data/specs/spec.toml`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/steadyflow/corner2d_2cmyr_5e5x1e5.vtu` & `pydrex-0.0.1rc2/src/pydrex/data/steadyflow/corner2d_2cmyr_5e5x1e5.vtu`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2001_GBMshear.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2001_GBMshear.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2002_ISAtime.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2002_ISAtime.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2004_AaxisDynamicShear.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2004_AaxisDynamicShear.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/Kaminski2004_GBSshear.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Kaminski2004_GBSshear.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/Skemer2016_ShearStrainAngles.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/Skemer2016_ShearStrainAngles.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/a_axis_GBS_fortran.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/a_axis_GBS_fortran.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/data/thirdparty/a_axis_GBS_long_fortran.scsv` & `pydrex-0.0.1rc2/src/pydrex/data/thirdparty/a_axis_GBS_long_fortran.scsv`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/diagnostics.py` & `pydrex-0.0.1rc2/src/pydrex/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,26 @@
     $$
     such that a[i, j] gives the direction cosine of the angle between the i-th
     grain axis and the j-th external axis (in the global Eulerian frame).
 
 """
 
 import functools as ft
+from multiprocessing import Pool
 
 import numba as nb
 import numpy as np
 import scipy.linalg as la
 
 from pydrex import geometry as _geo
 from pydrex import logger as _log
 from pydrex import stats as _stats
 from pydrex import tensors as _tensors
 from pydrex import utils as _utils
 
-Pool, HAS_RAY = _utils.import_proc_pool()
-if HAS_RAY:
-    import ray
-
-    from pydrex import distributed as _dstr
-
 
 def elasticity_components(voigt_matrices):
     """Calculate elasticity decompositions for the given elasticity tensors.
 
     Args:
     - `voigt_matrices` (array) — the Nx6x6 Voigt matrix representations of the averaged
       elasticity tensors for a series of polycrystal textures
@@ -280,24 +275,19 @@
 ):
     """Calculate M-indices for a series of polycrystal textures.
 
     Calculate M-index using `misorientation_index` for a series of texture snapshots.
     The `orientation_stack` is a NxMx3x3 array of orientations where N is the number of
     texture snapshots and M is the number of grains.
 
-    Uses either Ray or the Python multiprocessing library to calculate texture indices
-    for multiple snapshots simultaneously. The arguments `ncpus` and `pool` are only
-    relevant to the latter option: if `ncpus` is `None` the number of CPU cores to use
-    is chosen automatically based on the maximum number available to the Python
-    interpreter, otherwise the specified number of cores is requested. Alternatively, an
-    existing instance of `multiprocessing.Pool` can be provided.
-
-    If Ray is installed, it will be automatically preferred. In this case, the number of
-    parallel workers should be set upon initialisation of the Ray cluster (which can be
-    distributed over the network).
+    Uses the multiprocessing library to calculate texture indices for multiple snapshots
+    simultaneously. If `ncpus` is `None` the number of CPU cores to use is chosen
+    automatically based on the maximum number available to the Python interpreter,
+    otherwise the specified number of cores is requested. Alternatively, an existing
+    instance of `multiprocessing.Pool` can be provided.
 
     See `misorientation_index` for documentation of the remaining arguments.
 
     """
     if ncpus is not None and pool is not None:
         _log.warning("ignoring `ncpus` argument because a Pool was provided")
     m_indices = np.empty(len(orientation_stack))
@@ -309,28 +299,16 @@
     if pool is None:
         if ncpus is None:
             ncpus = _utils.default_ncpus()
         with Pool(processes=ncpus) as pool:
             for i, out in enumerate(pool.imap(_run, orientation_stack)):
                 m_indices[i] = out
     else:
-        if HAS_RAY:
-            m_indices = np.array(
-                ray.get(
-                    [
-                        _dstr.misorientation_index.remote(
-                            ray.put(a), system=system, bins=bins
-                        )
-                        for a in orientation_stack
-                    ]
-                )
-            )
-        else:
-            for i, out in enumerate(pool.imap(_run, orientation_stack)):
-                m_indices[i] = out
+        for i, out in enumerate(pool.imap(_run, orientation_stack)):
+            m_indices[i] = out
     return m_indices
 
 
 def misorientation_index(orientations, system: _geo.LatticeSystem, bins=None):
     r"""Calculate M-index for polycrystal orientations.
 
     The `bins` argument is passed to `numpy.histogram`.
```

### Comparing `pydrex-0.0.1/src/pydrex/exceptions.py` & `pydrex-0.0.1rc2/src/pydrex/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/geometry.py` & `pydrex-0.0.1rc2/src/pydrex/geometry.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/io.py` & `pydrex-0.0.1rc2/src/pydrex/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,15 @@
 
 import collections as c
 import csv
 import functools as ft
 import io
 import os
 import pathlib
-import sys
-
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    import tomli as tomllib
-
+import tomllib
 from importlib.resources import files
 
 import h5py
 import meshio
 import numpy as np
 import yaml
 from tqdm import tqdm
@@ -119,15 +113,15 @@
                 fractions_init=_fractions[0],
                 orientations_init=_orientations[0],
             )
             mineral.fractions = _fractions
             mineral.orientations = _orientations
             mineral.save(output, postfix=_postfix)
             save_scsv(
-                output[:-4] + f"_{_postfix}" + ".scsv",
+                output[:-4] + ".scsv",
                 {
                     "delimiter": ",",
                     "missing": "-",
                     "fields": [
                         {
                             "name": "strain",
                             "type": "float",
```

### Comparing `pydrex-0.0.1/src/pydrex/logger.py` & `pydrex-0.0.1rc2/src/pydrex/logger.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/mesh.py` & `pydrex-0.0.1rc2/src/pydrex/mesh.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/minerals.py` & `pydrex-0.0.1rc2/src/pydrex/minerals.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/mock.py` & `pydrex-0.0.1rc2/src/pydrex/mock.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/pathlines.py` & `pydrex-0.0.1rc2/src/pydrex/pathlines.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/stats.py` & `pydrex-0.0.1rc2/src/pydrex/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import itertools as it
 
 import numpy as np
 import scipy.special as sp
 from scipy.spatial.transform import Rotation
 
 from pydrex import geometry as _geo
+from pydrex import logger as _log
 from pydrex import stats as _stats
 from pydrex import utils as _utils
 
 
 def resample_orientations(orientations, fractions, n_samples=None, seed=None):
     """Return new samples from `orientations` weighted by the volume distribution.
 
@@ -82,15 +83,15 @@
     The `bins` argument is passed to `numpy.histogram`.
     If left as `None`, 1° bins will be used as recommended by the reference paper.
     The `symmetry` argument specifies the lattice system which determines intrinsic
     symmetry degeneracies and the maximum allowable misorientation angle.
     See `_geo.LatticeSystem` for supported systems.
 
     .. warning::
-        This method must be able to allocate $ \frac{N!}{(N-2)!} × 4M $ floats
+        This method must be able to allocate $ \frac{N!}{N-2!}× 4M $ floats
         for N the length of `orientations` and M the number of symmetry operations for
         the given `system` (`numpy.float32` values are used to reduce the memory
         requirements)
 
     See [Skemer et al. (2005)](https://doi.org/10.1016/j.tecto.2005.08.023).
 
     """
@@ -100,16 +101,16 @@
         (sp.comb(len(orientations), 2, exact=True), len(symmetry_ops), 4),
         dtype=np.float32,
     )
     q2_array = np.empty(
         (sp.comb(len(orientations), 2, exact=True), len(symmetry_ops), 4),
         dtype=np.float32,
     )
-    for i, e in enumerate(  # Copy is required for proper object referencing in Ray.
-        it.combinations(Rotation.from_matrix(orientations.copy()).as_quat(), 2)
+    for i, e in enumerate(
+        it.combinations(Rotation.from_matrix(orientations).as_quat(), 2)
     ):
         q1, q2 = list(e)
         for j, qs in enumerate(symmetry_ops):
             if qs.shape == (4, 4):  # Reflection, not a proper rotation.
                 q1_array[i, j] = qs @ q1
                 q2_array[i, j] = qs @ q2
             else:
```

### Comparing `pydrex-0.0.1/src/pydrex/tensors.py` & `pydrex-0.0.1rc2/src/pydrex/tensors.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/utils.py` & `pydrex-0.0.1rc2/src/pydrex/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,14 @@
 from matplotlib.legend_handler import HandlerLine2D, HandlerPathCollection
 from matplotlib.pyplot import Line2D
 from matplotlib.transforms import ScaledTranslation
 
 from pydrex import logger as _log
 
 
-def import_proc_pool():
-    """Import either `ray.util.multiprocessing.Pool` or `multiprocessing.Pool`.
-
-    Import a process `Pool` object either from Ray of from Python's stdlib.
-    Both offer the same API, the Ray implementation will be preferred if available.
-    Using the `Pool` provided by Ray allows for distributed memory multiprocessing.
-
-    Returns a tuple containing the `Pool` object and a boolean flag which is `True` if
-    Ray is available.
-
-    """
-    try:
-        from ray.util.multiprocessing import Pool
-
-        has_ray = True
-    except ImportError:
-        from multiprocessing import Pool
-
-        has_ray = False
-    return Pool, has_ray
-
-
 @nb.njit(fastmath=True)
 def strain_increment(dt, velocity_gradient):
     """Calculate strain increment for a given time increment and velocity gradient.
 
     Returns “tensorial” strain increment ε, which is equal to γ/2 where γ is the
     “(engineering) shear strain” increment.
 
@@ -307,18 +285,14 @@
     """
     for txt, ax in mosaic.items():
         if txt.lower() == "legend":
             continue
         _txt = labelmap[txt] if labelmap is not None else txt
         if internal:
             trans = ScaledTranslation(10 / 72, -5 / 72, ax.figure.dpi_scale_trans)
-            if isinstance(loc, str):
-                raise ValueError(
-                    "'loc' argument must be a sequence of float when 'internal' is 'True'"
-                )
             ax.text(
                 *loc,
                 _txt,
                 transform=ax.transAxes + trans,
                 fontsize=fontsize,
                 bbox={
                     "facecolor": (1.0, 1.0, 1.0, 0.3),
```

### Comparing `pydrex-0.0.1/src/pydrex/velocity.py` & `pydrex-0.0.1rc2/src/pydrex/velocity.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/src/pydrex/visualisation.py` & `pydrex-0.0.1rc2/src/pydrex/visualisation.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,16 +225,16 @@
             V[i] = v3d[vertical]
 
         velocities = ax.quiver(
             X_grid,
             Y_grid,
             U.reshape(X_grid.shape),
             V.reshape(Y_grid.shape),
-            pivot=kwargs.pop("pivot", "mid"),
-            alpha=kwargs.pop("alpha", 0.25),
+            pivot="mid",
+            alpha=0.25,
             **kwargs,
         )
 
     P = np.asarray([[p[horizontal], p[vertical]] for p in positions])
     if cpo_vectors is not None:
         if cpo_strengths is None:
             cpo_strengths = np.full(len(cpo_vectors), 1.0)
@@ -248,18 +248,18 @@
             P[:, 0],
             P[:, 1],
             C[:, 0],
             C[:, 1],
             colors,
             cmap=cmap,
             pivot="mid",
-            width=kwargs.pop("width", 3e-3),
+            width=3e-3,
             headaxislength=0,
             headlength=0,
-            zorder=kwargs.pop("zorder", 10) + 1,  # Always above velocity vectors.
+            zorder=10,
         )
     else:
         cpo = ax.scatter(P[:, 0], P[:, 1], marker=marker, c=colors, cmap=cmap)
     return fig, ax, velocities, cpo
 
 
 def alignment(
@@ -269,15 +269,14 @@
     markers,
     labels,
     err=None,
     θ_max=90,
     θ_fse=None,
     colors=None,
     cmaps=None,
-    **kwargs,
 ):
     """Plot `angles` (in degrees) versus `strains` on the given axis.
 
     Alignment angles could be either bingham averages or the a-axis in the hexagonal
     symmetry projection, measured from e.g. the shear direction. In the first case,
     they should be calculated from resampled grain orientations. Expects as many
     `markers` and `labels` as there are data series in `angles`.
@@ -296,17 +295,14 @@
       strain ellipsoid to the reference direction (e.g. shear direction)
     - `colors` (array, optional) — color coordinates for series of angles
     - `cmaps` (Matplotlib color maps, optional) — color maps for `colors`
 
     If `colors` and `cmaps` are used, then angle values are colored individually within
     each angle series.
 
-    Additional keyword arguments are passed to `matplotlib.axes.Axes.scatter` if
-    `colors` is not `None`, or to `matplotlib.axes.Axes.plot` otherwise.
-
     Returns a tuple of the figure handle, the axes handle and the set of colors used for
     the data series plots.
 
     """
     _strains = np.atleast_2d(strains)
     _angles = np.atleast_2d(angles)
     if err is not None:
@@ -328,21 +324,20 @@
             ax.scatter(
                 strains,
                 θ_cpo,
                 marker=marker,
                 label=label,
                 c=colors[i],
                 cmap=cmaps[i],
-                alpha=kwargs.pop("alpha", 0.6),
-                edgecolor=kwargs.pop("edgecolor", plt.rcParams["axes.edgecolor"]),
-                **kwargs,
+                alpha=0.6,
+                edgecolor=plt.rcParams["axes.edgecolor"],
             )
             _colors.append(colors[i])
         else:
-            lines = ax.plot(strains, θ_cpo, marker, alpha=0.6, label=label, **kwargs)
+            lines = ax.plot(strains, θ_cpo, marker, alpha=0.6, label=label)
             _colors.append(lines[0].get_color())
         if err is not None:
             ax.fill_between(
                 strains,
                 θ_cpo - _angles_err[i],
                 θ_cpo + _angles_err[i],
                 alpha=0.22,
@@ -363,15 +358,14 @@
     ylabel,
     markers,
     labels,
     err=None,
     cpo_threshold=None,
     colors=None,
     cmaps=None,
-    **kwargs,
 ):
     """Plot CPO `strengths` (e.g. M-indices) versus `strains` on the given axis.
 
     If `ax` is None, a new figure and axes are created with `figure_unless`.
 
     Args:
     - `strains` (array) — X-values, accumulated strain (tensorial) during CPO evolution,
@@ -383,17 +377,14 @@
     - `colors` (array, optional) — color coordinates for series of strengths
     - `cpo_threshold` (float, optional) — plot a dashed line at this threshold
     - `cmaps` (Matplotlib color maps, optional) — color maps for `colors`
 
     If `colors` and `cmaps` are used, then strength values are colored individually
     within each strength series.
 
-    Additional keyword arguments are passed to `matplotlib.axes.Axes.scatter` if
-    `colors` is not `None`, or to `matplotlib.axes.Axes.plot` otherwise.
-
     Returns a tuple of the figure handle, the axes handle and the set of colors used for
     the data series plots.
 
     """
     _strains = np.atleast_2d(strains)
     _strengths = np.atleast_2d(strengths)
     if err is not None:
@@ -418,23 +409,20 @@
             ax.scatter(
                 strains,
                 strength,
                 marker=marker,
                 label=label,
                 c=colors[i],
                 cmap=cmaps[i],
-                alpha=kwargs.pop("alpha", 0.6),
-                edgecolor=kwargs.pop("edgecolor", plt.rcParams["axes.edgecolor"]),
-                **kwargs,
+                alpha=0.6,
+                edgecolor=plt.rcParams["axes.edgecolor"],
             )
             _colors.append(colors[i])
         else:
-            lines = ax.plot(
-                strains, strength, marker, alpha=0.33, label=label, **kwargs
-            )
+            lines = ax.plot(strains, strength, marker, alpha=0.33, label=label)
             _colors.append(lines[0].get_color())
         if err is not None:
             ax.fill_between(
                 strains,
                 strength - _strengths_err[i],
                 strength + _strengths_err[i],
                 alpha=0.22,
@@ -460,15 +448,14 @@
         [np.log10(f * n_grains) for f in fractions], positions=strains, widths=0.8
     )
     for part in parts["bodies"]:
         part.set_color("black")
         part.set_alpha(1)
     parts["cbars"].set_alpha(0)
     parts["cmins"].set_visible(False)
-    parts["cmaxes"].set_visible(False)
     # parts["cmaxes"].set_color("red")
     # parts["cmaxes"].set_alpha(0.5)
     return fig, ax, parts
 
 
 def show_Skemer2016_ShearStrainAngles(
     ax, studies, markers, colors, fillstyles, labels, fabric
```

### Comparing `pydrex-0.0.1/src/pydrex.egg-info/PKG-INFO` & `pydrex-0.0.1rc2/src/pydrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrex
-Version: 0.0.1
+Version: 0.0.1rc2
 Summary: Dynamic CPO calculations for olivine-enstatite polycrystal aggregates
 Author: Chris Mathews
 Author-email: Thomas Duvernay <td75013@hotmail.fr>, Leon Bilton <adigitoleo@posteo.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,18 +683,17 @@
 Project-URL: documentation, https://seismic-anisotropy.github.io/PyDRex/
 Keywords: CPO,LPO,olivine,deformation,anisotropy,crystallography
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: numpy>=1.8
 Requires-Dist: numba>=0.57
 Requires-Dist: scipy>=1.2
 Requires-Dist: pyyaml
 Requires-Dist: meshio
 Requires-Dist: matplotlib
 Requires-Dist: cmcrameri
@@ -702,24 +701,24 @@
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: pdoc; extra == "doc"
 Provides-Extra: mesh
 Requires-Dist: gmsh; extra == "mesh"
-Provides-Extra: ray
-Requires-Dist: ray>=2.0.0; extra == "ray"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: uniplot; extra == "dev"
 Requires-Dist: pdoc; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: ptpython; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Provides-Extra: lsp
 Requires-Dist: python-lsp-server; extra == "lsp"
 Requires-Dist: pyls-isort; extra == "lsp"
 Requires-Dist: python-lsp-black; extra == "lsp"
 Requires-Dist: python-lsp-ruff; extra == "lsp"
 
 # PyDRex
```

### Comparing `pydrex-0.0.1/src/pydrex.egg-info/SOURCES.txt` & `pydrex-0.0.1rc2/src/pydrex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .pre-commit-config.yaml
-CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 setup.py
 .github/workflows/ci.yml
 .github/workflows/docs.yml
 docs/assets/pydrex.png
@@ -32,15 +31,14 @@
 src/initial_implementation/visualisation/PlotDRex.py
 src/initial_implementation/visualisation/pathlineIVP.py
 src/pydrex/__init__.py
 src/pydrex/axes.py
 src/pydrex/cli.py
 src/pydrex/core.py
 src/pydrex/diagnostics.py
-src/pydrex/distributed.py
 src/pydrex/exceptions.py
 src/pydrex/geometry.py
 src/pydrex/io.py
 src/pydrex/logger.py
 src/pydrex/mesh.py
 src/pydrex/minerals.py
 src/pydrex/mock.py
@@ -92,14 +90,11 @@
 tests/test_scsv.py
 tests/test_simple_shear_2d.py
 tests/test_simple_shear_3d.py
 tests/test_tensors.py
 tests/test_vortex_2d.py
 tools/drex_forward_simpleshear.f90
 tools/find_45_seeds.py
-tools/pbs_start_ray_cluster.sh
-tools/pbs_start_ray_worker.sh
 tools/perf_compare.sh
 tools/run_fortran_ensemble.sh
 tools/simple_shear_2d.py
-tools/venv_install.sh
-tools/pbs_scripts/run_test_ray_cluster_setup.sh
+tools/venv_install.sh
```

### Comparing `pydrex-0.0.1/tests/README.md` & `pydrex-0.0.1rc2/tests/README.md`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tests/conftest.py` & `pydrex-0.0.1rc2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """> Configuration and fixtures for PyDRex tests."""
 
-import sys
-
 import matplotlib
 import pytest
 from _pytest.logging import LoggingPlugin, _LiveLoggingStreamHandler
 
 from pydrex import io as _io
 from pydrex import logger as _log
 from pydrex import mock as _mock
 from pydrex import utils as _utils
 from tests import test_vortex_2d as _test_vortex_2d
 
 _log.quiet_aliens()  # Stop imported modules from spamming the logs.
-_, HAS_RAY = _utils.import_proc_pool()
-if HAS_RAY:
-    import ray
 
 
 # Set up custom pytest CLI arguments.
 def pytest_addoption(parser):
     parser.addoption(
         "--outdir",
         metavar="DIR",
@@ -143,35 +138,14 @@
 
 
 @pytest.fixture(scope="session")
 def ncpus(request):
     return max(1, request.config.getoption("--ncpus"))
 
 
-@pytest.fixture(scope="session")
-def named_tempfile_kwargs(request):
-    if sys.platform == "win32":
-        return {"delete": False}
-    else:
-        return dict()
-
-
-@pytest.fixture(scope="session")
-def ray_session():
-    if HAS_RAY:
-        # NOTE: Expects a running Ray cluster with a number of CPUS matching --ncpus.
-        if not ray.is_initialized():
-            ray.init(address="auto")
-            _log.info("using Ray cluster with %s", ray.cluster_resources())
-        yield
-        if ray.is_initialized():
-            ray.shutdown()
-    yield
-
-
 @pytest.fixture(scope="function")
 def console_handler(request):
     if request.config.option.verbose > 0:  # Show console logs if -v/--verbose given.
         return request.config.pluginmanager.get_plugin(
             "pytest-console-logger"
         ).log_cli_handler
     return _log.CONSOLE_LOGGER
```

### Comparing `pydrex-0.0.1/tests/test_config.py` & `pydrex-0.0.1rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tests/test_core.py` & `pydrex-0.0.1rc2/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """> PyDRex: Tests for core D-Rex routines."""
 
 import contextlib as cl
-import sys
 
 import numpy as np
-import pytest
 from numpy import testing as nt
 from scipy.spatial.transform import Rotation
 
 from pydrex import core as _core
 from pydrex import io as _io
 from pydrex import logger as _log
 from pydrex import minerals as _minerals
-from pydrex import utils as _utils
 from pydrex import visualisation as _vis
+from pydrex import utils as _utils
 
 # Subdirectory of `outdir` used to store outputs from these tests.
 SUBDIR = "core"
 
 
 class TestDislocationCreepOPX:
     """Single-grain orthopyroxene crystallographic rotation rate tests."""
 
     class_id = "dislocation_creep_OPX"
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Not equal to tolerance")
     def test_shear_dudz(self, outdir):
         test_id = "dudz"
         optional_logging = cl.nullcontext()
         if outdir is not None:
             optional_logging = _log.logfile_enable(
                 f"{outdir}/{SUBDIR}/{self.class_id}_{test_id}.log"
             )
@@ -105,15 +102,14 @@
 
 
 class TestDislocationCreepOlivineA:
     """Single-grain A-type olivine analytical rotation rate tests."""
 
     class_id = "dislocation_creep_OlA"
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Not equal to tolerance")
     def test_shear_dvdx_slip_010_100(self, outdir):
         r"""Single grain of A-type olivine, slip on (010)[100].
 
         Velocity gradient:
         $$\bm{L} = \begin{bmatrix} 0 & 0 & 0 \cr 2 & 0 & 0 \cr 0 & 0 & 0 \end{bmatrix}$$
 
         """
@@ -336,15 +332,14 @@
                 ncols=3,
                 mode="expand",
             )
             fig.savefig(
                 _io.resolve_path(f"{outdir}/{SUBDIR}/{self.class_id}_{test_id}.pdf")
             )
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Not equal to tolerance")
     def test_shear_dwdx_slip_001_100(self, outdir):
         r"""Single grain of A-type olivine, slip on (001)[100].
 
         Velocity gradient:
         $$\bm{L} = \begin{bmatrix} 0 & 0 & 0 \cr 0 & 0 & 0 \cr 2 & 0 & 0 \end{bmatrix}$$
 
         """
@@ -452,15 +447,14 @@
                 ncols=3,
                 mode="expand",
             )
             fig.savefig(
                 _io.resolve_path(f"{outdir}/{SUBDIR}/{self.class_id}_{test_id}.pdf")
             )
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Not equal to tolerance")
     def test_shear_dvdz_slip_010_001(self, outdir):
         r"""Single grain of A-type olivine, slip on (010)[001].
 
         Velocity gradient:
         $$\bm{L} = \begin{bmatrix} 0 & 0 & 0 \cr 0 & 0 & 2 \cr 0 & 0 & 0 \end{bmatrix}$$
 
         """
```

### Comparing `pydrex-0.0.1/tests/test_corner_flow_2d.py` & `pydrex-0.0.1rc2/tests/test_corner_flow_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """> PyDRex: 2D corner flow tests."""
 
 import contextlib as cl
 import functools as ft
 import pathlib as pl
+from multiprocessing import Pool
 from time import perf_counter
 
 import numpy as np
 import pytest
 
 from pydrex import core as _core
 from pydrex import diagnostics as _diagnostics
@@ -16,16 +17,14 @@
 from pydrex import minerals as _minerals
 from pydrex import pathlines as _path
 from pydrex import stats as _stats
 from pydrex import utils as _utils
 from pydrex import velocity as _velocity
 from pydrex import visualisation as _vis
 
-Pool, HAS_RAY = _utils.import_proc_pool()
-
 # Subdirectory of `outdir` used to store outputs from these tests.
 SUBDIR = "2d_cornerflow"
 
 
 class TestOlivineA:
     """Tests for pure A-type olivine polycrystals in 2D corner flows."""
```

### Comparing `pydrex-0.0.1/tests/test_diagnostics.py` & `pydrex-0.0.1rc2/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tests/test_doctests.py` & `pydrex-0.0.1rc2/tests/test_doctests.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 def _get_submodule_list():
     # Reset NumPy print options because doctests are just string matches, and typing out
     # so many significant digits in doctests is annoying.
     np.set_printoptions()
     np.set_string_function(None)
     modules = ["pydrex." + m.name for m in pkgutil.iter_modules(pydrex.__path__)]
-    modules.remove("pydrex.distributed")
     try:
         from pydrex import mesh
     except ImportError:
         modules.remove("pydrex.mesh")
     return modules
 
 
@@ -35,21 +34,21 @@
         try:
             n_fails, n_tests = doctest.testmod(
                 importlib.import_module(module),
                 raise_on_error=True,
                 verbose=False,  # Change to True to debug doctest failures.
             )
             if n_fails > 0:
-                raise AssertionError(f"there were {n_fails} doctest failures from {module}")
+                raise Error(f"there were {n_fails} doctest failures from {module}")
         except doctest.DocTestFailure as e:
             if e.test.lineno is None:
                 lineno = ""
             else:
                 lineno = f":{e.test.lineno + 1 + e.example.lineno}"
-            raise AssertionError(
+            raise Error(
                 f"{e.test.name} ({module}{lineno}) failed with:"
                 + os.linesep
                 + os.linesep
                 + e.got
             ) from None
         except doctest.UnexpectedException as e:
             if e.test.lineno is None:
```

### Comparing `pydrex-0.0.1/tests/test_geometry.py` & `pydrex-0.0.1rc2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tests/test_scsv.py` & `pydrex-0.0.1rc2/tests/test_scsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """> PyDRex: tests for the SCSV plain text file format."""
 
-import sys
 import tempfile
 
 import numpy as np
 import pytest
 from numpy import testing as nt
 
 from pydrex import exceptions as _err
@@ -94,16 +93,15 @@
     nt.assert_equal(data.second_column, ["A", "B, b", ""])
     nt.assert_equal(data.third_column, [999999, 10, 1])
     nt.assert_equal(data.float_column, [1.1, np.nan, 1.0])
     nt.assert_equal(data.bool_column, [True, False, True])
     nt.assert_equal(data.complex_column, [0.1 + 0 * 1j, np.nan + 0 * 1j, 1.0 + 1 * 1j])
 
 
-@pytest.mark.skipif(sys.platform == "win32", reason="Items are not equal")
-def test_save_specfile(outdir, named_tempfile_kwargs):
+def test_save_specfile(outdir):
     """Test SCSV spec file reproduction."""
     schema = {
         "delimiter": ",",
         "missing": "-",
         "fields": [
             {
                 "name": "first_column",
@@ -154,17 +152,16 @@
 
     # The test writes two variants of the file, with identical CSV contents but
     # different YAML header specs. Contents after the header must match.
     if outdir is not None:
         _io.save_scsv(f"{outdir}/spec_out.scsv", schema, data)
         _io.save_scsv(f"{outdir}/spec_out_alt.scsv", schema_alt, data_alt)
 
-    # https://docs.python.org/3/library/tempfile.html#tempfile.NamedTemporaryFile
-    temp = tempfile.NamedTemporaryFile(**named_tempfile_kwargs)
-    temp_alt = tempfile.NamedTemporaryFile(**named_tempfile_kwargs)
+    temp = tempfile.NamedTemporaryFile()
+    temp_alt = tempfile.NamedTemporaryFile()
     _io.save_scsv(temp.name, schema, data)
     _io.save_scsv(temp_alt.name, schema_alt, data_alt)
     raw_read = []
     raw_read_alt = []
     with open(temp.name) as stream:
         raw_read = stream.readlines()[23:]  # Extra spec for first column 'fill' value.
     with open(temp_alt.name) as stream:
@@ -190,29 +187,28 @@
             [0.05, 0.10, 0.20, 0.30, 0.35, 0.40, 0.45, 0.50, 0.55, 0.60,
              0.65, 0.70, 0.75, 0.80, 0.85, 0.90, 0.95, 1.00]
         ),
     )
     # fmt: on
 
 
-def test_save_scsv_errors(named_tempfile_kwargs):
+def test_save_scsv_errors():
     """Check that we raise errors when attempting to write bad SCSV data."""
     schema = {
         "delimiter": ",",
         "missing": "-",
         "fields": [
             {
                 "name": "foo",
                 "type": "integer",
                 "fill": 999999,
             }
         ],
     }
-    # https://docs.python.org/3/library/tempfile.html#tempfile.NamedTemporaryFile
-    temp = tempfile.NamedTemporaryFile(**named_tempfile_kwargs)
+    temp = tempfile.NamedTemporaryFile()
     with pytest.raises(_err.SCSVError):
         foo = [1, 5, 0.2]
         _io.save_scsv(temp.name, schema, [foo])
         foo = [1, "foo"]
         _io.save_scsv(temp.name, schema, [foo])
         foo = ["foo"]
         _io.save_scsv(temp.name, schema, [foo])
```

### Comparing `pydrex-0.0.1/tests/test_simple_shear_2d.py` & `pydrex-0.0.1rc2/tests/test_simple_shear_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """> PyDRex: 2D simple shear tests."""
 
 import contextlib as cl
 import functools as ft
-import sys
+from multiprocessing import Pool
 from time import process_time
 
 import numpy as np
 import pytest
 from numpy import asarray as Ŋ
 from numpy import testing as nt
 from scipy.interpolate import PchipInterpolator
@@ -19,16 +19,14 @@
 from pydrex import minerals as _minerals
 from pydrex import pathlines as _paths
 from pydrex import stats as _stats
 from pydrex import utils as _utils
 from pydrex import velocity as _velocity
 from pydrex import visualisation as _vis
 
-Pool, HAS_RAY = _utils.import_proc_pool()
-
 # Subdirectory of `outdir` used to store outputs from these tests.
 SUBDIR = "2d_simple_shear"
 
 
 class TestPreliminaries:
     """Preliminary tests to check that various auxiliary routines are working."""
 
@@ -248,15 +246,14 @@
         )
         cs_X0d4 = PchipInterpolator(
             _utils.remove_nans(data.dimensionless_time_X0d4),
             45 + _utils.remove_nans(data.angle_X0d4),
         )
         return [cs_X0(strains), cs_X0d2(strains), cs_X0d4(strains)]
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Unable to allocate memory")
     def test_zero_recrystallisation(self, seed):
         """Check that M*=0 is a reliable switch to turn off recrystallisation."""
         params = _io.DEFAULT_PARAMS
         params["gbm_mobility"] = 0
         strain_rate = 1
         timestamps = np.linspace(0, 1, 25)  # Solve until D₀t=1 (tensorial strain).
         shear_direction = Ŋ([0, 1, 0], dtype=np.float64)
@@ -268,15 +265,14 @@
             get_velocity_gradient,
             shear_direction,
             seed=seed,
         )
         for fractions in mineral.fractions[1:]:
             nt.assert_allclose(fractions, mineral.fractions[0], atol=1e-15, rtol=0)
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Unable to allocate memory")
     @pytest.mark.parametrize("gbm_mobility", [50, 100, 150])
     def test_grainsize_median(self, seed, gbm_mobility):
         """Check that M*={50,100,150}, λ*=5 causes decreasing grain size median."""
         params = _io.DEFAULT_PARAMS
         params["gbm_mobility"] = gbm_mobility
         params["nucleation_efficiency"] = 5
         strain_rate = 1
```

### Comparing `pydrex-0.0.1/tests/test_simple_shear_3d.py` & `pydrex-0.0.1rc2/tests/test_simple_shear_3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 """> PyDRex: Simple shear 3D tests."""
 
 import contextlib as cl
 import functools as ft
+from multiprocessing import Pool
 from time import process_time
 
 import numpy as np
 import pytest
 
 from pydrex import core as _core
 from pydrex import diagnostics as _diagnostics
 from pydrex import geometry as _geo
 from pydrex import io as _io
 from pydrex import logger as _log
 from pydrex import minerals as _minerals
 from pydrex import stats as _stats
-from pydrex import utils as _utils
 from pydrex import velocity as _velocity
 
-Pool, HAS_RAY = _utils.import_proc_pool()
-if HAS_RAY:
-    import ray
-
-    from pydrex import distributed as _dstr
-
 # Subdirectory of `outdir` used to store outputs from these tests.
 SUBDIR = "3d_simple_shear"
 
 
 class TestFraters2021:
     """Tests inspired by the benchmarks presented in [Fraters & Billen, 2021].
 
@@ -108,15 +102,15 @@
                 get_velocity_gradient(np.nan, np.full(3, np.nan)).flatten(),
             )
         return olivine, enstatite
 
     @pytest.mark.slow
     @pytest.mark.parametrize("switch_time_Ma", [0, 1, 2.5, np.inf])
     def test_direction_change(
-        self, outdir, seeds, params_Fraters2021, switch_time_Ma, ncpus, ray_session
+        self, outdir, seeds, params_Fraters2021, switch_time_Ma, ncpus
     ):
         """Test a-axis alignment in simple shear with instantaneous geometry change.
 
         The simulation runs for 5 Ma with a strain rate of 1.58e-14/s, resulting in an
         accumulated strain invariant of 2.5.
 
         The initial shear has nonzero du/dz and the final shear has nonzero dv/dx where
@@ -187,21 +181,17 @@
                     )
                     olA_from_proj_YX[s, :] = np.array(
                         [
                             _diagnostics.smallest_angle(v, v - v * [0, 0, 1])
                             for v in olA_mean_vectors
                         ]
                     )
-                    olA_downsampled, _ = _stats.resample_orientations(
-                        olivine.orientations, olivine.fractions, seed=_seeds[s], n_samples=1000
-                    )
                     olA_strength[s, :] = _diagnostics.misorientation_indices(
-                        olA_downsampled, _geo.LatticeSystem.orthorhombic, pool=pool
+                        olA_resampled, _geo.LatticeSystem.orthorhombic, pool=pool
                     )
-
                     del olivine, olA_resampled, olA_mean_vectors
 
                     _log.info("%s; # %d; postprocessing enstatite...", _id, _seeds[s])
                     ens_resampled, _ = _stats.resample_orientations(
                         enstatite.orientations, enstatite.fractions, seed=_seeds[s]
                     )
                     ens_mean_vectors = np.array(
@@ -218,19 +208,16 @@
                     )
                     ens_from_proj_YX[s, :] = np.array(
                         [
                             _diagnostics.smallest_angle(v, v - v * [0, 0, 1])
                             for v in ens_mean_vectors
                         ]
                     )
-                    ens_downsampled, _ = _stats.resample_orientations(
-                        enstatite.orientations, enstatite.fractions, seed=_seeds[s], n_samples=1000
-                    )
                     ens_strength[s, :] = _diagnostics.misorientation_indices(
-                        ens_downsampled, _geo.LatticeSystem.orthorhombic, pool=pool
+                        ens_resampled, _geo.LatticeSystem.orthorhombic, pool=pool
                     )
                     del enstatite, ens_resampled, ens_mean_vectors
 
             _log.info("elapsed CPU time: %s", np.abs(process_time() - clock_start))
             _log.info("calculating ensemble averages...")
             olA_from_proj_XZ_mean = olA_from_proj_XZ.mean(axis=0)
             olA_from_proj_XZ_err = olA_from_proj_XZ.std(axis=0)
```

### Comparing `pydrex-0.0.1/tests/test_tensors.py` & `pydrex-0.0.1rc2/tests/test_tensors.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tests/test_vortex_2d.py` & `pydrex-0.0.1rc2/tests/test_vortex_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """> PyDRex: tests for CPO stability in 2D vortex and Stokes cell flows."""
 
 import functools as ft
-import sys
+from multiprocessing import Pool
 
 import numpy as np
 import pytest
 
 from pydrex import core as _core
 from pydrex import diagnostics as _diagnostics
 from pydrex import io as _io
 from pydrex import logger as _log
 from pydrex import minerals as _minerals
 from pydrex import pathlines as _path
 from pydrex import utils as _utils
 from pydrex import velocity as _velocity
 from pydrex import visualisation as _vis
 
-Pool, HAS_RAY = _utils.import_proc_pool()
-
 # Subdirectory of `outdir` used to store outputs from these tests.
 SUBDIR = "2d_vortex"
 
 
 class TestCellOlivineA:
     """Tests for A-type olivine polycrystals in a 2D Stokes cell."""
 
@@ -123,15 +121,14 @@
         return timestamps, positions, strains, mineral, deformation_gradient
 
     @pytest.mark.big
     def test_xz_10k(self, outdir, seed):
         """Run 2D cell test with 10000 grains (~14GiB RAM requirement)."""
         self.test_xz(outdir, seed, 10000)
 
-    @pytest.mark.skipif(sys.platform == "win32", reason="Unable to allocate memory")
     @pytest.mark.parametrize("n_grains", [100, 500, 1000, 5000])
     def test_xz(self, outdir, seed, n_grains):
         """Test to check that 5000 grains is "enough" to resolve transient features."""
         if outdir is not None:
             out_basepath = f"{outdir}/{SUBDIR}/{self.class_id}_xz_N{n_grains}"
 
         params = _io.DEFAULT_PARAMS
@@ -164,16 +161,14 @@
                 positions,
                 ".",
                 [-1, -1],
                 [1, 1],
                 [20, 20],
                 cmap="cmc.batlow_r",
                 tick_formatter=lambda x, pos: str(x),
-                aspect="equal",
-                alpha=1,
             )
             fig_path.colorbar(s, ax=ax_path, aspect=25, label="Strain (ε)")
             fig_path.savefig(_io.resolve_path(f"{out_basepath}_path.pdf"))
             # Second figure with the angles and grain sizes at every 10 strain values.
             fig = _vis.figure()
             axθ = fig.add_subplot(2, 1, 1)
             fig, axθ, colors = _vis.alignment(
```

### Comparing `pydrex-0.0.1/tools/drex_forward_simpleshear.f90` & `pydrex-0.0.1rc2/tools/drex_forward_simpleshear.f90`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tools/find_45_seeds.py` & `pydrex-0.0.1rc2/tools/find_45_seeds.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tools/perf_compare.sh` & `pydrex-0.0.1rc2/tools/perf_compare.sh`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tools/run_fortran_ensemble.sh` & `pydrex-0.0.1rc2/tools/run_fortran_ensemble.sh`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tools/simple_shear_2d.py` & `pydrex-0.0.1rc2/tools/simple_shear_2d.py`

 * *Files identical despite different names*

### Comparing `pydrex-0.0.1/tools/venv_install.sh` & `pydrex-0.0.1rc2/tools/venv_install.sh`

 * *Files identical despite different names*

