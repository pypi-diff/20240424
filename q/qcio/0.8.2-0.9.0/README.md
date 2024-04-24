# Comparing `tmp/qcio-0.8.2.tar.gz` & `tmp/qcio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.8.2.tar", max compression
+gzip compressed data, was "qcio-0.9.0.tar", max compression
```

## Comparing `qcio-0.8.2.tar` & `qcio-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1079 2024-04-10 00:42:54.581444 qcio-0.8.2/LICENSE
--rw-r--r--   0        0        0     7503 2024-04-10 00:42:54.581444 qcio-0.8.2/README.md
--rw-r--r--   0        0        0     1226 2024-04-10 00:42:54.581444 qcio-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      614 2024-04-10 00:42:54.581444 qcio-0.8.2/qcio/__init__.py
--rw-r--r--   0        0        0     1753 2024-04-10 00:42:54.581444 qcio-0.8.2/qcio/constants.py
--rw-r--r--   0        0        0      748 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/helper_types.py
--rw-r--r--   0        0        0      235 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/__init__.py
--rw-r--r--   0        0        0     8752 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/base_models.py
--rw-r--r--   0        0        0     3034 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/inputs.py
--rw-r--r--   0        0        0     2800 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     9122 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/molecule.py
--rw-r--r--   0        0        0    10301 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/outputs.py
--rw-r--r--   0        0        0     1936 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/models/outputs_base.py
--rw-r--r--   0        0        0        0 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/py.typed
--rw-r--r--   0        0        0     4892 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/qcel.py
--rw-r--r--   0        0        0     1142 2024-04-10 00:42:54.585444 qcio-0.8.2/qcio/utils.py
--rw-r--r--   0        0        0     8308 1970-01-01 00:00:00.000000 qcio-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-24 01:05:13.352785 qcio-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7503 2024-04-24 01:05:13.352785 qcio-0.9.0/README.md
+-rw-r--r--   0        0        0     1357 2024-04-24 01:05:13.352785 qcio-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      594 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/__init__.py
+-rw-r--r--   0        0        0     1916 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/constants.py
+-rw-r--r--   0        0        0      464 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/helper_types.py
+-rw-r--r--   0        0        0      152 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/__init__.py
+-rw-r--r--   0        0        0    10129 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/base_models.py
+-rw-r--r--   0        0        0     4519 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/inputs.py
+-rw-r--r--   0        0        0     9378 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/molecule.py
+-rw-r--r--   0        0        0    12716 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1569 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/models/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/py.typed
+-rw-r--r--   0        0        0     3026 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/qcel.py
+-rw-r--r--   0        0        0      602 2024-04-24 01:05:13.352785 qcio-0.9.0/qcio/utils.py
+-rw-r--r--   0        0        0     8380 1970-01-01 00:00:00.000000 qcio-0.9.0/PKG-INFO
```

### Comparing `qcio-0.8.2/LICENSE` & `qcio-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.8.2/README.md` & `qcio-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.8.2/pyproject.toml` & `qcio-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.8.2"
+version = "0.9.0"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/coltonbh/qcio"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = ">=2.0.0"
-numpy = ">=1.20"
+pydantic = "^2.0.0,!=2.0.1,!=2.1.0"
+numpy = "^1.20"
 toml = "^0.10.2"
 pyyaml = "^6.0"
 typing-extensions = "^4.7.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.0.0"
 mypy = "^1.1.1"
@@ -45,14 +46,18 @@
 isort = { known-first-party = ["qcio", "tests"] }
 target-version = "py38"
 
 [tool.coverage.run]
 branch = true
 omit = ["*/tests/*", "*__init__.py"]
 
+[tool.pytest.ini_options]
+filterwarnings = ["ignore::FutureWarning"]
+
+
 [tool.mypy]
 plugins = "pydantic.mypy"
 ignore_missing_imports = true
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
```

### Comparing `qcio-0.8.2/qcio/__init__.py` & `qcio-0.9.0/qcio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 from .models import *  # noqa: F403
 from .utils import json_dumps
 
 __version__ = metadata.version(__name__)
 
 __all__ = [  # noqa: F405
     # Core Models
+    "CalcType",
+    "Model",
+    "Provenance",
     "Molecule",
     "Files",
-    "OutputBase",
-    "Files",
     "FileInput",
-    "FileOutput",
-    "Provenance",
-    "Model",
-    "CalcType",
     "ProgramInput",
+    "ProgramOutput",
+    "DualProgramInput",
+    "NoResults",
     "SinglePointResults",
+    "OptimizationResults",
     "SinglePointOutput",
     "Wavefunction",
-    "ProgramFailure",
     "ProgramArgs",
-    "QCProgramArgs",
-    "SubProgramArgs",
-    # Core Utils
+    "ProgramArgsSub",
     "json_dumps",
 ]
```

### Comparing `qcio-0.8.2/qcio/models/base_models.py` & `qcio-0.9.0/qcio/models/base_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """The Base model from which all QCIO Model objects inherit."""
 
 import json
 from abc import ABC
 from base64 import b64decode, b64encode
+from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import numpy as np
 import toml
 import yaml
 from pydantic import BaseModel, field_serializer, field_validator
 from typing_extensions import Self
 
 from ..helper_types import StrOrPath
+from .utils import deprecated_function
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic.typing import ReprArgs
 
 
-__all__ = ["Files", "Provenance"]
+__all__ = ["Files", "Provenance", "Model", "CalcType"]
 
 
 class QCIOModelBase(BaseModel, ABC):
     """Base Model for all QCIO objects.
 
     Attributes:
         version: The version of the schema.
@@ -151,15 +153,15 @@
                 f"base64:{b64encode(data).decode('utf-8')}"
                 if isinstance(data, bytes)
                 else data
             )
             for filename, data in files.items()
         }
 
-    def open_file(
+    def add_file(
         self, filepath: Union[Path, str], relative_dir: Optional[Path] = None
     ) -> None:
         """Create a File object from a file on disk.
 
         Args:
             filepath: The path to the file.
             relative_dir: The directory to make the file relative to. Helpful when
@@ -176,15 +178,21 @@
         if relative_dir:
             filename = str(filepath.relative_to(relative_dir))
         else:
             filename = filepath.name
 
         self.files[filename] = data
 
-    def open_files(
+    @deprecated_function("add_file")
+    def open_file(
+        self, filepath: Union[Path, str], relative_dir: Optional[Path] = None
+    ) -> None:
+        self.add_file(filepath, relative_dir)
+
+    def add_files(
         self,
         directory: StrOrPath,
         recursive: bool = False,
         exclude: Optional[List[str]] = None,
     ) -> None:
         """Add all files in a directory to the object.
 
@@ -198,15 +206,24 @@
             exclude = []
         if recursive:
             files = directory.rglob("*")
         else:
             files = directory.glob("*")
         for filepath in files:
             if filepath.is_file() and filepath.name not in exclude:
-                self.open_file(filepath, directory)
+                self.add_file(filepath, directory)
+
+    @deprecated_function("add_files")
+    def open_files(
+        self,
+        directory: StrOrPath,
+        recursive: bool = False,
+        exclude: Optional[List[str]] = None,
+    ) -> None:
+        self.add_files(directory, recursive, exclude)
 
     def save_files(self, directory: StrOrPath = Path(".")) -> None:
         """Write all files to the specified directory"""
         directory = Path(directory)
         directory.mkdir(exist_ok=True)
         for filename, data in self.files.items():
             mode = "w" if isinstance(data, str) else "wb"
@@ -253,7 +270,36 @@
     program: str
     program_version: Optional[str] = None
     scratch_dir: Optional[StrOrPath] = None
     wall_time: Optional[float] = None
     hostname: Optional[str] = None
     hostcpus: Optional[int] = None
     hostmem: Optional[int] = None
+
+
+class CalcType(str, Enum):
+    """The Calculation type."""
+
+    energy = "energy"
+    gradient = "gradient"
+    hessian = "hessian"
+    optimization = "optimization"
+    transition_state = "transition_state"
+
+    def __repr__(self) -> str:
+        """Custom repr for CalcType"""
+        return f"'{self.name}'"  # pragma: no cover
+
+
+class Model(QCIOModelBase):
+    """The model for the quantum chemistry calculation.
+
+    Attributes:
+        method: The name of the method to be used in the calculation. Named according to
+            the convention of the program being called. If an MM calculation then the
+            name of the force field.
+        basis: The name of the basis set to be used in the calculation. Named according
+            to the convention of the program being called.
+    """
+
+    method: str
+    basis: Optional[str] = None
```

### Comparing `qcio-0.8.2/qcio/models/molecule.py` & `qcio-0.9.0/qcio/models/molecule.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from pydantic import field_serializer, field_validator
 from typing_extensions import Self
 
-from qcio.constants import BOHR_TO_ANGSTROM
-from qcio.helper_types import ArrayLike2D
+from qcio.constants import _ELEMENTS, BOHR_TO_ANGSTROM
+from qcio.helper_types import SerializableNDArray
 
 from .base_models import QCIOModelBase
 
 if TYPE_CHECKING:
     from pydantic.typing import ReprArgs
 
 __all__ = ["Molecule", "Identifiers"]
@@ -83,15 +83,15 @@
             E.g., [(0, 1, 1.0), (1, 2, 2.0)] indicates a single bond between atoms 0
             and 1 and a double bond between atoms 1 and 2.
         masses: Explicit masses for the atoms. If not set, default isotopic masses are
             used.
     """
 
     symbols: List[str]
-    geometry: ArrayLike2D
+    geometry: SerializableNDArray  # Coerced to 2D array
     charge: int = 0
     multiplicity: int = 1
     identifiers: Identifiers = Identifiers()
     connectivity: List[Tuple[int, int, float]] = []
     # masses: List[float] = []
 
     def __repr_args__(self) -> "ReprArgs":
@@ -121,14 +121,19 @@
 
         Cannot have homogeneous data types in .toml files so must cast all values to
         floats.
         """
         return [[float(val) for val in bond] for bond in connectivity]
 
     @property
+    def atomic_numbers(self) -> List[int]:
+        """Return the atomic numbers of the atoms in the molecule."""
+        return [_ELEMENTS[symbol] for symbol in self.symbols]
+
+    @property
     def formula(self) -> str:
         """Return the molecular formula of the molecule using the Hill System.
         # noqa: E501
         https://chemistry.stackexchange.com/questions/1239/order-of-elements-in-a-formula
         """
         counter_elements = Counter(self.symbols)
 
@@ -241,8 +246,8 @@
         symbols = []
         geometry = []
         for line in lines[2 : 2 + num_atoms]:
             split_line = line.split()
             symbols.append(split_line[0])
             geometry.append([float(val) / BOHR_TO_ANGSTROM for val in split_line[1:]])
 
-        return cls(symbols=symbols, geometry=geometry, **qcio_kwargs)
+        return cls(symbols=symbols, geometry=geometry, **qcio_kwargs)  # type: ignore
```

### Comparing `qcio-0.8.2/qcio/models/outputs.py` & `qcio-0.9.0/qcio/models/outputs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,87 @@
 """End user output and results objects from a calculation."""
 
+from __future__ import annotations
+
+import sys
+import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Literal, Optional, Union
+from typing import TYPE_CHECKING, Generic, List, Literal, Optional, TypeVar, Union
 
 import numpy as np
-from pydantic import field_validator
+from pydantic import field_validator, model_validator
+from typing_extensions import Self
 
-from qcio.helper_types import ArrayLike2D, ArrayLike3D
+from qcio.helper_types import SerializableNDArray
 
-from .base_models import QCIOModelBase
-from .inputs import DualProgramInput, FileInput, ProgramInput
+from .base_models import CalcType, Files, Provenance, QCIOModelBase
+from .inputs import DualProgramInput, FileInput, Inputs, InputType, ProgramInput
 from .molecule import Molecule
-from .outputs_base import OutputBase, ResultsBase, SuccessfulOutputBase
+from .utils import deprecated_class
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic.typing import ReprArgs
 
 
 __all__ = [
-    "FileOutput",
-    "SinglePointOutput",
-    "OptimizationOutput",
-    "ProgramFailure",
     "SinglePointResults",
     "Wavefunction",
     "OptimizationResults",
+    "ProgramOutput",
+    "ResultsType",
+    "Results",
+    "NoResults",
+    "SinglePointOutput",
+    "ProgramFailure",
+    "OptimizationOutput",
 ]
 
 
-class FileOutput(SuccessfulOutputBase):
-    """Generic output class for pure file based I/O.
-
-    Attributes:
-        input_data: The FileInput object used for the computation.
-        files: A dict mapping filename to str or bytes data.
-        success: A boolean indicator that the operation succeeded (always True)
-        stdout: The primary logging output of the program. Contains a union of stdout
-            and stderr.
-        provenance: An object containing the provenance information for the results.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
-
-    """
-
-    input_data: FileInput
-
-
 class Wavefunction(QCIOModelBase):
     """The wavefunction for a single point calculation.
 
     Attributes:
         scf_eigenvalues_a: The SCF alpha-spin orbital eigenvalues.
         scf_eigenvalues_b: The SCF beta-spin orbital eigenvalues.
         scf_occupations_a: The SCF alpha-spin orbital occupations.
         scf_occupations_b: The SCF beta-spin orbital occupations.
     """
 
-    scf_eigenvalues_a: Optional[ArrayLike2D] = None
-    scf_eigenvalues_b: Optional[ArrayLike2D] = None
-    scf_occupations_a: Optional[ArrayLike2D] = None
-    scf_occupations_b: Optional[ArrayLike2D] = None
+    scf_eigenvalues_a: Optional[SerializableNDArray] = None
+    scf_eigenvalues_b: Optional[SerializableNDArray] = None
+    scf_occupations_a: Optional[SerializableNDArray] = None
+    scf_occupations_b: Optional[SerializableNDArray] = None
 
     @field_validator(
         "scf_eigenvalues_a",
         "scf_eigenvalues_b",
         "scf_occupations_a",
         "scf_occupations_b",
     )
     @classmethod
     def to_numpy(cls, val, _info) -> Optional[np.ndarray]:
         return np.asarray(val) if val is not None else None
 
 
-class SinglePointResults(ResultsBase):
+class NoResults(QCIOModelBase):
+    """Am empty results object for when no results are present.
+
+    This is used to avoid having to use Optional[Results] in ProgramOutput which gives
+    greater type safety by ensuring that results are always present. Also, this object
+    functions as an empty container so that end user code doesn't have to check if
+    results are None before accessing them--akin to returning an empty list instead of
+    None for a function.
+    """
+
+    def __bool__(self):
+        """Behave like an empty container."""
+        return False
+
+
+class SinglePointResults(QCIOModelBase):
     """The computed results from a single point calculation.
 
     Attributes:
         calcinfo_natoms: The number of atoms as computed by the program.
         calcinfo_nalpha: The number of alpha electrons as computed by the program.
         calcinfo_nbeta: The number of beta electrons as computed by the program.
         calcinfo_nbasis: The number of basis functions in the calculation.
@@ -107,116 +112,104 @@
     calcinfo_nbasis: Optional[int] = None
     calcinfo_nmo: Optional[int] = None
     calcinfo_nalpha: Optional[int] = None
     calcinfo_nbeta: Optional[int] = None
 
     # Core properties
     energy: Optional[float] = None
-    gradient: Optional[ArrayLike2D] = None
-    hessian: Optional[ArrayLike2D] = None
+    gradient: Optional[SerializableNDArray] = None  # Coerced to 2D array
+    hessian: Optional[SerializableNDArray] = None  # Coerced to 2D array
     nuclear_repulsion_energy: Optional[float] = None
 
     # Wavefunction data
     wavefunction: Optional[Wavefunction] = None
 
     # Frequency data
     freqs_wavenumber: List[float] = []
-    normal_modes_cartesian: Optional[ArrayLike3D] = None
+    normal_modes_cartesian: Optional[SerializableNDArray] = None  # Coerced to 3D array
     gibbs_free_energy: Optional[float] = None
 
     # SCF results
     scf_dipole_moment: Optional[List[float]] = None
 
     @field_validator("normal_modes_cartesian")
     @classmethod
-    def validate_normal_modes_cartesian_shape(cls, v: ArrayLike3D):
+    def validate_normal_modes_cartesian_shape(cls, v: SerializableNDArray):
         if v is not None:
             # Assume array has length of the number of normal modes
             n_normal_modes = len(v)
             return np.asarray(v).reshape(n_normal_modes, -1, 3)
 
     @field_validator("gradient")
     @classmethod
-    def validate_gradient_shape(cls, v: ArrayLike2D):
+    def validate_gradient_shape(cls, v: SerializableNDArray):
         """Validate gradient is n x 3"""
         if v is not None:
             return np.asarray(v).reshape(-1, 3)
 
     @field_validator("hessian")
     @classmethod
-    def validate_hessian_shape(cls, v: ArrayLike2D):
+    def validate_hessian_shape(cls, v: SerializableNDArray):
         """Validate hessian is square"""
         if v is not None:
             v = np.asarray(v)
             n = int(np.sqrt(v.size))
             return v.reshape((n, n))
 
-
-class SinglePointOutput(SuccessfulOutputBase):
-    """Output from a successful single point calculation.
-
-    Attributes:
-        input_data: The SinglePointInput object for the computation.
-        success: Always True for a successful computation.
-        results: The results computed by the program.
-        files: A dict mapping filename to str or bytes data.
-        stdout: The primary logging output of the program. Contains a union of stdout
-            and stderr.
-        provenance: An object containing the provenance information for the results.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
-    """
-
-    input_data: ProgramInput
-    results: SinglePointResults
-
-    @property
-    def return_result(self) -> Union[float, ArrayLike2D]:
-        """Return the result of the calculation.
-
-        Returns:
-            The explicitly requested result of the calculation, i.e., the energy,
-                gradient, or hessian.
-        """
-        return getattr(self.results, self.input_data.calctype.value)
+    def return_result(self, calctype: CalcType) -> Union[float, SerializableNDArray]:
+        """Return the primary result of the calculation."""
+        return getattr(self, calctype.value)
 
 
-class OptimizationResults(ResultsBase):
+class OptimizationResults(QCIOModelBase):
     """Computed properties for an optimization.
 
     Attributes:
         energies: The energies for each step of the optimization.
         molecules: The Molecule objects for each step of the optimization.
-        final_molecule: The final, optimized molecule.
+        final_molecule: The final, optimized Molecule.
         trajectory: The SinglePointOutput objects for each step of the optimization.
     """
 
-    trajectory: List[SinglePointOutput] = []
+    trajectory: List[
+        Union[
+            ProgramOutput[ProgramInput, SinglePointResults],
+            ProgramOutput[ProgramInput, NoResults],
+        ]
+    ] = []
 
     @property
     def final_molecule(self) -> Optional[Molecule]:
         """The final molecule in the optimization."""
         try:
             return self.trajectory[-1].input_data.molecule
         except IndexError:  # Empty trajectory
             return None
 
     @property
     def energies(self) -> List[float]:
         """The energies for each step of the optimization."""
         # or 0.0 covers null case for mypy
-        return [output.results.energy or 0.0 for output in self.trajectory]
+        return [
+            output.results.energy or 0.0
+            for output in self.trajectory
+            if not isinstance(output.results, NoResults)
+        ]
 
     @property
     def molecules(self) -> List[Molecule]:
         """The Molecule objects for each step of the optimization."""
         return [output.input_data.molecule for output in self.trajectory]
 
+    def return_result(self, calctype: CalcType) -> Optional[Molecule]:
+        """Return the primary result of the calculation."""
+        return self.final_molecule
+
     def __repr_args__(self):
-        """Custom repr to avoid printing the entire collection objects."""
+        """Custom repr to avoid printing the entire collection of objects."""
         return [
             ("final_molecule", f"{self.final_molecule}"),
             ("trajectory", "[...]"),
             ("energies", "[...]"),
             ("molecules", "[...]"),
         ]
 
@@ -238,55 +231,120 @@
         Notes:
             If the filepath has a .xyz extension, the trajectory will be saved to an XYZ
             file.
         """
         filepath = Path(filepath)
         if filepath.suffix == ".xyz":
             text = "".join(
-                sp_output.input_data.molecule.to_xyz() for sp_output in self.trajectory
+                prog_output.input_data.molecule.to_xyz()
+                for prog_output in self.trajectory
             )
             filepath.write_text(text)
             return
         super().save(filepath, exclude_none, indent, **kwargs)
 
 
-class OptimizationOutput(SuccessfulOutputBase):
-    """Output from a successful optimization.
+Results = Union[NoResults, SinglePointResults, OptimizationResults]
+ResultsType = TypeVar("ResultsType", bound=Results)
 
-    Attributes:
-        input_data: The OptimizationInput object for the computation.
-        results: The results computed by the program.
-    """
 
-    input_data: Union[DualProgramInput, ProgramInput]
-    results: OptimizationResults
+class ProgramOutput(Files, Generic[InputType, ResultsType]):
+    input_data: InputType
+    provenance: Provenance
+    success: Literal[True, False]
+    results: ResultsType = NoResults()  # type: ignore
+    stdout: Optional[str] = None
+    traceback: Optional[str] = None
 
+    def model_post_init(self, __context) -> None:
+        """
+        Parameterize the class (if not set explicitly) and register the class so pickle
+        can find it.
+        """
+        # Check if the current class is still generic, do not override if explicitly set
+        if self.__class__ is ProgramOutput:
+            input_type = type(self.input_data)
+            # TODO: Make sure this is valid for results == None
+            results_type = type(self.results)
+            self.__class__ = ProgramOutput[input_type, results_type]  # type: ignore # noqa 501
+
+        # Add class to module so that pickle can find it
+        if not sys.modules[self.__class__.__module__].__dict__.get(
+            self.__class__.__name__
+        ):
+            setattr(
+                sys.modules[self.__class__.__module__],
+                self.__class__.__name__,
+                self.__class__,
+            )
 
-class ProgramFailure(OutputBase):
-    """A object containing details about a failed calculation.
+    @model_validator(mode="after")
+    def ensure_traceback_on_failure(self) -> Self:
+        if self.success is False and self.traceback is None:
+            raise ValueError("A traceback must be provided for failed calculations.")
+        return self
+
+    @model_validator(mode="after")
+    def ensure_results_on_success(self) -> Self:
+        if self.success is True and type(self.input_data) is not FileInput:
+            # Ensure results are provided for successful calculations
+            assert not isinstance(
+                self.results, NoResults
+            ), "Results must be provided for successful, non FileInput calculations."
+
+            if type(self.results) is SinglePointResults:
+                # Ensure the primary calctype result is present
+                calctype_val = self.input_data.calctype.value  # type: ignore
+                assert (
+                    getattr(self.results, calctype_val) is not None
+                ), f"Missing the primary result: {calctype_val}."
 
-    Attributes:
-        input_data: The input object for the computation.
-        success: Always False for a Failed output.
-        traceback: String representation of the traceback of the exception that caused
-            the failure.
-        results: Any compted data that was able to be extracted before program failed.
-        stdout: The primary logging output of the program. Contains a union of stdout
-            and stderr.
-        provenance: An object containing the provenance information for the output.
-    """
+        return self
 
-    input_data: Union[DualProgramInput, ProgramInput, FileInput]
-    success: Literal[False] = False
-    traceback: Optional[str] = None
+    @property
+    def pstdout(self) -> None:
+        """Print the stdout text"""
+        print(self.stdout)
 
     @property
     def ptraceback(self) -> None:
         """Print the traceback text"""
         print(self.traceback)
 
     def __repr_args__(self) -> "ReprArgs":
-        """Exclude traceback from the repr"""
+        """Exclude stdout and traceback from the repr"""
         return [
-            (key, value if key != "traceback" else "<...>")
+            (key, value if key not in {"stdout", "traceback"} else "<...>")
             for key, value in super().__repr_args__()
         ]
+
+    @property
+    def return_result(self) -> Union[float, SerializableNDArray, Optional[Molecule]]:
+        """Return the primary result of the calculation."""
+        warnings.warn(
+            ".return_result is being depreciated and will be removed in a future. "
+            "Please access results directly at .results instead.",
+            category=FutureWarning,
+            stacklevel=2,
+        )
+        # For mypy
+        assert self.results is not None, "No results exist on this ProgramOutput"
+        assert type(self.input_data) is not FileInput, "FileInputs have no results."
+        return self.results.return_result(self.input_data.calctype)  # type: ignore
+
+
+# For compatibility with old API
+@deprecated_class("ProgramOutput[StructuredInputs, OptimizationResults]")
+class OptimizationOutput(ProgramOutput[DualProgramInput, OptimizationResults]):
+    success: Literal[True] = True
+    traceback: Optional[str] = None
+
+
+@deprecated_class("ProgramOutput[ProgramInput, SinglePointResults]")
+class SinglePointOutput(ProgramOutput[ProgramInput, SinglePointResults]):
+    success: Literal[True] = True
+    traceback: Optional[str] = None
+
+
+@deprecated_class("ProgramOutput[StructuredInputs, Results]")
+class ProgramFailure(ProgramOutput[Inputs, Results]):
+    success: Literal[False] = False
```

### Comparing `qcio-0.8.2/PKG-INFO` & `qcio-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.8.2
+Version: 0.9.0
 Summary: Beautiful and user friendly data structures for quantum chemistry.
+Home-page: https://github.com/coltonbh/qcio
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
-Requires-Dist: numpy (>=1.20)
-Requires-Dist: pydantic (>=2.0.0)
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0,!=2.0.1,!=2.1.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Quantum Chemistry I/O
```

