# Comparing `tmp/glytrait-0.1.1.tar.gz` & `tmp/glytrait-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.1.tar", max compression
+gzip compressed data, was "glytrait-0.1.2.tar", max compression
```

## Comparing `glytrait-0.1.1.tar` & `glytrait-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.1/LICENSE
--rw-r--r--   0        0        0    13933 2024-04-20 04:25:00.882511 glytrait-0.1.1/README.md
--rw-r--r--   0        0        0     1263 2024-04-20 04:23:15.911626 glytrait-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-20 04:08:28.908891 glytrait-0.1.1/src/glytrait/__init__.py
--rw-r--r--   0        0        0    10712 2024-04-20 03:37:48.972694 glytrait-0.1.1/src/glytrait/api.py
--rw-r--r--   0        0        0     4748 2024-02-10 13:59:57.519954 glytrait-0.1.1/src/glytrait/cli.py
--rw-r--r--   0        0        0     2683 2024-04-14 11:59:08.462417 glytrait-0.1.1/src/glytrait/data_export.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.1/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.1/src/glytrait/exception.py
--rw-r--r--   0        0        0    27106 2024-04-20 03:32:01.149878 glytrait-0.1.1/src/glytrait/formula.py
--rw-r--r--   0        0        0    13768 2024-02-10 13:59:57.574326 glytrait-0.1.1/src/glytrait/glycan.py
--rw-r--r--   0        0        0    14569 2024-03-08 09:00:51.155221 glytrait-0.1.1/src/glytrait/load_data.py
--rw-r--r--   0        0        0    18283 2024-04-14 11:59:08.464441 glytrait-0.1.1/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.1/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     4621 2024-02-10 13:59:57.532082 glytrait-0.1.1/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     8081 2024-04-14 11:59:08.465266 glytrait-0.1.1/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    55082 2024-04-14 11:59:08.465614 glytrait-0.1.1/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     3743 2024-04-20 03:31:49.134440 glytrait-0.1.1/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.1/src/glytrait/trait.py
--rw-r--r--   0        0        0    14358 1970-01-01 00:00:00.000000 glytrait-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.2/LICENSE
+-rw-r--r--   0        0        0    13926 2024-04-22 06:43:14.845523 glytrait-0.1.2/README.md
+-rw-r--r--   0        0        0     1263 2024-04-24 15:26:12.292440 glytrait-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-24 15:40:24.623283 glytrait-0.1.2/src/glytrait/__init__.py
+-rw-r--r--   0        0        0    16589 2024-04-24 15:40:09.461712 glytrait-0.1.2/src/glytrait/api.py
+-rw-r--r--   0        0        0     8032 2024-04-24 15:43:00.391548 glytrait-0.1.2/src/glytrait/cli.py
+-rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.2/src/glytrait/data_export.py
+-rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.2/src/glytrait/data_input.py
+-rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.2/src/glytrait/data_type.py
+-rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.2/src/glytrait/exception.py
+-rw-r--r--   0        0        0    26284 2024-04-24 12:35:20.622266 glytrait-0.1.2/src/glytrait/formula.py
+-rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.2/src/glytrait/glycan.py
+-rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.2/src/glytrait/meta_property.py
+-rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.2/src/glytrait/post_filtering.py
+-rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.2/src/glytrait/preprocessing.py
+-rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.2/src/glytrait/resources/comp_formula.txt
+-rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.2/src/glytrait/resources/struc_formula.txt
+-rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.2/src/glytrait/stat.py
+-rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.2/src/glytrait/trait.py
+-rw-r--r--   0        0        0    14351 1970-01-01 00:00:00.000000 glytrait-0.1.2/PKG-INFO
```

### Comparing `glytrait-0.1.1/LICENSE` & `glytrait-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.1/README.md` & `glytrait-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/fubin1999/glytrait/badge.svg?branch=main)](https://coveralls.io/github/fubin1999/glytrait?branch=main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/e3e6a19dccb749f786264247738fa585)](https://app.codacy.com/gh/fubin1999/glytrait/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 ## Overview
 
 *Q: What is GlyTrait?*
 
-*A: GlyTrait is a tool for calculating derived traits for N-glycomic data.*
+*A: GlyTrait is a tool to calculate derived traits for N-glycomic data.*
 
 *Q: Sounds cool! So..., what are derived traits again?*
 
 *A: Well, derived traits are artificial variables that summarize certain aspects of 
 the glycome. 
 For example, the proportion of core-fucosylated glycans, 
 the average number of sialic acids per glycan, 
@@ -27,31 +27,30 @@
 *Q: So, GlyTrait does the dirty work for me, 
 saving my time and energy for more interesting analysis?*
 
 *A: You bet!*
 
 ## Contents
 
+- [Web app](#web-app)
 - [Installation](#installation)
-    - [Requirement](#requirement)
-    - [Using pipx (recommended)](#using-pipx-recommended)
 - [Usage](#usage)
     - [Quick start](#quick-start)
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
     - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
 - [License](#license)
 
 ## Web app
 
-> Let there be no command line apps!
+> Let there be no code!
 > 
 > -- my colleagues
 
 A web app version of GlyTrait is on its way here...
 Ready to say goodbye to the command line?
 
 ## Installation
@@ -104,18 +103,19 @@
 ## Usage
 
 ### Quick start
 
 1. Download the [example files](https://github.com/fubin1999/glytrait/tree/main/example_data)
 to a new directory: `glytrait_example`.
 
-2. Open a terminal and navigate to the directory:
+2. Open a terminal and navigate to the directory 
+(you need to replace `path/to/glytrait_example` with the actual path):
 
 ```shell
-cd glytrait_example
+cd path/to/glytrait_example
 ```
 
 3. Run the following command:
 
 ```shell
 glytrait abundance.csv structures.csv
 ```
```

### Comparing `glytrait-0.1.1/pyproject.toml` & `glytrait-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glytrait"
-version = "0.1.1"
+version = "0.1.2"
 description = "A tool for calculating derived traits for N-glycome"
 authors = ["fubin1999 <65430559+fubin1999@users.noreply.github.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "http://mirrors.aliyun.com/pypi/simple"
```

### Comparing `glytrait-0.1.1/src/glytrait/data_export.py` & `glytrait-0.1.2/src/glytrait/data_export.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 from collections.abc import Iterable, Callable
 from pathlib import Path
 from typing import Type, TypeVar, Any
 
 import pandas as pd
 
-from glytrait.formula import TraitFormula
-
 __all__ = ["export_all"]
 
 
 def export_all(to_export: Iterable[tuple[str, Any]], base_path: str) -> None:
     """Export all data to the directory given by `base_path`.
 
     Notes:
```

### Comparing `glytrait-0.1.1/src/glytrait/data_type.py` & `glytrait-0.1.2/src/glytrait/data_type.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.1/src/glytrait/exception.py` & `glytrait-0.1.2/src/glytrait/exception.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.1/src/glytrait/formula.py` & `glytrait-0.1.2/src/glytrait/formula.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,50 +10,47 @@
     load_formulas: Load all trait formulas from default formula files and custom formulas files.
     save_trait_formulas_tepmlate: Save a template of trait formulas to a file.
     save_builtin_formula: Save a built-in trait formulas to a file.
 """
 
 from __future__ import annotations
 
-import itertools
 import functools
+import itertools
 import re
-from collections.abc import Callable, Iterator
+from collections.abc import Callable, Iterator, Iterable
 from importlib.resources import files, as_file
 from pathlib import Path
-from typing import Literal, Optional, Generator, Type, Protocol
+from typing import Literal, Optional, Type, Protocol
 
+import attrs
 import numpy as np
 import pandas as pd
-import attrs
 from attrs import field, define
 
 from glytrait.data_type import AbundanceTable, MetaPropertyTable
 
 __all__ = [
     "TraitFormula",
-    "load_formulas",
+    "parse_formulas",
+    "load_formulas_from_file",
     "load_default_formulas",
     "save_builtin_formula",
 ]
 
 from glytrait.exception import GlyTraitError
 
 default_struc_formula_file = files("glytrait.resources").joinpath("struc_formula.txt")
 default_comp_formula_file = files("glytrait.resources").joinpath("comp_formula.txt")
 
 
 class FormulaError(GlyTraitError):
     """Raised if a formula is invalid."""
 
 
-class FormulaFileError(GlyTraitError):
-    """Raised if a formula file is in wrong format."""
-
-
 class FormulaParseError(FormulaError):
     """Raised when failing parsing a formula expression."""
 
     def __init__(self, expr: str, reason: str = ""):
         super().__init__()
         self.expr = expr
         self.reason = reason
@@ -707,90 +704,79 @@
             try:
                 return term_cls.from_expr(expr)  # Let the exception pass through
             except FormulaTermParseError:
                 continue
         raise FormulaTermParseError(expr, "Does not belong to any term class.")
 
 
-@define
-class FormulaFileParser:
-    """Parser for a formula file."""
-
-    expr_parser: FormulaParserType = field(kw_only=True, default=FormulaParser())
-
-    def parse(self, filepath: str) -> Iterator[TraitFormula]:
-        """Parse the formula file and return a list of `TraitFormula` objects."""
-        for description, expression in self._deconvolute_formula_file(filepath):
-            yield TraitFormula.from_expr(expression, parser=self.expr_parser)
-
-    @staticmethod
-    def _deconvolute_formula_file(formula_file: str) -> Iterator[tuple[str, str]]:
-        """A generator that yields the formula description and the formula expression.
+# ===== High-level functions =====
+def parse_formulas(exprs: Iterable[str]) -> list[TraitFormula]:
+    """Parse formula expressions.
 
-        Args:
-            formula_file (str): The path of the formula file.
-
-        Yields:
-            tuple[str, str]: The formula description and the formula expression.
+    Args:
+        exprs: The formula expressions.
 
-        Raises:
-            FormulaFileError: If the formula file is in a wrong format.
-        """
-        with open(formula_file, "r", encoding="utf8") as f:
-            description, expression = None, None
+    Returns:
+        list[TraitFormula]: The formulas.
 
-            for line in f:
-                line = line.strip()
-                if not line or line.startswith("#"):
-                    continue
-
-                if line.startswith("@"):
-                    if description is not None:
-                        msg = f"No expression follows description '{description}'."
-                        raise FormulaFileError(msg)
-                    description = line[1:].strip()
-
-                elif line.startswith("$"):
-                    expression = line[1:].strip()
-                    if description is None:
-                        msg = f"No description before expression '{expression}'."
-                        raise FormulaFileError(msg)
-                    yield description, expression
-                    description, expression = None, None
-
-        if description is not None:
-            raise FormulaFileError(
-                f"No expression follows description '{description}'."
-            )
+    Raises:
+        FormulaParseError: If any expression is invalid.
+            All the invalid expressions will be reported in the error message.
+    """
+    formulas: list[TraitFormula] = []
+    failed_exprs: list[str] = []
+    parser = FormulaParser()
+    for expr in exprs:
+        try:
+            formula = parser.parse(expr)
+        except FormulaParseError:
+            failed_exprs.append(expr)
+        else:
+            formulas.append(formula)
+    if failed_exprs:
+        failed_exprs_str = ", ".join(f"'{expr}'" for expr in failed_exprs)
+        msg = "Failed to parse the following expressions: " + failed_exprs_str
+        raise FormulaParseError(msg)
+    return formulas
 
 
-def load_formulas(
+def load_formulas_from_file(
     file: str,
     sia_linkage: bool = False,
 ) -> list[TraitFormula]:
     """Load formulas from a formula file.
 
     Args:
         file: The path of the formula file.
         sia_linkage: Whether to include formulas with sia-linkage
             meta-properties. Defaults to False.
 
     Returns:
         list[TraitFormula]: The formulas.
 
     Raises:
-        FormulaFileError: If the formula file is in a wrong format.
         FormulaParseError: If a formula string cannot be parsed.
     """
-    formulas = [f for f in FormulaFileParser().parse(file)]
+    exprs = list(_get_formula_exprs_from_file(file))
+    formulas = parse_formulas(exprs)
     if not sia_linkage:
         formulas = [f for f in formulas if not f.sia_linkage]
     return formulas
 
 
+def _get_formula_exprs_from_file(file: str) -> Iterator[str]:
+    """Get all the formula expressions from a formula file."""
+    with open(file, encoding="utf8") as f:
+        for line in f:
+            line = line.strip()
+            if not line or line.startswith("#"):
+                continue
+            yield line
+
+
 def load_default_formulas(
     mode: Literal["structure", "composition"],
     sia_linkage: bool = False,
 ) -> list[TraitFormula]:
     """Load the default formulas.
 
     Args:
@@ -804,15 +790,15 @@
     if mode == "composition":
         file_traversable = default_comp_formula_file
     elif mode == "structure":
         file_traversable = default_struc_formula_file
     else:
         raise ValueError("Invalid formula type.")
     with as_file(file_traversable) as file:
-        return load_formulas(str(file), sia_linkage=sia_linkage)
+        return load_formulas_from_file(str(file), sia_linkage=sia_linkage)
 
 
 def save_builtin_formula(dirpath: str | Path) -> None:
     """Copy the builtin formula file to the given path.
 
     Args:
         dirpath (str): The path to save the built-in formula file.
```

### Comparing `glytrait-0.1.1/src/glytrait/glycan.py` & `glytrait-0.1.2/src/glytrait/glycan.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     get_mono_str: Helper function for checking the identity of a `glypy.MonosaccarideResidue`.
 """
 
 from __future__ import annotations
 
 import re
 from collections.abc import Generator, Mapping, Iterator, Callable
-from typing import Literal, Iterable, Optional, Final, Union, TypeVar, NewType
+from typing import Literal, Iterable, Optional, Final, Union, TypeVar
 
 from attrs import frozen, field
 from glypy.io.glycoct import loads as glycoct_loads, GlycoCTError  # type: ignore
 from glypy.structure.glycan import Glycan as GlypyGlycan  # type: ignore
 from glypy.structure.glycan_composition import (  # type: ignore
     GlycanComposition,
     MonosaccharideResidue,
@@ -27,42 +27,23 @@
 from glytrait.exception import (
     GlycanParseError,
     StructureParseError,
     CompositionParseError,
 )
 
 __all__ = [
-    "StructureDict",
-    "CompositionDict",
-    "GlycanDict",
     "parse_structures",
     "parse_compositions",
     "Structure",
     "Composition",
     "get_mono_str",
 ]
 
-StructureDict = NewType("StructureDict", dict[str, "Structure"])
-"""A type hint for a dictionary of `Structure` instances.
-The keys are the names of the structures, and the values are the structures.
-"""
-
-CompositionDict = NewType("CompositionDict", dict[str, "Composition"])
-"""A type hint for a dictionary of `Composition` instances.
-The keys are the names of the compositions, and the values are the compositions.
-"""
-
-GlycanDict = Union[StructureDict, CompositionDict]
-"""A type hint for a dictionary of `Structure` or `Composition` instances.
-The keys are the names of the structures or compositions, 
-and the values are the structures or compositions.
-"""
-
 
-def parse_structures(__iter: Iterable[tuple[str, str]]) -> StructureDict:
+def parse_structures(__iter: Iterable[tuple[str, str]]) -> dict[str, Structure]:
     """Parse glycan structures from a list of structure strings.
 
     Args:
         An iterable of tuples of (name, structure_string).
 
     Returns:
         A dictionary of `Structure` instances, with the keys being the names of the structures.
@@ -73,18 +54,18 @@
             in the error message.
     """
     try:
         result: dict[str, Structure] = _load_glycans(__iter, Structure.from_string)
     except GlycanParseError as exc:
         raise StructureParseError(f"Could not parse structures for: {exc}.")
     else:
-        return StructureDict(result)
+        return result
 
 
-def parse_compositions(__iter: Iterable[tuple[str, str]]) -> CompositionDict:
+def parse_compositions(__iter: Iterable[tuple[str, str]]) -> dict[str, Composition]:
     """Parse glycan compositions from a list of composition strings.
 
     Args:
         An iterable of tuples of (name, composition_string).
 
     Returns:
         A dictionary of `Composition` instances, with the keys being the names of the compositions.
@@ -95,15 +76,15 @@
             in the error message.
     """
     try:
         result: dict[str, Composition] = _load_glycans(__iter, Composition.from_string)
     except GlycanParseError as exc:
         raise CompositionParseError(f"Could not parse compositions for: {exc}.")
     else:
-        return CompositionDict(result)
+        return result
 
 
 Glycan = TypeVar("Glycan", bound=Union["Structure", "Composition"])
 GlycanBuilder = Callable[[str, str], Glycan]
 
 
 def _load_glycans(
```

### Comparing `glytrait-0.1.1/src/glytrait/load_data.py` & `glytrait-0.1.2/src/glytrait/data_input.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,51 +9,35 @@
     load_input_data: Load all the input data for GlyTrait, including
         abundance table, glycans, and groups.
         Returns a `GlyTraitInputData` object.
 """
 
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
 from collections.abc import Iterable, Callable
-from typing import Optional, Literal, Protocol, cast, ClassVar
+from typing import Optional, Literal, Any, cast
 
 import pandas as pd
 from attrs import define, field
 from numpy import dtype
 
 from glytrait.data_type import (
     AbundanceTable,
     GroupSeries,
 )
 from glytrait.exception import DataInputError
-from glytrait.glycan import (
-    parse_structures,
-    parse_compositions,
-    StructureDict,
-    CompositionDict,
-    GlycanDict,
-)
+from glytrait.glycan import parse_structures, parse_compositions, Structure, Composition
 
 __all__ = [
+    "load_data",
     "GlyTraitInputData",
-    "load_input_data_from_csv",
 ]
 
-
-# ===== Loaders =====
-class AbundanceLoaderProto(Protocol):
-    def load(self) -> AbundanceTable: ...
-
-
-class GlycanLoaderProto(Protocol):
-    def load(self) -> StructureDict | CompositionDict: ...
-
-
-class GroupsLoaderProto(Protocol):
-    def load(self) -> GroupSeries: ...
+GlycanDict = dict[str, Structure] | dict[str, Composition]
 
 
 @define
 class DFValidator:
     """Validator for pandas DataFrame.
 
     Attributes:
@@ -117,122 +101,79 @@
             msg = (
                 f"The following columns have incorrect types: {', '.join(wrong_type_cols)}. "
                 f"Expected types: {self.default_type}, got: {got}."
             )
             raise DataInputError(msg)
 
 
-@define
-class CSVLoader:
-    """Base class for data loaders from csv files."""
-
-    filepath: str
-    validator: DFValidator = field(kw_only=True, default=lambda df: None)
+class DataLoader(ABC):
+    """Base class for a data loader."""
 
-    # Dependency injection
-    reader: Callable[[str], pd.DataFrame] = field(kw_only=True, default=pd.read_csv)
-
-    def load(self):
-        """Load the data from the file."""
+    def load(self, df: pd.DataFrame) -> Any:
+        """Load data from the DataFrame."""
+        self._validate_data(df)
+        return self._load_data(df)
+
+    @abstractmethod
+    def _validate_data(self, df: pd.DataFrame) -> None:
+        """Validate the DataFrame."""
         raise NotImplementedError
 
-    def load_df(self) -> pd.DataFrame:
-        """Returns the DataFrame loaded from the file.
-
-        Raises:
-            FileNotFoundError: If the file does not exist.
-            DataInputError: If one of the following conditions is met:
-                (1) the file is empty; (2) the file could not be parsed.
-        """
-        df = self.read_csv()
-        self.validator(df)
-        return df
-
-    def read_csv(self) -> pd.DataFrame:
-        """A thin wrapper for `pd.read_csv`, with custum exceptions."""
-        try:
-            return self.reader(self.filepath)
-        # FileNotFoundError is not caught here
-        except pd.errors.EmptyDataError as e:
-            raise DataInputError("Empty CSV file.") from e
-        except pd.errors.ParserError as e:
-            raise DataInputError("This CSV file could not be parsed.") from e
+    @abstractmethod
+    def _load_data(self, df: pd.DataFrame) -> Any:
+        """Load data from the DataFrame."""
+        raise NotImplementedError
 
 
 @define
-class AbundanceCSVLoader(CSVLoader):
-    """Loader for abundance table from a csv file."""
+class AbundanceLoader(DataLoader):
+    """Loader of the abundance table."""
 
-    validator: DFValidator = field(
-        kw_only=True,
-        default=DFValidator(
+    def _validate_data(self, df: pd.DataFrame) -> None:
+        validator = DFValidator(
             must_have=["Sample"],
             unique=["Sample"],
             types={"Sample": "object"},
             default_type=dtype("float64"),
-        ),
-    )
-
-    def load(self) -> AbundanceTable:
-        """Returns the abundance table loaded from the file.
+        )
+        validator(df)
 
-        Raises:
-            FileNotFoundError: If the file does not exist.
-            DataInputError: If the file format is incorrect.
-                This includes: (1) the file is empty; (2) the file could not be parsed;
-                (3) the "Sample" column is not found.
-        """
-        df = self.load_df()
+    def _load_data(self, df: pd.DataFrame) -> AbundanceTable:
         return AbundanceTable(df.set_index("Sample"))
 
 
 @define
-class GroupsCSVLoader(CSVLoader):
-    """Loader for groups from a csv file."""
+class GroupsLoader(DataLoader):
+    """Loader of the group series."""
 
-    validator: DFValidator = field(
-        kw_only=True,
-        default=DFValidator(
+    def _validate_data(self, df: pd.DataFrame) -> None:
+        validator = DFValidator(
             must_have=["Group", "Sample"],
             unique=["Sample"],
             types={"Sample": "object"},
-        ),
-    )
-
-    def load(self) -> GroupSeries:
-        """Returns the groups loaded from the file.
+        )
+        validator(df)
 
-        Raises:
-            FileNotFoundError: If the file does not exist.
-            DataInputError: If the file format is incorrect.
-                This includes: (1) the file is empty; (2) the file could not be parsed;
-                (3) the "Sample" column is not found; (4) the "Group" column is not found.
-        """
-        df = self.load_df()
+    def _load_data(self, df: pd.DataFrame) -> GroupSeries:
         return GroupSeries(df.set_index("Sample")["Group"])
 
 
-GlycanParserType = Callable[
-    [Iterable[tuple[str, str]]], StructureDict | CompositionDict
-]
+GlycanParserType = Callable[[Iterable[tuple[str, str]]], GlycanDict]
 
 
 @define
-class GlycanCSVLoader(CSVLoader):
+class GlycanLoader(DataLoader):
     """Loader for structures or compositions from a csv file."""
 
     mode: Literal["structure", "composition"] = field(kw_only=True)
-    validator: DFValidator = field(kw_only=True, default=None)
     parser: GlycanParserType = field(kw_only=True, default=None)
 
     def __attrs_post_init__(self):
         if self.parser is None:
             self.parser = self._glycan_parser_factory(self.mode)
-        if self.validator is None:
-            self.validator = self._validator_factory(self.mode)
 
     @staticmethod
     def _glycan_parser_factory(
         mode: Literal["structure", "composition"]
     ) -> GlycanParserType:
         parser = parse_structures if mode == "structure" else parse_compositions
         return cast(GlycanParserType, parser)
@@ -242,35 +183,22 @@
         glycan_col = "Structure" if mode == "structure" else "Composition"
         return DFValidator(
             must_have=["GlycanID", glycan_col],
             unique=["GlycanID", glycan_col],
             types={"GlycanID": "object", glycan_col: "object"},
         )
 
-    def load(self) -> GlycanDict:
-        """Returns the glycans loaded from the file.
+    def _validate_data(self, df: pd.DataFrame) -> None:
+        validator = self._validator_factory(self.mode)
+        validator(df)
 
-        Raises:
-            FileNotFoundError: If the file does not exist.
-            FileFormatError: If the file format is incorrect.
-                This includes: (1) the file is empty; (2) the file could not be parsed;
-                (3) the "GlycanID" column is not found; (4) the "Structure" or
-                "Composition" column is not found.
-            StructureParseError: If any structure cannot be parsed,
-                when `mode` is "structure".
-            CompositionParseError: If any composition cannot be parsed,
-                when `mode` is "composition".
-        """
-        df = self.load_df()
+    def _load_data(self, df: pd.DataFrame) -> GlycanDict:
         ids = df["GlycanID"].to_list()
         glycan_col = self.mode.capitalize()
-        try:
-            strings = df[glycan_col].to_list()
-        except KeyError as e:
-            raise DataInputError(f"The '{glycan_col}' column is not found.") from e
+        strings = df[glycan_col].to_list()
         return self.parser(zip(ids, strings))
 
 
 # ===== Input data =====
 @define(kw_only=True)
 class GlyTraitInputData:
     """GlyTrait input data.
@@ -282,60 +210,83 @@
         groups: Sample groups as a pandas Series.
 
     Notes:
         The glycan dict should have the same keys as the abundance table.
         The samples in the abundance table should have the same names as the
         samples in the groups.
 
+        Accessing the attributes will return a copy of the data.
+        This prevents the original data from being modified in place,
+        which will bypass the validation checks.
+        If you need to modify the data, you should set the attributes
+        with the new data.
+
     Raises:
-        FileFormatError: If the abundance table has different samples as the groups,
+        DataInputError: If the abundance table has different samples as the groups,
             or if the glycan dict has different glycans as the abundance table.
     """
 
-    abundance_table: AbundanceTable
-    glycans: StructureDict | CompositionDict
-    groups: Optional[GroupSeries] = None
-
-
-# ===== Input data validators =====
-ValidatorType = Callable[[GlyTraitInputData], None]
-
-
-@define
-class InputDataValidator:
-    """Validator for the input data.
-
-    This class only validates the interaction between the input data.
-    The format of each input data is validated by the loaders.
-    """
-
-    validators: ClassVar[list[ValidatorType]] = []
-
-    def __call__(self, input_data: GlyTraitInputData) -> None:
-        for validator in self.validators:
-            validator(input_data)
+    _abundance_table: AbundanceTable
+    _glycans: GlycanDict
+    _groups: Optional[GroupSeries] = None
 
-    @classmethod
-    def add_validator(cls, validator: ValidatorType) -> ValidatorType:
-        """A decorator to add a validator to the list of validators."""
-        cls.validators.append(validator)
-        return validator
-
-
-@InputDataValidator.add_validator
-def same_samples_in_abundance_and_groups(input_data: GlyTraitInputData) -> None:
+    def __attrs_post_init__(self):
+        if self._groups is not None:
+            check_same_samples_in_abund_and_groups(self._abundance_table, self._groups)
+        check_all_glycans_have_struct_or_comp(self._abundance_table, self._glycans)
+
+    @property
+    def abundance_table(self) -> AbundanceTable:
+        """The abundance table as a pandas DataFrame."""
+        return AbundanceTable(self._abundance_table.copy())
+
+    @abundance_table.setter
+    def abundance_table(self, value: pd.DataFrame) -> None:
+        if self._groups is not None:
+            check_same_samples_in_abund_and_groups(value, self._groups)
+        check_all_glycans_have_struct_or_comp(value, self._glycans)
+        self._abundance_table = AbundanceTable(value)
+
+    @property
+    def glycans(self) -> GlycanDict:
+        """The glycans as a dict of `Structure` or `Composition` objects."""
+        return self._glycans.copy()
+
+    @glycans.setter
+    def glycans(self, value: GlycanDict) -> None:
+        check_all_glycans_have_struct_or_comp(self._abundance_table, value)
+        self._glycans = value
+
+    @property
+    def groups(self) -> GroupSeries | None:
+        """The sample groups as a pandas Series."""
+        return GroupSeries(self._groups.copy()) if self._groups is not None else None
+
+    @groups.setter
+    def groups(self, value: pd.Series | None) -> None:
+        if value is not None:
+            check_same_samples_in_abund_and_groups(self._abundance_table, value)
+        self._groups = GroupSeries(value) if value is not None else None
+
+
+def check_same_samples_in_abund_and_groups(
+    abundance_df: pd.DataFrame,
+    groups: pd.Series,
+) -> None:
     """Check if the abundance table and the groups have the same samples.
 
+    Args:
+        abundance_df: Abundance table as a pandas DataFrame.
+        groups: Sample groups as a pandas Series.
+
     Raises:
         DataInputError: If the samples in the abundance table and the groups are different.
     """
-    if input_data.groups is None:
-        return
-    abund_samples = set(input_data.abundance_table.index)
-    groups_samples = set(input_data.groups.index)
+    abund_samples = set(abundance_df.index)
+    groups_samples = set(groups.index)
     if abund_samples != groups_samples:
         samples_in_abund_not_in_groups = abund_samples - groups_samples
         samples_in_groups_not_in_abund = groups_samples - abund_samples
         msg = ""
         if samples_in_abund_not_in_groups:
             msg += (
                 f"The following samples are in the abundance table but not in the groups: "
@@ -345,89 +296,69 @@
             msg += (
                 f"The following samples are in the groups but not in the abundance table: "
                 f"{', '.join(samples_in_groups_not_in_abund)}."
             )
         raise DataInputError(msg)
 
 
-@InputDataValidator.add_validator
-def all_glycans_have_structures_or_compositions(input_data: GlyTraitInputData) -> None:
+def check_all_glycans_have_struct_or_comp(
+    abundance_df: pd.DataFrame,
+    glycans: GlycanDict,
+) -> None:
     """Check if all glycans in the abundance table have structures or compositions.
 
     Glycans in the structure or composition dict that are not in the abundance table
     are not checked.
 
+    Args:
+        abundance_df: Abundance table as a pandas DataFrame.
+        glycans: Glycans, either a dict of `Structure` objects or a dict of `Composition` objects.
+
     Raises:
         DataInputError: If any glycan in the abundance table does not
             have a structure or composition.
     """
-    abund_glycans = set(input_data.abundance_table.columns)
-    glycans = set(input_data.glycans.keys())
-    if diff := abund_glycans - glycans:
+    abund_glycans = set(abundance_df.columns)
+    glycan_names = set(glycans.keys())
+    if diff := abund_glycans - glycan_names:
         msg = (
             f"The following glycans in the abundance table do not have structures or "
             f"compositions: {', '.join(diff)}."
         )
         raise DataInputError(msg)
 
 
-# ===== The low-level API =====
-def load_input_data(
+def load_data(
+    abundance_df: pd.DataFrame,
+    glycan_df: pd.DataFrame,
+    group_df: Optional[pd.DataFrame] = None,
     *,
-    abundance_loader: AbundanceLoaderProto,
-    glycan_loader: GlycanLoaderProto,
-    group_loader: Optional[GroupsLoaderProto] = None,
-    validator: ValidatorType = InputDataValidator(),
+    mode: Literal["structure", "composition"] = "structure",
 ) -> GlyTraitInputData:
     """Load all the input data for GlyTrait.
 
     Args:
-        abundance_loader: Loader for the abundance table.
-        glycan_loader: Loader for the glycans.
-        group_loader: Loader for the groups. Optional.
-        mode: Either "structure" or "composition".
-        validator: Validator for the input data.
+        abundance_df: Abundance table as a pandas DataFrame.
+        glycan_df: Glycan structures or compositions as a pandas DataFrame.
+        group_df: Sample groups as a pandas DataFrame. Optional.
+        mode: Mode of the glycan data, either "structure" or "composition".
 
     Returns:
-        GlyTraitInputData: Input data for GlyTrait.
+        A `GlyTraitInputData` object.
+
+    Raises:
+        DataInputError: If the input data is not valid.
     """
-    abundance_table = abundance_loader.load()
-    glycans = glycan_loader.load()
-    groups = group_loader.load() if group_loader else None
+    abundance_loader = AbundanceLoader()
+    structure_loader = GlycanLoader(mode=mode)
+    group_loader = GroupsLoader()
+
+    abundance_table = abundance_loader.load(abundance_df)
+    glycans = structure_loader.load(glycan_df)
+    groups = group_loader.load(group_df) if group_df is not None else None
 
     input_data = GlyTraitInputData(
         abundance_table=abundance_table,
         glycans=glycans,
         groups=groups,
     )
-
-    validator(input_data)
     return input_data
-
-
-# ===== The high-level API =====
-def load_input_data_from_csv(
-    *,
-    abundance_file: str,
-    glycan_file: str,
-    group_file: Optional[str] = None,
-    mode: Literal["structure", "composition"],
-) -> GlyTraitInputData:
-    """Load all the input data for GlyTrait from csv files.
-
-    Args:
-        abundance_file: Path to the abundance table csv file.
-        glycan_file: Path to the glycans csv file.
-        group_file: Path to the groups csv file. Optional.
-        mode: Either "structure" or "composition".
-
-    Returns:
-        GlyTraitInputData: Input data for GlyTrait.
-    """
-    abundance_loader = AbundanceCSVLoader(filepath=abundance_file)
-    glycan_loader = GlycanCSVLoader(filepath=glycan_file, mode=mode)
-    group_loader = GroupsCSVLoader(filepath=group_file) if group_file else None
-    return load_input_data(
-        abundance_loader=abundance_loader,
-        glycan_loader=glycan_loader,
-        group_loader=group_loader,
-    )
```

### Comparing `glytrait-0.1.1/src/glytrait/meta_property.py` & `glytrait-0.1.2/src/glytrait/meta_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,30 +19,32 @@
     - nE: The number of sialic acids with an alpha-2,6 linkage.
 """
 
 from __future__ import annotations
 
 from enum import Enum, auto
 from functools import singledispatch, cache
-from typing import Literal, Any, ClassVar, Type
+from typing import Literal, ClassVar, Type
 
 import pandas as pd
 from attrs import define
 from glypy import Monosaccharide  # type: ignore
 
 from glytrait.data_type import MetaPropertyTable
 from glytrait.exception import SiaLinkageError
-from glytrait.glycan import Structure, Composition, get_mono_str, GlycanDict
+from glytrait.glycan import Structure, Composition, get_mono_str
 
 __all__ = [
     "build_meta_property_table",
     "available_meta_properties",
     "get_meta_property",
 ]
 
+GlycanDict = dict[str, Structure] | dict[str, Composition]
+
 
 def build_meta_property_table(
     glycans: GlycanDict,
     mode: Literal["composition", "structure"],
     sia_linkage: bool = False,
 ) -> MetaPropertyTable:
     """Build a table of meta-properties for glycans.
```

### Comparing `glytrait-0.1.1/src/glytrait/post_filtering.py` & `glytrait-0.1.2/src/glytrait/post_filtering.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.1/src/glytrait/preprocessing.py` & `glytrait-0.1.2/src/glytrait/preprocessing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 """Preprocess the abundance table.
 
 The only high-level function that client code will use is `preprocess`.
 """
 
 from typing import Literal, Protocol
 
-from attrs import define
+from attrs import define, field
+from attrs.validators import in_
 
-from glytrait.load_data import GlyTraitInputData
 from glytrait.data_type import AbundanceTable
 
 __all__ = ["preprocess"]
 
 
 # This is the high-level function that client code will use.
 def preprocess(
-    data: GlyTraitInputData,
+    data: AbundanceTable,
     filter_max_na: float,
     impute_method: Literal["zero", "min", "lod", "mean", "median"],
-) -> None:
+) -> AbundanceTable:
     """Preprocess the abundance table.
 
     Notes:
         This function will modify the input data in place.
 
     Args:
-        data (GlyTraitInputData): The input data.
+        data (AbundanceTable): The abundance table.
         filter_max_na (float): The maximum proportion of missing values allowed for a glycan.
         impute_method (Literal["zero", "min", "lod", "mean", "median"]): The imputation method.
+
+    Returns:
+        AbundanceTable: The preprocessed abundance table.
     """
     steps = [
         FilterGlycans(max_na=filter_max_na),
         Impute(method=impute_method),
         Normalize(),
     ]
     pipeline = ProcessingPipeline(steps=steps)
-    pipeline(data)
+    return pipeline(data)
 
 
 class ProcessingStep(Protocol):
     """The protocol for processing steps."""
 
-    def __call__(self, data: GlyTraitInputData) -> None: ...
+    def __call__(self, data: AbundanceTable) -> AbundanceTable: ...
 
 
 @define
 class ProcessingPipeline:
     """The pipeline for processing the abundance table."""
 
     _steps: list[ProcessingStep]
 
-    def __call__(self, data: GlyTraitInputData) -> None:
+    def __call__(self, data: AbundanceTable) -> AbundanceTable:
         for step in self._steps:
-            step(data)
+            data = step(data)
+        return data
 
 
 @define
 class FilterGlycans(ProcessingStep):
     """Filter glycans with too many missing values.
 
     Args:
         max_na (float): The maximum proportion of missing values allowed for a glycan.
     """
 
     max_na: float
 
-    def __call__(self, data: GlyTraitInputData) -> None:
-        glycans_to_keep = _filter_glycans(data.abundance_table, self.max_na)
-        data.abundance_table = AbundanceTable(
-            data.abundance_table.filter(items=glycans_to_keep)
-        )
-        for glycan in set(data.glycans).difference(glycans_to_keep):
-            del data.glycans[glycan]
-
-
-def _filter_glycans(abundance_df: AbundanceTable, max_na: float) -> list[str]:
-    to_keep_mask = abundance_df.isna().mean() <= max_na
-    glycans_to_keep = list(abundance_df.columns[to_keep_mask])
-    return glycans_to_keep
+    def __call__(self, data: AbundanceTable) -> AbundanceTable:
+        to_keep_mask = data.isna().mean() <= self.max_na
+        return AbundanceTable(data.loc[:, to_keep_mask])
 
 
 @define
 class Impute(ProcessingStep):
     """Impute the missing values of the abundance table.
 
     The following imputation methods supported:
@@ -93,53 +87,33 @@
         - "median": Replace the missing values with the median value of the corresponding glycan.
 
     Args:
         method (str): The imputation method.
             Can be "zero", "min", "lod", "mean", "median".
     """
 
-    method: Literal["zero", "min", "lod", "mean", "median"]
-
-    def __call__(self, data: GlyTraitInputData) -> None:
-        data.abundance_table = _impute(data.abundance_table, self.method)
-
-
-def _impute(
-    abundance_df: AbundanceTable,
-    method: Literal["zero", "min", "lod", "mean", "median"],
-) -> AbundanceTable:
-    if method == "zero":
-        imputed_df = abundance_df.fillna(0)
-    elif method == "min":
-        imputed_df = abundance_df.fillna(abundance_df.min())
-    elif method == "lod":
-        imputed_df = abundance_df.fillna(abundance_df.min() / 5)
-    elif method == "mean":
-        imputed_df = abundance_df.fillna(abundance_df.mean())
-    elif method == "median":
-        imputed_df = abundance_df.fillna(abundance_df.median())
-    else:
-        raise ValueError("The imputation method is not supported.")
-    return AbundanceTable(imputed_df)
+    method: Literal["zero", "min", "lod", "mean", "median"] = field(
+        validator=in_(["zero", "min", "lod", "mean", "median"])
+    )
+
+    def __call__(self, data: AbundanceTable) -> AbundanceTable:
+        if self.method == "zero":
+            imputed_df = data.fillna(0)
+        elif self.method == "min":
+            imputed_df = data.fillna(data.min())
+        elif self.method == "lod":
+            imputed_df = data.fillna(data.min() / 5)
+        elif self.method == "mean":
+            imputed_df = data.fillna(data.mean())
+        elif self.method == "median":
+            imputed_df = data.fillna(data.median())
+        return AbundanceTable(imputed_df)
 
 
 @define
 class Normalize(ProcessingStep):
     """Normalize the abundance table by dividing the sum of each sample."""
 
-    def __call__(self, data: GlyTraitInputData) -> None:
-        data.abundance_table = _normalization(data.abundance_table)
-
-
-def _normalization(abundance_df: AbundanceTable) -> AbundanceTable:
-    """Normalize the abundance table by dividing the sum of each sample.
-
-    Args:
-        abundance_df (AbundanceTable): The abundance table,
-            with samples as index and Compositions as columns.
-
-    Returns:
-        normalized_df (AbundanceTable): The normalized abundance table.
-    """
-    row_sums = abundance_df.sum(axis=1)
-    normalized_df = abundance_df.div(row_sums, axis=0).round(6)
-    return AbundanceTable(normalized_df)
+    def __call__(self, data: AbundanceTable) -> AbundanceTable:
+        row_sums = data.sum(axis=1)
+        normalized_df = data.div(row_sums, axis=0)
+        return AbundanceTable(normalized_df)
```

### Comparing `glytrait-0.1.1/src/glytrait/resources/struc_formula.txt` & `glytrait-0.1.2/src/glytrait/resources/struc_formula.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,1087 +1,1087 @@
 # Glycan type
 
-@ Relative abundance of high mannose type glycans within total spectrum
-$ TM = [type == 'high_mannose'] / [1]
+# Relative abundance of high mannose type glycans within total spectrum
+TM = [type == 'high_mannose'] / [1]
 
-@ Relative abundance of hybrid type glycans within total spectrum
-$ THy = [type == 'hybrid'] / [1]
+# Relative abundance of hybrid type glycans within total spectrum
+THy = [type == 'hybrid'] / [1]
 
-@ The ratio of high-mannose to hybrid glycans
-$ MHy = [type == 'high_mannose'] / [type == 'hybrid']
+# The ratio of high-mannose to hybrid glycans
+MHy = [type == 'high_mannose'] / [type == 'hybrid']
 
-@ Average number of mannoses on high mannose type glycans
-$ MM = [nM] // [type == 'high_mannose']
+# Average number of mannoses on high mannose type glycans
+MM = [nM] // [type == 'high_mannose']
 
-@ Relative abundance of monoantennary glycans within complex type glycans
-$ CA1 = [nAnt == 1] // [type == 'complex']
+# Relative abundance of monoantennary glycans within complex type glycans
+CA1 = [nAnt == 1] // [type == 'complex']
 
-@ Relative abundance of diantennary glycans within complex type glycans
-$ CA2 = [nAnt == 2] // [type == 'complex']
+# Relative abundance of diantennary glycans within complex type glycans
+CA2 = [nAnt == 2] // [type == 'complex']
 
-@ Relative abundance of triantennary glycans within complex type glycans
-$ CA3 = [nAnt == 3] // [type == 'complex']
+# Relative abundance of triantennary glycans within complex type glycans
+CA3 = [nAnt == 3] // [type == 'complex']
 
-@ Relative abundance of tetra-antennary glycans within complex type glycans
-$ CA4 = [nAnt == 4] // [type == 'complex']
+# Relative abundance of tetra-antennary glycans within complex type glycans
+CA4 = [nAnt == 4] // [type == 'complex']
 
 
 # Core Fucosylation
 
-@ Core fucosylation within complex type glycans
-$ CFc = [nFc > 0] // [type == 'complex']
+# Core fucosylation within complex type glycans
+CFc = [nFc > 0] // [type == 'complex']
 
-@ Core fucosylation within monoantennary glycans
-$ A1Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1)]
+# Core fucosylation within monoantennary glycans
+A1Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1)]
 
-@ Core fucosylation within diantennary glycans
-$ A2Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2)]
+# Core fucosylation within diantennary glycans
+A2Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2)]
 
-@ Core fucosylation within triantennary glycans
-$ A3Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3)]
+# Core fucosylation within triantennary glycans
+A3Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3)]
 
-@ Core fucosylation within tetra-antennary glycans
-$ A4Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4)]
+# Core fucosylation within tetra-antennary glycans
+A4Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4)]
 
-@ Core fucosylation within sialylated monoantennary glycans
-$ A1SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
+# Core fucosylation within sialylated monoantennary glycans
+A1SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
 
-@ Core fucosylation within sialylated diantennary glycans
-$ A2SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
+# Core fucosylation within sialylated diantennary glycans
+A2SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
 
-@ Core fucosylation within sialylated triantennary glycans
-$ A3SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
+# Core fucosylation within sialylated triantennary glycans
+A3SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
 
-@ Core fucosylation within sialylated tetra-antennary glycans
-$ A4SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
+# Core fucosylation within sialylated tetra-antennary glycans
+A4SFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
 
-@ Core fucosylation within non-sialylated monoantennary glycans
-$ A1S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
+# Core fucosylation within non-sialylated monoantennary glycans
+A1S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
 
-@ Core fucosylation within non-sialylated diantennary glycans
-$ A2S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
+# Core fucosylation within non-sialylated diantennary glycans
+A2S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
 
-@ Core fucosylation within non-sialylated triantennary glycans
-$ A3S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
+# Core fucosylation within non-sialylated triantennary glycans
+A3S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
 
-@ Core fucosylation within non-sialylated tetra-antennary glycans
-$ A4S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
+# Core fucosylation within non-sialylated tetra-antennary glycans
+A4S0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
 
-@ Core fucosylation within monoantennary glycans with α2,6-linked sialic acid
-$ A1EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
+# Core fucosylation within monoantennary glycans with α2,6-linked sialic acid
+A1EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
 
-@ Core fucosylation within diantennary glycans with α2,6-linked sialic acid
-$ A2EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
+# Core fucosylation within diantennary glycans with α2,6-linked sialic acid
+A2EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
 
-@ Core fucosylation within triantennary glycans with α2,6-linked sialic acid
-$ A3EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
+# Core fucosylation within triantennary glycans with α2,6-linked sialic acid
+A3EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
 
-@ Core fucosylation within tetra-antennary glycans with α2,6-linked sialic acid
-$ A4EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
+# Core fucosylation within tetra-antennary glycans with α2,6-linked sialic acid
+A4EFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
 
-@ Core fucosylation within monoantennary glycans without α2,6-linked sialic acid
-$ A1E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
+# Core fucosylation within monoantennary glycans without α2,6-linked sialic acid
+A1E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
 
-@ Core fucosylation within diantennary glycans without α2,6-linked sialic acid
-$ A2E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
+# Core fucosylation within diantennary glycans without α2,6-linked sialic acid
+A2E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
 
-@ Core fucosylation within triantennary glycans without α2,6-linked sialic acid
-$ A3E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
+# Core fucosylation within triantennary glycans without α2,6-linked sialic acid
+A3E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
 
-@ Core fucosylation within tetra-antennary glycans without α2,6-linked sialic acid
-$ A4E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
+# Core fucosylation within tetra-antennary glycans without α2,6-linked sialic acid
+A4E0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
 
-@ Core fucosylation within monoantennary glycans with α2,3-linked sialic acid
-$ A1LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
+# Core fucosylation within monoantennary glycans with α2,3-linked sialic acid
+A1LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
 
-@ Core fucosylation within diantennary glycans with α2,3-linked sialic acid
-$ A2LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
+# Core fucosylation within diantennary glycans with α2,3-linked sialic acid
+A2LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
 
-@ Core fucosylation within triantennary glycans with α2,3-linked sialic acid
-$ A3LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
+# Core fucosylation within triantennary glycans with α2,3-linked sialic acid
+A3LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
 
-@ Core fucosylation within tetra-antennary glycans with α2,3-linked sialic acid
-$ A4LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
+# Core fucosylation within tetra-antennary glycans with α2,3-linked sialic acid
+A4LFc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
 
-@ Core fucosylation within monoantennary glycans without α2,3-linked sialic acid
-$ A1L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
+# Core fucosylation within monoantennary glycans without α2,3-linked sialic acid
+A1L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
 
-@ Core fucosylation within diantennary glycans without α2,3-linked sialic acid
-$ A2L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
+# Core fucosylation within diantennary glycans without α2,3-linked sialic acid
+A2L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
 
-@ Core fucosylation within triantennary glycans without α2,3-linked sialic acid
-$ A3L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
+# Core fucosylation within triantennary glycans without α2,3-linked sialic acid
+A3L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
 
-@ Core fucosylation within tetra-antennary glycans without α2,3-linked sialic acid
-$ A4L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
+# Core fucosylation within tetra-antennary glycans without α2,3-linked sialic acid
+A4L0Fc = [nFc > 0] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
 
 
 # Antennary fucosylation
 
-@ Antennary fucosylation within complex type glycans
-$ CFa = [nFa] // [type == 'complex']
+# Antennary fucosylation within complex type glycans
+CFa = [nFa] // [type == 'complex']
 
-@ Antennary fucosylation within monoantennary glycans
-$ A1Fa = [nFa] // [(type == 'complex') * (nAnt == 1)]
+# Antennary fucosylation within monoantennary glycans
+A1Fa = [nFa] // [(type == 'complex') * (nAnt == 1)]
 
-@ Antennary fucosylation within diantennary glycans
-$ A2Fa = [nFa] // [(type == 'complex') * (nAnt == 2)]
+# Antennary fucosylation within diantennary glycans
+A2Fa = [nFa] // [(type == 'complex') * (nAnt == 2)]
 
-@ Antennary fucosylation within triantennary glycans
-$ A3Fa = [nFa] // [(type == 'complex') * (nAnt == 3)]
+# Antennary fucosylation within triantennary glycans
+A3Fa = [nFa] // [(type == 'complex') * (nAnt == 3)]
 
-@ Antennary fucosylation within tetra-antennary glycans
-$ A4Fa = [nFa] // [(type == 'complex') * (nAnt == 4)]
+# Antennary fucosylation within tetra-antennary glycans
+A4Fa = [nFa] // [(type == 'complex') * (nAnt == 4)]
 
-@ Antennary fucosylation within sialylated monoantennary glycans
-$ A1SFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
+# Antennary fucosylation within sialylated monoantennary glycans
+A1SFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
 
-@ Antennary fucosylation within sialylated diantennary glycans
-$ A2SFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
+# Antennary fucosylation within sialylated diantennary glycans
+A2SFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
 
-@ Antennary fucosylation within sialylated triantennary glycans
-$ A3SFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
+# Antennary fucosylation within sialylated triantennary glycans
+A3SFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
 
-@ Antennary fucosylation within sialylated tetra-antennary glycans
-$ A4SFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
+# Antennary fucosylation within sialylated tetra-antennary glycans
+A4SFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
 
-@ Antennary fucosylation within non-sialylated monoantennary glycans
-$ A1S0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
+# Antennary fucosylation within non-sialylated monoantennary glycans
+A1S0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
 
-@ Antennary fucosylation within non-sialylated diantennary glycans
-$ A2S0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
+# Antennary fucosylation within non-sialylated diantennary glycans
+A2S0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
 
-@ Antennary fucosylation within non-sialylated triantennary glycans
-$ A3S0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
+# Antennary fucosylation within non-sialylated triantennary glycans
+A3S0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
 
-@ Antennary fucosylation within non-sialylated tetra-antennary glycans
-$ A4S0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
+# Antennary fucosylation within non-sialylated tetra-antennary glycans
+A4S0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
 
-@ Antennary fucosylation within monoantennary glycans with α2,6-linked sialic acid
-$ A1EFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nE > 0)]
+# Antennary fucosylation within monoantennary glycans with α2,6-linked sialic acid
+A1EFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nE > 0)]
 
-@ Antennary fucosylation within diantennary glycans with α2,6-linked sialic acid
-$ A2EFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
+# Antennary fucosylation within diantennary glycans with α2,6-linked sialic acid
+A2EFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
 
-@ Antennary fucosylation within triantennary glycans with α2,6-linked sialic acid
-$ A3EFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
+# Antennary fucosylation within triantennary glycans with α2,6-linked sialic acid
+A3EFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
 
-@ Antennary fucosylation within tetra-antennary glycans with α2,6-linked sialic acid
-$ A4EFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
+# Antennary fucosylation within tetra-antennary glycans with α2,6-linked sialic acid
+A4EFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
 
-@ Antennary fucosylation within monoantennary glycans without α2,6-linked sialic acid
-$ A1E0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
+# Antennary fucosylation within monoantennary glycans without α2,6-linked sialic acid
+A1E0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
 
-@ Antennary fucosylation within diantennary glycans without α2,6-linked sialic acid
-$ A2E0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
+# Antennary fucosylation within diantennary glycans without α2,6-linked sialic acid
+A2E0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
 
-@ Antennary fucosylation within triantennary glycans without α2,6-linked sialic acid
-$ A3E0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
+# Antennary fucosylation within triantennary glycans without α2,6-linked sialic acid
+A3E0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
 
-@ Antennary fucosylation within tetra-antennary glycans without α2,6-linked sialic acid
-$ A4E0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
+# Antennary fucosylation within tetra-antennary glycans without α2,6-linked sialic acid
+A4E0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
 
-@ Antennary fucosylation within monoantennary glycans with α2,3-linked sialic acid
-$ A1LFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
+# Antennary fucosylation within monoantennary glycans with α2,3-linked sialic acid
+A1LFa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
 
-@ Antennary fucosylation within diantennary glycans with α2,3-linked sialic acid
-$ A2LFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
+# Antennary fucosylation within diantennary glycans with α2,3-linked sialic acid
+A2LFa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
 
-@ Antennary fucosylation within triantennary glycans with α2,3-linked sialic acid
-$ A3LFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
+# Antennary fucosylation within triantennary glycans with α2,3-linked sialic acid
+A3LFa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
 
-@ Antennary fucosylation within tetra-antennary glycans with α2,3-linked sialic acid
-$ A4LFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
+# Antennary fucosylation within tetra-antennary glycans with α2,3-linked sialic acid
+A4LFa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
 
-@ Antennary fucosylation within monoantennary glycans without α2,3-linked sialic acid
-$ A1L0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
+# Antennary fucosylation within monoantennary glycans without α2,3-linked sialic acid
+A1L0Fa = [nFa] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
 
-@ Antennary fucosylation within diantennary glycans without α2,3-linked sialic acid
-$ A2L0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
+# Antennary fucosylation within diantennary glycans without α2,3-linked sialic acid
+A2L0Fa = [nFa] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
 
-@ Antennary fucosylation within triantennary glycans without α2,3-linked sialic acid
-$ A3L0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
+# Antennary fucosylation within triantennary glycans without α2,3-linked sialic acid
+A3L0Fa = [nFa] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
 
-@ Antennary fucosylation within tetra-antennary glycans without α2,3-linked sialic acid
-$ A4L0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
+# Antennary fucosylation within tetra-antennary glycans without α2,3-linked sialic acid
+A4L0Fa = [nFa] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
 
 
 # Bisection
 
-@ Relative abundance of species with a bisecting GlcNAc within all complex glycans
-$ CB = [B] // [type == 'complex']
+# Relative abundance of species with a bisecting GlcNAc within all complex glycans
+CB = [B] // [type == 'complex']
 
-@ Relative abundance of species with a bisecting GlcNAc within diantennary glycans
-$ A2B = [B] // [(type == 'complex') * (nAnt == 2)]
+# Relative abundance of species with a bisecting GlcNAc within diantennary glycans
+A2B = [B] // [(type == 'complex') * (nAnt == 2)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated diantennary
-$ A2FB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated diantennary
+A2FB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated diantennary glycans
-$ A2F0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated diantennary glycans
+A2F0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within sialylated diantennary glycans
-$ A2SB = [B] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within sialylated diantennary glycans
+A2SB = [B] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-sialylated diantennary glycans
-$ A2S0B = [B] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-sialylated diantennary glycans
+A2S0B = [B] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated diantennary glycans
-$ A2FSB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated diantennary glycans
+A2FSB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated diantennary glycans
-$ A2F0SB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated diantennary glycans
+A2F0SB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated diantennary glycans
-$ A2FS0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated diantennary glycans
+A2FS0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated diantennary glycans
-$ A2F0S0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated diantennary glycans
+A2F0S0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated diantennary glycans
-$ A2LB = [B] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated diantennary glycans
+A2LB = [B] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated diantennary glycans
-$ A2L0B = [B] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated diantennary glycans
+A2L0B = [B] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated diantennary glycans
-$ A2FLB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated diantennary glycans
+A2FLB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated diantennary glycans
-$ A2F0LB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated diantennary glycans
+A2F0LB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated diantennary glycans
-$ A2FL0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated diantennary glycans
+A2FL0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated diantennary glycans
-$ A2F0L0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated diantennary glycans
+A2F0L0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated diantennary glycans
-$ A2EB = [B] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated diantennary glycans
+A2EB = [B] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated diantennary glycans
-$ A2E0B = [B] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated diantennary glycans
+A2E0B = [B] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated diantennary glycans
-$ A2FEB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated diantennary glycans
+A2FEB = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated diantennary glycans
-$ A2F0EB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated diantennary glycans
+A2F0EB = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated diantennary glycans
-$ A2FE0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated diantennary glycans
+A2FE0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated diantennary glycans
-$ A2F0E0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated diantennary glycans
+A2F0E0B = [B] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within triantennary glycans
-$ A3B = [B] // [(type == 'complex') * (nAnt == 3)]
+# Relative abundance of species with a bisecting GlcNAc within triantennary glycans
+A3B = [B] // [(type == 'complex') * (nAnt == 3)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated triantennary glycans
-$ A3FB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated triantennary glycans
+A3FB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated triantennary glycans
-$ A3F0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated triantennary glycans
+A3F0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within sialylated triantennary glycans
-$ A3SB = [B] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within sialylated triantennary glycans
+A3SB = [B] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-sialylated triantennary glycans
-$ A3S0B = [B] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-sialylated triantennary glycans
+A3S0B = [B] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated triantennary glycans
-$ A3FSB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated triantennary glycans
+A3FSB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated triantennary glycans
-$ A3F0SB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated triantennary glycans
+A3F0SB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated triantennary glycans
-$ A3FS0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated triantennary glycans
+A3FS0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated triantennary glycans
-$ A3F0S0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated triantennary glycans
+A3F0S0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated triantennary glycans
-$ A3LB = [B] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated triantennary glycans
+A3LB = [B] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated triantennary glycans
-$ A3L0B = [B] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated triantennary glycans
+A3L0B = [B] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated triantennary glycans
-$ A3FLB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated triantennary glycans
+A3FLB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated triantennary glycans
-$ A3F0LB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated triantennary glycans
+A3F0LB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated triantennary glycans
-$ A3FL0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated triantennary glycans
+A3FL0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated triantennary glycans
-$ A3F0L0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated triantennary glycans
+A3F0L0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated triantennary glycans
-$ A3EB = [B] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated triantennary glycans
+A3EB = [B] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated triantennary glycans
-$ A3E0B = [B] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated triantennary glycans
+A3E0B = [B] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated triantennary glycans
-$ A3FEB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated triantennary glycans
+A3FEB = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated triantennary glycans
-$ A3F0EB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated triantennary glycans
+A3F0EB = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated triantennary glycans
-$ A3FE0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated triantennary glycans
+A3FE0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated triantennary glycans
-$ A3F0E0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated triantennary glycans
+A3F0E0B = [B] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within tetra-antennary glycans
-$ A4B = [B] // [(type == 'complex') * (nAnt == 4)]
+# Relative abundance of species with a bisecting GlcNAc within tetra-antennary glycans
+A4B = [B] // [(type == 'complex') * (nAnt == 4)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated tetra-antennary glycans
-$ A4FB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated tetra-antennary glycans
+A4FB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated tetra-antennary glycans
-$ A4F0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated tetra-antennary glycans
+A4F0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within sialylated tetra-antennary glycans
-$ A4SB = [B] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within sialylated tetra-antennary glycans
+A4SB = [B] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-sialylated tetra-antennary glycans
-$ A4S0B = [B] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-sialylated tetra-antennary glycans
+A4S0B = [B] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated tetra-antennary glycans
-$ A4FSB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated sialylated tetra-antennary glycans
+A4FSB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated tetra-antennary glycans
-$ A4F0SB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated sialylated tetra-antennary glycans
+A4F0SB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated tetra-antennary glycans
-$ A4FS0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-sialylated tetra-antennary glycans
+A4FS0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated tetra-antennary glycans
-$ A4F0S0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-sialylated tetra-antennary glycans
+A4F0S0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated tetra-antennary glycans
-$ A4LB = [B] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,3-sialylated tetra-antennary glycans
+A4LB = [B] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated tetra-antennary glycans
-$ A4L0B = [B] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,3-sialylated tetra-antennary glycans
+A4L0B = [B] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4FLB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,3-sialylated tetra-antennary glycans
+A4FLB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4F0LB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,3-sialylated tetra-antennary glycans
+A4F0LB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated tetra-antennary glycans
-$ A4FL0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,3-sialylated tetra-antennary glycans
+A4FL0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated tetra-antennary glycans
-$ A4F0L0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,3-sialylated tetra-antennary glycans
+A4F0L0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated tetra-antennary glycans
-$ A4EB = [B] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within a2,6-sialylated tetra-antennary glycans
+A4EB = [B] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated tetra-antennary glycans
-$ A4E0B = [B] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-a2,6-sialylated tetra-antennary glycans
+A4E0B = [B] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4FEB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated a2,6-sialylated tetra-antennary glycans
+A4FEB = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4F0EB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated a2,6-sialylated tetra-antennary glycans
+A4F0EB = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated tetra-antennary glycans
-$ A4FE0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within fucosylated non-a2,6-sialylated tetra-antennary glycans
+A4FE0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated tetra-antennary glycans
-$ A4F0E0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with a bisecting GlcNAc within non-fucosylated non-a2,6-sialylated tetra-antennary glycans
+A4F0E0B = [B] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
 
 
 # Galactosylaiton
 
-@ Average number of galactoses on complex glycans
-$ CG = [nG] // [type == 'complex']
+# Average number of galactoses on complex glycans
+CG = [nG] // [type == 'complex']
 
-@ Galactosylation per antenna within monoantennary glycans
-$ A1G = [nG] // [(type == 'complex') * (nAnt == 1)]
+# Galactosylation per antenna within monoantennary glycans
+A1G = [nG] // [(type == 'complex') * (nAnt == 1)]
 
-@ Galactosylation per antenna within diantennary glycans
-$ A2G = [nG / 2] // [(type == 'complex') * (nAnt == 2)]
+# Galactosylation per antenna within diantennary glycans
+A2G = [nG / 2] // [(type == 'complex') * (nAnt == 2)]
 
-@ Galactosylation per antenna within triantennary glycans
-$ A3G = [nG / 3] // [(type == 'complex') * (nAnt == 3)]
+# Galactosylation per antenna within triantennary glycans
+A3G = [nG / 3] // [(type == 'complex') * (nAnt == 3)]
 
-@ Galactosylation per antenna within tetra-antennary glycans
-$ A4G = [nG / 4] // [(type == 'complex') * (nAnt == 4)]
+# Galactosylation per antenna within tetra-antennary glycans
+A4G = [nG / 4] // [(type == 'complex') * (nAnt == 4)]
 
-@ Galactosylation per antenna within fucosylated monoantennary glycans
-$ A1FG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# Galactosylation per antenna within fucosylated monoantennary glycans
+A1FG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ Galactosylation per antenna within fucosylated diantennary glycans
-$ A2FG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# Galactosylation per antenna within fucosylated diantennary glycans
+A2FG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ Galactosylation per antenna within fucosylated triantennary glycans
-$ A3FG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# Galactosylation per antenna within fucosylated triantennary glycans
+A3FG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ Galactosylation per antenna within fucosylated tetra-antennary glycans
-$ A4FG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# Galactosylation per antenna within fucosylated tetra-antennary glycans
+A4FG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ Galactosylation per antenna within non-fucosylated monoantennary glycans
-$ A1F0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# Galactosylation per antenna within non-fucosylated monoantennary glycans
+A1F0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ Galactosylation per antenna within non-fucosylated diantennary glycans
-$ A2F0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# Galactosylation per antenna within non-fucosylated diantennary glycans
+A2F0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ Galactosylation per antenna within non-fucosylated triantennary glycans
-$ A3F0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# Galactosylation per antenna within non-fucosylated triantennary glycans
+A3F0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ Galactosylation per antenna within non-fucosylated tetra-antennary glycans
-$ A4F0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# Galactosylation per antenna within non-fucosylated tetra-antennary glycans
+A4F0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ Galactosylation per antenna within sialylated monoantennary glycans
-$ A1SG = [nG] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
+# Galactosylation per antenna within sialylated monoantennary glycans
+A1SG = [nG] // [(type == 'complex') * (nAnt == 1) * (nS > 0)]
 
-@ Galactosylation per antenna within sialylated diantennary glycans
-$ A2SG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
+# Galactosylation per antenna within sialylated diantennary glycans
+A2SG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
 
-@ Galactosylation per antenna within sialylated triantennary glycans
-$ A3SG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
+# Galactosylation per antenna within sialylated triantennary glycans
+A3SG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
 
-@ Galactosylation per antenna within sialylated tetra-antennary glycans
-$ A4SG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
+# Galactosylation per antenna within sialylated tetra-antennary glycans
+A4SG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
 
-@ Galactosylation per antenna within non-sialylated monoantennary glycans
-$ A1S0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
+# Galactosylation per antenna within non-sialylated monoantennary glycans
+A1S0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nS == 0)]
 
-@ Galactosylation per antenna within non-sialylated diantennary glycans
-$ A2S0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
+# Galactosylation per antenna within non-sialylated diantennary glycans
+A2S0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
 
-@ Galactosylation per antenna within non-sialylated triantennary glycans
-$ A3S0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
+# Galactosylation per antenna within non-sialylated triantennary glycans
+A3S0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
 
-@ Galactosylation per antenna within non-sialylated tetra-antennary glycans
-$ A4S0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
+# Galactosylation per antenna within non-sialylated tetra-antennary glycans
+A4S0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
 
-@ Galactosylation per antenna within fucosylated sialylated monoantennary glycans
-$ A2FSG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nS > 0)]
+# Galactosylation per antenna within fucosylated sialylated monoantennary glycans
+A2FSG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nS > 0)]
 
-@ Galactosylation per antenna within fucosylated sialylated diantennary glycans
-$ A2FSG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
+# Galactosylation per antenna within fucosylated sialylated diantennary glycans
+A2FSG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
 
-@ Galactosylation per antenna within fucosylated sialylated triantennary glycans
-$ A3FSG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
+# Galactosylation per antenna within fucosylated sialylated triantennary glycans
+A3FSG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
 
-@ Galactosylation per antenna within fucosylated sialylated tetra-antennary glycans
-$ A4FSG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
+# Galactosylation per antenna within fucosylated sialylated tetra-antennary glycans
+A4FSG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
 
-@ Galactosylation per antenna within non-fucosylated sialylated monoantennary glycans
-$ A1F0SG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nS > 0)]
+# Galactosylation per antenna within non-fucosylated sialylated monoantennary glycans
+A1F0SG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nS > 0)]
 
-@ Galactosylation per antenna within non-fucosylated sialylated diantennary glycans
-$ A2F0SG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
+# Galactosylation per antenna within non-fucosylated sialylated diantennary glycans
+A2F0SG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
 
-@ Galactosylation per antenna within non-fucosylated sialylated triantennary glycans
-$ A3F0SG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
+# Galactosylation per antenna within non-fucosylated sialylated triantennary glycans
+A3F0SG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
 
-@ Galactosylation per antenna within non-fucosylated sialylated tetra-antennary glycans
-$ A4F0SG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
+# Galactosylation per antenna within non-fucosylated sialylated tetra-antennary glycans
+A4F0SG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
 
-@ Galactosylation per antenna within fucosylated non-sialylated monoantennary glycans
-$ A1FS0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nS == 0)]
+# Galactosylation per antenna within fucosylated non-sialylated monoantennary glycans
+A1FS0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nS == 0)]
 
-@ Galactosylation per antenna within fucosylated non-sialylated diantennary glycans
-$ A2FS0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
+# Galactosylation per antenna within fucosylated non-sialylated diantennary glycans
+A2FS0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
 
-@ Galactosylation per antenna within fucosylated non-sialylated triantennary glycans
-$ A3FS0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
+# Galactosylation per antenna within fucosylated non-sialylated triantennary glycans
+A3FS0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
 
-@ Galactosylation per antenna within fucosylated non-sialylated tetra-antennary glycans
-$ A4FS0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
+# Galactosylation per antenna within fucosylated non-sialylated tetra-antennary glycans
+A4FS0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-sialylated monoantennary glycans
-$ A1F0S0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nS == 0)]
+# Galactosylation per antenna within non-fucosylated, non-sialylated monoantennary glycans
+A1F0S0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nS == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-sialylated diantennary glycans
-$ A2F0S0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
+# Galactosylation per antenna within non-fucosylated, non-sialylated diantennary glycans
+A2F0S0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-sialylated triantennary glycans
-$ A3F0S0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
+# Galactosylation per antenna within non-fucosylated, non-sialylated triantennary glycans
+A3F0S0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-sialylated tetra-antennary glycans
-$ A4F0S0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
+# Galactosylation per antenna within non-fucosylated, non-sialylated tetra-antennary glycans
+A4F0S0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
 
-@ Galactosylation per antenna within a2,3-sialylated monoantennary glycans
-$ A1LG = [nG] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
+# Galactosylation per antenna within a2,3-sialylated monoantennary glycans
+A1LG = [nG] // [(type == 'complex') * (nAnt == 1) * (nL > 0)]
 
-@ Galactosylation per antenna within a2,3-sialylated diantennary glycans
-$ A2LG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
+# Galactosylation per antenna within a2,3-sialylated diantennary glycans
+A2LG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
 
-@ Galactosylation per antenna within a2,3-sialylated triantennary glycans
-$ A3LG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
+# Galactosylation per antenna within a2,3-sialylated triantennary glycans
+A3LG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
 
-@ Galactosylation per antenna within a2,3-sialylated tetra-antennary glycans
-$ A4LG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
+# Galactosylation per antenna within a2,3-sialylated tetra-antennary glycans
+A4LG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
 
-@ Galactosylation per antenna within non-a2,3-sialylated monoantennary glycans
-$ A1L0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
+# Galactosylation per antenna within non-a2,3-sialylated monoantennary glycans
+A1L0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nL == 0)]
 
-@ Galactosylation per antenna within non-a2,3-sialylated diantennary glycans
-$ A2L0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
+# Galactosylation per antenna within non-a2,3-sialylated diantennary glycans
+A2L0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
 
-@ Galactosylation per antenna within non-a2,3-sialylated triantennary glycans
-$ A3L0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
+# Galactosylation per antenna within non-a2,3-sialylated triantennary glycans
+A3L0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
 
-@ Galactosylation per antenna within non-a2,3-sialylated tetra-antennary glycans
-$ A4L0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
+# Galactosylation per antenna within non-a2,3-sialylated tetra-antennary glycans
+A4L0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
 
-@ Galactosylation per antenna within fucosylated a2,3-sialylated monoantennary glycans
-$ A1FLG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nL > 0)]
+# Galactosylation per antenna within fucosylated a2,3-sialylated monoantennary glycans
+A1FLG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nL > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,3-sialylated diantennary glycans
-$ A2FLG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
+# Galactosylation per antenna within fucosylated a2,3-sialylated diantennary glycans
+A2FLG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,3-sialylated triantennary glycans
-$ A3FLG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
+# Galactosylation per antenna within fucosylated a2,3-sialylated triantennary glycans
+A3FLG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4FLG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
+# Galactosylation per antenna within fucosylated a2,3-sialylated tetra-antennary glycans
+A4FLG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,3-sialylated monoantennary glycans
-$ A1F0LG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nL > 0)]
+# Galactosylation per antenna within non-fucosylated a2,3-sialylated monoantennary glycans
+A1F0LG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nL > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,3-sialylated diantennary glycans
-$ A2F0LG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
+# Galactosylation per antenna within non-fucosylated a2,3-sialylated diantennary glycans
+A2F0LG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,3-sialylated triantennary glycans
-$ A3F0LG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
+# Galactosylation per antenna within non-fucosylated a2,3-sialylated triantennary glycans
+A3F0LG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4F0LG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
+# Galactosylation per antenna within non-fucosylated a2,3-sialylated tetra-antennary glycans
+A4F0LG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,3-sialylated monoantennary glycans
-$ A1FL0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nL == 0)]
+# Galactosylation per antenna within fucosylated non-a2,3-sialylated monoantennary glycans
+A1FL0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nL == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,3-sialylated diantennary glycans
-$ A2FL0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
+# Galactosylation per antenna within fucosylated non-a2,3-sialylated diantennary glycans
+A2FL0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,3-sialylated triantennary glycans
-$ A3FL0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
+# Galactosylation per antenna within fucosylated non-a2,3-sialylated triantennary glycans
+A3FL0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,3-sialylated tetra-antennary glycans
-$ A4FL0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
+# Galactosylation per antenna within fucosylated non-a2,3-sialylated tetra-antennary glycans
+A4FL0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated monoantennary glycans
-$ A1F0L0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nL == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated monoantennary glycans
+A1F0L0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nL == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated diantennary glycans
-$ A2F0L0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated diantennary glycans
+A2F0L0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated triantennary glycans
-$ A3F0L0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated triantennary glycans
+A3F0L0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated tetra-antennary glycans
-$ A4F0L0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,3-sialylated tetra-antennary glycans
+A4F0L0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
 
-@ Galactosylation per antenna within a2,6-sialylated monoantennary glycans
-$ A1EG = [nG] // [(type == 'complex') * (nAnt == 1) * (nE > 0)]
+# Galactosylation per antenna within a2,6-sialylated monoantennary glycans
+A1EG = [nG] // [(type == 'complex') * (nAnt == 1) * (nE > 0)]
 
-@ Galactosylation per antenna within a2,6-sialylated diantennary glycans
-$ A2EG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
+# Galactosylation per antenna within a2,6-sialylated diantennary glycans
+A2EG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
 
-@ Galactosylation per antenna within a2,6-sialylated triantennary glycans
-$ A3EG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
+# Galactosylation per antenna within a2,6-sialylated triantennary glycans
+A3EG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
 
-@ Galactosylation per antenna within a2,6-sialylated tetra-antennary glycans
-$ A4EG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
+# Galactosylation per antenna within a2,6-sialylated tetra-antennary glycans
+A4EG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
 
-@ Galactosylation per antenna within non-a2,6-sialylated monoantennary glycans
-$ A1E0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
+# Galactosylation per antenna within non-a2,6-sialylated monoantennary glycans
+A1E0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nE == 0)]
 
-@ Galactosylation per antenna within non-a2,6-sialylated diantennary glycans
-$ A2E0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
+# Galactosylation per antenna within non-a2,6-sialylated diantennary glycans
+A2E0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
 
-@ Galactosylation per antenna within non-a2,6-sialylated triantennary glycans
-$ A3E0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
+# Galactosylation per antenna within non-a2,6-sialylated triantennary glycans
+A3E0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
 
-@ Galactosylation per antenna within non-a2,6-sialylated tetra-antennary glycans
-$ A4E0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
+# Galactosylation per antenna within non-a2,6-sialylated tetra-antennary glycans
+A4E0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
 
-@ Galactosylation per antenna within fucosylated a2,6-sialylated monoantennary glycans
-$ A1FEG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nE > 0)]
+# Galactosylation per antenna within fucosylated a2,6-sialylated monoantennary glycans
+A1FEG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nE > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,6-sialylated diantennary glycans
-$ A2FEG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
+# Galactosylation per antenna within fucosylated a2,6-sialylated diantennary glycans
+A2FEG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,6-sialylated triantennary glycans
-$ A3FEG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
+# Galactosylation per antenna within fucosylated a2,6-sialylated triantennary glycans
+A3FEG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
 
-@ Galactosylation per antenna within fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4FEG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
+# Galactosylation per antenna within fucosylated a2,6-sialylated tetra-antennary glycans
+A4FEG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,6-sialylated monoantennary glycans
-$ A1F0EG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nE > 0)]
+# Galactosylation per antenna within non-fucosylated a2,6-sialylated monoantennary glycans
+A1F0EG = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nE > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,6-sialylated diantennary glycans
-$ A2F0EG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
+# Galactosylation per antenna within non-fucosylated a2,6-sialylated diantennary glycans
+A2F0EG = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,6-sialylated triantennary glycans
-$ A3F0EG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
+# Galactosylation per antenna within non-fucosylated a2,6-sialylated triantennary glycans
+A3F0EG = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
 
-@ Galactosylation per antenna within non-fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4F0EG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
+# Galactosylation per antenna within non-fucosylated a2,6-sialylated tetra-antennary glycans
+A4F0EG = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,6-sialylated monoantennary glycans
-$ A1FE0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nE == 0)]
+# Galactosylation per antenna within fucosylated non-a2,6-sialylated monoantennary glycans
+A1FE0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0) * (nE == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,6-sialylated diantennary glycans
-$ A2FE0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
+# Galactosylation per antenna within fucosylated non-a2,6-sialylated diantennary glycans
+A2FE0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,6-sialylated triantennary glycans
-$ A3FE0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
+# Galactosylation per antenna within fucosylated non-a2,6-sialylated triantennary glycans
+A3FE0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
 
-@ Galactosylation per antenna within fucosylated non-a2,6-sialylated tetra-antennary glycans
-$ A4FE0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
+# Galactosylation per antenna within fucosylated non-a2,6-sialylated tetra-antennary glycans
+A4FE0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated monoantennary glycans
-$ A1F0E0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nE == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated monoantennary glycans
+A1F0E0G = [nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0) * (nE == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated diantennary glycans
-$ A2F0E0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated diantennary glycans
+A2F0E0G = [nG / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated triantennary glycans
-$ A3F0E0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated triantennary glycans
+A3F0E0G = [nG / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
 
-@ Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated tetra-antennary glycans
-$ A4F0E0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
+# Galactosylation per antenna within non-fucosylated, non-a2,6-sialylated tetra-antennary glycans
+A4F0E0G = [nG / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
 
 
 # Sialylation
 
-@ Average number of sialic acids on complex glycans
-$ CS = [nS] // [type == 'complex']
+# Average number of sialic acids on complex glycans
+CS = [nS] // [type == 'complex']
 
-@ Sialylation per antenna within monoantennary glycans
-$ A1S = [nS] // [(type == 'complex') * (nAnt == 1)]
+# Sialylation per antenna within monoantennary glycans
+A1S = [nS] // [(type == 'complex') * (nAnt == 1)]
 
-@ Sialylation per antenna within diantennary glycans
-$ A2S = [nS / 2] // [(type == 'complex') * (nAnt == 2)]
+# Sialylation per antenna within diantennary glycans
+A2S = [nS / 2] // [(type == 'complex') * (nAnt == 2)]
 
-@ Sialylation per antenna within triantennary glycans
-$ A3S = [nS / 3] // [(type == 'complex') * (nAnt == 3)]
+# Sialylation per antenna within triantennary glycans
+A3S = [nS / 3] // [(type == 'complex') * (nAnt == 3)]
 
-@ Sialylation per antenna within tetra-antennary glycans
-$ A4S = [nS / 4] // [(type == 'complex') * (nAnt == 4)]
+# Sialylation per antenna within tetra-antennary glycans
+A4S = [nS / 4] // [(type == 'complex') * (nAnt == 4)]
 
-@ Sialylation per antenna within fucosylated monoantennary glycans
-$ A1FS = [nS] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# Sialylation per antenna within fucosylated monoantennary glycans
+A1FS = [nS] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ Sialylation per antenna within fucosylated diantennary glycans
-$ A2FS = [nS / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# Sialylation per antenna within fucosylated diantennary glycans
+A2FS = [nS / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ Sialylation per antenna within fucosylated triantennary glycans
-$ A3FS = [nS / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# Sialylation per antenna within fucosylated triantennary glycans
+A3FS = [nS / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ Sialylation per antenna within fucosylated tetra-antennary glycans
-$ A4FS = [nS / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# Sialylation per antenna within fucosylated tetra-antennary glycans
+A4FS = [nS / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ Sialylation per antenna within non-fucosylated monoantennary glycans
-$ A1F0S = [nS] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# Sialylation per antenna within non-fucosylated monoantennary glycans
+A1F0S = [nS] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ Sialylation per antenna within non-fucosylated diantennary glycans
-$ A2F0S = [nS / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# Sialylation per antenna within non-fucosylated diantennary glycans
+A2F0S = [nS / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ Sialylation per antenna within non-fucosylated triantennary glycans
-$ A3F0S = [nS / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# Sialylation per antenna within non-fucosylated triantennary glycans
+A3F0S = [nS / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ Sialylation per antenna within non-fucosylated tetra-antennary glycans
-$ A4F0S = [nS / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# Sialylation per antenna within non-fucosylated tetra-antennary glycans
+A4F0S = [nS / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ Sialylation per galactose within monoantennary glycans
-$ A1GS = [nS / nG] // [(type == 'complex') * (nAnt == 1)]
+# Sialylation per galactose within monoantennary glycans
+A1GS = [nS / nG] // [(type == 'complex') * (nAnt == 1)]
 
-@ Sialylation per galactose within diantennary glycans
-$ A2GS = [nS / nG] // [(type == 'complex') * (nAnt == 2)]
+# Sialylation per galactose within diantennary glycans
+A2GS = [nS / nG] // [(type == 'complex') * (nAnt == 2)]
 
-@ Sialylation per galactose within triantennary glycans
-$ A3GS = [nS / nG] // [(type == 'complex') * (nAnt == 3)]
+# Sialylation per galactose within triantennary glycans
+A3GS = [nS / nG] // [(type == 'complex') * (nAnt == 3)]
 
-@ Sialylation per galactose within tetra-antennary glycans
-$ A4GS = [nS / nG] // [(type == 'complex') * (nAnt == 4)]
+# Sialylation per galactose within tetra-antennary glycans
+A4GS = [nS / nG] // [(type == 'complex') * (nAnt == 4)]
 
-@ Sialylation per galactose within fucosylated monoantennary glycans
-$ A1FGS = [nS / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# Sialylation per galactose within fucosylated monoantennary glycans
+A1FGS = [nS / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ Sialylation per galactose within fucosylated diantennary glycans
-$ A2FGS = [nS / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# Sialylation per galactose within fucosylated diantennary glycans
+A2FGS = [nS / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ Sialylation per galactose within fucosylated triantennary glycans
-$ A3FGS = [nS / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# Sialylation per galactose within fucosylated triantennary glycans
+A3FGS = [nS / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ Sialylation per galactose within fucosylated tetra-antennary glycans
-$ A4FGS = [nS / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# Sialylation per galactose within fucosylated tetra-antennary glycans
+A4FGS = [nS / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ Sialylation per galactose within non-fucosylated monoantennary glycans
-$ A1F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# Sialylation per galactose within non-fucosylated monoantennary glycans
+A1F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ Sialylation per galactose within non-fucosylated diantennary glycans
-$ A2F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# Sialylation per galactose within non-fucosylated diantennary glycans
+A2F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ Sialylation per galactose within non-fucosylated triantennary glycans
-$ A3F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# Sialylation per galactose within non-fucosylated triantennary glycans
+A3F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ Sialylation per galactose within non-fucosylated tetra-antennary glycans
-$ A4F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# Sialylation per galactose within non-fucosylated tetra-antennary glycans
+A4F0GS = [nS / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
 
 # α2,3-linked sialylation
 
-@ Average number of α2,3-linked sialic acids on complex glycans
-$ CL = [nL] // [type == 'complex']
+# Average number of α2,3-linked sialic acids on complex glycans
+CL = [nL] // [type == 'complex']
 
-@ α2,3-sialylation per antenna within monoantennary glycans
-$ A1L = [nL] // [(type == 'complex') * (nAnt == 1)]
+# α2,3-sialylation per antenna within monoantennary glycans
+A1L = [nL] // [(type == 'complex') * (nAnt == 1)]
 
-@ α2,3-sialylation per antenna within diantennary glycans
-$ A2L = [nL / 2] // [(type == 'complex') * (nAnt == 2)]
+# α2,3-sialylation per antenna within diantennary glycans
+A2L = [nL / 2] // [(type == 'complex') * (nAnt == 2)]
 
-@ α2,3-sialylation per antenna within triantennary glycans
-$ A3L = [nL / 3] // [(type == 'complex') * (nAnt == 3)]
+# α2,3-sialylation per antenna within triantennary glycans
+A3L = [nL / 3] // [(type == 'complex') * (nAnt == 3)]
 
-@ α2,3-sialylation per antenna within tetra-antennary glycans
-$ A4L = [nL / 4] // [(type == 'complex') * (nAnt == 4)]
+# α2,3-sialylation per antenna within tetra-antennary glycans
+A4L = [nL / 4] // [(type == 'complex') * (nAnt == 4)]
 
-@ α2,3-sialylation per antenna within fucosylated monoantennary glycans
-$ A1FL = [nL] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# α2,3-sialylation per antenna within fucosylated monoantennary glycans
+A1FL = [nL] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ α2,3-sialylation per antenna within fucosylated diantennary glycans
-$ A2FL = [nL / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# α2,3-sialylation per antenna within fucosylated diantennary glycans
+A2FL = [nL / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ α2,3-sialylation per antenna within fucosylated triantennary glycans
-$ A3FL = [nL / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# α2,3-sialylation per antenna within fucosylated triantennary glycans
+A3FL = [nL / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ α2,3-sialylation per antenna within fucosylated tetra-antennary glycans
-$ A4FL = [nL / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# α2,3-sialylation per antenna within fucosylated tetra-antennary glycans
+A4FL = [nL / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ α2,3-sialylation per antenna within non-fucosylated monoantennary glycans
-$ A1F0L = [nL] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# α2,3-sialylation per antenna within non-fucosylated monoantennary glycans
+A1F0L = [nL] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ α2,3-sialylation per antenna within non-fucosylated diantennary glycans
-$ A2F0L = [nL / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# α2,3-sialylation per antenna within non-fucosylated diantennary glycans
+A2F0L = [nL / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ α2,3-sialylation per antenna within non-fucosylated triantennary glycans
-$ A3F0L = [nL / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# α2,3-sialylation per antenna within non-fucosylated triantennary glycans
+A3F0L = [nL / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ α2,3-sialylation per antenna within non-fucosylated tetra-antennary glycans
-$ A4F0L = [nL / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# α2,3-sialylation per antenna within non-fucosylated tetra-antennary glycans
+A4F0L = [nL / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ α2,3-sialylation per galactose within monoantennary glycans
-$ A1GL = [nL / nG] // [(type == 'complex') * (nAnt == 1)]
+# α2,3-sialylation per galactose within monoantennary glycans
+A1GL = [nL / nG] // [(type == 'complex') * (nAnt == 1)]
 
-@ α2,3-sialylation per galactose within diantennary glycans
-$ A2GL = [nL / nG] // [(type == 'complex') * (nAnt == 2)]
+# α2,3-sialylation per galactose within diantennary glycans
+A2GL = [nL / nG] // [(type == 'complex') * (nAnt == 2)]
 
-@ α2,3-sialylation per galactose within triantennary glycans
-$ A3GL = [nL / nG] // [(type == 'complex') * (nAnt == 3)]
+# α2,3-sialylation per galactose within triantennary glycans
+A3GL = [nL / nG] // [(type == 'complex') * (nAnt == 3)]
 
-@ α2,3-sialylation per galactose within tetra-antennary glycans
-$ A4GL = [nL / nG] // [(type == 'complex') * (nAnt == 4)]
+# α2,3-sialylation per galactose within tetra-antennary glycans
+A4GL = [nL / nG] // [(type == 'complex') * (nAnt == 4)]
 
-@ α2,3-sialylation per galactose within fucosylated monoantennary glycans
-$ A1FGL = [nL / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# α2,3-sialylation per galactose within fucosylated monoantennary glycans
+A1FGL = [nL / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ α2,3-sialylation per galactose within fucosylated diantennary glycans
-$ A2FGL = [nL / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# α2,3-sialylation per galactose within fucosylated diantennary glycans
+A2FGL = [nL / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ α2,3-sialylation per galactose within fucosylated triantennary glycans
-$ A3FGL = [nL / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# α2,3-sialylation per galactose within fucosylated triantennary glycans
+A3FGL = [nL / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ α2,3-sialylation per galactose within fucosylated tetra-antennary glycans
-$ A4FGL = [nL / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# α2,3-sialylation per galactose within fucosylated tetra-antennary glycans
+A4FGL = [nL / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ α2,3-sialylation per galactose within non-fucosylated monoantennary glycans
-$ A1F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# α2,3-sialylation per galactose within non-fucosylated monoantennary glycans
+A1F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ α2,3-sialylation per galactose within non-fucosylated diantennary glycans
-$ A2F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# α2,3-sialylation per galactose within non-fucosylated diantennary glycans
+A2F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ α2,3-sialylation per galactose within non-fucosylated triantennary glycans
-$ A3F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# α2,3-sialylation per galactose within non-fucosylated triantennary glycans
+A3F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ α2,3-sialylation per galactose within non-fucosylated tetra-antennary glycans
-$ A4F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# α2,3-sialylation per galactose within non-fucosylated tetra-antennary glycans
+A4F0GL = [nL / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
 
 # α2,6-linked sialylation
 
-@ Average number of α2,6-linked sialic acids on complex glycans
-$ CE = [nE] // [type == 'complex']
+# Average number of α2,6-linked sialic acids on complex glycans
+CE = [nE] // [type == 'complex']
 
-@ α2,6-sialylation per antenna within monoantennary glycans
-$ A1E = [nE] // [(type == 'complex') * (nAnt == 1)]
+# α2,6-sialylation per antenna within monoantennary glycans
+A1E = [nE] // [(type == 'complex') * (nAnt == 1)]
 
-@ α2,6-sialylation per antenna within diantennary glycans
-$ A2E = [nE / 2] // [(type == 'complex') * (nAnt == 2)]
+# α2,6-sialylation per antenna within diantennary glycans
+A2E = [nE / 2] // [(type == 'complex') * (nAnt == 2)]
 
-@ α2,6-sialylation per antenna within triantennary glycans
-$ A3E = [nE / 3] // [(type == 'complex') * (nAnt == 3)]
+# α2,6-sialylation per antenna within triantennary glycans
+A3E = [nE / 3] // [(type == 'complex') * (nAnt == 3)]
 
-@ α2,6-sialylation per antenna within tetra-antennary glycans
-$ A4E = [nE / 4] // [(type == 'complex') * (nAnt == 4)]
+# α2,6-sialylation per antenna within tetra-antennary glycans
+A4E = [nE / 4] // [(type == 'complex') * (nAnt == 4)]
 
-@ α2,6-sialylation per antenna within fucosylated monoantennary glycans
-$ A1FE = [nE] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# α2,6-sialylation per antenna within fucosylated monoantennary glycans
+A1FE = [nE] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ α2,6-sialylation per antenna within fucosylated diantennary glycans
-$ A2FE = [nE / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# α2,6-sialylation per antenna within fucosylated diantennary glycans
+A2FE = [nE / 2] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ α2,6-sialylation per antenna within fucosylated triantennary glycans
-$ A3FE = [nE / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# α2,6-sialylation per antenna within fucosylated triantennary glycans
+A3FE = [nE / 3] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ α2,6-sialylation per antenna within fucosylated tetra-antennary glycans
-$ A4FE = [nE / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# α2,6-sialylation per antenna within fucosylated tetra-antennary glycans
+A4FE = [nE / 4] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ α2,6-sialylation per antenna within non-fucosylated monoantennary glycans
-$ A1F0E = [nE] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# α2,6-sialylation per antenna within non-fucosylated monoantennary glycans
+A1F0E = [nE] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ α2,6-sialylation per antenna within non-fucosylated diantennary glycans
-$ A2F0E = [nE / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# α2,6-sialylation per antenna within non-fucosylated diantennary glycans
+A2F0E = [nE / 2] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ α2,6-sialylation per antenna within non-fucosylated triantennary glycans
-$ A3F0E = [nE / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# α2,6-sialylation per antenna within non-fucosylated triantennary glycans
+A3F0E = [nE / 3] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ α2,6-sialylation per antenna within non-fucosylated tetra-antennary glycans
-$ A4F0E = [nE / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# α2,6-sialylation per antenna within non-fucosylated tetra-antennary glycans
+A4F0E = [nE / 4] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ α2,6-sialylation per galactose within monoantennary glycans
-$ A1GE = [nE / nG] // [(type == 'complex') * (nAnt == 1)]
+# α2,6-sialylation per galactose within monoantennary glycans
+A1GE = [nE / nG] // [(type == 'complex') * (nAnt == 1)]
 
-@ α2,6-sialylation per galactose within diantennary glycans
-$ A2GE = [nE / nG] // [(type == 'complex') * (nAnt == 2)]
+# α2,6-sialylation per galactose within diantennary glycans
+A2GE = [nE / nG] // [(type == 'complex') * (nAnt == 2)]
 
-@ α2,6-sialylation per galactose within triantennary glycans
-$ A3GE = [nE / nG] // [(type == 'complex') * (nAnt == 3)]
+# α2,6-sialylation per galactose within triantennary glycans
+A3GE = [nE / nG] // [(type == 'complex') * (nAnt == 3)]
 
-@ α2,6-sialylation per galactose within tetra-antennary glycans
-$ A4GE = [nE / nG] // [(type == 'complex') * (nAnt == 4)]
+# α2,6-sialylation per galactose within tetra-antennary glycans
+A4GE = [nE / nG] // [(type == 'complex') * (nAnt == 4)]
 
-@ α2,6-sialylation per galactose within fucosylated monoantennary glycans
-$ A1FGE = [nE / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
+# α2,6-sialylation per galactose within fucosylated monoantennary glycans
+A1FGE = [nE / nG] // [(type == 'complex') * (nAnt == 1) * (nF > 0)]
 
-@ α2,6-sialylation per galactose within fucosylated diantennary glycans
-$ A2FGE = [nE / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# α2,6-sialylation per galactose within fucosylated diantennary glycans
+A2FGE = [nE / nG] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ α2,6-sialylation per galactose within fucosylated triantennary glycans
-$ A3FGE = [nE / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# α2,6-sialylation per galactose within fucosylated triantennary glycans
+A3FGE = [nE / nG] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ α2,6-sialylation per galactose within fucosylated tetra-antennary glycans
-$ A4FGE = [nE / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# α2,6-sialylation per galactose within fucosylated tetra-antennary glycans
+A4FGE = [nE / nG] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ α2,6-sialylation per galactose within non-fucosylated monoantennary glycans
-$ A1F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
+# α2,6-sialylation per galactose within non-fucosylated monoantennary glycans
+A1F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 1) * (nF == 0)]
 
-@ α2,6-sialylation per galactose within non-fucosylated diantennary glycans
-$ A2F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# α2,6-sialylation per galactose within non-fucosylated diantennary glycans
+A2F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ α2,6-sialylation per galactose within non-fucosylated triantennary glycans
-$ A3F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# α2,6-sialylation per galactose within non-fucosylated triantennary glycans
+A3F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ α2,6-sialylation per galactose within non-fucosylated tetra-antennary glycans
-$ A4F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# α2,6-sialylation per galactose within non-fucosylated tetra-antennary glycans
+A4F0GE = [nE / nG] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
 
 # Poly-LacNAc
 
-@ Relative abundance of species with poly-LacNAc within all complex glycans
-$ CPl = [Pl] // [type == 'complex']
+# Relative abundance of species with poly-LacNAc within all complex glycans
+CPl = [Pl] // [type == 'complex']
 
-@ Relative abundance of species with poly-LacNAc within diantennary glycans
-$ A2Pl = [Pl] // [(type == 'complex') * (nAnt == 2)]
+# Relative abundance of species with poly-LacNAc within diantennary glycans
+A2Pl = [Pl] // [(type == 'complex') * (nAnt == 2)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated diantennary
-$ A2FPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated diantennary
+A2FPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated diantennary glycans
-$ A2F0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated diantennary glycans
+A2F0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0)]
 
-@ Relative abundance of species with poly-LacNAc within sialylated diantennary glycans
-$ A2SPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within sialylated diantennary glycans
+A2SPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-sialylated diantennary glycans
-$ A2S0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-sialylated diantennary glycans
+A2S0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated sialylated diantennary glycans
-$ A2FSPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated sialylated diantennary glycans
+A2FSPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated sialylated diantennary glycans
-$ A2F0SPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated sialylated diantennary glycans
+A2F0SPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-sialylated diantennary glycans
-$ A2FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-sialylated diantennary glycans
+A2FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated diantennary glycans
-$ A2F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated diantennary glycans
+A2F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,3-sialylated diantennary glycans
-$ A2LPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within a2,3-sialylated diantennary glycans
+A2LPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,3-sialylated diantennary glycans
-$ A2L0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,3-sialylated diantennary glycans
+A2L0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated diantennary glycans
-$ A2FLPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated diantennary glycans
+A2FLPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated diantennary glycans
-$ A2F0LPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated diantennary glycans
+A2F0LPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated diantennary glycans
-$ A2FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated diantennary glycans
+A2FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated diantennary glycans
-$ A2F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated diantennary glycans
+A2F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,6-sialylated diantennary glycans
-$ A2EPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within a2,6-sialylated diantennary glycans
+A2EPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,6-sialylated diantennary glycans
-$ A2E0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,6-sialylated diantennary glycans
+A2E0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated diantennary glycans
-$ A2FEPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated diantennary glycans
+A2FEPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated diantennary glycans
-$ A2F0EPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated diantennary glycans
+A2F0EPl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated diantennary glycans
-$ A2FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated diantennary glycans
+A2FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated diantennary glycans
-$ A2F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated diantennary glycans
+A2F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 2) * (nF == 0) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within triantennary glycans
-$ A3Pl = [Pl] // [(type == 'complex') * (nAnt == 3)]
+# Relative abundance of species with poly-LacNAc within triantennary glycans
+A3Pl = [Pl] // [(type == 'complex') * (nAnt == 3)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated triantennary
-$ A3FPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated triantennary
+A3FPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated triantennary glycans
-$ A3F0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated triantennary glycans
+A3F0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0)]
 
-@ Relative abundance of species with poly-LacNAc within sialylated triantennary glycans
-$ A3SPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within sialylated triantennary glycans
+A3SPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-sialylated triantennary glycans
-$ A3S0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-sialylated triantennary glycans
+A3S0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated sialylated triantennary glycans
-$ A3FSPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated sialylated triantennary glycans
+A3FSPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated sialylated triantennary glycans
-$ A3F0SPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated sialylated triantennary glycans
+A3F0SPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-sialylated triantennary glycans
-$ A3FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-sialylated triantennary glycans
+A3FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated triantennary glycans
-$ A3F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated triantennary glycans
+A3F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,3-sialylated triantennary glycans
-$ A3LPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within a2,3-sialylated triantennary glycans
+A3LPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,3-sialylated triantennary glycans
-$ A3L0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,3-sialylated triantennary glycans
+A3L0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated triantennary glycans
-$ A3FLPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated triantennary glycans
+A3FLPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated triantennary glycans
-$ A3F0LPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated triantennary glycans
+A3F0LPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated triantennary glycans
-$ A3FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated triantennary glycans
+A3FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated triantennary glycans
-$ A3F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated triantennary glycans
+A3F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,6-sialylated triantennary glycans
-$ A3EPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within a2,6-sialylated triantennary glycans
+A3EPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,6-sialylated triantennary glycans
-$ A3E0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,6-sialylated triantennary glycans
+A3E0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated triantennary glycans
-$ A3FEPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated triantennary glycans
+A3FEPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated triantennary glycans
-$ A3F0EPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated triantennary glycans
+A3F0EPl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated triantennary glycans
-$ A3FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated triantennary glycans
+A3FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated triantennary glycans
-$ A3F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated triantennary glycans
+A3F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 3) * (nF == 0) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within tetra-antennary glycans
-$ A4Pl = [Pl] // [(type == 'complex') * (nAnt == 4)]
+# Relative abundance of species with poly-LacNAc within tetra-antennary glycans
+A4Pl = [Pl] // [(type == 'complex') * (nAnt == 4)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated tetra-antennary
-$ A4FPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated tetra-antennary
+A4FPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated tetra-antennary glycans
-$ A4F0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated tetra-antennary glycans
+A4F0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0)]
 
-@ Relative abundance of species with poly-LacNAc within sialylated tetra-antennary glycans
-$ A4SPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within sialylated tetra-antennary glycans
+A4SPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-sialylated tetra-antennary glycans
-$ A4S0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-sialylated tetra-antennary glycans
+A4S0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated sialylated tetra-antennary glycans
-$ A4FSPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated sialylated tetra-antennary glycans
+A4FSPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated sialylated tetra-antennary glycans
-$ A4F0SPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated sialylated tetra-antennary glycans
+A4F0SPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-sialylated tetra-antennary glycans
-$ A4FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-sialylated tetra-antennary glycans
+A4FS0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated tetra-antennary glycans
-$ A4F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-sialylated tetra-antennary glycans
+A4F0S0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nS == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,3-sialylated tetra-antennary glycans
-$ A4LPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within a2,3-sialylated tetra-antennary glycans
+A4LPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,3-sialylated tetra-antennary glycans
-$ A4L0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,3-sialylated tetra-antennary glycans
+A4L0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4FLPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,3-sialylated tetra-antennary glycans
+A4FLPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated tetra-antennary glycans
-$ A4F0LPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,3-sialylated tetra-antennary glycans
+A4F0LPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated tetra-antennary glycans
-$ A4FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,3-sialylated tetra-antennary glycans
+A4FL0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated tetra-antennary glycans
-$ A4F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,3-sialylated tetra-antennary glycans
+A4F0L0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nL == 0)]
 
-@ Relative abundance of species with poly-LacNAc within a2,6-sialylated tetra-antennary glycans
-$ A4EPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within a2,6-sialylated tetra-antennary glycans
+A4EPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-a2,6-sialylated tetra-antennary glycans
-$ A4E0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-a2,6-sialylated tetra-antennary glycans
+A4E0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4FEPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated a2,6-sialylated tetra-antennary glycans
+A4FEPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated tetra-antennary glycans
-$ A4F0EPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated a2,6-sialylated tetra-antennary glycans
+A4F0EPl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE > 0)]
 
-@ Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated tetra-antennary glycans
-$ A4FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within fucosylated non-a2,6-sialylated tetra-antennary glycans
+A4FE0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF > 0) * (nE == 0)]
 
-@ Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated tetra-antennary glycans
-$ A4F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
+# Relative abundance of species with poly-LacNAc within non-fucosylated non-a2,6-sialylated tetra-antennary glycans
+A4F0E0Pl = [Pl] // [(type == 'complex') * (nAnt == 4) * (nF == 0) * (nE == 0)]
```

### Comparing `glytrait-0.1.1/src/glytrait/stat.py` & `glytrait-0.1.2/src/glytrait/stat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,44 @@
 import warnings
 
 import pandas as pd
 import pingouin as pg
 
 from glytrait.data_type import DerivedTraitTable, GroupSeries
 
-__all__ = ["t_test", "anova"]
+__all__ = ["auto_test", "t_test", "anova"]
+
+
+def auto_test(
+    trait_df: DerivedTraitTable, groups: GroupSeries
+) -> dict[str, pd.DataFrame]:
+    """Perform statistical tests for the trait data.
+
+    If the number of groups is 2, perform t-test.
+    If the number of groups is more than 2, perform ANOVA, followed by post-hoc test.
+
+    Args:
+        trait_df (DerivedTraitTable): Dataframe containing the trait data.
+        groups (GroupSeries): Series containing the group information.
+
+    Returns:
+        dict[str, pd.DataFrame]: Dictionary containing the test results.
+            If the number of groups is 2, the key is "t_test".
+            If the number of groups is more than 2, the keys are "anova" and "post_hoc".
+
+    Raises:
+        ValueError: If only one group is provided.
+    """
+    if len(groups.unique()) == 1:
+        raise ValueError("Only one group is provided.")
+    elif len(groups.unique()) == 2:
+        return {"t_test": t_test(trait_df, groups)}
+    else:
+        anova_result, post_hoc_result = anova(trait_df, groups)
+        return {"anova": anova_result, "post_hoc": post_hoc_result}
 
 
 def t_test(trait_df: DerivedTraitTable, groups: GroupSeries) -> pd.DataFrame:
     """Perform t-test for the trait data.
 
     Args:
         trait_df (DerivedTraitTable): Dataframe containing the trait data.
```

### Comparing `glytrait-0.1.1/src/glytrait/trait.py` & `glytrait-0.1.2/src/glytrait/trait.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.1/PKG-INFO` & `glytrait-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glytrait
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for calculating derived traits for N-glycome
 Author: fubin1999
 Author-email: 65430559+fubin1999@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,15 +29,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/fubin1999/glytrait/badge.svg?branch=main)](https://coveralls.io/github/fubin1999/glytrait?branch=main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/e3e6a19dccb749f786264247738fa585)](https://app.codacy.com/gh/fubin1999/glytrait/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 ## Overview
 
 *Q: What is GlyTrait?*
 
-*A: GlyTrait is a tool for calculating derived traits for N-glycomic data.*
+*A: GlyTrait is a tool to calculate derived traits for N-glycomic data.*
 
 *Q: Sounds cool! So..., what are derived traits again?*
 
 *A: Well, derived traits are artificial variables that summarize certain aspects of 
 the glycome. 
 For example, the proportion of core-fucosylated glycans, 
 the average number of sialic acids per glycan, 
@@ -48,31 +48,30 @@
 *Q: So, GlyTrait does the dirty work for me, 
 saving my time and energy for more interesting analysis?*
 
 *A: You bet!*
 
 ## Contents
 
+- [Web app](#web-app)
 - [Installation](#installation)
-    - [Requirement](#requirement)
-    - [Using pipx (recommended)](#using-pipx-recommended)
 - [Usage](#usage)
     - [Quick start](#quick-start)
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
     - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
 - [License](#license)
 
 ## Web app
 
-> Let there be no command line apps!
+> Let there be no code!
 > 
 > -- my colleagues
 
 A web app version of GlyTrait is on its way here...
 Ready to say goodbye to the command line?
 
 ## Installation
@@ -125,18 +124,19 @@
 ## Usage
 
 ### Quick start
 
 1. Download the [example files](https://github.com/fubin1999/glytrait/tree/main/example_data)
 to a new directory: `glytrait_example`.
 
-2. Open a terminal and navigate to the directory:
+2. Open a terminal and navigate to the directory 
+(you need to replace `path/to/glytrait_example` with the actual path):
 
 ```shell
-cd glytrait_example
+cd path/to/glytrait_example
 ```
 
 3. Run the following command:
 
 ```shell
 glytrait abundance.csv structures.csv
 ```
```

