# Comparing `tmp/qbraid-0.7.0.dev20240417171913.tar.gz` & `tmp/qbraid-0.7.0.dev20240423224133.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.7.0.dev20240417171913.tar", last modified: Wed Apr 17 17:19:16 2024, max compression
+gzip compressed data, was "qbraid-0.7.0.dev20240423224133.tar", last modified: Tue Apr 23 22:41:36 2024, max compression
```

## Comparing `qbraid-0.7.0.dev20240417171913.tar` & `qbraid-0.7.0.dev20240423224133.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55229 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.027361 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.027361 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.transforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 17:19:13.000000 qbraid-0.7.0.dev20240417171913/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/ionq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/custom_instr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/custom_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55229 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-17 17:19:16.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tools/set_provider_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55236 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.341251 qbraid-0.7.0.dev20240423224133/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.345251 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.345251 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.transforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.349251 qbraid-0.7.0.dev20240423224133/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 22:41:33.000000 qbraid-0.7.0.dev20240423224133/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.353251 qbraid-0.7.0.dev20240423224133/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/abc_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.357251 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/providers/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/ionq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.361251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/custom_instr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/custom_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/transpiler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55236 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 22:41:36.000000 qbraid-0.7.0.dev20240423224133/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:41:36.373251 qbraid-0.7.0.dev20240423224133/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:36.365251 qbraid-0.7.0.dev20240423224133/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tools/set_provider_configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-23 22:41:25.000000 qbraid-0.7.0.dev20240423224133/tox.ini
```

### Comparing `qbraid-0.7.0.dev20240417171913/CODE_OF_CONDUCT.md` & `qbraid-0.7.0.dev20240423224133/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/CONTRIBUTING.md` & `qbraid-0.7.0.dev20240423224133/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/LICENSE` & `qbraid-0.7.0.dev20240423224133/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/PKG-INFO` & `qbraid-0.7.0.dev20240423224133/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.7.0.dev20240417171913
+Version: 0.7.0.dev20240423224133
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,21 +701,21 @@
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
 Requires-Dist: qbraid-core<0.2.0,>=0.1.3
 Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk<1.78.0,>=1.42.1; extra == "braket"
+Requires-Dist: amazon-braket-sdk<1.79.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
-Requires-Dist: pytket<1.27.0,>=1.16.0; extra == "pytket"
+Requires-Dist: pytket<1.28.0,>=1.16.0; extra == "pytket"
 Provides-Extra: pyquil
 Requires-Dist: pyquil<4.4.0,>=3.5.4; extra == "pyquil"
 Provides-Extra: qir
 Requires-Dist: qbraid-qir<0.2.0,>=0.1.1; extra == "qir"
 Provides-Extra: qiskit
 Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit"
 Requires-Dist: qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "qiskit"
@@ -733,16 +733,16 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
+Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<2.2,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 <p align="center">
   <a href="https://github.com/qBraid/qBraid/actions/workflows/main.yml">
```

### Comparing `qbraid-0.7.0.dev20240417171913/README.md` & `qbraid-0.7.0.dev20240423224133/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/cards/jupyter.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/cards/python.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/cards/terminal.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/favicon.ico` & `qbraid-0.7.0.dev20240423224133/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/logo.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/braket.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/cirq.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qasm.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qir.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/get_devices.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.7.0.dev20240423224133/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/conf.py` & `qbraid-0.7.0.dev20240423224133/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/index.rst` & `qbraid-0.7.0.dev20240423224133/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/devices.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/jobs.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/overview.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/programs.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/programs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/results.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/docs/sdk/transpiler.rst` & `qbraid-0.7.0.dev20240423224133/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/pyproject.toml` & `qbraid-0.7.0.dev20240423224133/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,26 @@
 Documentation = "https://docs.qbraid.com/en/stable/"
 "Source Code" = "https://github.com/qBraid/qBraid"
 "Bug Tracker" = "https://github.com/qBraid/qBraid/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git"
 
 [project.optional-dependencies]
-braket = ["amazon-braket-sdk>=1.42.1,<1.78.0"]
+braket = ["amazon-braket-sdk>=1.42.1,<1.79.0"]
 cirq = ["cirq-core>=1.3.0,<1.4.0"]
 pennylane = ["pennylane>=0.33.1,<0.36.0"]
-pytket = ["pytket>=1.16.0,<1.27.0"]
+pytket = ["pytket>=1.16.0,<1.28.0"]
 pyquil = ["pyquil>=3.5.4,<4.4.0"]
 qir = ["qbraid-qir>=0.1.1,<0.2.0"]
 qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-provider>=0.5.3,<0.11.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0", "qiskit[visualization]"]
 ionq = ["cirq-core>=1.3.0,<1.4.0", "cirq-ionq>=1.3.0,<1.4.0", "pytket-braket>=0.30.0,<0.36.0"]
 visualization = ["ipython", "matplotlib", "pylatexenc"]
 test = ["pytest", "pytest-cov"]
 lint = ["black", "isort", "pylint"]
-docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22"]
+docs = ["sphinx>=7.2.6,<7.4.0", "sphinx-autodoc-typehints>=1.24,<2.2", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22"]
 
 [project.entry-points."qbraid.programs"]
 braket = "qbraid.programs.libs.braket:BraketCircuit"
 cirq = "qbraid.programs.libs.cirq:CirqCircuit"
 pennylane = "qbraid.programs.libs.pennylane:PennylaneTape"
 pyquil = "qbraid.programs.libs.pyquil:PyQuilProgram"
 qiskit = "qbraid.programs.libs.qiskit:QiskitCircuit"
```

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/_about.py` & `qbraid-0.7.0.dev20240423224133/qbraid/_about.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/_compat.py` & `qbraid-0.7.0.dev20240423224133/qbraid/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/_display.py` & `qbraid-0.7.0.dev20240423224133/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/_import.py` & `qbraid-0.7.0.dev20240423224133/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/get_devices.py` & `qbraid-0.7.0.dev20240423224133/qbraid/get_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/get_jobs.py` & `qbraid-0.7.0.dev20240423224133/qbraid/get_jobs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/circuit_equality.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/circuit_equality.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/cirq_random.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qasm3_random.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qiskit_random.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/random.py` & `qbraid-0.7.0.dev20240423224133/qbraid/interface/random/random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/_import.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/abc_program.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/abc_program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/inspector.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/inspector.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/braket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/cirq.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pennylane.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pyquil.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pytket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm2.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm3.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qiskit.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/loader.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/loader.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_passes.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_qelib1.py` & `qbraid-0.7.0.dev20240423224133/qbraid/programs/qasm_qelib1.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/_import.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/device.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/job.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/provider.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/result.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/tracker.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/aws/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/device.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/enums.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/device.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/job.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/provider.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/result.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/job.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/provider.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/result.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/providers/status_maps.py` & `qbraid-0.7.0.dev20240423224133/qbraid/providers/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transforms/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transforms/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transforms/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/ionq.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transforms/pytket/ionq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/annotations.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/cirq_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_cirq.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/custom_instr.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/braket/custom_instr.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/custom_ops.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/cirq/custom_ops.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pennylane/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/conversions_cirq.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pyquil/conversions_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_braket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/pytket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_braket.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_qasm.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/conversions/qiskit/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/converter.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/converter.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/edge.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/edge.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/graph.py` & `qbraid-0.7.0.dev20240423224133/qbraid/transpiler/graph.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/__init__.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_circuit.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_qasm3.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/exceptions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_conversions.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_counts.py` & `qbraid-0.7.0.dev20240423224133/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/PKG-INFO` & `qbraid-0.7.0.dev20240423224133/qbraid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.7.0.dev20240417171913
+Version: 0.7.0.dev20240423224133
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,21 +701,21 @@
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
 Requires-Dist: qbraid-core<0.2.0,>=0.1.3
 Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk<1.78.0,>=1.42.1; extra == "braket"
+Requires-Dist: amazon-braket-sdk<1.79.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
-Requires-Dist: pytket<1.27.0,>=1.16.0; extra == "pytket"
+Requires-Dist: pytket<1.28.0,>=1.16.0; extra == "pytket"
 Provides-Extra: pyquil
 Requires-Dist: pyquil<4.4.0,>=3.5.4; extra == "pyquil"
 Provides-Extra: qir
 Requires-Dist: qbraid-qir<0.2.0,>=0.1.1; extra == "qir"
 Provides-Extra: qiskit
 Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit"
 Requires-Dist: qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "qiskit"
@@ -733,16 +733,16 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
+Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<2.2,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 <p align="center">
   <a href="https://github.com/qBraid/qBraid/actions/workflows/main.yml">
```

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/SOURCES.txt` & `qbraid-0.7.0.dev20240423224133/qbraid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/entry_points.txt` & `qbraid-0.7.0.dev20240423224133/qbraid.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/requires.txt` & `qbraid-0.7.0.dev20240423224133/qbraid.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 networkx<4.0,>=2.5
 numpy<1.27,>=1.17
 openqasm3[parser]<0.6.0,>=0.4.0
 ply>=3.6
 qbraid-core<0.2.0,>=0.1.3
 
 [braket]
-amazon-braket-sdk<1.78.0,>=1.42.1
+amazon-braket-sdk<1.79.0,>=1.42.1
 
 [cirq]
 cirq-core<1.4.0,>=1.3.0
 
 [docs]
-sphinx~=7.2.6
-sphinx-autodoc-typehints<2.1,>=1.24
+sphinx<7.4.0,>=7.2.6
+sphinx-autodoc-typehints<2.2,>=1.24
 sphinx-rtd-theme<2.1,>=1.3
 docutils<0.22
 
 [ionq]
 cirq-core<1.4.0,>=1.3.0
 cirq-ionq<1.4.0,>=1.3.0
 pytket-braket<0.36.0,>=0.30.0
@@ -29,15 +29,15 @@
 [pennylane]
 pennylane<0.36.0,>=0.33.1
 
 [pyquil]
 pyquil<4.4.0,>=3.5.4
 
 [pytket]
-pytket<1.27.0,>=1.16.0
+pytket<1.28.0,>=1.16.0
 
 [qir]
 qbraid-qir<0.2.0,>=0.1.1
 
 [qiskit]
 qiskit<1.1.0,>=0.44.0
 qiskit-ibm-provider<0.11.0,>=0.5.3
```

### Comparing `qbraid-0.7.0.dev20240417171913/tools/set_provider_configs.py` & `qbraid-0.7.0.dev20240423224133/tools/set_provider_configs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/tools/verify_headers.py` & `qbraid-0.7.0.dev20240423224133/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240417171913/tox.ini` & `qbraid-0.7.0.dev20240423224133/tox.ini`

 * *Files identical despite different names*

