# Comparing `tmp/tensorrt_llm-0.9.0.dev2024040200.tar.gz` & `tmp/tensorrt_llm-0.9.0.dev2024040900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt_llm-0.9.0.dev2024040200.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "tensorrt_llm-0.9.0.dev2024040900.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `tensorrt_llm-0.9.0.dev2024040200.tar` & `tensorrt_llm-0.9.0.dev2024040900.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     2286 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     2217 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-llm
-Version: 0.9.0.dev2024040200
+Version: 0.9.0.dev2024040900
 Summary: TensorRT-LLM: A TensorRT Toolbox for Large Language Models
 Home-page: https://github.com/NVIDIA/TensorRT-LLM
 Download-URL: https://github.com/NVIDIA/TensorRT-LLM/tags
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Keywords: nvidia tensorrt deeplearning inference
 Classifier: Development Status :: 4 - Beta
@@ -33,24 +33,22 @@
 Requires-Dist: torch <=2.3.0a,>=2.2.0a
 Requires-Dist: nvidia-ammo ~=0.7.0
 Requires-Dist: transformers ==4.38.2
 Requires-Dist: wheel
 Requires-Dist: optimum
 Requires-Dist: evaluate
 Requires-Dist: janus
-Requires-Dist: setuptools
 Requires-Dist: mpmath ==1.3.0
 Requires-Dist: nvidia-cudnn-cu12 ~=8.9 ; platform_machine == "x86_64"
 Provides-Extra: benchmarking
 Requires-Dist: click ; extra == 'benchmarking'
 Requires-Dist: pydantic ; extra == 'benchmarking'
 Provides-Extra: devel
 Requires-Dist: datasets ; extra == 'devel'
 Requires-Dist: einops ; extra == 'devel'
-Requires-Dist: evaluate ; extra == 'devel'
 Requires-Dist: graphviz ; extra == 'devel'
 Requires-Dist: mypy ; extra == 'devel'
 Requires-Dist: parameterized ; extra == 'devel'
 Requires-Dist: pre-commit ; extra == 'devel'
 Requires-Dist: pybind11 ; extra == 'devel'
 Requires-Dist: pybind11-stubgen ; extra == 'devel'
 Requires-Dist: pytest-cov ; extra == 'devel'
```

