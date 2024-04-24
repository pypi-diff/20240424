# Comparing `tmp/quingo-0.2.2.tar.gz` & `tmp/quingo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quingo-0.2.2.tar", last modified: Sun Dec 10 11:14:55 2023, max compression
+gzip compressed data, was "quingo-0.3.1.tar", last modified: Wed Apr 24 03:57:53 2024, max compression
```

## Comparing `quingo-0.2.2.tar` & `quingo-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.211885 quingo-0.2.2/
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)    11356 2023-10-17 01:38:25.000000 quingo-0.2.2/LICENSE
--rw-r--r--   0 chenwenjin  (1006) chenwenjin  (1006)     4876 2023-12-10 11:14:55.211885 quingo-0.2.2/PKG-INFO
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)     4168 2023-12-10 11:09:49.000000 quingo-0.2.2/README.md
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      119 2023-10-17 01:38:25.000000 quingo-0.2.2/pyproject.toml
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      743 2023-12-10 11:14:55.211885 quingo-0.2.2/setup.cfg
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)       38 2023-10-17 01:38:25.000000 quingo-0.2.2/setup.py
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.203884 quingo-0.2.2/src/
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.207885 quingo-0.2.2/src/quingo/
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)      263 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/__init__.py
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.211885 quingo-0.2.2/src/quingo/backend/
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/__init__.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)     2845 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/backend_hub.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)      750 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/if_backend.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)     1779 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/pyqcisim_quantumsim.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      955 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/pyqcisim_tequila.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      920 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/qisa.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     2514 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/qualesim_quantumsim.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     2907 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/qualesim_tequila.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     1223 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/result_formatter.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     2067 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/symqc.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     2484 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/backend/xiaohong.py
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.211885 quingo-0.2.2/src/quingo/core/
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-10-17 01:38:25.000000 quingo-0.2.2/src/quingo/core/__init__.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     2585 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/compile.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     3512 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/compiler_config.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      439 2023-10-17 01:38:25.000000 quingo-0.2.2/src/quingo/core/data.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)    10241 2023-10-17 01:38:25.000000 quingo-0.2.2/src/quingo/core/data_transfer.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)      793 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/exe_config.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)     1508 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/manager.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     3829 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/preparation.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     4632 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/quingo_task.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)     1637 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/core/utils.py
--rwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)      906 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/global_config.py
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)    13075 2023-12-10 11:09:49.000000 quingo-0.2.2/src/quingo/install_quingoc.py
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.211885 quingo-0.2.2/src/quingo/lib/
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-10-17 01:38:25.000000 quingo-0.2.2/src/quingo/lib/__init__.py
-drwxrwxr-x   0 chenwenjin  (1006) chenwenjin  (1006)        0 2023-12-10 11:14:55.211885 quingo-0.2.2/src/quingo.egg-info/
--rw-r--r--   0 chenwenjin  (1006) chenwenjin  (1006)     4876 2023-12-10 11:14:55.000000 quingo-0.2.2/src/quingo.egg-info/PKG-INFO
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)     1004 2023-12-10 11:14:55.000000 quingo-0.2.2/src/quingo.egg-info/SOURCES.txt
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)        1 2023-12-10 11:14:55.000000 quingo-0.2.2/src/quingo.egg-info/dependency_links.txt
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)       67 2023-12-10 11:14:55.000000 quingo-0.2.2/src/quingo.egg-info/requires.txt
--rw-rw-r--   0 chenwenjin  (1006) chenwenjin  (1006)        7 2023-12-10 11:14:55.000000 quingo-0.2.2/src/quingo.egg-info/top_level.txt
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.935487 quingo-0.3.1/
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)    11356 2023-07-06 12:05:30.000000 quingo-0.3.1/LICENSE
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3957 2024-04-24 03:57:53.935487 quingo-0.3.1/PKG-INFO
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)     3451 2024-04-24 03:55:03.000000 quingo-0.3.1/README.md
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      119 2023-07-06 12:05:30.000000 quingo-0.3.1/pyproject.toml
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      810 2024-04-24 03:57:53.935487 quingo-0.3.1/setup.cfg
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)       38 2023-07-06 12:05:30.000000 quingo-0.3.1/setup.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.931487 quingo-0.3.1/src/
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.931487 quingo-0.3.1/src/quingo/
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)      276 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/__init__.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.935487 quingo-0.3.1/src/quingo/backend/
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)      302 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/__init__.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)     2653 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/backend_hub.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)      676 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/if_backend.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)     1709 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/pyqcisim_quantumsim.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     1503 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/pyqcisim_tequila.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      920 2023-12-13 03:48:08.000000 quingo-0.3.1/src/quingo/backend/qisa.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3619 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/qualesim.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3215 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/result_formatter.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     1667 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/symqc.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     2456 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/backend/xiaohong.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.935487 quingo-0.3.1/src/quingo/core/
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        0 2023-07-06 12:05:30.000000 quingo-0.3.1/src/quingo/core/__init__.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     2658 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/compile.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3531 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/compiler_config.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      439 2023-07-27 07:16:00.000000 quingo-0.3.1/src/quingo/core/data.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)    10273 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/data_transfer.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     1030 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/exe_config.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)     2310 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/manager.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3836 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/preparation.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)     1468 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/core/quingo_logger.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     4623 2024-04-24 03:55:03.000000 quingo-0.3.1/src/quingo/core/quingo_task.py
+-rwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)      906 2023-12-13 03:48:08.000000 quingo-0.3.1/src/quingo/global_config.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)    13075 2023-12-13 03:48:08.000000 quingo-0.3.1/src/quingo/install_quingoc.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.935487 quingo-0.3.1/src/quingo/lib/
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        0 2023-07-06 12:05:30.000000 quingo-0.3.1/src/quingo/lib/__init__.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     1306 2024-04-24 03:23:01.000000 quingo-0.3.1/src/quingo/utils.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-24 03:57:53.931487 quingo-0.3.1/src/quingo.egg-info/
+-rw-r--r--   0 xiangfu   (1005) xiangfu   (1005)     3957 2024-04-24 03:57:53.000000 quingo-0.3.1/src/quingo.egg-info/PKG-INFO
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      982 2024-04-24 03:57:53.000000 quingo-0.3.1/src/quingo.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        1 2024-04-24 03:57:53.000000 quingo-0.3.1/src/quingo.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      123 2024-04-24 03:57:53.000000 quingo-0.3.1/src/quingo.egg-info/requires.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        7 2024-04-24 03:57:53.000000 quingo-0.3.1/src/quingo.egg-info/top_level.txt
```

### Comparing `quingo-0.2.2/LICENSE` & `quingo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quingo-0.2.2/PKG-INFO` & `quingo-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 Metadata-Version: 2.1
 Name: quingo
-Version: 0.2.2
+Version: 0.3.1
 Summary: Quingo Runtime System
 Home-page: https://gitee.com/quingo/quingo-runtime
 Author: Xiang Fu
 Author-email: gtaifu@gmail.com
 Project-URL: Bug Tracker, https://gitee.com/quingo/quingo-runtime/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pyqcas
-Requires-Dist: pyqcisim
-Requires-Dist: symqc
-Requires-Dist: colorama
-Requires-Dist: termcolor
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: pyezq
 
 # Quingo Runtime System
 
 Along with quingo compilers, the Quingo runtime system which provides users the capability to program and simulate Quingo programs.
 
 ## Installation
 
@@ -34,27 +25,20 @@
 Install Quingo runtime system with required simulators using the following command:
 ```sh
 pip install -e .
 ```
 
 ```sh
 # for simulators used:
+# The Tequila backend is not yet open source and needs to be installed separately.
 git clone https://gitee.com/hpcl_quanta/tequila.git
-git checkout xbackend
-pip install -e .
-
-git clone https://gitee.com/quingo/pyqcisim.git
-git checkout bug-fix
-pip install -e .
-
-git clone https://gitee.com/quingo/SymQC.git
 pip install -e .
 ```
 
-Upon success, it will automatically install the Quingo runtime system (this package), the PyQCAS simulator and the PyQCISim simulator.
+Upon success, it will automatically install the Quingo runtime system (this package), the SymQC simulator, the PyQCISim simulator and the QuaLeSim simulator.
 
 ### Install the Quingo compiler
 
 We can install mlir-based quingo compiler in two ways:
 
 + Install the mlir-based Quingo compiler using the following command:
   ```sh
@@ -81,26 +65,28 @@
 sim res:  (['Q1', 'Q2'], [[0, 0], [0, 0], [1, 1], [1, 1], [0, 0], [0, 0], [0, 0], [1, 1], [0, 0], [1, 1]])
 ```
 For different simulation backend, please refer to `src/examples/sim_backend`, which shows the use of SymQC, QuantumSim, and Tequila backend that are currently running stably.
 
 For different simulation modes, please refer to `src/examples/sim_exemode`, which displays the output of two different simulation results currently available.
 
 ## APIs of the Quingo runtime system
-The `Quingo_interface` class expose the following methods:
- - `set_log_level(<log_level>)`: `<log_level>` can be one of `DEBUG`, `INFO`, `WARNING`, `ERROR`, or `CRITICAL`.
- - `connect_backend(<backend>)`: `<backend>` currently can be `'pyqcas_quantumsim'` or `'pyqcisim_quantumsim'`.
-- `get_backend_name()`: return the name of the backend that is being used. An empty string will be returned if no backend has been set.
-- `get_last_qasm()`: get the qasm code generated by the last execution.
-- `config_execution(<mode>, <num_shots>)`:
-  -  Configure the execution mode to `'one_shot'` or `'state_vector'`.
-  -  When the execution mode is `'one_shot'`, the number of times to run the uploaded quantum circuit can be configured using the parameter `num_shots` at the same time.
--  `call_quingo(<qg_filename>, <qg_func_name>, *args)`:
-   - the main entry to call Quingo operation.
-   - `<qg_filename (str)>` :  the name of the Qingo file which contains the quantum function called by the host program.
-   - `<qg_func_name (str)>` : the name of the quantum function
-   - `<args (dict)>`: a variable length of parameters used to call the Quingo operation in the form `qg_func_name(<args>)`.
- - `read_result()`: read the computation result from the quantum kernel.
-   - For eQASM-based backend, the result is a binary block which encodes the quantum computation result.
-   - For QCIS-based backend, the result format is defined by PyQCISim. Please refer to the docstring of `quingo.if_backend.non_arch_backend.pyqcisim_quantumsim.PyQCISim_quantumsim::execute()`
+1. `class Quingo_task`:
+   - 输入：
+      - `called_qu_fn`: `Path`，qu文件路径。
+      - `called_func`: `str`，调用 quingo 函数名。
+      - `debug_mode`(optional): `True` or `False`。
+      - `qisa`(optional): 前端指令集类型。
+      - `backend`(optional): 后端模拟器类型。
+2. `function compile()`:
+   - 输入：
+      - `Quingo_task`: 待编译 qu 任务
+      - `params`: `Quingo_task` 中调用函数 `called_func` 所需参数
+   - 输出：`qasm_fn`：输出对应指令集文件(.qcis / .qi)
+3. `function execute()`:
+   - 输入：
+      - `qasm_fn`: `Path`，对应指令集文件(.qcis / .qi)
+      - `be_type`: `BackendType`，模拟器后端类型
+      - `exe_config`: 执行模式，`ExeMode.SimShots`、`ExeMode.SimFinalResult`、`ExeMode.SimStateVector` 
+   - 输出：`sim_result`：具体输出格式详见`src/quingo/backend/quingo_result_format_spec.md`
 
 ## Quingo programming tutorial
 At present, Qingguo runtime system has included sample programs such as `Bell_state`, `GHZ`, `VQE`, etc. Details can be found [here](https://gitee.com/quingo/quingo-runtime/tree/master/src/examples).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quingo-0.2.2/README.md` & `quingo-0.3.1/src/quingo.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: quingo
+Version: 0.3.1
+Summary: Quingo Runtime System
+Home-page: https://gitee.com/quingo/quingo-runtime
+Author: Xiang Fu
+Author-email: gtaifu@gmail.com
+Project-URL: Bug Tracker, https://gitee.com/quingo/quingo-runtime/issues
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Quingo Runtime System
 
 Along with quingo compilers, the Quingo runtime system which provides users the capability to program and simulate Quingo programs.
 
 ## Installation
 
 The Quingo installation comprises of two main steps:
@@ -10,27 +25,20 @@
 Install Quingo runtime system with required simulators using the following command:
 ```sh
 pip install -e .
 ```
 
 ```sh
 # for simulators used:
+# The Tequila backend is not yet open source and needs to be installed separately.
 git clone https://gitee.com/hpcl_quanta/tequila.git
-git checkout xbackend
-pip install -e .
-
-git clone https://gitee.com/quingo/pyqcisim.git
-git checkout bug-fix
-pip install -e .
-
-git clone https://gitee.com/quingo/SymQC.git
 pip install -e .
 ```
 
-Upon success, it will automatically install the Quingo runtime system (this package), the PyQCAS simulator and the PyQCISim simulator.
+Upon success, it will automatically install the Quingo runtime system (this package), the SymQC simulator, the PyQCISim simulator and the QuaLeSim simulator.
 
 ### Install the Quingo compiler
 
 We can install mlir-based quingo compiler in two ways:
 
 + Install the mlir-based Quingo compiler using the following command:
   ```sh
@@ -57,26 +65,28 @@
 sim res:  (['Q1', 'Q2'], [[0, 0], [0, 0], [1, 1], [1, 1], [0, 0], [0, 0], [0, 0], [1, 1], [0, 0], [1, 1]])
 ```
 For different simulation backend, please refer to `src/examples/sim_backend`, which shows the use of SymQC, QuantumSim, and Tequila backend that are currently running stably.
 
 For different simulation modes, please refer to `src/examples/sim_exemode`, which displays the output of two different simulation results currently available.
 
 ## APIs of the Quingo runtime system
-The `Quingo_interface` class expose the following methods:
- - `set_log_level(<log_level>)`: `<log_level>` can be one of `DEBUG`, `INFO`, `WARNING`, `ERROR`, or `CRITICAL`.
- - `connect_backend(<backend>)`: `<backend>` currently can be `'pyqcas_quantumsim'` or `'pyqcisim_quantumsim'`.
-- `get_backend_name()`: return the name of the backend that is being used. An empty string will be returned if no backend has been set.
-- `get_last_qasm()`: get the qasm code generated by the last execution.
-- `config_execution(<mode>, <num_shots>)`:
-  -  Configure the execution mode to `'one_shot'` or `'state_vector'`.
-  -  When the execution mode is `'one_shot'`, the number of times to run the uploaded quantum circuit can be configured using the parameter `num_shots` at the same time.
--  `call_quingo(<qg_filename>, <qg_func_name>, *args)`:
-   - the main entry to call Quingo operation.
-   - `<qg_filename (str)>` :  the name of the Qingo file which contains the quantum function called by the host program.
-   - `<qg_func_name (str)>` : the name of the quantum function
-   - `<args (dict)>`: a variable length of parameters used to call the Quingo operation in the form `qg_func_name(<args>)`.
- - `read_result()`: read the computation result from the quantum kernel.
-   - For eQASM-based backend, the result is a binary block which encodes the quantum computation result.
-   - For QCIS-based backend, the result format is defined by PyQCISim. Please refer to the docstring of `quingo.if_backend.non_arch_backend.pyqcisim_quantumsim.PyQCISim_quantumsim::execute()`
+1. `class Quingo_task`:
+   - 输入：
+      - `called_qu_fn`: `Path`，qu文件路径。
+      - `called_func`: `str`，调用 quingo 函数名。
+      - `debug_mode`(optional): `True` or `False`。
+      - `qisa`(optional): 前端指令集类型。
+      - `backend`(optional): 后端模拟器类型。
+2. `function compile()`:
+   - 输入：
+      - `Quingo_task`: 待编译 qu 任务
+      - `params`: `Quingo_task` 中调用函数 `called_func` 所需参数
+   - 输出：`qasm_fn`：输出对应指令集文件(.qcis / .qi)
+3. `function execute()`:
+   - 输入：
+      - `qasm_fn`: `Path`，对应指令集文件(.qcis / .qi)
+      - `be_type`: `BackendType`，模拟器后端类型
+      - `exe_config`: 执行模式，`ExeMode.SimShots`、`ExeMode.SimFinalResult`、`ExeMode.SimStateVector` 
+   - 输出：`sim_result`：具体输出格式详见`src/quingo/backend/quingo_result_format_spec.md`
 
 ## Quingo programming tutorial
-At present, Qingguo runtime system has included sample programs such as `Bell_state`, `GHZ`, `VQE`, etc. Details can be found [here](https://gitee.com/quingo/quingo-runtime/tree/master/src/examples).
+At present, Qingguo runtime system has included sample programs such as `Bell_state`, `GHZ`, `VQE`, etc. Details can be found [here](https://gitee.com/quingo/quingo-runtime/tree/master/src/examples).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quingo-0.2.2/setup.cfg` & `quingo-0.3.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = quingo
-version = 0.2.2
+version = 0.3.1
 author = Xiang Fu
 author_email = gtaifu@gmail.com
 use_2to3 = False
 description = Quingo Runtime System
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/quingo/quingo-runtime
@@ -18,22 +18,23 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy
-	pyqcas
-	pyqcisim
-	symqc
+	pyqcisim >= 1.3.1
+	symqc >= 1.1.1
 	colorama
 	termcolor
 	requests
 	tqdm
-	pyezq
+	qualesim >= 1.0.2
+	qualesim-tequila >= 1.0.2
+	pyquiet >= 0.0.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `quingo-0.2.2/src/quingo/backend/backend_hub.py` & `quingo-0.3.1/src/quingo/backend/backend_hub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 import importlib
 import enum
-from .qisa import Qisa
+from quingo.backend.qisa import Qisa
+from quingo.utils import singleton
 
 
 class BackendType(enum.Enum):
     QUANTUM_SIM = enum.auto()
     TEQUILA = enum.auto()
     SYMQC = enum.auto()
     QUANTIFY = enum.auto()
     XIAOHONG = enum.auto()
-    # QUALESIM_TEQUILA = enum.auto()
-    # QUALESIM_QUANTUMSIM = enum.auto()
-
-
-def singleton(cls):
-    _instance = {}
-
-    def inner():
-        if cls not in _instance:
-            _instance[cls] = cls()
-        return _instance[cls]
-
-    return inner
+    QUALESIM_TEQUILA = enum.auto()
+    QUALESIM_QUANTUMSIM = enum.auto()
 
 
 @singleton
 class Backend_hub:
     def __init__(self):
         self.backends = {
             BackendType.QUANTUM_SIM: (
@@ -54,26 +44,26 @@
             ),
             BackendType.XIAOHONG: (
                 "XiaoHong",
                 "xiaohong",
                 False,
                 Qisa.QCIS,
             ),
-            # BackendType.QUALESIM_TEQUILA: (
-            #     "QuaLeSim_tequila",
-            #     "qualesim_tequila",
-            #     True,
-            #     Qisa.QCIS,
-            # ),
-            # BackendType.QUALESIM_QUANTUMSIM: (
-            #     "QuaLeSim_quantumsim",
-            #     "qualesim_quantumsim",
-            #     True,
-            #     Qisa.QCIS,
-            # ),
+            BackendType.QUALESIM_TEQUILA: (
+                "QuaLeSim",
+                "qualesim",
+                True,
+                Qisa.QCIS,
+            ),
+            BackendType.QUALESIM_QUANTUMSIM: (
+                "QuaLeSim",
+                "qualesim",
+                True,
+                Qisa.QCIS,
+            ),
         }
 
     def support(self, backend_type):
         return backend_type in self.backends
 
     def import_be_module(self, module_path):
         """import the backend module based on the module_path.
```

### Comparing `quingo-0.2.2/src/quingo/backend/if_backend.py` & `quingo-0.3.1/src/quingo/backend/if_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import re
-from quingo.core.utils import *
-import logging
-from pathlib import Path
 from .backend_hub import BackendType, Backend_hub
-from quingo.core.exe_config import *
+from quingo.core.exe_config import ExeConfig
 
 
 class If_backend:
     """The interface class for Quingo backends.
 
     Any backend should inherit from this interface.
     """
```

### Comparing `quingo-0.2.2/src/quingo/backend/pyqcisim_quantumsim.py` & `quingo-0.3.1/src/quingo/backend/pyqcisim_tequila.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,45 @@
+from quingo.utils import ensure_path
 from .backend_hub import BackendType
 from .if_backend import If_backend
-from quingo.core.exe_config import *
-from quingo.core.utils import *
+from quingo.core.exe_config import ExeConfig, ExeMode
 from pyqcisim.simulator import PyQCISim
+import numpy as np
 
 
-class PyQCISim_quantumsim(If_backend):
-    """A functional QCIS simulation backend using PyQCISim and QuantumSim."""
+class PyQCISim_tequila(If_backend):
+    """A functional QCIS simulation backend using PyQCISim and Tequila."""
 
     def __init__(self):
-        super().__init__(BackendType.QUANTUM_SIM)
+        super().__init__(BackendType.TEQUILA)
         self.sim = PyQCISim()
+        self.sim.setBackend("tequila")
+        self.res = None
 
     def upload_program(self, prog_fn):
-        """
-        Upload assembly or binary program to the simulator.
-
-        Args:
-            prog_fn: the name of the assembly or binary file.
-        """
         prog_fn = ensure_path(prog_fn)
 
         program = prog_fn.open("r").read()
         self.sim.compile(program)
 
     def execute(self, exe_config: ExeConfig):
         """Execute the given quantum circuit.
         Args:
-          - mode (str): the simulation mode to use:
-              - "one_shot": the simulation result is a dictionary with each key being a qubit
-                  measured, and the value is the outcome of measuring this qubit.
-              - "final_state": the simulation result is a two-level dictionary:
-                  {
-                    'classical': {'Q1': 1, 'Q2': 0},
-                    'quantum': (['Q3', 'Q4'], array([0, 1, 0, 0]))
-                  }
-          - num_shots (int): the number of iterations performed in `one_shot` mode.
+          - exe_config (ExeConfig): the configuration used to perform simulation by SymQC.
+
+        The number of shots is specified in exe_config.num_shots, which is only valid for
+          ExeMode.SimShots.
         """
-        if exe_config.mode == ExeMode.SimStateVector:
-            raw_res = self.sim.simulate("final_state")
-            return raw_res
 
-        if exe_config.mode == ExeMode.SimFinalResult:
+        if exe_config.mode == ExeMode.SimShots:
             return self.sim.simulate("one_shot", exe_config.num_shots)
 
+        if exe_config.mode == ExeMode.SimFinalResult:
+            return self.sim.simulate("final_result")
+
+        if exe_config.mode == ExeMode.SimStateVector:
+            names, nd_array_values = self.sim.simulate("state_vector")
+            return (names, nd_array_values)
+
         raise ValueError(
-            "Unsupported execution mode ({}) for quantumsim.".format(exe_config.mode)
+            "Unsupported execution mode ({}) for TEQUILA.".format(exe_config.mode)
         )
```

### Comparing `quingo-0.2.2/src/quingo/backend/qisa.py` & `quingo-0.3.1/src/quingo/backend/qisa.py`

 * *Files identical despite different names*

### Comparing `quingo-0.2.2/src/quingo/backend/qualesim_tequila.py` & `quingo-0.3.1/src/quingo/backend/qualesim.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,101 @@
-# from .backend_hub import BackendType
-# from .if_backend import If_backend
-# from quingo.core.exe_config import *
-# from quingo.core.utils import *
-# from dqcsim.plugin import *
-# from dqcsim.host import *
-
-# logger = get_logger((__name__).split(".")[-1])
-
-
-# def bitwise_reverse_sort(lst, k):
-#     sorted_lst = []
-#     for i in range(len(lst)):
-#         sorted_lst.append(lst[int("0b" + bin(i)[2:].zfill(k)[::-1], 2)])
-#     return sorted_lst
-
-
-# class QuaLeSim_tequila(If_backend):
-#     """A functional QCIS simulation backend using PyQCISim and Tequila."""
-
-#     def __init__(self):
-#         super().__init__(BackendType.QUALESIM_TEQUILA)
-#         self.sim = Simulator(stderr_verbosity=Loglevel.OFF)
-#         self.sim.with_backend("tequila", verbosity=Loglevel.OFF)
-#         self.res = None
-
-#     def upload_program(self, prog_fn):
-#         prog_fn = ensure_path(prog_fn)
-#         if str(prog_fn).endswith(".qcis") or str(prog_fn).endswith(".qi"):
-#             self.sim.with_frontend(str(prog_fn), verbosity=Loglevel.OFF)
-#         else:
-#             raise TypeError(
-#                 "The tequila simulator can only accept QCIS or QUIET-S instructions."
-#             )
-
-#     def execute(self, exe_config: ExeConfig):
-#         if exe_config.mode == ExeMode.SimFinalResult:
-#             measure_mod = "one_shot"
-#             try:
-#                 self.sim.simulate()
-#                 res = self.sim.run(
-#                     measure_mod=measure_mod, num_shots=exe_config.num_shots
-#                 )
-#                 self.sim.stop()
-#                 final_state = res["res"]
-#                 final_state["quantum"] = tuple(final_state["quantum"])
-#                 return final_state["quantum"]
-#             except:
-#                 raise ValueError(
-#                     "Here is some wrong with ({}) for QUALESIM_TEQUILA.".format(
-#                         exe_config.mode
-#                     )
-#                 )
-
-#         if exe_config.mode == ExeMode.SimStateVector:
-#             measure_mod = "state_vector"
-#             try:
-#                 self.sim.simulate()
-#                 res = self.sim.run(measure_mod=measure_mod)
-#                 self.sim.stop()
-#                 final_state = eval(res["res"])
-#                 qu = bitwise_reverse_sort(
-#                     final_state["quantum"][1], len(final_state["quantum"][0])
-#                 )
-#                 final_state["quantum"] = (final_state["quantum"][0], qu)
-#                 return final_state
-#             except:
-#                 raise ValueError(
-#                     "Here is some wrong with ({}) for QUALESIM_TEQUILA.".format(
-#                         exe_config.mode
-#                     )
-#                 )
-
-#         raise ValueError(
-#             "Unsupported execution mode ({}) for QUALESIM_TEQUILA.".format(
-#                 exe_config.mode
-#             )
-#         )
+from __future__ import annotations
+from typing import Union
+from quingo.utils import ensure_path
+from pathlib import Path
+from quingo.backend.backend_hub import BackendType
+from quingo.backend.if_backend import If_backend
+from quingo.core.exe_config import ExeConfig, ExeMode
+from qualesim.plugin import Loglevel
+from qualesim.host import Simulator
+
+
+class QuaLeSim(If_backend):
+
+    def __init__(self, backend_type=BackendType.QUALESIM_QUANTUMSIM):
+        super().__init__(backend_type)
+        self.sim = Simulator(stderr_verbosity=Loglevel.OFF)
+        if backend_type == BackendType.QUALESIM_QUANTUMSIM:
+            self.sim.with_backend("quantumsim", verbosity=Loglevel.OFF)
+        elif backend_type == BackendType.QUALESIM_TEQUILA:
+            self.sim.with_backend("tequila", verbosity=Loglevel.OFF)
+        else:
+            raise ValueError(
+                "The QuaLeSim backend only supports QUALESIM_QUANTUMSIM and QUALESIM_TEQUILA."
+            )
+
+        self.res = None
+
+    def upload_program(self, prog_fn: Union[Path | str]):
+        prog_fn = ensure_path(prog_fn)
+
+        if prog_fn.suffix in [".qcis", ".qi"]:
+            self.sim.with_frontend(str(prog_fn), verbosity=Loglevel.OFF)
+        else:
+            raise TypeError(
+                "found unsupported file suffix ({}). Currently supported are "
+                "'.qcis' (for QCIS) and '.qi' (for QUIET-s)".format(prog_fn.suffix)
+            )
+
+    def execute(self, exe_config: ExeConfig):
+        if exe_config.mode == ExeMode.SimShots:
+            measure_mod = "one_shot"
+            try:
+                self.sim.simulate()
+                res = self.sim.run(
+                    measure_mod=measure_mod, num_shots=exe_config.num_shots
+                )
+                self.sim.stop()
+
+                final_state = res["res"]
+                final_state["quantum"] = tuple(final_state["quantum"])
+                result = final_state["quantum"]
+
+                return result
+
+            except Exception as e:
+                raise ValueError(
+                    "error in QuaLeSim simulation with mode ({}): {}".format(
+                        exe_config.mode, e
+                    )
+                )
+
+        if exe_config.mode == ExeMode.SimFinalResult:
+            measure_mod = "one_shot"
+            try:
+                self.sim.simulate()
+                res = self.sim.run(
+                    measure_mod=measure_mod, num_shots=exe_config.num_shots
+                )
+                self.sim.stop()
+                final_state = res["res"]
+                final_state["quantum"] = tuple(final_state["quantum"])
+                return final_state["quantum"]
+
+            except Exception as e:
+                raise ValueError(
+                    "error in QuaLeSim simulation with mode ({}): {}".format(
+                        exe_config.mode, e
+                    )
+                )
+
+        if exe_config.mode == ExeMode.SimStateVector:
+            measure_mod = "state_vector"
+            try:
+                self.sim.simulate()
+                res = self.sim.run(measure_mod=measure_mod)
+                self.sim.stop()
+                final_state = eval(res["res"])
+                return final_state["quantum"]
+
+            except Exception as e:
+                raise ValueError(
+                    "error in QuaLeSim simulation with mode ({}): {}".format(
+                        exe_config.mode, e
+                    )
+                )
+
+        raise ValueError(
+            "Unsupported execution mode ({}) for QuaLeSim_QuantumSim.".format(
+                exe_config.mode
+            )
+        )
```

### Comparing `quingo-0.2.2/src/quingo/backend/symqc.py` & `quingo-0.3.1/src/quingo/backend/symqc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
+from quingo.utils import ensure_path
 from .backend_hub import BackendType
 from .if_backend import If_backend
-from quingo.core.exe_config import *
-from quingo.core.utils import *
+from quingo.core.exe_config import ExeConfig, ExeMode
 from symqc.simulator import SymQC
 
 
-logger = get_logger((__name__).split(".")[-1])
-
-
 class IfSymQC(If_backend):
     """A functional QCIS simulation backend based on symbolic computation."""
 
     def __init__(self):
         super().__init__(BackendType.SYMQC)
         self.sim = SymQC()
 
@@ -27,32 +24,26 @@
             self.sim.compile_file(prog_fn)
         else:
             raise TypeError("The SymQC simulator can only accept QCIS instructions.")
 
     def execute(self, exe_config: ExeConfig):
         """Execute the given quantum circuit.
         Args:
-          - mode (str): the simulation mode to use:
-              - "one_shot": the simulation result is a dictionary with each key being a qubit
-                  measured, and the value is the outcome of measuring this qubit.
-              - "final_state": the simulation result is a two-level dictionary:
-                  {
-                    'classical': {'Q1': 1, 'Q2': 0},
-                    'quantum': (['Q3', 'Q4'], array([0, 1, 0, 0]))
-                  }
-          - num_shots (int): the number of iterations performed in `one_shot` mode.
+          - exe_config (ExeConfig): the configuration used to perform simulation by SymQC.
+
+        The number of shots is specified in exe_config.num_shots, which is only valid for
+          ExeMode.SimShots.
         """
-        if exe_config.mode == ExeMode.SimStateVector:
-            raw_res = self.sim.simulate("final_state")
-            return raw_res
+        if exe_config.mode == ExeMode.SimShots:
+            return self.sim.simulate("one_shot", exe_config.num_shots)
 
         if exe_config.mode == ExeMode.SimFinalResult:
-            return self.sim.simulate("one_shot", exe_config.num_shots)
+            raw_res = self.sim.simulate("final_state")
+            return raw_res
 
-        if exe_config.mode == ExeMode.SimMatrix:
-            raise NotImplementedError(
-                "Runtime has not supported SimMatrix with SymQC yet."
-            )
+        if exe_config.mode == ExeMode.SimStateVector:
+            raw_res = self.sim.simulate("final_state")
+            return raw_res["quantum"]
 
         raise ValueError(
             "Unsupported execution mode ({}) for symqc.".format(exe_config.mode)
         )
```

### Comparing `quingo-0.2.2/src/quingo/backend/xiaohong.py` & `quingo-0.3.1/src/quingo/backend/xiaohong.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+from quingo.utils import ensure_path
 from .backend_hub import BackendType
 from .if_backend import If_backend
-from quingo.core.exe_config import *
-from quingo.core.utils import *
-from pyezQ import *
-
-
-logger = get_logger((__name__).split(".")[-1])
+from quingo.core.exe_config import ExeConfig, ExeMode
+import pyezQ
 
 
 class XiaoHong(If_backend):
     def __init__(self):
         super().__init__(BackendType.XIAOHONG)
         self.account = None
         self.qcis_circuit = None
@@ -55,15 +52,15 @@
 
         # read result
         result = self.account.query_experiment(query_id, max_wait_time=360000)
         result = self.format_result(result)
         return result
 
     def set_account(self, login_key, machine_name):
-        self.account = Account(login_key=login_key, machine_name=machine_name)
+        self.account = pyezQ.Account(login_key=login_key, machine_name=machine_name)
         print(f"Set account successfully:")
         print(f"   login key = {login_key[0:5]}" + "*" * (len(login_key) - 5))
         print(f"   machine name = {machine_name}")
 
     def format_result(self, result):
         origin_result = result[0]["results"]
         return {"qubits": origin_result[0], "results": origin_result[1:]}
```

### Comparing `quingo-0.2.2/src/quingo/core/compile.py` & `quingo-0.3.1/src/quingo/core/compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import subprocess, logging
 from pathlib import Path
-from .compiler_config import get_mlir_path
+import subprocess, logging
+from quingo.core.compiler_config import get_mlir_path
 from quingo.core.quingo_task import Quingo_task
 from quingo.core.preparation import gen_main_file
-from quingo.core.utils import quingo_err, get_logger, ensure_path
-from quingo.backend.qisa import *
+from quingo.core.quingo_logger import quingo_err, get_logger
+from quingo.utils import ensure_path
+from quingo.backend.qisa import Qisa, get_qisa_name, get_suffix
 
 
 logger = get_logger((__name__).split(".")[-1])
 
 
 def compile(task: Quingo_task, params: tuple, qasm_fn: Path = None, config_file=""):
     """Compile the quingo file with given parameters and return the path of
```

### Comparing `quingo-0.2.2/src/quingo/core/compiler_config.py` & `quingo-0.3.1/src/quingo/core/compiler_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from .utils import quingo_err, quingo_info
+from quingo.core.quingo_logger import quingo_err, quingo_info
 import quingo.global_config as gc
 import distutils.spawn
 import requests
 import json
 
 
 def get_text(link):
```

### Comparing `quingo-0.2.2/src/quingo/core/data_transfer.py` & `quingo-0.3.1/src/quingo/core/data_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import struct
 import numpy
 
 import quingo.global_config as gc
 from quingo.core.data import Time
-from quingo.core.utils import *
+import logging
+from quingo.core.quingo_logger import get_logger
 from typing import Tuple
 
 logger = get_logger((__name__).split(".")[-1])
 logger.setLevel(logging.WARNING)
 
 
 def check_if_param_type(arg) -> str:
```

### Comparing `quingo-0.2.2/src/quingo/core/exe_config.py` & `quingo-0.3.1/src/quingo/core/exe_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import enum
 
 
 class ExeMode(enum.Enum):
+    """
+    Enumeration representing different result format.
+
+    Attributes:
+        SimFinalResult: for obtaining the final result.
+        SimStateVector: Simulation mode for obtaining the state vector.
+        SimMatrix: Simulation mode for obtaining the matrix representation.
+        RealMachine: Mode for executing on a real quantum machine.
+    """
+
+    SimShots = enum.auto()
     SimFinalResult = enum.auto()
     SimStateVector = enum.auto()
-    SimMatrix = enum.auto()
+    SymbolicStateVector = enum.auto()
     RealMachine = enum.auto()
 
 
-def is_simulation(exe_mode):
-    return exe_mode in [
-        ExeMode.SimFinalResult,
-        ExeMode.SimStateVector,
-        ExeMode.SimMatrix,
-    ]
-
-
 class ExeConfig:
     def __init__(
         self,
-        mode: ExeMode = ExeMode.SimFinalResult,
+        mode: ExeMode = ExeMode.SimShots,
         num_shots: int = 1,
         xh_login_key: str = None,  # use for connecting XIAOHONG
         xh_machine_name: str = None,  # use for connecting XIAOHONG
     ):
         self.mode = mode
         self.num_shots = num_shots
         self.xh_login_key = xh_login_key
```

### Comparing `quingo-0.2.2/src/quingo/core/preparation.py` & `quingo-0.3.1/src/quingo/core/preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """The task of this module is to prepare the Quingo source file for the compilation.
 """
 
-
 import re
 from pathlib import Path
-from quingo.core.utils import get_logger
 import logging
+from quingo.core.quingo_logger import get_logger
 import quingo.core.data_transfer as dt
 
 logger = get_logger((__name__).split(".")[-1])
 
 
 def remove_comment(qu_src):
     search_annotation_string = r"\/\/.*\n"
```

### Comparing `quingo-0.2.2/src/quingo/core/quingo_task.py` & `quingo-0.3.1/src/quingo/core/quingo_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import shutil
 import quingo.global_config as gc
 import tempfile
 from quingo.backend.backend_hub import BackendType
 from quingo.backend.qisa import Qisa
-from quingo.core.utils import ensure_path
+from quingo.utils import ensure_path
 
 DEBUG_MODE = False
 
 
 def create_empty_dir(dir_path: Path):
     if dir_path.exists():
         shutil.rmtree(str(dir_path))
@@ -103,16 +103,16 @@
             return self._qisa
 
         if self._backend in [
             BackendType.QUANTUM_SIM,
             BackendType.TEQUILA,
             BackendType.SYMQC,
             BackendType.XIAOHONG,
-            # BackendType.QUALESIM_QUANTUMSIM,
-            # BackendType.QUALESIM_TEQUILA,
+            BackendType.QUALESIM_QUANTUMSIM,
+            BackendType.QUALESIM_TEQUILA,
         ]:
             return Qisa.QCIS
 
         if self._backend in [BackendType.QUANTIFY]:
             return Qisa.Quantify
 
         raise ValueError(f"Found unknown backend {self._backend}")
```

### Comparing `quingo-0.2.2/src/quingo/core/utils.py` & `quingo-0.3.1/src/quingo/core/quingo_logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from logging.handlers import TimedRotatingFileHandler
 import sys
 import colorama as cm
 import termcolor as tc
-from pathlib import Path
 
 cm.init()
 
 # Fore: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
 # Back: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
 # Style: DIM, NORMAL, BRIGHT, RESET_ALL
 
@@ -51,14 +50,7 @@
     # better to have too much log than not enough
     logger.setLevel(logging.DEBUG)
     logger.addHandler(get_console_handler())
     # logger.addHandler(get_file_handler())
     # with this pattern, it's rarely necessary to propagate the error up to parent
     logger.propagate = False
     return logger
-
-
-def ensure_path(fn) -> Path:
-    assert isinstance(fn, (str, Path))
-    if isinstance(fn, str):
-        fn = Path(fn).resolve()
-    return fn
```

### Comparing `quingo-0.2.2/src/quingo/global_config.py` & `quingo-0.3.1/src/quingo/global_config.py`

 * *Files identical despite different names*

### Comparing `quingo-0.2.2/src/quingo/install_quingoc.py` & `quingo-0.3.1/src/quingo/install_quingoc.py`

 * *Files identical despite different names*

### Comparing `quingo-0.2.2/src/quingo.egg-info/SOURCES.txt` & `quingo-0.3.1/src/quingo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/quingo/__init__.py
 src/quingo/global_config.py
 src/quingo/install_quingoc.py
+src/quingo/utils.py
 src/quingo.egg-info/PKG-INFO
 src/quingo.egg-info/SOURCES.txt
 src/quingo.egg-info/dependency_links.txt
 src/quingo.egg-info/requires.txt
 src/quingo.egg-info/top_level.txt
 src/quingo/backend/__init__.py
 src/quingo/backend/backend_hub.py
 src/quingo/backend/if_backend.py
 src/quingo/backend/pyqcisim_quantumsim.py
 src/quingo/backend/pyqcisim_tequila.py
 src/quingo/backend/qisa.py
-src/quingo/backend/qualesim_quantumsim.py
-src/quingo/backend/qualesim_tequila.py
+src/quingo/backend/qualesim.py
 src/quingo/backend/result_formatter.py
 src/quingo/backend/symqc.py
 src/quingo/backend/xiaohong.py
 src/quingo/core/__init__.py
 src/quingo/core/compile.py
 src/quingo/core/compiler_config.py
 src/quingo/core/data.py
 src/quingo/core/data_transfer.py
 src/quingo/core/exe_config.py
 src/quingo/core/manager.py
 src/quingo/core/preparation.py
+src/quingo/core/quingo_logger.py
 src/quingo/core/quingo_task.py
-src/quingo/core/utils.py
 src/quingo/lib/__init__.py
```

