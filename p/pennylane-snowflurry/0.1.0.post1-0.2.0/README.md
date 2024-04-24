# Comparing `tmp/pennylane-snowflurry-0.1.0.post1.tar.gz` & `tmp/pennylane_snowflurry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-snowflurry-0.1.0.post1.tar", last modified: Fri Feb 23 22:25:15 2024, max compression
+gzip compressed data, was "pennylane_snowflurry-0.2.0.tar", last modified: Wed Apr 24 13:15:32 2024, max compression
```

## Comparing `pennylane-snowflurry-0.1.0.post1.tar` & `pennylane_snowflurry-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12518 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/pennylane_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/snowflurry_device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-23 22:25:15.000000 pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:25:15.091552 pennylane-snowflurry-0.1.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/tests/test_pennylaneConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/tests/test_pennylaneTests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/tests/test_pyjulia-snowflurry.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-23 22:24:59.000000 pennylane-snowflurry-0.1.0.post1/tests/test_snowflurryQubitDevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:32.292391 pennylane_snowflurry-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-24 13:15:32.292391 pennylane_snowflurry-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:32.288391 pennylane_snowflurry-0.2.0/pennylane_snowflurry/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry/pennylane_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry/snowflurry_device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:32.292391 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 13:15:32.000000 pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:15:32.292391 pennylane_snowflurry-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:32.292391 pennylane_snowflurry-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/tests/test_pennylaneConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/tests/test_pennylaneSubroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/tests/test_pennylaneTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/tests/test_pyjulia-snowflurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-24 13:15:26.000000 pennylane_snowflurry-0.2.0/tests/test_snowflurryQubitDevice.py
```

### Comparing `pennylane-snowflurry-0.1.0.post1/LICENSE` & `pennylane_snowflurry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-snowflurry-0.1.0.post1/PKG-INFO` & `pennylane_snowflurry-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-snowflurry
-Version: 0.1.0.post1
+Version: 0.2.0
 Summary: PennyLane plugin for interfacing with Anyon's quantum computers
 Maintainer-email: Calcul Québec <support@tech.alliancecan.ca>
 License: Apache Software License (Apache License 2.0)
 Project-URL: Source, https://github.com/calculquebec/pennylane-snowflurry
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -28,25 +28,25 @@
 Requires-Dist: julia>=0.6.0
 Requires-Dist: pennylane>=0.30.0
 
 # pennylane-snowflurry
 
 The PennyLane-Snowflurry plugin provides a PennyLane device that allows the use of Anyon Systems' Snowflurry quantum computing platform with PennyLane.
 
-[Penylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+[Pennylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 [Snowflurry](https://snowflurry.org/) is a quantum computing framework developed in Julia by Anyon Systems and aims to provide access to quantum hardware and simulators.
 
 PennyLane-Snowflurry makes use of dependencies such as PyJulia and PyCall to allow interfacing between Python and Julia, and thus between PennyLane and Snowflurry.
 
 ## Project structure
 
 As shown in the diagram below, this plugin is used in Pennylane as a [device](https://pennylane.ai/plugins/) named `snowflurry.qubit`. This device is defined by the class `SnowflurryQubitDevice`. It converts a PennyLane circuit into a Snowflurry circuit, thanks to packages like PyJulia that allow the communication between Python and Julia environments. The Snowflurry circuit can then be used with the available backends, either a simulator or real quantum hardware. The results are then converted back into PennyLane's format and returned to the user.
 
-![interaction_diagram](./doc/interaction_diagram_extended.png)
+![interaction_diagram](https://raw.githubusercontent.com/calculquebec/pennylane-snowflurry/main/doc/interaction_diagram_extended.png)
 
 ## Local installation
 
 Since this plugin interfaces between Python and Julia, it requires both languages to be installed on your machine. As Python is widely used amongst the quantum computing community, we assume you already have it installed. The rest of this section will guide you through the installation of Julia and the plugin.
 
 ### Julia
```

### Comparing `pennylane-snowflurry-0.1.0.post1/README.md` & `pennylane_snowflurry-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # pennylane-snowflurry
 
 The PennyLane-Snowflurry plugin provides a PennyLane device that allows the use of Anyon Systems' Snowflurry quantum computing platform with PennyLane.
 
-[Penylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+[Pennylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 [Snowflurry](https://snowflurry.org/) is a quantum computing framework developed in Julia by Anyon Systems and aims to provide access to quantum hardware and simulators.
 
 PennyLane-Snowflurry makes use of dependencies such as PyJulia and PyCall to allow interfacing between Python and Julia, and thus between PennyLane and Snowflurry.
 
 ## Project structure
 
 As shown in the diagram below, this plugin is used in Pennylane as a [device](https://pennylane.ai/plugins/) named `snowflurry.qubit`. This device is defined by the class `SnowflurryQubitDevice`. It converts a PennyLane circuit into a Snowflurry circuit, thanks to packages like PyJulia that allow the communication between Python and Julia environments. The Snowflurry circuit can then be used with the available backends, either a simulator or real quantum hardware. The results are then converted back into PennyLane's format and returned to the user.
 
-![interaction_diagram](./doc/interaction_diagram_extended.png)
+![interaction_diagram](https://raw.githubusercontent.com/calculquebec/pennylane-snowflurry/main/doc/interaction_diagram_extended.png)
 
 ## Local installation
 
 Since this plugin interfaces between Python and Julia, it requires both languages to be installed on your machine. As Python is widely used amongst the quantum computing community, we assume you already have it installed. The rest of this section will guide you through the installation of Julia and the plugin.
 
 ### Julia
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/_version.py` & `pennylane_snowflurry-0.2.0/pennylane_snowflurry/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.1.0.post1"
+
+__version__ = "0.2.0"
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/execution_config.py` & `pennylane_snowflurry-0.2.0/pennylane_snowflurry/execution_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Contains the :class:`ExecutionConfig` data class.
+
+This module has not been modified from the original Pennylane source.
+
 """
 from dataclasses import dataclass
 from typing import Optional
 
-from pennylane.interfaces import SUPPORTED_INTERFACES
+from pennylane.workflow import SUPPORTED_INTERFACES
 from pennylane.gradients import SUPPORTED_GRADIENT_KWARGS
 
 SUPPORTED_GRADIENT_METHODS = [
     "best",
     "parameter-shift",
     "backprop",
     "finite-diff",
@@ -95,14 +98,17 @@
 
         if self.device_options is None:
             self.device_options = {}
 
         if self.gradient_keyword_arguments is None:
             self.gradient_keyword_arguments = {}
 
-        if any(arg not in SUPPORTED_GRADIENT_KWARGS for arg in self.gradient_keyword_arguments):
+        if any(
+            arg not in SUPPORTED_GRADIENT_KWARGS
+            for arg in self.gradient_keyword_arguments
+        ):
             raise ValueError(
                 f"All gradient_keyword_arguments keys must be in {SUPPORTED_GRADIENT_KWARGS}, got unexpected values: {set(self.gradient_keyword_arguments) - set(SUPPORTED_GRADIENT_KWARGS)}"
             )
 
 
 DefaultExecutionConfig = ExecutionConfig()
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry/pennylane_converter.py` & `pennylane_snowflurry-0.2.0/pennylane_snowflurry/pennylane_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     MeasurementValue,
     ProbabilityMP,
     SampleMP,
     ExpectationMP,
     CountsMP,
 )
 import time
+import re
 from pennylane.typing import TensorLike
 from typing import Callable
 from pennylane.ops import Sum, Hamiltonian
 
 # Dictionary mapping PennyLane operations to Snowflurry operations
 # The available Snowflurry operations are listed here:
 # https://snowflurrysdk.github.io/Snowflurry.jl/dev/library/quantum_toolkit.html
@@ -27,85 +28,98 @@
 # https://snowflurrysdk.github.io/Snowflurry.jl/dev/library/quantum_circuit.html
 SNOWFLURRY_OPERATION_MAP = {
     "PauliX": "sigma_x({0})",
     "PauliY": "sigma_y({0})",
     "PauliZ": "sigma_z({0})",
     "Hadamard": "hadamard({0})",
     "CNOT": "control_x({0},{1})",
+    "CY": "controlled(sigma_y({1}),[{0}])",  # 0 is the control qubit, 1 is the target qubit
     "CZ": "control_z({0},{1})",
     "SWAP": "swap({0},{1})",
     "ISWAP": "iswap({0},{1})",
     "RX": "rotation_x({1},{0})",
     "RY": "rotation_y({1},{0})",
-    "RZ": "rotation_z({1},{0})",  # NOTE : rotation_z is not implemented in snowflurry, phase_shift is the closest thing
+    "RZ": "rotation_z({1},{0})",
     "Identity": "identity_gate({0})",
-    "CSWAP": NotImplementedError,
-    "CRX": "controlled(rotation_x({1},{0}),{1})",  # gates using controlled probably wont work, might have to do a special operations for those cases.
-    "CRY": NotImplementedError,
-    "CRZ": NotImplementedError,
-    "PhaseShift": "phase_shift({1},{0})",
+    "CSWAP": "controlled(swap({1},{2}),[{0}])",  # 0 is the control qubit, 1 and 2 are the target qubits
+    "CRX": "controlled(rotation_x({2},{0}),[{1}])",  # 0 is the angle, 1 is the control qubit, 2 is the target qubit
+    "CRY": "controlled(rotation_y({2},{0}),[{1}])",
+    "CRZ": "controlled(rotation_z({2},{0}),[{1}])",
+    "PhaseShift": "phase_shift({1},{0})",  # 0 is the angle, 1 is the wire
+    "ControlledPhaseShift": "controlled(phase_shift({2},{0}),[{1}])",  # 0 is the angle, 1 is the control qubit, 2 is the target qubit
     "QubitStateVector": NotImplementedError,
     "StatePrep": NotImplementedError,
-    "Toffoli": "toffoli({0},{1},{2})",  # order might be wrong on that one
+    "Toffoli": "toffoli({0},{1},{2})",
     "QubitUnitary": NotImplementedError,
     "U1": NotImplementedError,
     "U2": NotImplementedError,
     "U3": "universal({3},{0},{1},{2})",
     "IsingZZ": NotImplementedError,
     "IsingYY": NotImplementedError,
     "IsingXX": NotImplementedError,
     "T": "pi_8({0})",
     "Rot": "rotation({3},{0},{1})",  # theta, phi but no omega so we skip {2}, {3} is the wire
     "QubitUnitary": NotImplementedError,  # might correspond to apply_gate!(state::Ket, gate::Gate) from snowflurry
-    "QFT": NotImplementedError,
 }
 
 
 """
 if host, user, access_token are left blank, the code will be ran on the simulator
 if host, user, access_token are filled, the code will be sent to Anyon's API
 """
 
 
 class PennylaneConverter:
     """
-    supported measurements :
-    counts([op, wires, all_outcomes]) arguments have no effect
-    expval(op)
-    state()
-    sample([op, wires]) arguments have no effect
-    probs([wires, op]) arguments have no effect
-
-    currently not supported measurements :
-    var(op)
-    density_matrix(wires)
-    vn_entropy(wires[, log_base])
-    mutual_info(wires0, wires1[, log_base])
-    purity(wires)
-    classical_shadow(wires[, seed])
-    shadow_expval(H[, k, seed])
+    A PennyLane converter for the Snowflurry device.
+
+    Is in charge of interfacing with the Snowflurry.jl package and converting PennyLane circuits to
+    Snowflurry circuits.
     """
 
+    ###################################
+    # Class attributes used for logic #
+    ###################################
+    snowflurry_readout_name = "Readout"
+    snowflurry_gate_object_name = "Gate Object"
+
+    # Pattern is found in PyCall.jlwrap object of Snowflurry.QuantumCircuit.instructions
+    snowflurry_str_search_pattern = r"Gate Object: (.*)\n"
+
+    #################
+    # Class methods #
+    #################
+
     def __init__(
         self,
         circuit: qml.tape.QuantumScript,
         rng=None,
         debugger=None,
         interface=None,
         host="",
         user="",
         access_token="",
+        project_id="",
     ) -> Result:
+
+        # Instance attributes related to PennyLane
         self.circuit = circuit
         self.rng = rng
         self.debugger = debugger
         self.interface = interface
-        if len(host) != 0 and len(user) != 0 and len(access_token) != 0:
+
+        # Instance attributes related to Snowflurry
+        if (
+            len(host) != 0
+            and len(user) != 0
+            and len(access_token) != 0
+            and len(project_id) != 0
+        ):
             Main.currentClient = Main.Eval(
-                "Client(host={host},user={user},access_token={access_token})"
+                "Client(host={host},user={user},access_token={access_token}, project_id={project_id})"
             )  # TODO : I think this pauses the execution, check if threading is needed
         else:
             Main.currentClient = None
 
     def simulate(self):
         sf_circuit, is_state_batched = self.convert_circuit(
             self.circuit, debugger=self.debugger, interface=self.interface
@@ -144,33 +158,158 @@
         for op in pennylane_circuit.map_to_standard_wires().operations[bool(prep) :]:
             if op.name in SNOWFLURRY_OPERATION_MAP:
                 if SNOWFLURRY_OPERATION_MAP[op.name] == NotImplementedError:
                     print(f"{op.name} is not implemented yet, skipping...")
                     continue
                 parameters = op.parameters + [i + 1 for i in op.wires.tolist()]
                 gate = SNOWFLURRY_OPERATION_MAP[op.name].format(*parameters)
-                print(f"placed {gate}")
                 Main.eval(f"push!(sf_circuit,{gate})")
             else:
                 print(f"{op.name} is not supported by this device. skipping...")
 
-        Main.print(Main.sf_circuit)
-
         return Main.sf_circuit, False
 
-    def apply_readouts(self, wires_nb):
+    def apply_readouts(self, wires_nb, obs):
         """
         Apply readouts to all wires in the snowflurry circuit.
 
         Args:
-            sf_circuit: The snowflurry circuit to modify.
             wires_nb (int): The number of wires in the circuit.
+            obs (Optional[Observable]): The observable mentioned in the measurement process. If None,
+                readouts are applied to all wires because we assume the user wants to measure all wires.
+        """
+
+        if obs is None:  # if no observable is given, we apply readouts to all wires
+            for wire in range(wires_nb):
+                Main.eval(f"push!(sf_circuit, readout({wire + 1}, {wire + 1}))")
+
+        else:
+            # if an observable is given, we apply readouts to the wires mentioned in the observable,
+            # TODO : could add Pauli rotations to get the correct observable
+            self.apply_single_readout(obs.wires[0])
+
+    def get_circuit_as_dictionary(self):
+        """
+        Take the snowflurry QuantumCircuit.instructions and convert it to an array of operations.
+        When instruction is called from Snowflurry, PyCall returns a jlwrap object which is not easily
+        iterable. This function is used to convert the jlwrap object to a Python dictionary.
+
+        Returns:
+            Dict [str, [int]]: A dictionary containing the operations and an array of the wires they are
+                applied to.
+
+        Example:
+            >>> Main.sf_circuit.instructions
+            [<PyCall.jlwrap Gate Object: Snowflurry.Hadamard
+            Connected_qubits        : [1]
+            Operator:
+            (2, 2)-element Snowflurry.DenseOperator:
+            Underlying data ComplexF64:
+            0.7071067811865475 + 0.0im    0.7071067811865475 + 0.0im
+            0.7071067811865475 + 0.0im    -0.7071067811865475 + 0.0im
+            >, <PyCall.jlwrap Gate Object: Snowflurry.ControlX
+            Connected_qubits        : [2, 1]
+            Operator:
+            (4, 4)-element Snowflurry.DenseOperator:
+            Underlying data ComplexF64:
+            1.0 + 0.0im    0.0 + 0.0im    0.0 + 0.0im    0.0 + 0.0im
+            0.0 + 0.0im    1.0 + 0.0im    0.0 + 0.0im    0.0 + 0.0im
+            0.0 + 0.0im    0.0 + 0.0im    0.0 + 0.0im    1.0 + 0.0im
+            0.0 + 0.0im    0.0 + 0.0im    1.0 + 0.0im    0.0 + 0.0im
+            >, <PyCall.jlwrap Explicit Readout object:
+            connected_qubit: 1
+            destination_bit: 1
+            >]
+
+            Becomes:
+            [{'gate': 'Snowflurry.Hadamard', 'connected_qubits': [1]},
+            {'gate': 'Snowflurry.ControlX', 'connected_qubits': [1, 2]},
+            {'gate': 'Readout', 'connected_qubits': [1]}]
+
+
+        """
+        ops = []
+        instructions = Main.sf_circuit.instructions  # instructions is a jlwrap object
+        gate_str = ""
+        gate_name = ""
+
+        for inst in instructions:
+
+            gate_str = str(inst)  # convert the jlwrap object to a string
+
+            try:
+                if self.snowflurry_gate_object_name in gate_str:
+                    # if the gate is a Gate object, we extract the name and the connected qubits
+                    # from the string with a regex
+                    gate_name = re.search(
+                        self.snowflurry_str_search_pattern, gate_str
+                    ).group(1)
+                    op_data = {
+                        "gate": gate_name,
+                        "connected_qubits": list(inst.connected_qubits),
+                    }
+                if self.snowflurry_readout_name in gate_str:
+                    # if the gate is a Readout object, we extract the connected qubit from the string
+                    gate_name = self.snowflurry_readout_name
+                    op_data = {
+                        "gate": gate_name,
+                        "connected_qubits": [inst.connected_qubit],
+                    }
+                # NOTE : attribute for the Gate object is connected_qubits (plural)
+                # while the attribute for the Readout object is connected_qubit (singular)
+
+            except:
+                raise ValueError(f"Error while parsing {gate_str}")
+
+            ops.append(op_data)
+
+        return ops
+
+    def has_readout(self) -> bool:
+        """
+        Check if a readout is applied on any of the wires in the snowflurry circuit.
+
+        Returns:
+            bool: True if a readout is applied, False otherwise.
+        """
+        ops = self.get_circuit_as_dictionary()
+        for op in ops:
+            if op["gate"] == self.snowflurry_readout_name:
+                return True
+        return False
+
+    def remove_readouts(self):
+        """
+        Remove all readouts from the snowflurry circuit with pop!() function.
+
+        """
+        # RFE : eventually, removing the readouts could be done by making a copy
+        # of the instructions vector and removing the readouts from it before
+        # contructing a new QuantumCircuit with that vector.
+        while self.has_readout():
+            Main.eval("pop!(sf_circuit)")
+
+    def apply_single_readout(self, wire):
         """
-        for wire in range(wires_nb):
-            Main.eval(f"push!(sf_circuit, readout({wire + 1}, {wire + 1}))")
+        Apply a readout to a single wire in the snowflurry circuit.
+
+        Args:
+            wire (int): The wire to apply the readout to.
+        """
+        ops = self.get_circuit_as_dictionary()
+
+        for op in ops:
+            # if a readout is already applied to the wire, we don't apply another one
+            if op["gate"] == self.snowflurry_readout_name:
+                if op["connected_qubits"] == wire - 1:  # wire is 1-indexed in Julia
+                    return
+
+        # if no readout is applied to the wire, we apply one while taking into account that
+        # the wire number is 1-indexed in Julia
+        Main.eval(f"push!(sf_circuit, readout({wire+1}, {wire+1}))")
 
     def measure_final_state(self, circuit, sf_circuit, is_state_batched, rng):
         """
         Perform the measurements required by the circuit on the provided state.
 
         This is an internal function that will be called by the successor to ``default.qubit``.
 
@@ -191,26 +330,51 @@
 
         circuit = circuit.map_to_standard_wires()
         shots = circuit.shots.total_shots
         if shots is None:
             shots = 1
 
         if len(circuit.measurements) == 1:
-            return self.measure(circuit.measurements[0], sf_circuit, shots)
+            results = self.measure(circuit.measurements[0], sf_circuit, shots)
         else:
-            return tuple(
+            results = tuple(
                 self.measure(mp, sf_circuit, shots) for mp in circuit.measurements
             )
 
+        Main.print(Main.sf_circuit)
+
+        return results
+
     def measure(self, mp: MeasurementProcess, sf_circuit, shots):
+        """
+        Measure the quantum state using the provided measurement process.
+
+        Args:
+            mp (MeasurementProcess): The measurement process to perform
+            sf_circuit : The snowflurry circuit used
+            shots (int): The number of shots
+
+        Returns:
+            result: The measurement result TODO : type needs to be unified
+
+        Currently supported measurements :
+            - counts(works with Snowflurry.simulate_shots)
+            - sample(works with Snowflurry.simulate_shots)
+            - probs(works with Snowflurry.get_measurement_probabilities)
+            - expval(works with Snowflurry.simulate and Snowflurry.expected_value)
+            - state(works with Snowflurry.simulate and Snowflurry.result_state)
+
+        """
+
         # if measurement is a qml.counts
         if isinstance(mp, CountsMP):  # this measure can run on hardware
             if Main.currentClient is None:
                 # since we use simulate_shots, we need to add readouts to the circuit
-                self.apply_readouts(len(self.circuit.op_wires))
+                self.remove_readouts()
+                self.apply_readouts(len(self.circuit.op_wires), mp.obs)
                 shots_results = Main.simulate_shots(Main.sf_circuit, shots)
                 result = dict(Counter(shots_results))
                 return result
             else:  # if we have a client, we try to use the real machine
                 # NOTE : THE FOLLOWING WILL VERY LIKELY NOT WORK AS IT WAS NOT TESTED
                 # I DID NOT RECEIVE THE AUTHENTICATION INFORMATION IN TIME TO TEST IT.
                 # WHOEVER WORK ON THIS ON THE FUTURE, CONSIDER THIS LIKE PSEUDOCODE
@@ -234,15 +398,16 @@
                 if status == "succeeded":
                     return Main.get_result(circuitID)
 
         # if measurement is a qml.sample
         if isinstance(mp, SampleMP):  # this measure can run on hardware
             if Main.currentClient is None:
                 # since we use simulate_shots, we need to add readouts to the circuit
-                self.apply_readouts(len(self.circuit.op_wires))
+                self.remove_readouts()
+                self.apply_readouts(len(self.circuit.op_wires), mp.obs)
                 shots_results = Main.simulate_shots(Main.sf_circuit, shots)
                 return np.asarray(shots_results).astype(int)
             else:  # if we have a client, we try to use the real machine
                 # NOTE : THE FOLLOWING WILL VERY LIKELY NOT WORK AS IT WAS NOT TESTED
                 # I DID NOT RECEIVE THE AUTHENTICATION INFORMATION IN TIME TO TEST IT.
                 # WHOEVER WORK ON THIS ON THE FUTURE, CONSIDER THIS LIKE PSEUDOCODE
                 # THE CIRCUITID WILL PROBABLY NEED TO BE RAN ON A DIFFERENT THREAD TO NOT STALL THE EXECUTION,
@@ -263,32 +428,38 @@
                     ):  # it won't be "failed", need to check what Main.get_status return
                         break
                 if status == "succeeded":
                     return Main.get_result(circuitID)
 
         # if measurement is a qml.probs
         if isinstance(mp, ProbabilityMP):
+            self.remove_readouts()
             wires_list = mp.wires.tolist()
             if len(wires_list) == 0:
                 return Main.get_measurement_probabilities(Main.sf_circuit)
             else:
                 return Main.get_measurement_probabilities(
                     Main.sf_circuit, [i + 1 for i in wires_list]
                 )
 
         # if measurement is a qml.expval
         if isinstance(mp, ExpectationMP):
-            Main.result_state = Main.simulate(sf_circuit)
+            # FIXME : this measurement only works with a single wire
+            # Requires some processing to work with larger matrices
+            self.remove_readouts()
+            Main.result_state = Main.simulate(Main.sf_circuit)
             if mp.obs is not None and mp.obs.has_matrix:
                 print(type(mp.obs))
                 observable_matrix = qml.matrix(mp.obs)
                 return Main.expected_value(
                     Main.DenseOperator(observable_matrix), Main.result_state
                 )
 
         # if measurement is a qml.state
         if isinstance(mp, StateMeasurement):
-            Main.result_state = Main.simulate(sf_circuit)
+            self.remove_readouts()
+            Main.result_state = Main.simulate(Main.sf_circuit)
             # Convert the final state from pyjulia to a NumPy array
             final_state_np = np.array([element for element in Main.result_state])
             return final_state_np
+
         return NotImplementedError
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/PKG-INFO` & `pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-snowflurry
-Version: 0.1.0.post1
+Version: 0.2.0
 Summary: PennyLane plugin for interfacing with Anyon's quantum computers
 Maintainer-email: Calcul Québec <support@tech.alliancecan.ca>
 License: Apache Software License (Apache License 2.0)
 Project-URL: Source, https://github.com/calculquebec/pennylane-snowflurry
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -28,25 +28,25 @@
 Requires-Dist: julia>=0.6.0
 Requires-Dist: pennylane>=0.30.0
 
 # pennylane-snowflurry
 
 The PennyLane-Snowflurry plugin provides a PennyLane device that allows the use of Anyon Systems' Snowflurry quantum computing platform with PennyLane.
 
-[Penylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
+[Pennylane](https://pennylane.ai/) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
 [Snowflurry](https://snowflurry.org/) is a quantum computing framework developed in Julia by Anyon Systems and aims to provide access to quantum hardware and simulators.
 
 PennyLane-Snowflurry makes use of dependencies such as PyJulia and PyCall to allow interfacing between Python and Julia, and thus between PennyLane and Snowflurry.
 
 ## Project structure
 
 As shown in the diagram below, this plugin is used in Pennylane as a [device](https://pennylane.ai/plugins/) named `snowflurry.qubit`. This device is defined by the class `SnowflurryQubitDevice`. It converts a PennyLane circuit into a Snowflurry circuit, thanks to packages like PyJulia that allow the communication between Python and Julia environments. The Snowflurry circuit can then be used with the available backends, either a simulator or real quantum hardware. The results are then converted back into PennyLane's format and returned to the user.
 
-![interaction_diagram](./doc/interaction_diagram_extended.png)
+![interaction_diagram](https://raw.githubusercontent.com/calculquebec/pennylane-snowflurry/main/doc/interaction_diagram_extended.png)
 
 ## Local installation
 
 Since this plugin interfaces between Python and Julia, it requires both languages to be installed on your machine. As Python is widely used amongst the quantum computing community, we assume you already have it installed. The rest of this section will guide you through the installation of Julia and the plugin.
 
 ### Julia
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pennylane_snowflurry.egg-info/SOURCES.txt` & `pennylane_snowflurry-0.2.0/pennylane_snowflurry.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 pennylane_snowflurry.egg-info/PKG-INFO
 pennylane_snowflurry.egg-info/SOURCES.txt
 pennylane_snowflurry.egg-info/dependency_links.txt
 pennylane_snowflurry.egg-info/entry_points.txt
 pennylane_snowflurry.egg-info/requires.txt
 pennylane_snowflurry.egg-info/top_level.txt
 tests/test_pennylaneConverter.py
+tests/test_pennylaneSubroutine.py
 tests/test_pennylaneTests.py
 tests/test_pyjulia-snowflurry.py
 tests/test_snowflurryQubitDevice.py
```

### Comparing `pennylane-snowflurry-0.1.0.post1/pyproject.toml` & `pennylane_snowflurry-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -31,17 +31,14 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [project.urls]
 Source = "https://github.com/calculquebec/pennylane-snowflurry"
 
-[project.scripts]
-# Not sure if this is where we configure entry points
-
 [project.optional-dependencies]
 # No optional dependencies yet
 
 [project.entry-points."pennylane.plugins"]
 "snowflurry.qubit" = "pennylane_snowflurry:SnowflurryQubitDevice"
 
 [project.entry-points."pennylane.io"]
```

### Comparing `pennylane-snowflurry-0.1.0.post1/tests/test_pennylaneConverter.py` & `pennylane_snowflurry-0.2.0/tests/test_pennylaneConverter.py`

 * *Files identical despite different names*

### Comparing `pennylane-snowflurry-0.1.0.post1/tests/test_snowflurryQubitDevice.py` & `pennylane_snowflurry-0.2.0/tests/test_snowflurryQubitDevice.py`

 * *Files identical despite different names*

