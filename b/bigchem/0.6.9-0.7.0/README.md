# Comparing `tmp/bigchem-0.6.9.tar.gz` & `tmp/bigchem-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigchem-0.6.9.tar", max compression
+gzip compressed data, was "bigchem-0.7.0.tar", max compression
```

## Comparing `bigchem-0.6.9.tar` & `bigchem-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1079 2024-04-13 05:45:14.885089 bigchem-0.6.9/LICENSE
--rw-r--r--   0        0        0    39427 2024-04-13 05:45:14.885089 bigchem-0.6.9/README.md
--rw-r--r--   0        0        0      213 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/__init__.py
--rw-r--r--   0        0        0     4093 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/algos.py
--rw-r--r--   0        0        0     1540 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/app.py
--rw-r--r--   0        0        0      164 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/canvas.py
--rw-r--r--   0        0        0     1982 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/config.py
--rw-r--r--   0        0        0     6718 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/tasks.py
--rw-r--r--   0        0        0     1504 2024-04-13 05:45:14.885089 bigchem-0.6.9/bigchem/utils.py
--rw-r--r--   0        0        0     1908 2024-04-13 05:45:14.889090 bigchem-0.6.9/pyproject.toml
--rw-r--r--   0        0        0    40448 1970-01-01 00:00:00.000000 bigchem-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-24 01:28:49.894488 bigchem-0.7.0/LICENSE
+-rw-r--r--   0        0        0    39427 2024-04-24 01:28:49.894488 bigchem-0.7.0/README.md
+-rw-r--r--   0        0        0      213 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/__init__.py
+-rw-r--r--   0        0        0     4108 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/algos.py
+-rw-r--r--   0        0        0     1540 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/app.py
+-rw-r--r--   0        0        0      164 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/canvas.py
+-rw-r--r--   0        0        0     1982 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/config.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/py.typed
+-rw-r--r--   0        0        0     6765 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/tasks.py
+-rw-r--r--   0        0        0     1504 2024-04-24 01:28:49.894488 bigchem-0.7.0/bigchem/utils.py
+-rw-r--r--   0        0        0     1923 2024-04-24 01:28:49.894488 bigchem-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    40456 1970-01-01 00:00:00.000000 bigchem-0.7.0/PKG-INFO
```

### Comparing `bigchem-0.6.9/LICENSE` & `bigchem-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.9/README.md` & `bigchem-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.9/bigchem/algos.py` & `bigchem-0.7.0/bigchem/algos.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from typing import List, Union
 
 from qcio import (
     CalcType,
     DualProgramInput,
     Molecule,
+    ProgramArgs,
+    ProgramArgsSub,
     ProgramInput,
-    QCProgramArgs,
-    SubProgramArgs,
 )
 
 from .canvas import Signature, group
 from .config import settings
 from .tasks import assemble_hessian, compute, frequency_analysis, output_to_input
 from .utils import _gradient_inputs
 
@@ -80,30 +80,30 @@
     return hessian_sig | frequency_analysis.s(**kwargs)
 
 
 def multistep_opt(
     molecule: Molecule,
     calctype: CalcType,
     programs: List[str],
-    program_args: List[Union[QCProgramArgs, SubProgramArgs]],
+    program_args: List[Union[ProgramArgs, ProgramArgsSub]],
     **kwargs,
 ) -> Signature:
     """Use multiple steps to sequentially optimize a molecule
 
     Params:
         program: The name of the program use for optimization
         prog_inputs: Program inputs for each optimization step.
         kwargs: All kwargs for qcop.compute() function
     """
     # Create first optimization in the chain
-    if isinstance(program_args[0], QCProgramArgs):
+    if isinstance(program_args[0], ProgramArgs):
         first_opt = ProgramInput(
             calctype=calctype, molecule=molecule, **program_args[0].model_dump()
         )
-    else:
+    else:  # is ProgramArgsSub
         first_opt = DualProgramInput(
             calctype=calctype, molecule=molecule, **program_args[0].model_dump()
         )
     task_chain = compute.s(programs[0], first_opt, **kwargs)
 
     # Add subsequent optimizations to the chain
     for program, prog_args in zip(programs[1:], program_args[1:]):
```

### Comparing `bigchem-0.6.9/bigchem/app.py` & `bigchem-0.7.0/bigchem/app.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.9/bigchem/config.py` & `bigchem-0.7.0/bigchem/config.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.9/bigchem/tasks.py` & `bigchem-0.7.0/bigchem/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from itertools import zip_longest
 from typing import List, Union
 
 import numpy as np
 from qcio import (
     CalcType,
     DualProgramInput,
-    InputBase,
-    OptimizationOutput,
-    OutputBase,
-    ProgramFailure,
+    Inputs,
+    OptimizationResults,
+    ProgramArgs,
+    ProgramArgsSub,
     ProgramInput,
-    QCProgramArgs,
-    SinglePointOutput,
-    SubProgramArgs,
+    ProgramOutput,
+    Results,
+    SinglePointResults,
+    StructuredInputs,
 )
 from qcop import compute as qcop_compute
 
 from .app import bigchem
 
 __all__ = [
     "compute",
-    "output_to_input",
+    # "output_to_input",
     "assemble_hessian",
     "frequency_analysis",
 ]
 
 
 @bigchem.task
 def compute(
-    program: Union[str, InputBase],
-    inp_obj: Union[InputBase, str],
+    program: Union[str, Inputs],
+    inp_obj: Union[Inputs, str],
     **kwargs,
-) -> OutputBase:
+) -> ProgramOutput[Inputs, Results]:
     """Wrapper around qcop.compute.
 
     Checks first and second argument order as they may be reversed due to chaining.
     For example, output_to_input returns an output object, but compute expects program
     as the first argument. Chains can only pass the output object as the first argument
     to the next task in the chain. This wrapper allows the user to pass the program
     first or second.
@@ -44,38 +45,34 @@
         # If the first argument is a string, then the second argument is the input
         program, inp_obj = inp_obj, program
     return qcop_compute(program, inp_obj, **kwargs)
 
 
 @bigchem.task
 def output_to_input(
-    output: Union[SinglePointOutput, ProgramFailure, OptimizationOutput],
+    output: ProgramOutput[StructuredInputs, Results],
     calctype: CalcType,
-    program_args: Union[QCProgramArgs, SubProgramArgs],
+    program_args: Union[ProgramArgs, ProgramArgsSub],
 ) -> Union[ProgramInput, DualProgramInput]:
     """Propagate output values from a calculation onto a new input object.
 
     Args:
         output: SinglePointOutput, OptimizationOutput, or ProgramFailure object
         program_args: QCProgramArgs or SubProgramArgs object
         calctype: Calculation type for the new input
 
     NOTE: This task requires additional work to cover more general cases. This skeleton
         is primarily to give an initial example of basic multi-package geometry
         optimization.
     """
-    if isinstance(output, ProgramFailure):
-        raise ValueError(
-            "Previous operation failed and cannot be converted to a new input."
-        )
-
     input_model = (
-        ProgramInput if isinstance(program_args, QCProgramArgs) else DualProgramInput
+        ProgramInput if isinstance(program_args, ProgramArgs) else DualProgramInput
     )
-    if isinstance(output, OptimizationOutput):
+    if output.input_data.calctype in {CalcType.optimization, CalcType.transition_state}:
+        assert isinstance(output.results, OptimizationResults)  # mypy
         # Take final geometry from optimization and pass to next input
         return input_model(
             molecule=output.results.final_molecule,
             calctype=calctype,
             **program_args.model_dump(),
         )
     else:
@@ -84,16 +81,16 @@
             f"No implementation for transforming {output.__class__.__name__} objects "
             f"into {input_model.__name__} objects yet."
         )
 
 
 @bigchem.task
 def assemble_hessian(
-    gradients: List[SinglePointOutput], dh: float
-) -> Union[SinglePointOutput, ProgramFailure]:
+    gradients: List[ProgramOutput[ProgramInput, SinglePointResults]], dh: float
+) -> ProgramOutput[ProgramInput, SinglePointResults]:
     """Assemble hessian from an array of gradient computations
 
     Params:
         gradients: List of gradient AtomicResult objects alternating between a
             "forward" and "backward" computation. NOTE: The last computation on the
             list is a basic energy calculation of the original geometry.
         dh: The displacement used for finite difference displacements of gradient
@@ -103,41 +100,39 @@
         Another way I've tested this algorithm is to compute the hessian using psi4
         and then using this algorithm at the save level of theory and then compare
         their eigenvalues. The results have always matched up to two decimal places.
         The matrices can't be compared directly because it appears psi4 does some sort
         of rotation on their matrix, so the eigenvalues are a better mechanism for
         comparison.
     """
-    # Validate input array; return FailedOperation if a gradient or energy failed
-    for gradient in gradients:
-        if isinstance(gradient, ProgramFailure):
-            return gradient
-
     # Pop energy calculation of original geometry from gradients (last value in
     # gradients list)
     energy_output = gradients.pop()
 
+    # # Verify data integrity of gradients
+    # for gradient in gradients:
+
     dim = len(gradients[0].input_data.molecule.symbols) * 3
     hessian = np.zeros((dim, dim), dtype=float)
 
     for i, (forward, backward) in enumerate(zip_longest(*[iter(gradients)] * 2)):
-        val = (forward.return_result - backward.return_result) / (dh * 2)
+        val = (forward.results.gradient - backward.results.gradient) / (dh * 2)  # type: ignore # noqa: E501
         hessian[i] = val.flatten()
 
     output = energy_output.model_dump()
     output["input_data"]["calctype"] = CalcType.hessian
     output["results"]["hessian"] = hessian
 
-    return SinglePointOutput(**output)
+    return ProgramOutput[ProgramInput, SinglePointResults](**output)
 
 
 @bigchem.task
 def frequency_analysis(
-    sp_output: SinglePointOutput, **kwargs
-) -> Union[SinglePointOutput, ProgramFailure]:
+    sp_output: ProgramOutput[ProgramInput, SinglePointResults], **kwargs
+) -> ProgramOutput[ProgramInput, SinglePointResults]:
     """Adds geomeTRIC's frequency analysis results to hessian SinglePointOutput
 
     Params:
         sp_output: SinglePointOutput with .results.hessian value
         kwargs: Keywords passed to geomeTRIC's frequency_analysis function
             temperature: float - Temperature passed to the harmonic free energy module;
                 default: 300.0
@@ -152,29 +147,29 @@
 
     """
     # Import here so client applications don't need to install geomeTRIC
     from geometric.normal_modes import frequency_analysis as geometric_freqs_analysis
 
     freqs, n_modes, g_tot = geometric_freqs_analysis(
         sp_output.input_data.molecule.geometry.flatten(),  # numpy array
-        sp_output.results.hessian,
+        sp_output.results.hessian,  # type: ignore
         elem=sp_output.input_data.molecule.symbols,  # regular python list
         # Electronic energy passed to free energy module
-        energy=sp_output.results.energy,
+        energy=sp_output.results.energy,  # type: ignore
         **kwargs,
     )
     output = sp_output.model_dump()
     output["results"].update(
         {
             "freqs_wavenumber": freqs.tolist(),
             "normal_modes_cartesian": n_modes,
             "gibbs_free_energy": g_tot,
         }
     )
-    return SinglePointOutput(**output)
+    return ProgramOutput[ProgramInput, SinglePointResults](**output)
 
 
 @bigchem.task
 def add(x, y):
     """Add two numbers
 
     NOTE: Used for design testing
```

### Comparing `bigchem-0.6.9/bigchem/utils.py` & `bigchem-0.7.0/bigchem/utils.py`

 * *Files identical despite different names*

### Comparing `bigchem-0.6.9/pyproject.toml` & `bigchem-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "bigchem"
-version = "0.6.9"
+version = "0.7.0"
 description = "A distributed system for scaling and parallelizing quantum chemistry calculations"
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 readme = "README.md"
 homepage = "https://github.com/mtzgroup/bigchem"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 celery = { version = "^5.3.4", extras = ["redis"] }
 pydantic = "^2.0.0"
-qcio = ">=0.8.1"
+qcio = "^0.9.0"
+qcop = "^0.6.0"
 pydantic-settings = "^2.0.3"
+
 # A list of all of the optional dependencies, some of which are included in the below
 # `extras`. They can be opted into by apps. Clients should not need to install these.
 geometric = { version = "^1.0.1", optional = true }
 qcengine = { version = "^0.27.0", optional = true }
-qcop = "^0.5.5"
 
 [tool.poetry.extras]
 geometric = ["geometric"]
 qcengine = ["qcengine"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.0.0"
@@ -32,14 +33,16 @@
 pytest-cov = "^3.0.0"
 pytest-timeout = "^2.1.0"
 boto3 = "^1.26.82"
 paramiko = "^3.0.0"
 types-paramiko = "^3.0.0.4"
 ruff = "^0.0.278"
 geometric = ">=1.0.1"
+xtb = "^22.1"
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
```

### Comparing `bigchem-0.6.9/PKG-INFO` & `bigchem-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigchem
-Version: 0.6.9
+Version: 0.7.0
 Summary: A distributed system for scaling and parallelizing quantum chemistry calculations
 Home-page: https://github.com/mtzgroup/bigchem
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Provides-Extra: geometric
 Provides-Extra: qcengine
 Requires-Dist: celery[redis] (>=5.3.4,<6.0.0)
 Requires-Dist: geometric (>=1.0.1,<2.0.0) ; extra == "geometric"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: qcengine (>=0.27.0,<0.28.0) ; extra == "qcengine"
-Requires-Dist: qcio (>=0.8.1)
-Requires-Dist: qcop (>=0.5.5,<0.6.0)
+Requires-Dist: qcio (>=0.9.0,<0.10.0)
+Requires-Dist: qcop (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # BigChem
 
 A distributed system for scaling and parallelizing quantum chemistry calculations.
 
 ## ⚠️ A Note About x86 and ARM Architectures
```

