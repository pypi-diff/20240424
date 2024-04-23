# Comparing `tmp/basic_pitch-0.3.2.tar.gz` & `tmp/basic_pitch-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_pitch-0.3.2.tar", last modified: Mon Apr 22 12:53:29 2024, max compression
+gzip compressed data, was "basic_pitch-0.3.3.tar", last modified: Tue Apr 23 22:25:28 2024, max compression
```

## Comparing `basic_pitch-0.3.2.tar` & `basic_pitch-0.3.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.809470 basic_pitch-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/OWNERS.md
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-22 12:53:29.805470 basic_pitch-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.793470 basic_pitch-0.3.2/basic_pitch/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/commandline_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22517 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.793470 basic_pitch-0.3.2/basic_pitch/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/layers/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26130 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/layers/nnaudio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/layers/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/note_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.789470 basic_pitch-0.3.2/basic_pitch/saved_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.797470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.797470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/
--rw-r--r--   0 runner    (1001) docker     (127)  1084140 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.801470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/variables/
--rw-r--r--   0 runner    (1001) docker     (127)   219309 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.797470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.789470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.797470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/
--rw-r--r--   0 runner    (1001) docker     (127)   123027 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.797470 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/
--rw-r--r--   0 runner    (1001) docker     (127)   145956 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   230444 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.onnx
--rw-r--r--   0 runner    (1001) docker     (127)   204448 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.tflite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.805470 basic_pitch-0.3.2/basic_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 12:53:29.000000 basic_pitch-0.3.2/basic_pitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:53:29.809470 basic_pitch-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.801470 basic_pitch-0.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.801470 basic_pitch-0.3.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:53:29.805470 basic_pitch-0.3.2/tests/resources/vocadito_10/
--rw-r--r--   0 runner    (1001) docker     (127)  1376949 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/resources/vocadito_10/model_output.npz
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/resources/vocadito_10/note_events.npz
--rw-r--r--   0 runner    (1001) docker     (127)   802472 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/resources/vocadito_10.wav
--rw-r--r--   0 runner    (1001) docker     (127)  1075892 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/resources/vocadito_14.wav
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tests/test_note_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-22 12:53:19.000000 basic_pitch-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.844115 basic_pitch-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/OWNERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-23 22:25:28.844115 basic_pitch-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.832115 basic_pitch-0.3.3/basic_pitch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/commandline_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22517 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.832115 basic_pitch-0.3.3/basic_pitch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/layers/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26130 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/layers/nnaudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/layers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.828115 basic_pitch-0.3.3/basic_pitch/saved_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/
+-rw-r--r--   0 runner    (1001) docker     (127)  1084140 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)   219309 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.828115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/
+-rw-r--r--   0 runner    (1001) docker     (127)   123027 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.836115 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)   145956 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   230444 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)   204448 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.tflite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.844115 basic_pitch-0.3.3/basic_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 22:25:28.000000 basic_pitch-0.3.3/basic_pitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:25:28.844115 basic_pitch-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.840115 basic_pitch-0.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.840115 basic_pitch-0.3.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:25:28.844115 basic_pitch-0.3.3/tests/resources/vocadito_10/
+-rw-r--r--   0 runner    (1001) docker     (127)  1376949 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/resources/vocadito_10/model_output.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/resources/vocadito_10/note_events.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   802472 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/resources/vocadito_10.wav
+-rw-r--r--   0 runner    (1001) docker     (127)  1075892 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/resources/vocadito_14.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tests/test_note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-23 22:25:04.000000 basic_pitch-0.3.3/tox.ini
```

### Comparing `basic_pitch-0.3.2/CODE_OF_CONDUCT.md` & `basic_pitch-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/CONTRIBUTING.md` & `basic_pitch-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/LICENSE` & `basic_pitch-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/NOTICE` & `basic_pitch-0.3.3/NOTICE`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/OWNERS.md` & `basic_pitch-0.3.3/OWNERS.md`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/PKG-INFO` & `basic_pitch-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 Requires-Dist: numpy>=1.18
 Requires-Dist: onnxruntime; platform_system == "Windows" and python_version < "3.11"
 Requires-Dist: pretty_midi>=0.2.9
 Requires-Dist: resampy<0.4.3,>=0.2.2
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: tensorflow<2.15.1,>=2.4.1; platform_system != "Darwin" and python_version >= "3.11"
-Requires-Dist: tensorflow-macos<2.15.1,>=2.4.1; platform_system == "Darwin"
+Requires-Dist: tensorflow-macos<2.15.1,>=2.4.1; platform_system == "Darwin" and python_version > "3.11"
 Requires-Dist: tflite-runtime; platform_system == "Linux" and python_version < "3.11"
 Requires-Dist: typing_extensions
 Provides-Extra: test
 Requires-Dist: coverage>=5.0.2; extra == "test"
 Requires-Dist: pytest>=6.1.1; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: tf
```

### Comparing `basic_pitch-0.3.2/README.md` & `basic_pitch-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/SECURITY.md` & `basic_pitch-0.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/__init__.py` & `basic_pitch-0.3.3/basic_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/commandline_printing.py` & `basic_pitch-0.3.3/basic_pitch/commandline_printing.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/constants.py` & `basic_pitch-0.3.3/basic_pitch/constants.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/inference.py` & `basic_pitch-0.3.3/basic_pitch/inference.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/layers/math.py` & `basic_pitch-0.3.3/basic_pitch/layers/math.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/layers/nnaudio.py` & `basic_pitch-0.3.3/basic_pitch/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/layers/signal.py` & `basic_pitch-0.3.3/basic_pitch/layers/signal.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/models.py` & `basic_pitch-0.3.3/basic_pitch/models.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/nn.py` & `basic_pitch-0.3.3/basic_pitch/nn.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/note_creation.py` & `basic_pitch-0.3.3/basic_pitch/note_creation.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/predict.py` & `basic_pitch-0.3.3/basic_pitch/predict.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/model.mlmodel`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Data/com.apple.CoreML/weights/weight.bin`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.mlpackage/Manifest.json`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.onnx` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.onnx`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch/saved_models/icassp_2022/nmp.tflite` & `basic_pitch-0.3.3/basic_pitch/saved_models/icassp_2022/nmp.tflite`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch.egg-info/PKG-INFO` & `basic_pitch-0.3.3/basic_pitch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.3.2
+Version: 0.3.3
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 Requires-Dist: numpy>=1.18
 Requires-Dist: onnxruntime; platform_system == "Windows" and python_version < "3.11"
 Requires-Dist: pretty_midi>=0.2.9
 Requires-Dist: resampy<0.4.3,>=0.2.2
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: tensorflow<2.15.1,>=2.4.1; platform_system != "Darwin" and python_version >= "3.11"
-Requires-Dist: tensorflow-macos<2.15.1,>=2.4.1; platform_system == "Darwin"
+Requires-Dist: tensorflow-macos<2.15.1,>=2.4.1; platform_system == "Darwin" and python_version > "3.11"
 Requires-Dist: tflite-runtime; platform_system == "Linux" and python_version < "3.11"
 Requires-Dist: typing_extensions
 Provides-Extra: test
 Requires-Dist: coverage>=5.0.2; extra == "test"
 Requires-Dist: pytest>=6.1.1; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: tf
```

### Comparing `basic_pitch-0.3.2/basic_pitch.egg-info/SOURCES.txt` & `basic_pitch-0.3.3/basic_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/basic_pitch.egg-info/requires.txt` & `basic_pitch-0.3.3/basic_pitch.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 typing_extensions
 
 [:platform_system != "Darwin" and python_version >= "3.11"]
 tensorflow<2.15.1,>=2.4.1
 
 [:platform_system == "Darwin"]
 coremltools
+
+[:platform_system == "Darwin" and python_version > "3.11"]
 tensorflow-macos<2.15.1,>=2.4.1
 
 [:platform_system == "Linux" and python_version < "3.11"]
 tflite-runtime
 
 [:platform_system == "Windows" and python_version < "3.11"]
 onnxruntime
```

### Comparing `basic_pitch-0.3.2/pyproject.toml` & `basic_pitch-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basic-pitch"
-version = "0.3.2"
+version = "0.3.3"
 description = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection."
 readme = "README.md"
 keywords = []
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Natural Language :: English",
 	"Operating System :: POSIX :: Linux",
@@ -24,15 +24,15 @@
 	"numpy>=1.18",
 	"onnxruntime; platform_system == 'Windows' and python_version < '3.11'",
 	"pretty_midi>=0.2.9",
 	"resampy>=0.2.2,<0.4.3",
 	"scikit-learn",
 	"scipy>=1.4.1",
 	"tensorflow>=2.4.1,<2.15.1; platform_system != 'Darwin' and python_version >= '3.11'",
-	"tensorflow-macos>=2.4.1,<2.15.1; platform_system == 'Darwin'",
+	"tensorflow-macos>=2.4.1,<2.15.1; platform_system == 'Darwin' and python_version > '3.11'",
 	"tflite-runtime; platform_system == 'Linux' and python_version < '3.11'",
 	"typing_extensions",
 ]
 
 [metadata]
 author = "Spotify"
 author_email = "basic-pitch@spotify.com"
```

### Comparing `basic_pitch-0.3.2/setup.py` & `basic_pitch-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/resources/vocadito_10/model_output.npz` & `basic_pitch-0.3.3/tests/resources/vocadito_10/model_output.npz`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/resources/vocadito_10/note_events.npz` & `basic_pitch-0.3.3/tests/resources/vocadito_10/note_events.npz`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/resources/vocadito_10.wav` & `basic_pitch-0.3.3/tests/resources/vocadito_10.wav`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/resources/vocadito_14.wav` & `basic_pitch-0.3.3/tests/resources/vocadito_14.wav`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/test_inference.py` & `basic_pitch-0.3.3/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/test_nn.py` & `basic_pitch-0.3.3/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tests/test_note_creation.py` & `basic_pitch-0.3.3/tests/test_note_creation.py`

 * *Files identical despite different names*

### Comparing `basic_pitch-0.3.2/tox.ini` & `basic_pitch-0.3.3/tox.ini`

 * *Files identical despite different names*

