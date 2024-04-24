# Comparing `tmp/qcop-0.5.5.tar.gz` & `tmp/qcop-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcop-0.5.5.tar", max compression
+gzip compressed data, was "qcop-0.6.0.tar", max compression
```

## Comparing `qcop-0.5.5.tar` & `qcop-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-04-13 05:12:32.886919 qcop-0.5.5/LICENSE
--rw-r--r--   0        0        0     7283 2024-04-13 05:12:32.886919 qcop-0.5.5/README.md
--rw-r--r--   0        0        0     1832 2024-04-13 05:12:32.886919 qcop-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      248 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/__init__.py
--rw-r--r--   0        0        0      360 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/__init__.py
--rw-r--r--   0        0        0    12404 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/base.py
--rw-r--r--   0        0        0     1487 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/file.py
--rw-r--r--   0        0        0    11141 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/geometric.py
--rw-r--r--   0        0        0     2111 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/qcengine.py
--rw-r--r--   0        0        0     4602 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/terachem.py
--rw-r--r--   0        0        0     8891 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/utils.py
--rw-r--r--   0        0        0     4492 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/adapters/xtb.py
--rw-r--r--   0        0        0     3639 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/exceptions.py
--rw-r--r--   0        0        0     3134 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/main.py
--rw-r--r--   0        0        0        0 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/py.typed
--rw-r--r--   0        0        0     3363 2024-04-13 05:12:32.886919 qcop-0.5.5/qcop/utils.py
--rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-24 01:15:45.604299 qcop-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7084 2024-04-24 01:15:45.604299 qcop-0.6.0/README.md
+-rw-r--r--   0        0        0     1876 2024-04-24 01:15:45.608299 qcop-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/__init__.py
+-rw-r--r--   0        0        0    12876 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/base.py
+-rw-r--r--   0        0        0     1506 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/file.py
+-rw-r--r--   0        0        0    11920 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/geometric.py
+-rw-r--r--   0        0        0     2123 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/qcengine.py
+-rw-r--r--   0        0        0     4697 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/terachem.py
+-rw-r--r--   0        0        0     8891 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/utils.py
+-rw-r--r--   0        0        0     4396 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/adapters/xtb.py
+-rw-r--r--   0        0        0     4108 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/exceptions.py
+-rw-r--r--   0        0        0     2964 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/main.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/py.typed
+-rw-r--r--   0        0        0     3347 2024-04-24 01:15:45.608299 qcop-0.6.0/qcop/utils.py
+-rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 qcop-0.6.0/PKG-INFO
```

### Comparing `qcop-0.5.5/LICENSE` & `qcop-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcop-0.5.5/README.md` & `qcop-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,41 +42,41 @@
 prog_input = ProgramInput(
     molecule=h2o,
     calctype="energy",
     model={"method": "hf", "basis": "sto-3g"},
     keywords={"purify": "no", "restricted": False},
 )
 
-# Run the calculation; will return SinglePointOutput or raise an exception
+# Run the calculation; will return ProgramOutput or raise an exception
 try:
-    output = compute("terachem", prog_input, collect_files=True)
+    po = compute("terachem", prog_input, collect_files=True)
 except ExternalProgramError as e:
     # External QQ program failed in some way
-    prog_failure = e.program_failure
-    prog_failure.input_data # Input data used by the QC program
-    prog_failure.success # Will be False
-    prog_failure.results # Any half-computed results before the failure
-    prog_failure.traceback # Stack trace from the calculation
-    prog_failure.ptraceback # Shortcut to print out the traceback in human readable format
-    prog_failure.stdout # Stdout log from the calculation
+    po = e.program_output
+    po.input_data # Input data used by the QC program
+    po.success # Will be False
+    po.results # Any half-computed results before the failure
+    po.traceback # Stack trace from the calculation
+    po.ptraceback # Shortcut to print out the traceback in human readable format
+    po.stdout # Stdout log from the calculation
     raise e
 else:
     # Calculation succeeded
-    output.input_data # Input data used by the QC program
-    output.success # Will be True
-    output.results # All structured results from the calculation
-    output.stdout # Stdout log from the calculation
-    output.pstdout # Shortcut to print out the stdout in human readable format
-    output.files # Any files returned by the calculation
-    output.provenance # Provenance information about the calculation
-    output.extras # Any extra information not in the schema
+    po.input_data # Input data used by the QC program
+    po.success # Will be True
+    po.results # All structured results from the calculation
+    po.stdout # Stdout log from the calculation
+    po.pstdout # Shortcut to print out the stdout in human readable format
+    po.files # Any files returned by the calculation
+    po.provenance # Provenance information about the calculation
+    po.extras # Any extra information not in the schema
 
 ```
 
-One may also call `compute(..., raise_exc=False)` to return a `ProgramFailure` object rather than raising an exception when a calculation fails. This may allow easier handling of failures in some cases.
+One may also call `compute(..., raise_exc=False)` to return a `ProgramOutput` object rather than raising an exception when a calculation fails. This may allow easier handling of failures in some cases.
 
 ```python
 from qcio import Molecule, ProgramInput
 from qcop import compute
 from qcop.exceptions import ExternalProgramError
 # Create the molecule
 h2o = Molecule.open("h2o.xyz")
@@ -85,35 +85,35 @@
 prog_input = ProgramInput(
     molecule=h2o,
     calctype="energy",
     model={"method": "hf", "basis": "sto-3g"},
     keywords={"purify": "no", "restricted": False},
 )
 
-# Run the calculation; will return either a SinglePointOutput or a ProgramFailure
-output = compute("terachem", prog_input, collect_files=True, raise_exc=False)
-if not output.success:
+# Run the calculation; will return a ProgramOutput objects
+po = compute("terachem", prog_input, collect_files=True, raise_exc=False)
+if not po.success:
     # External QQ program failed in some way
-    output.input_data # Input data used by the QC program
-    output.success # Will be False
-    output.results # Any half-computed results before the failure
-    output.traceback # Stack trace from the calculation
-    output.ptraceback # Shortcut to print out the traceback in human readable format
-    output.stdout # Stdout log from the calculation
+    po.input_data # Input data used by the QC program
+    po.success # Will be False
+    po.results # Any half-computed results before the failure
+    po.traceback # Stack trace from the calculation
+    po.ptraceback # Shortcut to print out the traceback in human readable format
+    po.stdout # Stdout log from the calculation
 
 else:
     # Calculation succeeded
-    output.input_data # Input data used by the QC program
-    output.success # Will be True
-    output.results # All structured results from the calculation
-    output.stdout # Stdout log from the calculation
-    output.pstdout # Shortcut to print out the stdout in human readable format
-    output.files # Any files returned by the calculation
-    output.provenance # Provenance information about the calculation
-    output.extras # Any extra information not in the schema
+    po.input_data # Input data used by the QC program
+    po.success # Will be True
+    po.results # All structured results from the calculation
+    po.stdout # Stdout log from the calculation
+    po.pstdout # Shortcut to print out the stdout in human readable format
+    po.files # Any files returned by the calculation
+    po.provenance # Provenance information about the calculation
+    po.extras # Any extra information not in the schema
 
 ```
 
 Alternatively, the `compute_args` function can be used to run a calculation with the input data structures passed in as arguments rather than as a single `ProgramInput` object.
 
 ```python
 from qcio import Molecule
```

### Comparing `qcop-0.5.5/pyproject.toml` & `qcop-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "qcop"
-version = "0.5.5"
+version = "0.6.0"
 description = "A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/coltonbh/qcop"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-qcio = "^0.8.2"
+qcio = "^0.9.0"
 qcparse = "^0.5.2"
 
 # A list of all of the optional dependencies, some of which are included in the below
 # `extras`. They can be opted into by apps.
-qcelemental = { version = ">=0.26.0", optional = true }
-qcengine = { version = ">=0.27.0", optional = true }
-geometric = { version = ">=1.0.1", optional = true }
+qcelemental = { version = "^0.26.0", optional = true }
+qcengine = { version = "^0.27.0", optional = true }
+geometric = { version = "^1.0.1", optional = true }
+
 
 [tool.poetry.extras]
 qcengine = ["qcelemental", "qcengine"]
 geometric = ["geometric"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.0.0"
```

### Comparing `qcop-0.5.5/qcop/adapters/base.py` & `qcop-0.6.0/qcop/adapters/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,100 @@
 import traceback
 from abc import ABC, abstractmethod
 from time import time
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Union
 
-from qcio import CalcType, FileInput, InputBase, OutputBase, ProgramFailure, ResultsBase
+from qcio import (
+    CalcType,
+    FileInput,
+    InputType,
+    NoResults,
+    ProgramOutput,
+    Results,
+    ResultsType,
+    StructuredInputs,
+)
 from qcio.helper_types import StrOrPath
-from qcio.models.base_models import QCIOModelBase
-from qcio.models.inputs_base import StructuredInputBase
-from qcio.utils import calctype_to_output
 
 from qcop.exceptions import AdapterInputError, QCOPBaseError
 
 from .utils import construct_provenance, tmpdir
 
 __all__ = ["BaseAdapter", "registry"]
 
 # Registry for all Adaptors.
 # NOTE: Registry stores class objects, not instances.
 # Use registry[program]() to instantiate an adaptor
 # Or use the higher level qcop.utils.get_adapter() function.
 registry = {}
 
 
-class BaseAdapter(ABC):
+class BaseAdapter(ABC, Generic[InputType, ResultsType]):
     """Base class for all adapters."""
 
     # Whether to write files from inp_obj to disk before executing program.
     # If True, the adapter will write all files from inp_obj to disk before executing
     # the program. If False, the adapter must handle input files itself in some other
     # way. Generally this should be True for most adapters unless the program can
     # handle input files directly from memory, stdin, or some other mechanism that is
     # more efficient than writing to disk.
     write_files = True
     program: str  # All subclasses must define this attribute.
 
     def program_version(self, stdout: Optional[str]) -> Optional[str]:
-        """Return program version. Adapters should override this method."""
+        """Return program version. Adapters should override this method.
+
+        Args:
+            stdout: The stdout from the program. Because running "program --version"
+                can be extremely slow for some programs, the stdout from the program
+                is passed in here so that the version can be extracted from it if
+                possible. If the version cannot be extracted from the stdout, then
+                this function should return the program version in some other way.
+        """
         return None
 
     @abstractmethod
-    def validate_input(self, inp_obj: InputBase) -> None:
+    def validate_input(self, inp_obj: InputType) -> None:
         """Validate input object to ensure compatibility with adapter.
         Adapters should override this method.
         """
         raise NotImplementedError
 
     @abstractmethod
     def compute_results(
         self,
-        inp_obj: InputBase,
+        inp_obj: InputType,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
         **kwargs,
-    ) -> Tuple[ResultsBase, str]:
+    ) -> Tuple[ResultsType, str]:
         """Subclasses should implement this method with custom compute logic."""
         raise NotImplementedError
 
     def compute(
         self,
-        inp_obj: InputBase,
+        inp_obj: InputType,
         *,
         scratch_dir: Optional[StrOrPath] = None,
         rm_scratch_dir: bool = True,
         collect_stdout: bool = True,
         collect_files: bool = False,
         collect_wfn: bool = False,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
         print_stdout: bool = False,
         raise_exc: bool = True,
         propagate_wfn: bool = False,
         **kwargs,
-    ) -> OutputBase:
+    ) -> ProgramOutput[InputType, ResultsType]:
         """Compute the given input using the adapter's program.
 
         Args:
-            inp_obj: A qcio input object for a computation. A subclass of InputBase.
-                E.g. FileInput, FileInput, DualProgramInput.
+            inp_obj: A qcio input object for a computation. E.g. A FileInput,
+                ProgramInput or DualProgramInput.
             scratch_dir: The scratch directory for the program. If None, a new directory
                 is created in the system default temporary directory. If rm_scratch_dir
                 is True this directory will be deleted after the program finishes.
             rm_scratch_dir: Delete the scratch directory after the program exits.
             collect_stdout: Whether to collect stdout/stderr from the program as output.
                 Failed computations will always collect stdout/stderr.
             collect_files: Collect all files generated by the QC program as output.
@@ -90,60 +104,55 @@
             update_func: A function to call as the program executes. The function must
                 accept the in-process stdout/stderr output as a string for its first
                 argument.
             update_interval: The minimum time in seconds between calls to the
                 update_func.
             print_stdout: Whether to print stdout/stderr to the terminal in real time as
                 the program executes. Will be ignored if an update_func passed.
-            raise_exc: If False, qcop will return a ProgramFailure object when the QC
+            raise_exc: If False, qcop will return a ProgramOutput object when the QC
                 program fails rather than raise an exception.
             propagate_wfn: For any adapter performing a sequential task, such
                 as a geometry optimization, propagate the wavefunction from the previous
                 step to the next step. This is useful for accelerating convergence by
                 using a previously computed wavefunction as a starting guess. If an
                 adapter does not support wavefunction propagation, an AdapterInputError
                 will be raised.
             **kwargs: Additional keyword arguments to pass to the adapter or
                 qcng.compute().
 
         Returns:
-            The qcio output object for a calctype. A subclass of OutputBase. Will either
-            be a ProgramFailure object or the corresponding output object for the
-            calctype type. E.g., "energy" -> SinglePointOutput. "optimization" ->
-            OptimizationOutput.
+            A ProgramOutput object containing the results of the computation.
 
         Raises:
             AdapterNotFoundError: If the program is not supported (i.e., no Adapter
-                is implemented for it in qcop or qcengine).
+                is implemented for the program in qcop or qcengine).
             ProgramNotFoundError: If the program executable is not found on the
                 system at execution time. This likely means the program is not installed
-                on the system.
+                or not available on the $PATH.
             AdapterInputError: If the input is invalid for the adapter.
-            ExternalProgramExecutionError: If the program fails during execution and
-                raise_exc=True.
-            QCEngineError: If QCEngine performed the computation, fails and
-                raise_exc=True.
+            ExternalProgramExecutionError: If the QC program fails during execution.
+            QCEngineError: If QCEngine performs the computation raises an error.
         """
         # Print stdout to terminal in real time as program executes
         if print_stdout and update_func is None:
             update_func, update_interval = (
                 lambda _, stdout_new: print(stdout_new),
                 0.1,
             )
 
         # cd to a temporary directory to run the program.
         with tmpdir(scratch_dir, rm_scratch_dir) as final_scratch_dir:
             if self.write_files:  # Write non structured input files to disk.
                 inp_obj.save_files()
 
             # Define outputs
-            output_dict: Dict[str, Optional[Union[str, QCIOModelBase]]] = {}
+            output_dict: Dict[str, Any] = {}
             stdout: Optional[str] = None
             # TODO: Update when qcio updates to allow None results
-            results: Optional[ResultsBase] = None
+            results: Results = NoResults()
             exc: Optional[QCOPBaseError] = None
             program_version: Optional[str] = None
 
             start = time()
             try:
                 # Validate input object
                 self.validate_input(inp_obj)
@@ -153,26 +162,28 @@
                     inp_obj,
                     update_func,
                     update_interval,
                     propagate_wfn=propagate_wfn,
                     **kwargs,
                 )
                 # None value covers FileInput case
-                # TODO: Update this to ProgramOutput[type(inp_obj), type(results)]
-                output_cls = calctype_to_output(getattr(inp_obj, "calctype", None))
+                # TODO: Is there a type safe way to handle this??
+                output_dict["success"] = True
                 program_version = self.program_version(stdout)
 
                 # Optionally collect wavefunction file
                 if collect_wfn and not collect_files:
                     output_dict["files"] = self.collect_wfn()
 
             except QCOPBaseError as e:
-                # Set variables to construct a ProgramFailure object.
-                exc, output_cls = e, ProgramFailure
-                results = getattr(e, "results", results)  # Any half-completed results
+                # TODO: Is there a type safe way to handle this??
+                exc = e
+                output_dict["success"] = False
+                # Any half-completed results
+                results = getattr(e, "results") or NoResults()
                 stdout = getattr(e, "stdout", stdout)
                 # For mypy because e.stdout is not of a known type
                 stdout = str(stdout) if stdout is not None else None
                 output_dict["traceback"] = traceback.format_exc()
 
             wall_time = time() - start
 
@@ -181,38 +192,41 @@
                 self.program,
                 program_version,
                 final_scratch_dir,
                 wall_time,
             )
 
             # Always collect for failures; otherwise obey collect_stdout
-            stdout = stdout if collect_stdout or output_cls == ProgramFailure else None
+            stdout = stdout if not output_dict["success"] or collect_stdout else None
 
             # Construct output object
-            results = results if results is not None else ResultsBase()
             output_dict.update(
                 {
                     "input_data": inp_obj,
                     "stdout": stdout,
                     "results": results,
                     "provenance": provenance,
                 }
             )
-            output_obj = output_cls(**output_dict)
+
+            output_obj = ProgramOutput[InputType, ResultsType](**output_dict)
 
             # Collect files generated by the program
             if collect_files or isinstance(inp_obj, FileInput):
-                output_obj.open_files(
-                    final_scratch_dir, recursive=True, exclude=inp_obj.files.keys()
+                output_obj.add_files(
+                    final_scratch_dir,
+                    recursive=True,
+                    exclude=list(inp_obj.files.keys()),
                 )
 
-        # Append ProgramFailures to exception and raise if raise_exc=True
+        # Append ProgramOutput to exception and raise if raise_exc=True
         # Helpful for BigChem and ChemCloud exception handling
+
         if raise_exc and exc:
-            exc.program_failure = output_obj
+            exc.program_output = output_obj
             # Updating .args is necessary for Celery to properly serialize the exception
             exc.args = (*exc.args, output_obj)
             raise exc
 
         return output_obj
 
     def collect_wfn(self) -> Dict[str, Union[str, bytes]]:
@@ -225,15 +239,15 @@
         # Collect wavefunction file from the calc_dir
         raise AdapterInputError(
             self.program,
             f"Adapter for {self.program} does not support wavefunction collection.",
         )
 
 
-class ProgramAdapter(BaseAdapter):
+class ProgramAdapter(BaseAdapter, Generic[InputType, ResultsType]):
     """Base adapter for all program adapters (all but FileAdaptor)."""
 
     supported_calctypes: List[
         CalcType
     ]  # All subclasses must specify supported calctypes
 
     def __init_subclass__(cls, **kwargs):
@@ -263,15 +277,26 @@
             stdout: The stdout from the program. Because running "program --version"
                 can be extremely slow for some programs, the stdout from the program
                 is passed in here so that the version can be extracted from it if
                 possible. If the version cannot be extracted from the stdout, then
                 this function should return the program version in some other way.
         """
 
-    def validate_input(self, inp_obj: StructuredInputBase) -> None:
+    @abstractmethod
+    def compute_results(
+        self,
+        inp_obj: InputType,
+        update_func: Optional[Callable] = None,
+        update_interval: Optional[float] = None,
+        **kwargs,
+    ) -> Tuple[ResultsType, str]:
+        """All ProgramAdapters must return a ResultsType."""
+        raise NotImplementedError
+
+    def validate_input(self, inp_obj: StructuredInputs) -> None:
         """Validate the input object for compatibility with the adapter.
 
         Args:
             inp_obj: The input object to validate.
 
         Raises:
             AdapterInputError: If the input object's calctype is not supported.
```

### Comparing `qcop-0.5.5/qcop/adapters/file.py` & `qcop-0.6.0/qcop/adapters/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Callable, Optional, Tuple
 
-from qcio import FileInput, FileOutput, InputBase
+from qcio import FileInput, NoResults
 
 from qcop.adapters.base import BaseAdapter
 
 from .utils import execute_subprocess
 
 
-class FileAdapter(BaseAdapter):
+class FileAdapter(BaseAdapter[FileInput, NoResults]):
     """adapter for running a program on files."""
 
     def __init__(self, program: str) -> None:
         super().__init__()
         self.program = program
 
-    def validate_input(self, inp_obj: InputBase) -> None:
+    def validate_input(self, inp_obj: FileInput) -> None:
         """No validation checks performed for FileAdapter"""
         pass
 
     def compute_results(
         self,
         inp_obj: FileInput,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
         **kwargs,
-    ) -> Tuple[FileOutput, str]:
+    ) -> Tuple[NoResults, str]:
         """Compute the given program on the given files.
 
         Args:
             inp_obj: The qcio FileInput object for a computation.
             update_func: A callback function to call as the program executes.
             update_interval: The minimum time in seconds between calls to the
             update_func.
 
         Returns:
-            Tuple of None and FileOutput object for a computation. None is
+            Tuple of None and ProgramOutput object for a computation. None is
                 returned because no computed properties are returned for a file
                 computation.
 
         Raises:
             ProgramNotFoundException: If the program is not found.
 
         """
         stdout = execute_subprocess(
             self.program, inp_obj.cmdline_args, update_func, update_interval
         )
-        return None, stdout
+        return NoResults(), stdout
```

### Comparing `qcop-0.5.5/qcop/adapters/geometric.py` & `qcop-0.6.0/qcop/adapters/geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 
 import numpy as np
 from qcio import (
     CalcType,
     DualProgramInput,
     Molecule,
     OptimizationResults,
+    ProgramArgs,
     ProgramInput,
-    QCProgramArgs,
-    SinglePointOutput,
+    ProgramOutput,
+    SinglePointResults,
 )
 
 from qcop.exceptions import (
     AdapterInputError,
-    ExternalSubprocessError,
     GeometricError,
     ProgramNotFoundError,
+    QCOPBaseError,
 )
 from qcop.utils import get_adapter
 
 from .base import ProgramAdapter
 from .utils import capture_logs
 
 
-class GeometricAdapter(ProgramAdapter):
+class GeometricAdapter(ProgramAdapter[DualProgramInput, OptimizationResults]):
     program = "geometric"
     supported_calctypes = [CalcType.optimization, CalcType.transition_state]
 
     def __init__(self):
         super().__init__()
         # Check that geomeTRIC is installed
         self.geometric = self._ensure_geometric()
@@ -239,27 +240,27 @@
 
         class QCOPGeometricEngine(self.geometric.engine.Engine):
             """QCOP Engine for Geometric"""
 
             def __init__(
                 self,
                 qcio_adapter: ProgramAdapter,
-                qcio_program_args: QCProgramArgs,
+                qcio_program_args: ProgramArgs,
                 qcio_molecule: Molecule,
                 geometric_molecule,
                 propagate_wfn: bool = False,
                 update_func: Optional[Callable] = None,
                 update_interval: Optional[float] = None,
             ):
                 super().__init__(geometric_molecule)
                 self.qcio_adapter = qcio_adapter
                 self.qcio_program_args = qcio_program_args
                 self.qcio_molecule = qcio_molecule
                 self.propagate_wfn = propagate_wfn
-                self.qcio_trajectory: List[SinglePointOutput] = []
+                self.qcio_trajectory: List[ProgramOutput] = []
                 self.update_func = update_func
                 self.update_interval = update_interval
 
             def calc_new(self, coords, *args) -> Dict[str, Union[float, np.ndarray]]:
                 """Calculate the energy and gradient for a given geometry.
 
                 Args:
@@ -285,30 +286,44 @@
                     and hasattr(self.qcio_adapter, "propagate_wfn")
                 ):
                     self.qcio_adapter.propagate_wfn(
                         self.qcio_trajectory[-1], prog_input
                     )
 
                 # Calculate energy and gradient
-                # raise_exc=True so ProgramFailure objects don't get returned
                 try:
-                    output = self.qcio_adapter.compute(
-                        prog_input,
-                        raise_exc=True,
-                        collect_wfn=self.propagate_wfn,
-                        update_func=self.update_func,
-                        update_interval=self.update_interval,
+                    output: ProgramOutput[ProgramInput, SinglePointResults] = (
+                        self.qcio_adapter.compute(
+                            prog_input,
+                            raise_exc=True,
+                            collect_wfn=self.propagate_wfn,
+                            update_func=self.update_func,
+                            update_interval=self.update_interval,
+                        )
                     )
-                except ExternalSubprocessError as e:
-                    e.results = OptimizationResults(trajectory=self.qcio_trajectory)
+                except QCOPBaseError as e:
+                    if e.program_output:  # For mypy
+                        # Append error output
+                        self.qcio_trajectory.append(e.program_output)
+                    results = OptimizationResults(trajectory=self.qcio_trajectory)
+                    e.results = results
+                    # TODO: Add args/kwargs update for Celery serialization?
+                    # Maybe not because .results is folded into e.program_output in
+                    # BaseAdapter.compute()?
                     raise e
 
                 else:
                     self.qcio_trajectory.append(output)
 
+                assert (  # for mypy
+                    output.results is not None
+                    and output.results.energy is not None
+                    and output.results.gradient is not None
+                    and isinstance(output.results.gradient, np.ndarray)
+                )
                 return {
                     "energy": output.results.energy,
                     # geomeTRIC requires 1D array
                     "gradient": output.results.gradient.flatten(),
                 }
 
         return QCOPGeometricEngine
```

### Comparing `qcop-0.5.5/qcop/adapters/qcengine.py` & `qcop-0.6.0/qcop/adapters/qcengine.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         """Get the program version."""
         from qcengine import get_program
         from qcengine.exceptions import QCEngineException
 
         try:
             adapter = get_program(self.external_program)
             return adapter.get_version()
-        except QCEngineException:
+        except QCEngineException as e:
             raise QCEngineError(
                 f"Could not get version for program {self.external_program}."
-            )
+            ) from e
 
     def compute_results(
         self, inp_obj, *args, propagate_wfn=False, **kwargs
     ) -> Tuple[SinglePointResults, str]:
         from qcengine import compute as qcng_compute
         from qcengine.exceptions import QCEngineException
```

### Comparing `qcop-0.5.5/qcop/adapters/terachem.py` & `qcop-0.6.0/qcop/adapters/terachem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from pathlib import Path
 from typing import Callable, Dict, Optional, Tuple, Union
 
 import qcparse
-from qcio import CalcType, ProgramInput, SinglePointOutput, SinglePointResults
+from qcio import CalcType, ProgramInput, ProgramOutput, SinglePointResults
 from qcparse.encoders.terachem import XYZ_FILENAME
 from qcparse.parsers.terachem import parse_version_string
 
 from qcop.exceptions import AdapterError, AdapterInputError
 
 from .base import ProgramAdapter
 from .utils import execute_subprocess
 
 
-class TeraChemAdapter(ProgramAdapter):
+class TeraChemAdapter(ProgramAdapter[ProgramInput, SinglePointResults]):
     """Adapter for TeraChem."""
 
     supported_calctypes = [CalcType.energy, CalcType.gradient, CalcType.hessian]
     program = "terachem"
 
     def program_version(self, stdout: Optional[str] = None) -> str:
         """Get the program version.
@@ -33,15 +33,15 @@
             # Cut out "TeraChem version " (17 chars) from the output
             return execute_subprocess(self.program, ["--version"])[17:]
 
     # TODO: Need command line options for TeraChem e.g., -g 1 for GPUs MAYBE?
     # Try using it for a while without and see what roadblocks we run into
     def compute_results(
         self,
-        inp_obj,
+        inp_obj: ProgramInput,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
         **kwargs,
     ) -> Tuple[SinglePointResults, str]:
         """Execute TeraChem on the given input.
 
         Args:
@@ -81,15 +81,15 @@
 
         wfns: Dict[str, Union[str, bytes]] = {}
         for wfn_path in wfn_paths:
             if wfn_path.exists():
                 wfns[str(wfn_path)] = wfn_path.read_bytes()
         return wfns
 
-    def propagate_wfn(self, output: SinglePointOutput, prog_inp: ProgramInput) -> None:
+    def propagate_wfn(self, output: ProgramOutput, prog_inp: ProgramInput) -> None:
         """Propagate the wavefunction from the previous calculation.
 
         Args:
             output: The output from a previous calculation containing wavefunction data.
             prog_inp: The ProgramInput object on which to place the wavefunction data.
 
         Returns:
@@ -115,10 +115,11 @@
         # Load wavefunction data onto ProgramInput object
 
         if c0_bytes:
             prog_inp.files[c0] = c0_bytes
             prog_inp.keywords["guess"] = c0
 
         else:  # ca0_bytes and cb0_bytes
+            assert ca0_bytes and cb0_bytes  # for mypy
             prog_inp.files[ca0] = ca0_bytes
             prog_inp.files[cb0] = cb0_bytes
             prog_inp.keywords["guess"] = f"{ca0} {cb0}"
```

### Comparing `qcop-0.5.5/qcop/adapters/utils.py` & `qcop-0.6.0/qcop/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.5/qcop/adapters/xtb.py` & `qcop-0.6.0/qcop/adapters/xtb.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 
 import importlib
 import os
 from typing import Callable, Optional, Tuple
 
 import numpy as np
 from qcio import CalcType, ProgramInput, SinglePointResults, Wavefunction
-from qcio.constants import ELEMENTS
 
 from qcop.exceptions import (
     AdapterInputError,
     ExternalProgramError,
     ProgramNotFoundError,
 )
 
 from .base import ProgramAdapter
 from .utils import capture_sys_stdout
 
 
-class XTBAdapter(ProgramAdapter):
+class XTBAdapter(ProgramAdapter[ProgramInput, SinglePointResults]):
     """Adapter for xtb-python."""
 
     supported_calctypes = [CalcType.energy, CalcType.gradient]
     program = "xtb"
     write_files = False  # xtb-python does not use files written to disk
 
     def __init__(self):
@@ -85,20 +84,17 @@
                 update_func.
 
         Returns:
             A tuple of SinglePointComputedProps and the stdout str.
         """
         try:
             # Create Calculator
-            atomic_numbers = np.array(
-                [ELEMENTS[sym] for sym in inp_obj.molecule.symbols]
-            )
             calc = self.xtb.interface.Calculator(
                 getattr(self.xtb.interface.Param, inp_obj.model.method),
-                atomic_numbers,
+                np.array(inp_obj.molecule.atomic_numbers),
                 inp_obj.molecule.geometry,
                 inp_obj.molecule.charge,
                 # From https://github.com/grimme-lab/xtb-python/blob/a32309a43e5a6572b033814eacf396328a2a36ed/xtb/qcschema/harness.py#L126 # noqa: E501
                 inp_obj.molecule.multiplicity - 1,
             )
             calc.set_verbosity(self.xtb.libxtb.VERBOSITY_FULL)  # all logs
```

### Comparing `qcop-0.5.5/qcop/exceptions.py` & `qcop-0.6.0/qcop/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 """Experimental exception hierarchy. This may be too complex and unhelpful for now"""
 
+import warnings
 from typing import Optional
 
-from qcio import ProgramFailure, ResultsBase
+from qcio import ProgramOutput, Results
 
 
 class QCOPBaseError(Exception):
     """Base class for exceptions in qcop. All custom exceptions should inherit from
     this class."""
 
     def __init__(
-        self, *args, program_failure: Optional[ProgramFailure] = None, **kwargs
+        self,
+        *args,
+        program_output: Optional[ProgramOutput] = None,
+        results: Optional[Results] = None,
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
-        self.program_failure = program_failure
+        self.program_output = program_output
+        self.results = results
+
+    @property
+    def program_failure(self):
+        """Maintain backwards compatibility."""
+        warnings.warn(
+            "The 'program_failure' attribute is deprecated and will be removed in a "
+            "future release. Use 'program_output' instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
+        return self.program_output
 
 
 class AdapterError(QCOPBaseError):
     """Base class for exceptions thrown by adapters."""
 
     pass
 
@@ -109,18 +126,18 @@
     """
 
     def __init__(
         self,
         returncode: int,
         cmd: str,
         stdout: Optional[str] = None,
-        results: Optional[ResultsBase] = None,
+        **kwargs,
     ):
         self.returncode = returncode
         self.cmd = cmd
         self.stdout = stdout
-        self.results = results
+        self.results = kwargs.get("results", None)
         self.message = (
             f"External program failed with return code {self.returncode}. "
             f"Command: '{self.cmd}'"
         )
-        super().__init__(self.message)
+        super().__init__(self.message, **kwargs)
```

### Comparing `qcop-0.5.5/qcop/main.py` & `qcop-0.6.0/qcop/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Top level compute functions for qcop."""
 
 from typing import Any, Callable, Dict, Optional, Union
 
-from qcio import CalcType, Files, Model, Molecule, ProgramInput
+from qcio import (
+    CalcType,
+    Files,
+    InputType,
+    Model,
+    Molecule,
+    ProgramInput,
+    ProgramOutput,
+)
 from qcio.helper_types import StrOrPath
-from qcio.models import InputBase, OutputBase
 
 from .adapters import BaseAdapter
 from .utils import get_adapter, inherit_docstring_from
 
 
 @inherit_docstring_from(BaseAdapter.compute)
 def compute(
     program: str,
-    inp_obj: InputBase,
+    inp_obj: InputType,
     *,
     scratch_dir: Optional[StrOrPath] = None,
     rm_scratch_dir: bool = True,
     collect_stdout: bool = True,
     collect_files: bool = False,
     collect_wavefunction: bool = False,
     update_func: Optional[Callable] = None,
     update_interval: Optional[float] = None,
     print_stdout: bool = False,
     raise_exc: bool = True,
     qcng_fallback: bool = True,
     propagate_wfn: bool = False,
     **kwargs,
-) -> OutputBase:
+) -> ProgramOutput:
     """Use the given program to compute on the given input.
 
     See BaseAdapter.compute for more details.
     """
     adapter = get_adapter(program, inp_obj, qcng_fallback)
     return adapter.compute(
         inp_obj,
@@ -55,15 +62,15 @@
     *,
     calctype: Union[str, CalcType],
     model: Union[Dict[str, str], Model],
     keywords: Optional[Dict[str, Any]] = None,
     files: Optional[Union[Dict[str, Union[str, bytes]], Files]] = None,
     extras: Optional[Dict[str, Any]] = None,
     **kwargs,
-) -> OutputBase:
+) -> ProgramOutput:
     """Compute function that accepts independent argument for a ProgramInput.
 
     Args:
         program: The program to run.
         molecule: The molecule to use.
         calctype: The type of calculation to run.
         model: The model to use for the calculation.
@@ -73,25 +80,22 @@
         extras: Extra arguments to pass to the adapter.
         **kwargs: Extra arguments to pass to the compute function.
 
     Returns:
         The output of the computation.
 
     Raises:
-        AdapterNotFoundError: If no adapter is found for the given program.
-        AdapterInputError: If the adapter raises an exception when generating input
-            files.
-        QCEngineError: If the adapter raises an exception when running the program.
+        See compute function for details.
     """
     if isinstance(files, Files):  # Check in case Files object is passed instead of dict
         files = files.files
 
     inp_obj = ProgramInput(
-        calctype=calctype,
+        calctype=calctype,  # type: ignore
         molecule=molecule,
-        model=model,
+        model=model,  # type: ignore
         keywords=keywords or {},
         files=files or {},
         extras=extras or {},
     )
 
     return compute(program, inp_obj, **kwargs)
```

### Comparing `qcop-0.5.5/qcop/utils.py` & `qcop-0.6.0/qcop/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import shutil
 from functools import lru_cache
 
-from qcio.models import FileInput, InputBase
+from qcio import FileInput, Inputs
 
 from .adapters import BaseAdapter, FileAdapter, registry
 from .exceptions import AdapterNotFoundError, ProgramNotFoundError
 
 
 @lru_cache  # Improves perf of tests when repeatedly called
 def prog_available(program: str) -> bool:
@@ -69,30 +69,31 @@
     # Raised by QCEngine if program not installed on system
     # IndexError insulates from .pyenv/shims not covered in qcng
     except (ResourceError, IndexError):
         raise ProgramNotFoundError(program)
 
 
 def get_adapter(
-    program: str, inp_obj: InputBase, qcng_fallback: bool = False
+    program: str, inp_obj: Inputs, qcng_fallback: bool = False
 ) -> BaseAdapter:
     """Get the adapter for a program.
 
     Args:
         program: The program to get the adapter for.
         inp_obj: The input object for the calculation.
         qcng_fallback: Fallback to use QCEngine if the adapter is not in qcop.
 
     Returns:
         The adapter for the program.
 
     Raises:
         AdapterNotFoundError: If the adapter is not found.
     """
-    if isinstance(inp_obj, FileInput):
+
+    if type(inp_obj) is FileInput:
         return FileAdapter(program)
     try:
         return registry[program]()
     except KeyError:
         if qcng_fallback:
             # Raises AdapterNotFoundError or ProgramNotFoundError
             check_qcng_support(program)
```

### Comparing `qcop-0.5.5/PKG-INFO` & `qcop-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: qcop
-Version: 0.5.5
+Version: 0.6.0
 Summary: A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more.
+Home-page: https://github.com/coltonbh/qcop
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: geometric
 Provides-Extra: qcengine
-Requires-Dist: geometric (>=1.0.1) ; extra == "geometric"
-Requires-Dist: qcelemental (>=0.26.0) ; extra == "qcengine"
-Requires-Dist: qcengine (>=0.27.0) ; extra == "qcengine"
-Requires-Dist: qcio (>=0.8.2,<0.9.0)
+Requires-Dist: geometric (>=1.0.1,<2.0.0) ; extra == "geometric"
+Requires-Dist: qcelemental (>=0.26.0,<0.27.0) ; extra == "qcengine"
+Requires-Dist: qcengine (>=0.27.0,<0.28.0) ; extra == "qcengine"
+Requires-Dist: qcio (>=0.9.0,<0.10.0)
 Requires-Dist: qcparse (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # Quantum Chemistry Operate
 
 A package for operating Quantum Chemistry programs using [qcio](https://github.com/coltonbh/qcio) standardized data structures. Compatible with `TeraChem`, `psi4`, `QChem`, `NWChem`, `ORCA`, `Molpro`, `geomeTRIC` and many more.
 
@@ -66,41 +67,41 @@
 prog_input = ProgramInput(
     molecule=h2o,
     calctype="energy",
     model={"method": "hf", "basis": "sto-3g"},
     keywords={"purify": "no", "restricted": False},
 )
 
-# Run the calculation; will return SinglePointOutput or raise an exception
+# Run the calculation; will return ProgramOutput or raise an exception
 try:
-    output = compute("terachem", prog_input, collect_files=True)
+    po = compute("terachem", prog_input, collect_files=True)
 except ExternalProgramError as e:
     # External QQ program failed in some way
-    prog_failure = e.program_failure
-    prog_failure.input_data # Input data used by the QC program
-    prog_failure.success # Will be False
-    prog_failure.results # Any half-computed results before the failure
-    prog_failure.traceback # Stack trace from the calculation
-    prog_failure.ptraceback # Shortcut to print out the traceback in human readable format
-    prog_failure.stdout # Stdout log from the calculation
+    po = e.program_output
+    po.input_data # Input data used by the QC program
+    po.success # Will be False
+    po.results # Any half-computed results before the failure
+    po.traceback # Stack trace from the calculation
+    po.ptraceback # Shortcut to print out the traceback in human readable format
+    po.stdout # Stdout log from the calculation
     raise e
 else:
     # Calculation succeeded
-    output.input_data # Input data used by the QC program
-    output.success # Will be True
-    output.results # All structured results from the calculation
-    output.stdout # Stdout log from the calculation
-    output.pstdout # Shortcut to print out the stdout in human readable format
-    output.files # Any files returned by the calculation
-    output.provenance # Provenance information about the calculation
-    output.extras # Any extra information not in the schema
+    po.input_data # Input data used by the QC program
+    po.success # Will be True
+    po.results # All structured results from the calculation
+    po.stdout # Stdout log from the calculation
+    po.pstdout # Shortcut to print out the stdout in human readable format
+    po.files # Any files returned by the calculation
+    po.provenance # Provenance information about the calculation
+    po.extras # Any extra information not in the schema
 
 ```
 
-One may also call `compute(..., raise_exc=False)` to return a `ProgramFailure` object rather than raising an exception when a calculation fails. This may allow easier handling of failures in some cases.
+One may also call `compute(..., raise_exc=False)` to return a `ProgramOutput` object rather than raising an exception when a calculation fails. This may allow easier handling of failures in some cases.
 
 ```python
 from qcio import Molecule, ProgramInput
 from qcop import compute
 from qcop.exceptions import ExternalProgramError
 # Create the molecule
 h2o = Molecule.open("h2o.xyz")
@@ -109,35 +110,35 @@
 prog_input = ProgramInput(
     molecule=h2o,
     calctype="energy",
     model={"method": "hf", "basis": "sto-3g"},
     keywords={"purify": "no", "restricted": False},
 )
 
-# Run the calculation; will return either a SinglePointOutput or a ProgramFailure
-output = compute("terachem", prog_input, collect_files=True, raise_exc=False)
-if not output.success:
+# Run the calculation; will return a ProgramOutput objects
+po = compute("terachem", prog_input, collect_files=True, raise_exc=False)
+if not po.success:
     # External QQ program failed in some way
-    output.input_data # Input data used by the QC program
-    output.success # Will be False
-    output.results # Any half-computed results before the failure
-    output.traceback # Stack trace from the calculation
-    output.ptraceback # Shortcut to print out the traceback in human readable format
-    output.stdout # Stdout log from the calculation
+    po.input_data # Input data used by the QC program
+    po.success # Will be False
+    po.results # Any half-computed results before the failure
+    po.traceback # Stack trace from the calculation
+    po.ptraceback # Shortcut to print out the traceback in human readable format
+    po.stdout # Stdout log from the calculation
 
 else:
     # Calculation succeeded
-    output.input_data # Input data used by the QC program
-    output.success # Will be True
-    output.results # All structured results from the calculation
-    output.stdout # Stdout log from the calculation
-    output.pstdout # Shortcut to print out the stdout in human readable format
-    output.files # Any files returned by the calculation
-    output.provenance # Provenance information about the calculation
-    output.extras # Any extra information not in the schema
+    po.input_data # Input data used by the QC program
+    po.success # Will be True
+    po.results # All structured results from the calculation
+    po.stdout # Stdout log from the calculation
+    po.pstdout # Shortcut to print out the stdout in human readable format
+    po.files # Any files returned by the calculation
+    po.provenance # Provenance information about the calculation
+    po.extras # Any extra information not in the schema
 
 ```
 
 Alternatively, the `compute_args` function can be used to run a calculation with the input data structures passed in as arguments rather than as a single `ProgramInput` object.
 
 ```python
 from qcio import Molecule
```

