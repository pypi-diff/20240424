# Comparing `tmp/qiskit_alice_bob_provider-0.5.4.tar.gz` & `tmp/qiskit_alice_bob_provider-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.5.4.tar", last modified: Mon Apr 15 14:53:07 2024, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.6.0.tar", last modified: Wed Apr 24 08:39:32 2024, max compression
```

## Comparing `qiskit_alice_bob_provider-0.5.4.tar` & `qiskit_alice_bob_provider-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.968111 qiskit_alice_bob_provider-0.5.4/
--rw-r--r--   0 mdrutel    (501) staff       (20)    11342 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/LICENSE
--rw-r--r--   0 mdrutel    (501) staff       (20)       91 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/MANIFEST.in
--rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-15 14:53:07.967845 qiskit_alice_bob_provider-0.5.4/PKG-INFO
--rw-r--r--   0 mdrutel    (501) staff       (20)     3577 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/README.md
--rw-r--r--   0 mdrutel    (501) staff       (20)     2669 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/pyproject.toml
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.959881 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/
--rw-r--r--   0 mdrutel    (501) staff       (20)      867 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2490 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1039 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/errors.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962413 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/
--rw-r--r--   0 mdrutel    (501) staff       (20)      827 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7765 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/backend.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1905 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/coupling_maps.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7453 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/instruction_durations.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2295 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/job.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962670 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/
--rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7427 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2694 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/proc_to_qiskit.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6679 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/provider.py
--rw-r--r--   0 mdrutel    (501) staff       (20)    11750 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/quantum_errors.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/readout_errors.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.962821 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/
--rw-r--r--   0 mdrutel    (501) staff       (20)   257895 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
--rw-r--r--   0 mdrutel    (501) staff       (20)     4429 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/target.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.963534 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/
--rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6613 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/sk_synthesis.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     9375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/state_preparation.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.964320 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/
--rw-r--r--   0 mdrutel    (501) staff       (20)     1226 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4840 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/description.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     3112 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/interpolated_cat.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     8903 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/logical_cat.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     9624 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/physical_cat.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.964738 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/
--rw-r--r--   0 mdrutel    (501) staff       (20)     1005 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7780 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/interpolate.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4002 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/model.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7850 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/utils.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.965572 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/
--rw-r--r--   0 mdrutel    (501) staff       (20)      828 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/__init__.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.966187 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/
--rw-r--r--   0 mdrutel    (501) staff       (20)      760 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     3681 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/client.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4469 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/jobs.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1286 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/targets.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     5862 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/backend.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     8063 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/job.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2923 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/provider.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6149 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:53:07.966379 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 mdrutel    (501) staff       (20)     2162 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)        1 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)      207 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)      387 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)       26 2024-04-15 14:53:07.000000 qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)       38 2024-04-15 14:53:07.968159 qiskit_alice_bob_provider-0.5.4/setup.cfg
--rw-r--r--   0 mdrutel    (501) staff       (20)       69 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.5.4/setup.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.449397 qiskit_alice_bob_provider-0.6.0/
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11342 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/LICENSE
+-rw-r--r--   0 mdrutel    (501) staff       (20)       91 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/MANIFEST.in
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-24 08:39:32.449164 qiskit_alice_bob_provider-0.6.0/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3577 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/README.md
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2669 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/pyproject.toml
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.440059 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      867 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2490 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1039 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442420 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      827 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7765 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1905 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/coupling_maps.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7453 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/instruction_durations.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2295 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/job.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442679 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7427 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2694 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6679 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11750 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/quantum_errors.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/readout_errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442848 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/
+-rw-r--r--   0 mdrutel    (501) staff       (20)   257895 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4429 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/target.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.444416 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6613 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9375 2024-04-19 10:02:33.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/state_preparation.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.445480 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1226 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4840 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/description.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3112 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/interpolated_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     8903 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/logical_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9624 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/physical_cat.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.445920 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1005 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7780 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4002 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/model.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7850 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/utils.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.446843 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      828 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/__init__.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.447506 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      760 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3681 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/client.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4881 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/jobs.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2261 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/models.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1286 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/targets.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6806 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)    10829 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/job.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3479 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6149 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)      408 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/utils.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.447689 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2251 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)        1 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      207 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      387 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       26 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       38 2024-04-24 08:39:32.449442 qiskit_alice_bob_provider-0.6.0/setup.cfg
+-rw-r--r--   0 mdrutel    (501) staff       (20)       69 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/setup.py
```

### Comparing `qiskit_alice_bob_provider-0.5.4/LICENSE` & `qiskit_alice_bob_provider-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/PKG-INFO` & `qiskit_alice_bob_provider-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.5.4
+Version: 0.6.0
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.5.4/README.md` & `qiskit_alice_bob_provider-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/pyproject.toml` & `qiskit_alice_bob_provider-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.5.4"
+version = "0.6.0"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/backend.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/coupling_maps.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/coupling_maps.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/instruction_durations.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/instruction_durations.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/job.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/patch/local_noise_pass.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/proc_to_qiskit.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/provider.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/quantum_errors.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/quantum_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/readout_errors.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/readout_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/resources/lescanne_2020.json` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/local/target.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/target.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/sk_synthesis.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/plugins/state_preparation.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/state_preparation.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/description.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/description.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/interpolated_cat.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/interpolated_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/logical_cat.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/logical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/physical_cat.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/physical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/interpolate.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/serialization/model.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/model.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/processor/utils.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/__init__.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/client.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/jobs.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,27 @@
     Returns:
         dict: the API response object, which is the description of the
             requested job
     """
     return client.get(f'v1/jobs/{job_id}').json()
 
 
+def get_job_metrics(client: ApiClient, job_id: str) -> dict:
+    """Get exposed metrics about a job in the Alice & Bob API
+
+    Args:
+        client (ApiClient): a client for the Alice & Bob API
+        job_id (str): the ID of the job in the Alice & Bob API
+
+    Returns:
+        dict: the API response object, containing the recorded metrics.
+    """
+    return client.get(f'v1/jobs/{job_id}/metrics').json()
+
+
 def cancel_job(client: ApiClient, job_id: str) -> None:
     """Cancel a job in the Alice & Bob API
 
     This function will fail with a 409 Conflict if the job cannot be cancelled
     anymore.
 
     Args:
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/api/targets.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/backend.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from qiskit_qir import to_qir_module
 
 from ..plugins.state_preparation import EnsurePreparationPass
 from .api import jobs
 from .api.client import ApiClient
 from .job import AliceBobRemoteJob
 from .qir_to_qiskit import ab_target_to_qiskit_target
+from .utils import write_current_line
 
 
 class AliceBobRemoteBackend(BackendV2):
     """Class representing the targets accessible via the Alice & Bob API."""
 
     def __init__(self, api_client: ApiClient, target_description: Dict):
         """This class should be instantiated by the AliceBobRemoteProvider.
@@ -42,14 +43,15 @@
                 endpoint.
         """
         super().__init__(name=target_description['name'], backend_version=1)
         self._api_client = api_client
         self._target = ab_target_to_qiskit_target(target_description)
         self._options = _options_from_ab_target(target_description)
         self._translation_plugin = _determine_translation_plugin(self._target)
+        self._verbose = True
 
     def __repr__(self) -> str:
         return f'<AliceBobRemoteBackend(name={self.name})>'
 
     @property
     def target(self) -> Target:
         return self._target
@@ -60,15 +62,22 @@
 
     @property
     def max_circuits(self):
         return 1
 
     def get_translation_stage_plugin(self):
         """This hook tells Qiskit to run the transpilation passes contained
-        in translation_plugin.StatePreparationPlugin"""
+        in translation_plugin.StatePreparationPlugin.
+        This function is called before we start the circuit translation,
+        and we therefore also use it to inform that we are starting this step.
+        """
+        if self._verbose:
+            write_current_line(
+                'Translating circuit to supported operations...'
+            )
         return self._translation_plugin
 
     def update_options(self, option_updates: Dict[str, Any]) -> Options:
         options: Options = self.options
         for key, value in option_updates.items():
             if not hasattr(options, key):
                 raise ValueError(f'Backend does not support option "{key}"')
@@ -87,26 +96,37 @@
 
         Returns:
             AliceBobRemoteJob: A Qiskit job that is a reference to the job
                 created in the Alice & Bob API. The job is already started.
                 Wait for the results by calling
                 :func:`AliceBobRemoteJob.result`.
         """
+        if not isinstance(run_input, QuantumCircuit):
+            # Qiskit's execute() allows also for list[QuantumCircuit],
+            # Schedule and list[Schedule] as inputs. These types of experiments
+            # are not yet handled by the provider.
+            raise NotImplementedError(
+                'Experiments input not supported by the Alice & Bob provider. '
+                'Please provide an instance of QuantumCircuit.'
+            )
+        if self._verbose:
+            write_current_line('Sending circuit to the API...')
         options = self.update_options(kwargs)
         input_params = _ab_input_params_from_options(options)
         job = jobs.create_job(self._api_client, self.name, input_params)
         run_input = PassManager([EnsurePreparationPass()]).run(run_input)
         jobs.upload_input(
             self._api_client, job['id'], _qiskit_to_qir(run_input)
         )
         return AliceBobRemoteJob(
             backend=self,
             api_client=self._api_client,
             job_id=job['id'],
             circuit=run_input,
+            verbose=self._verbose,
         )
 
 
 def _qiskit_to_qir(circuit: QuantumCircuit) -> str:
     """Transform a Qiskit circuit into a human-readable QIR program"""
     return str(to_qir_module(circuit)[0])
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/job.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,54 +11,60 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 
 import csv
-import logging
+import time
 from dataclasses import dataclass
 from io import StringIO
-from typing import Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional
 
 from qiskit import QuantumCircuit
 from qiskit.providers import JobStatus, JobV1
 from qiskit.providers.backend import BackendV2
+from qiskit.providers.exceptions import JobTimeoutError
 from qiskit.providers.jobstatus import JOB_FINAL_STATES
 from qiskit.result import Result
 from qiskit.result.models import (
     ExperimentResult,
     ExperimentResultData,
     QobjExperimentHeader,
 )
 
 from .api import jobs
 from .api.client import ApiClient
+from .api.models import AliceBobEventType
+from .utils import write_current_line
 
 
 @dataclass
 class _DownloadedFile:
     """A class caching a file downloaded through the API."""
 
     # Tells whether this is the last version of the file
     final: bool
 
     # The content of the file if it was available and downloaded
     content: Optional[str]
 
 
+# pylint: disable=too-many-instance-attributes
 class AliceBobRemoteJob(JobV1):
     """A Qiskit job referencing a job executed in the Alice & Bob API"""
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         backend: BackendV2,
         api_client: ApiClient,
         job_id: str,
         circuit: QuantumCircuit,
+        verbose: bool,
     ):
         """A job should not be instantiated manually but created by calling
         :func:`AliceBobRemoteBackend.run` or :func:`qiskit.execute`.
 
         Args:
             backend (BackendV2): a reference to the backend that created this
                 job
@@ -67,29 +73,33 @@
             circuit (QuantumCircuit): the Qiskit circuit associated with this
                 job
         """
         super().__init__(backend, job_id)
         self._backend_v2 = backend
         self._api_client = api_client
         self._circuit = circuit
+        self._verbose = verbose
         self._last_response: Optional[Dict] = None
+        self._ab_status: Optional[AliceBobEventType] = None
         self._status: Optional[JobStatus] = None
         self._counts: Optional[Dict[str, int]] = None
         self._files: Dict[str, _DownloadedFile] = {}
+        self._metrics: Dict[str, Any] = {}
 
     def _refresh(self) -> None:
         """If the job status is not final, refresh the description of the API
         job stored by this Qiskit job
         """
         if self._status is not None and self._status in JOB_FINAL_STATES:
             return
         self._last_response = jobs.get_job(self._api_client, self.job_id())
-        self._status = _ab_event_to_qiskit_status(
+        self._ab_status = AliceBobEventType(
             self._last_response['events'][-1]['type']
         )
+        self._status = self._ab_status.to_qiskit_status()
 
     def submit(self):
         """Jobs can only be submitted by calling the ``run()`` method of the
         corresponding backend."""
         raise NotImplementedError
 
     def _get_file(
@@ -141,22 +151,92 @@
             StringIO(output),
             fieldnames=['memory', 'count'],
             delimiter=',',
         ):
             self._counts[hex(int(row['memory'], 2))] = int(row['count'])
         return self._counts
 
+    def _get_metrics(self) -> Dict[str, Any]:
+        self._metrics = jobs.get_job_metrics(self._api_client, self.job_id())
+        return self._metrics
+
+    def _monitor_state(
+        self, timeout: Optional[float] = None, wait: float = 2
+    ) -> None:
+        start_time = time.time()
+        status = self.status()
+
+        while status not in JOB_FINAL_STATES:
+            if (
+                self._verbose
+                and self._ab_status == AliceBobEventType.INPUT_READY
+            ):
+                write_current_line(
+                    f'Job {self.job_id()} is waiting to be compiled.'
+                )
+            if self._verbose and self._ab_status in {
+                AliceBobEventType.COMPILING,
+                AliceBobEventType.TRANSPILING,
+            }:
+                # We take the shortcut of assuming compilation + transpilation
+                # are the same things at the moment.
+                write_current_line(f'Job {self.job_id()} is being compiled.')
+            if (
+                self._verbose
+                and self._ab_status == AliceBobEventType.TRANSPILED
+            ):
+                write_current_line(
+                    f'Job {self.job_id()} is waiting to be executed.'
+                )
+            if (
+                self._verbose
+                and self._ab_status == AliceBobEventType.EXECUTING
+            ):
+                write_current_line(f'Job {self.job_id()} is being executed.')
+
+            elapsed_time = time.time() - start_time
+            if timeout is not None and elapsed_time >= timeout:
+                raise JobTimeoutError(
+                    f'Timeout while waiting for job {self.job_id()}.'
+                )
+
+            time.sleep(wait)
+            status = self.status()
+
+        if self._verbose and self._ab_status == AliceBobEventType.SUCCEEDED:
+            metrics = self._get_metrics()
+            success_msg = f'Job {self.job_id()} finished successfully.'
+            if 'qpu_duration_ns' in metrics and isinstance(
+                metrics['qpu_duration_ns'], int
+            ):
+                success_msg += (
+                    ' Time spent executing on QPU: '
+                    f'{_format_nanoseconds(metrics["qpu_duration_ns"])}.'
+                )
+            elif 'simulation_duration_ns' in metrics and isinstance(
+                metrics['simulation_duration_ns'], int
+            ):
+                success_msg += (
+                    ' Time spent simulating: '
+                    f'{_format_nanoseconds(metrics["simulation_duration_ns"])}'
+                    '.'
+                )
+            write_current_line(success_msg)
+        # For the other final states, Qiskit is already displaying the error
+        # with the relevant details.
+
     def result(
-        self, timeout: Optional[float] = None, wait: float = 5
+        self, timeout: Optional[float] = None, wait: float = 2
     ) -> Result:
         """Wait until the job is complete, then return a result."""
-        self.wait_for_final_state(timeout=timeout, wait=wait)
+        self._monitor_state(timeout, wait)
         status = self.status()
         assert self._last_response is not None
         success = status == JobStatus.DONE
+        print()  # Print a new line to display the next status.
         return Result(
             job_id=self.job_id(),
             backend_name=self._backend_v2.name,
             backend_version=self._backend_v2.backend_version,
             qobj_id=id(self._circuit),
             success=success,
             status=status.value,
@@ -187,44 +267,23 @@
 
     def status(self) -> JobStatus:
         """Return the status of the job, among the values of ``JobStatus``."""
         self._refresh()
         return self._status
 
 
-# pylint: disable=too-many-return-statements
-def _ab_event_to_qiskit_status(event: str) -> JobStatus:
-    """_summary_
-
-    Args:
-        event (str): an event from the Alice & Bob API, usually the latest
-            event about a given job
-
-    Returns:
-        JobStatus: a Qiskit job status
-    """
-    if event == 'CREATED':
-        return JobStatus.INITIALIZING
-    elif event in {'INPUT_READY', 'COMPILED', 'TRANSPILED'}:
-        return JobStatus.QUEUED
-    elif event in {'COMPILING', 'TRANSPILING'}:
-        return JobStatus.VALIDATING
-    elif event == 'EXECUTING':
-        return JobStatus.RUNNING
-    elif event in {
-        'COMPILATION_FAILED',
-        'TRANSPILATION_FAILED',
-        'EXECUTION_FAILED',
-        'TIMED_OUT',
-    }:
-        return JobStatus.ERROR
-    elif event == 'SUCCEEDED':
-        return JobStatus.DONE
-    elif event == 'CANCELLED':
-        return JobStatus.CANCELLED
-    logging.warning(
-        f'Received unexpected job event {event}. \n'
-        'Please ensure you are running the latest version of the Alice & Bob '
-        'Provider .'
-    )
-    # An unknown job status will be considered to be an Error by default.
-    return JobStatus.ERROR
+def _format_nanoseconds(time_ns: int) -> str:
+    """Format a given number of nanoseconds to a string containing a unit
+    and the time value converted to this unit in the most readable way.
+    This will convert the nanoseconds either to microseconds, milliseconds,
+    seconds or minutes."""
+    if time_ns < 1e3:  # < 1us
+        return f'{time_ns}ns'
+    elif time_ns < 1e6:  # < 1ms
+        return f'{(time_ns / 1e3):.2f}us'
+    elif time_ns < 1e9:  # < 1s
+        return f'{(time_ns / 1e6):.2f}ms'
+    elif time_ns < 60e9:  # < 1min
+        return f'{(time_ns / 1e9):.2f}s'
+    else:  # min & seconds format
+        minutes, seconds = divmod(time_ns / 1e9, 60)
+        return f'{minutes}min {seconds:.0f}s'
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/provider.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,20 +48,38 @@
             retries=retries,
             wait_between_retries_seconds=wait_between_retries_seconds,
         )
         self._backends = []
         for ab_target in list_targets(client):
             self._backends.append(AliceBobRemoteBackend(client, ab_target))
 
-    def get_backend(self, name=None, **kwargs) -> AliceBobRemoteBackend:
+    def get_backend(
+        self, name=None, verbose=True, **kwargs
+    ) -> AliceBobRemoteBackend:
+        """Return a single backend matching by its name.
+
+        Args:
+            name (str): name of the backend
+            verbose (bool): if True, will display information about the jobs
+                execution.
+                Defaults to True.
+            **kwargs: additional backend parameters
+                (see targets documentation).
+
+        Returns:
+            AliceBobRemoteBackend: backend matching the given name.
+        """
         backend = super().get_backend(name)
         # We allow to set the options when getting the backend,
         # to align with what we do in the local provider.
         if kwargs:
             backend.update_options(kwargs)
+
+        # pylint: disable=protected-access
+        backend._verbose = verbose
         return backend
 
     def backends(
         self, name: Optional[str] = None, **kwargs
     ) -> List[BackendV2]:
         """Return a list of backends matching the specified filtering.
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider/remote/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.5.4
+Version: 0.6.0
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.5.4/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,13 @@
 qiskit_alice_bob_provider/processor/serialization/interpolate.py
 qiskit_alice_bob_provider/processor/serialization/model.py
 qiskit_alice_bob_provider/remote/__init__.py
 qiskit_alice_bob_provider/remote/backend.py
 qiskit_alice_bob_provider/remote/job.py
 qiskit_alice_bob_provider/remote/provider.py
 qiskit_alice_bob_provider/remote/qir_to_qiskit.py
+qiskit_alice_bob_provider/remote/utils.py
 qiskit_alice_bob_provider/remote/api/__init__.py
 qiskit_alice_bob_provider/remote/api/client.py
 qiskit_alice_bob_provider/remote/api/jobs.py
+qiskit_alice_bob_provider/remote/api/models.py
 qiskit_alice_bob_provider/remote/api/targets.py
```

