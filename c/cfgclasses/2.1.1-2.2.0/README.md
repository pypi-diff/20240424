# Comparing `tmp/cfgclasses-2.1.1.tar.gz` & `tmp/cfgclasses-2.2.0.tar.gz`

## Comparing `cfgclasses-2.1.1.tar` & `cfgclasses-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/__init__.py
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/arghelper.py
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/argspec.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/configclass.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/configgroup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/py.typed
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/transforms.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/test/__init__.py
--rw-r--r--   0        0        0    19282 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/test/test_argspec.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/test/test_configclass.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/test/test_transforms.py
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/cfgclasses/test/test_typing.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/LICENSE
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/README.md
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 cfgclasses-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/__init__.py
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/arghelper.py
+-rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/argspec.py
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/configclass.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/py.typed
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/transforms.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/validation.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/__init__.py
+-rw-r--r--   0        0        0    19201 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/test_argspec.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/test_configclass.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/test_deprecated_api.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/test_transforms.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/cfgclasses/test/test_typing.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/README.md
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cfgclasses-2.2.0/PKG-INFO
```

### Comparing `cfgclasses-2.1.1/cfgclasses/__init__.py` & `cfgclasses-2.2.0/cfgclasses/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 cfgclasses are representations of a python tools CLI configuration options
 built on `dataclasses <https://docs.python.org/3/library/dataclasses.html>`_. This
 allows individual tools to focus on specifying their configuration structure
 without the overhead of interacting with argparse and the typeless Namespace it
 returns.
 
-The primary entrypoint for this module is :class:`cfgclasses.ConfigClass` and
-its ``parse_args()`` classmethod.
+The primary entrypoint for this module is the ``parse_args()`` function.
 
-.. autoclass:: cfgclasses.ConfigClass
-    :members:
-.. autoclass:: cfgclasses.MutuallyExclusiveConfigClass
-    :members:
+.. autofunction:: cfgclasses.parse_args
+.. autofunction:: cfgclasses.parse_args_with_submodes
 
 Additionally the following functions are provided to simplify the creation of
 the class fields.
 
 .. autofunction:: cfgclasses.arg
 .. autofunction:: cfgclasses.optional
 
@@ -23,38 +20,46 @@
 ``dataclasses.field()`` metadata in the key ``cfgclasses.CFG_METADATA_FIELD``.
 
 .. autodata:: cfgclasses.argspec.CFG_METADATA_FIELD
 
 .. autoclass:: cfgclasses.ConfigOpts
 .. autoclass:: cfgclasses.NonPositionalConfigOpts
 
-There are also equivalents for the creation of nested
-:class:`cfgclasses.ConfigClass` definitions.
+There are also equivalents for the creation of nested dataclass definitions.
 
 .. autofunction:: cfgclasses.cfgtransform
 
 Which in turn creates a :class:`cfgclasses.ConfigClassTransform` object in the
 key ``cfgclasses.CFG_METADATA_FIELD``.
 
 .. autoclass:: cfgclasses.ConfigClassTransform
 
 There is an additional submodule :mod:`cfgclasses.transforms` containing several
-common transform functions.
+common transform functions. See below.
+
+Finally, the following decorators are provided to allow the creation of
+mutually exclusive groups of options, and adding validation functions to a
+config class definition respectively.
+
+.. autofunction:: cfgclasses.mutually_exclusive
+.. autofunction:: cfgclasses.validator
 
 cfgclasses.transforms
 ---------------------
 
 .. automodule:: cfgclasses.transforms
 
 """
 
-from . import arghelper, argspec, configclass
+from . import arghelper, argspec, configclass, validation
 
 __all__ = (
     *arghelper.__all__,
     *argspec.__all__,
     *configclass.__all__,
+    *validation.__all__,
 )
 
 from .arghelper import *
 from .argspec import *
 from .configclass import *
+from .validation import *
```

### Comparing `cfgclasses-2.1.1/cfgclasses/arghelper.py` & `cfgclasses-2.2.0/cfgclasses/arghelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Module defining the arg() function for creating dataclass fields."""
+
 import dataclasses
 from typing import Any, Callable, Optional, Type, TypeVar, overload
 
 from .argspec import (
     CFG_METADATA_FIELD,
     ConfigClassTransform,
     ConfigOpts,
     NonPositionalConfigOpts,
 )
-from .configclass import ConfigClass
 
 __all__ = (
     "arg",
     "cfgtransform",
     "optional",
 )
 
 _T = TypeVar("_T")
 _U = TypeVar("_U")
-_ConfigClassT = TypeVar("_ConfigClassT", bound=ConfigClass)
 
 
 @overload
 def arg(
     helpstr: str,
     *optnames: str,
     metavar: Optional[str] = ...,
@@ -340,19 +339,19 @@
             choices=choices,
             default=None,
         )
     return ret
 
 
 def cfgtransform(
-    transform_type: Type[_ConfigClassT],
-    transform: Callable[[_ConfigClassT], _U],
+    transform_type: Type[_T],
+    transform: Callable[[_T], _U],
 ) -> _U:
     """
-    Create a field for a nested ConfigClass with a transform.
+    Create a field for a nested dataclass with a transform.
 
     :param transform_type: The type that the transform function takes as input.
     :param transform: The transform function to apply.
     :return: The resulting dataclass field.
     """
     ret: _U = dataclasses.field(
         metadata={
```

### Comparing `cfgclasses-2.1.1/cfgclasses/argspec.py` & `cfgclasses-2.2.0/cfgclasses/argspec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Module for defining the argument specification for a ConfigClass."""
+"""Module for defining the argument specification for a config class."""
+
 import abc
 import argparse
 import dataclasses
 from typing import (
     Any,
     Callable,
     Generic,
@@ -11,29 +12,36 @@
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 
-from .configgroup import ConfigGroup
+# typeshed not available at runtime, only for type checking
+try:
+    from _typeshed import DataclassInstance
+except ImportError:
+    DataclassInstance = None  # type: ignore
+
+_DataclassInstanceT = TypeVar("_DataclassInstanceT", bound=DataclassInstance)
 
 __all__ = (
     "CFG_METADATA_FIELD",
+    "CFG_MUTUALLY_EXCLUSIVE_ATTR",
     "ConfigOpts",
     "ConfigClassTransform",
     "NonPositionalConfigOpts",
 )
 
 #:Key in the dataclasses field metadata to store the ConfigOpts in.
 CFG_METADATA_FIELD = "cfgclasses.configopts"
+CFG_MUTUALLY_EXCLUSIVE_ATTR = "__mutually_exclusive_cfgclass__"
 
 _T = TypeVar("_T")
 _U = TypeVar("_U")
-_ConfigGroupT = TypeVar("_ConfigGroupT", bound=ConfigGroup)
 
 
 #:Identity function for use as a default transform.
 def identity_transform(value: _T) -> _T:
     """Identity function for use as a default transform."""
     return value
 
@@ -77,23 +85,23 @@
     """
 
     #: List of alternative names (such as ``["-f", "--force"]``) for the argument.
     optnames: list[str] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
-class ConfigClassTransform(Generic[_ConfigGroupT, _U]):
+class ConfigClassTransform(Generic[_T, _U]):
     """
     Data stored in a dataclass field's metadata for transforming config classes.
     """
 
     #: Transform function to modify the CLI values after parsing.
-    transform: Callable[[_ConfigGroupT], _U]
+    transform: Callable[[_T], _U]
     #: Input type to build the CLI from before transforming.
-    transform_type: Type[_ConfigGroupT]
+    transform_type: Type[_T]
 
 
 def _default_from_field(field: dataclasses.Field[_T]) -> _T | NotSpecified:
     """Determine the default value for the field."""
     if field.default is not dataclasses.MISSING:
         return field.default
     if field.default_factory is not dataclasses.MISSING:
@@ -327,20 +335,20 @@
                 f"Can't use type {field_type} with a positional argument."
             )
 
     return ret
 
 
 def _is_configcls_field(field: dataclasses.Field[Any]) -> bool:
-    """Check if the given field is a ConfigClass typed field."""
+    """Check if the given field is a class field to be treated as subcfg."""
     extraconfig = field.metadata.get(CFG_METADATA_FIELD)
     if isinstance(extraconfig, ConfigClassTransform):
         return True
     try:
-        return issubclass(field.type, ConfigGroup)
+        return dataclasses.is_dataclass(field.type)
     except TypeError:
         return False
 
 
 def _spec_from_field(
     field: dataclasses.Field[Any],
 ) -> "Specification[Any]":
@@ -353,37 +361,37 @@
     return Specification.from_class(
         type_,
         extraconfig.transform if extraconfig else None,
     )
 
 
 @dataclasses.dataclass
-class Specification(Generic[_ConfigGroupT]):
+class Specification(Generic[_DataclassInstanceT]):
     """
-    Representation of a ConfigClass in format suitable to pass to argparse.
+    Representation of a dataclass in format suitable to pass to argparse.
 
     This specification maps to an ArgumentGroup in argparse, each member
     SpecificationItem a call to add_argument() and each subspec another
     ArgumentGroup added with add_argument_group().
     """
 
-    #: The ConfigClass type this specification describes.
-    metatype: Type[_ConfigGroupT]
+    #: The dataclass type this specification describes.
+    metatype: Type[_DataclassInstanceT]
     #: List of SpecificationItems for the members of this group.
     members: list[SpecificationItem[Any]]
     #: Mapping of spec names to Specification for any subspecs of this spec.
     subspecs: dict[str, "Specification[Any]"]
     #: The transform to be applied to this specification
-    transform: Optional[Callable[[_ConfigGroupT], Any]]
+    transform: Optional[Callable[[_DataclassInstanceT], Any]]
 
     @staticmethod
     def from_class(
-        metatype: Type[_ConfigGroupT],
-        cfgtransform: Optional[Callable[[_ConfigGroupT], Any]] = None,
-    ) -> "Specification[_ConfigGroupT]":
+        metatype: Type[_DataclassInstanceT],
+        cfgtransform: Optional[Callable[[_DataclassInstanceT], Any]] = None,
+    ) -> "Specification[_DataclassInstanceT]":
         """Instantiate an instance of this class from the ConfigGroup class"""
         return Specification(
             metatype,
             [
                 _specitem_from_field(field)
                 for field in dataclasses.fields(metatype)
                 if not _is_configcls_field(field)
@@ -394,24 +402,29 @@
                 if _is_configcls_field(field)
             },
             cfgtransform if cfgtransform else None,
         )
 
     def add_to_parser(self, parser: argparse._ActionsContainer) -> None:
         """Add this argument group to the given parser."""
-        group = self.metatype.add_argument_group(parser)
+        group = (
+            parser.add_mutually_exclusive_group()
+            if hasattr(self.metatype, CFG_MUTUALLY_EXCLUSIVE_ATTR)
+            and getattr(self.metatype, CFG_MUTUALLY_EXCLUSIVE_ATTR)
+            else parser.add_argument_group()
+        )
         for member in self.members:
             member.add_to_parser(group)
         for subspec in self.subspecs.values():
             subspec.add_to_parser(group)
 
     def construct_from_namespace(
         self, namespace: argparse.Namespace
-    ) -> _ConfigGroupT:
-        """Construct an instance of the ConfigClass from the given namespace."""
+    ) -> _DataclassInstanceT:
+        """Construct an instance of the dataclass from the given namespace."""
         return self.metatype(
             **{
                 item.name: item.extract_value_from_namespace(namespace)
                 for item in self.members
             }
             | {
                 subspec_name: (subspec.transform or (lambda x: x))(
```

### Comparing `cfgclasses-2.1.1/cfgclasses/transforms.py` & `cfgclasses-2.2.0/cfgclasses/transforms.py`

 * *Files identical despite different names*

### Comparing `cfgclasses-2.1.1/cfgclasses/test/test_argspec.py` & `cfgclasses-2.2.0/cfgclasses/test/test_argspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Unit-tests for the argspec module."""
+
 import argparse
 import dataclasses
-from typing import Any, Optional, Sequence, Type
+from typing import Any, Optional, Sequence, Type, TypeVar
 
 import pytest
 
-from cfgclasses import (
-    ConfigClass,
-    MutuallyExclusiveConfigClass,
-    arg,
-    cfgtransform,
-    optional,
-)
+from cfgclasses import arg, cfgtransform, mutually_exclusive, optional
 from cfgclasses.argspec import (
     BoolSpecItem,
     ListPositionalSpecItem,
     ListSpecItem,
     NotSpecified,
     OptionalSpecItem,
     PositionalSpecItem,
     Specification,
     SpecificationItem,
     StandardSpecItem,
     identity_transform,
 )
 
+try:
+    from _typeshed import DataclassInstance
+except ImportError:
+    DataclassInstance = None  # type: ignore
+_T = TypeVar("_T", bound=DataclassInstance)
+
 
 # =============================================================================
 # Fixtures used in unit tests
 # =============================================================================
 @dataclasses.dataclass
-class SimpleOptCase(ConfigClass):
+class SimpleOptCase:
     """Case with a simple required option."""
 
     strfield: str = arg("A simple string field")
 
 
 simpleoptspec = Specification(
     SimpleOptCase,
@@ -52,15 +53,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class OptionalOptCase(ConfigClass):
+class OptionalOptCase:
     """Case with an optional option."""
 
     optfield: Optional[str] = optional("An optional string field")
 
 
 optionaloptspec = Specification(
     OptionalOptCase,
@@ -78,15 +79,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class ListOptCase(ConfigClass):
+class ListOptCase:
     """Case with a list option."""
 
     # First case has no default or default_factory so is required
     firstlist: list[str] = arg("A list string field")
     # Second case has a default_factory so is optional
     secondlist: list[str] = arg(
         "Another list string field", default_factory=list
@@ -119,15 +120,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class PositionalOptCase(ConfigClass):
+class PositionalOptCase:
     """Case with a positional option."""
 
     posfield: str = arg("A positional string field", positional=True)
     poslistfield: list[str] = arg("A positional list field", positional=True)
 
 
 posoptspec = Specification(
@@ -156,15 +157,15 @@
     transform=None,
 )
 
 
 # Additional complex case for positional argument to ensure they interact with
 # non-positional arguments as expected.
 @dataclasses.dataclass
-class PositionalAndOptionalCase(ConfigClass):
+class PositionalAndOptionalCase:
     """Case with a combination of positional and optional options."""
 
     strfield: str = arg("A simple string field")
     posfield: str = arg("A positional string field", positional=True)
     intfield: int = arg("An integer field")
     optfield: Optional[str] = optional("An optional string field")
     poslistfield: list[str] = arg(
@@ -228,15 +229,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class ChoicesOptCase(ConfigClass):
+class ChoicesOptCase:
     """Case with a choices option."""
 
     choicefield: str = arg(
         "A choice field", choices=["a", "b", "c"], default="a"
     )
 
 
@@ -256,15 +257,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class BooleanOptCase(ConfigClass):
+class BooleanOptCase:
     """Case with a store_true option."""
 
     boolfield: bool = arg("A boolean field")
     negativeboolfield: bool = arg(
         "An awkward boolean field with a 'True' default",
         default=True,
     )
@@ -296,15 +297,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class OptNameOptCase(ConfigClass):
+class OptNameOptCase:
     """Case with a custom option name."""
 
     strfield: str = arg("A simple string field", "-c", "--custom-name")
 
 
 optnameoptspec = Specification(
     OptNameOptCase,
@@ -322,38 +323,39 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class HasSubGroupCase(ConfigClass):
+class HasSubGroupCase:
     """Case with a subspec."""
 
     subspec: SimpleOptCase
 
 
 hassubspec = Specification(
     HasSubGroupCase,
     members=[],
     subspecs={"subspec": simpleoptspec},
     transform=None,
 )
 
 
+@mutually_exclusive
 @dataclasses.dataclass
-class MutuallyExclusiveGroup(MutuallyExclusiveConfigClass):
+class MutuallyExclusiveGroup:
     """Example mutually exclusive group."""
 
     opt_a: int = arg("Option A", default=0)
     opt_b: int = arg("Option B", default=0)
 
 
 @dataclasses.dataclass
-class HasMutuallyExclusiveGroupCase(ConfigClass):
+class HasMutuallyExclusiveGroupCase:
     """Case with a mutually exclusive subspec."""
 
     subspec: MutuallyExclusiveGroup
 
 
 hasmutuallyexclusivegroup = Specification(
     HasMutuallyExclusiveGroupCase,
@@ -388,15 +390,15 @@
         )
     },
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class TransformMembers(ConfigClass):
+class TransformMembers:
     """Example with a member that uses a transform."""
 
     opt_a: set[str] = arg("Option A", transform=set, transform_type=list[str])
 
 
 transformgroup = Specification(
     TransformMembers,
@@ -414,15 +416,15 @@
     ],
     subspecs={},
     transform=None,
 )
 
 
 @dataclasses.dataclass
-class TransformSubGroupCase(ConfigClass):
+class TransformSubGroupCase:
     """Case with a subspec to be transformed."""
 
     subspec: str = cfgtransform(SimpleOptCase, str)
 
 
 transformsubspec = Specification(
     TransformSubGroupCase,
@@ -465,15 +467,15 @@
 
 @pytest.mark.parametrize(
     ["configcls", "expectedspec"],
     test_spec_from_class_cases.values(),
     ids=test_spec_from_class_cases.keys(),
 )
 def test_spec_from_class(
-    configcls: Type[ConfigClass], expectedspec: Specification[ConfigClass]
+    configcls: Type[_T], expectedspec: Specification[_T]
 ) -> None:
     """
     Test the Specification.from_class function and internally the equivalent for
     SpecificationItem.
     """
     assert Specification.from_class(configcls) == expectedspec
 
@@ -713,17 +715,17 @@
 
 @pytest.mark.parametrize(
     ["spec", "args", "expectedconfig"],
     test_e2e_parser_cases.values(),
     ids=test_e2e_parser_cases.keys(),
 )
 def test_e2e_parser(
-    spec: Specification[ConfigClass],
+    spec: Specification[_T],
     args: Sequence[str],
-    expectedconfig: ConfigClass,
+    expectedconfig: _T,
 ) -> None:
     """
     Test the Specification.add_to_parser() and
     Specification.extract_args_from_namespace() methods together.
     """
     parser = argparse.ArgumentParser()
     spec.add_to_parser(parser)
```

### Comparing `cfgclasses-2.1.1/cfgclasses/test/test_configclass.py` & `cfgclasses-2.2.0/cfgclasses/test/test_deprecated_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-"""Unit-tests for the configclass module."""
+"""Regress tests to ensure that the deprecated API still works."""
+
 import dataclasses
 
 import pytest
 
 from cfgclasses import ConfigClass, MutuallyExclusiveConfigClass, arg
 
 
+def test_simple() -> None:
+    """Test the inheritance from ConfigClass."""
+
+    @dataclasses.dataclass
+    class TopLevelConfig(ConfigClass):
+        """Top level config class containing the mutually exclusive group."""
+
+        anum: int = arg("A simple integer field", default=0)
+
+    assert TopLevelConfig.parse_args(["--anum", "10000"]) == TopLevelConfig(
+        anum=10000
+    )
+
+
 def test_mutually_exclusive() -> None:
     """Test the use of mutually exclusive groups."""
 
     @dataclasses.dataclass
     class MEGroupConfig(MutuallyExclusiveConfigClass):
         """Config for mutually exclusive options relating to A."""
```

### Comparing `cfgclasses-2.1.1/cfgclasses/test/test_transforms.py` & `cfgclasses-2.2.0/cfgclasses/test/test_transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,71 +3,71 @@
 import json
 import pickle
 import tempfile
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 
-from .. import ConfigClass, arg
+from .. import arg, parse_args
 from ..transforms import filebytes, filetext, jsonfile, picklefile
 
 
 def test_file_content() -> None:
     """Test the file content transform usage."""
 
     @dataclass
-    class TestConfig(ConfigClass):
+    class TestConfig:
         """Test Config"""
 
         data: str = arg("Input data", transform=filetext, transform_type=Path)
         bits: bytes = arg(
             "Input binary data", transform=filebytes, transform_type=Path
         )
 
     content = "ABC\nDEF\nGHI\n"
     with tempfile.NamedTemporaryFile(mode="w") as tmp:
         tmp.write(content)
         tmp.flush()
 
-        config = TestConfig.parse_args(
-            ["--data", tmp.name, "--bits", tmp.name]
+        config = parse_args(
+            TestConfig, ["--data", tmp.name, "--bits", tmp.name]
         )
         assert config.data == content
         assert config.bits == content.encode("utf-8")
 
 
 def test_json() -> None:
     """Test the JSON file transform usage."""
 
     @dataclass
-    class TestConfig(ConfigClass):
+    class TestConfig:
         """Test Config"""
 
         data: Any = arg("Input data", transform=jsonfile, transform_type=Path)
 
     content = {"ABC": "DEF", "GHI": 123}
     with tempfile.NamedTemporaryFile(mode="w") as tmp:
         tmp.write(json.dumps(content))
         tmp.flush()
 
-        config = TestConfig.parse_args(["--data", tmp.name])
+        config = parse_args(TestConfig, ["--data", tmp.name])
         assert config.data == content
 
 
 def test_pickle() -> None:
     """Test the pickle file transform usage."""
 
     @dataclass
-    class TestConfig(ConfigClass):
+    class TestConfig:
         """Test Config"""
 
         data: Any = arg(
             "Input data", transform=picklefile, transform_type=Path
         )
 
     content = {"ABC": "DEF", "GHI": 123}
     with tempfile.NamedTemporaryFile(mode="wb") as tmp:
         tmp.write(pickle.dumps(content))
         tmp.flush()
 
-        config = TestConfig.parse_args(["--data", tmp.name])
+        config = parse_args(TestConfig, ["--data", tmp.name])
         assert config.data == content
```

### Comparing `cfgclasses-2.1.1/cfgclasses/test/test_typing.py` & `cfgclasses-2.2.0/cfgclasses/test/test_typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Testing that expected typing errors are raised by mypy."""
 
 from dataclasses import dataclass
 
 import pytest
 
-from cfgclasses import ConfigClass, arg, cfgtransform
+from cfgclasses import arg, cfgtransform
 
 # =============================================================================
 # The test cases in this file are run both as regular test cases and as
 # mypy_testing cases. Regular asserts can be made within the cases if needed.
 # =============================================================================
 
 
@@ -16,15 +16,15 @@
 def test_invalid_transform() -> None:
     """Test that invalid types in transforms are identified."""
 
     def typed_transform(i: int) -> str:
         return str(i)
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         # Invalid assignment type
         field_a: int = arg(  # E: [assignment]
             "Help", transform_type=int, transform=typed_transform
         )
         # Invalid assignment type with lambda
@@ -54,24 +54,24 @@
 
 
 @pytest.mark.mypy_testing
 def test_invalid_cfgtransform() -> None:
     """Test that invalid types in config class transforms are identified."""
 
     @dataclass
-    class SubTestClass(ConfigClass):
+    class SubTestClass:
         """Sub test class."""
 
         field_x: str
 
     def typed_transform(i: int) -> bytes:
         return bytes(i)
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         # No use of cfgtransform - should be fine
         subtest_a: SubTestClass
 
         # Simple transform - should be fine
         subtest_b: str = cfgtransform(SubTestClass, str)
@@ -93,15 +93,15 @@
 
 
 @pytest.mark.mypy_testing
 def test_invalid_choices() -> None:
     """Test that invalid types in choices are identified."""
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         field: str = arg(  # E: [assignment]
             "Help",
             choices=[1, 2, 3],
         )
 
@@ -109,15 +109,15 @@
 
 
 @pytest.mark.mypy_testing
 def test_invalid_default() -> None:
     """Test that invalid types in defaults are identified."""
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         field: str = arg(  # E: [assignment]
             "Help",
             default=1,
         )
         field2: str = arg(  # E: [assignment]
@@ -129,15 +129,15 @@
 
 
 @pytest.mark.mypy_testing
 def test_incompatible_default_args() -> None:
     """Test that default and default_factory can't both be set."""
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         field_a: str = arg(  # O: [call-overload]
             "Help", default="", default_factory=lambda: ""
         )
         field_b: str = arg(  # O: [call-overload]
             "Help", positional=True, default="", default_factory=lambda: ""
@@ -147,15 +147,15 @@
 
 
 @pytest.mark.mypy_testing
 def test_positional_optnames() -> None:
     """Test that option names can't be specified with a positional argument."""
 
     @dataclass
-    class TestClass(ConfigClass):
+    class TestClass:
         """Test class."""
 
         field_a: str = arg(  # O: [call-overload]
             "Help", "FIELD_A", positional=True
         )
 
     TestClass("A")
```

### Comparing `cfgclasses-2.1.1/LICENSE` & `cfgclasses-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgclasses-2.1.1/README.md` & `cfgclasses-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+Metadata-Version: 2.3
+Name: cfgclasses
+Version: 2.2.0
+Summary: Strongly typed tool configuration classes for argument parsing.
+Project-URL: Homepage, https://github.com/ollij93/cfgclasses
+Project-URL: Bug Tracker, https://github.com/ollij93/cfgclasses/issues
+Author-email: Olli Johnson <ollijohnson93@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Provides-Extra: dev-dependencies
+Description-Content-Type: text/markdown
+
 # Config Classes (cfgclasses)
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/ollij93/cfgclasses/actions/workflows/python.yml/badge.svg)](https://github.com/ollij93/cfgclasses/actions/workflows/python.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/cfgclasses.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/cfgclasses/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/cfgclasses.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/cfgclasses/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cfgclasses.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/cfgclasses/) |
 | Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![linting - pylint](https://img.shields.io/badge/lint-pylint-blue.svg)](https://github.com/pylint-dev/pylint) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
 
 -----
 
 Strongly typed tool configuration classes for argument parsing.
 
-ConfigClasses are representations of a python tools CLI configuration options built on [dataclasses](https://docs.python.org/3/library/dataclasses.html). This allows individual tools to focus on specifying their configuration structure without the overhead of interacting with argparse and the typeless Namespace it returns.
+Config classes are representations of a python tools CLI configuration options built on [dataclasses](https://docs.python.org/3/library/dataclasses.html). This allows individual tools to focus on specifying their configuration structure without the overhead of interacting with argparse and the typeless Namespace it returns.
 
 See the [documnentation](https://ollij93.github.io/cfgclasses/) for full user guides and API references.
 
 ## Installation
 
 ```sh
 pip install cfgclasses
@@ -26,25 +41,25 @@
 * Nested config and tool submodes reduce code repetition
 * Mutually exclusive groups support
 * Validation functions for reliable verification of config
 * Argument transformations reducing repetition of common patterns (e.g. reading contents of a file)
 
 ## Example Usage
 
-The following shows a simple script setup using a Config Class.
+The following shows a simple script setup using a Config class.
 
 ```python3
 import dataclasses
 import sys
-from cfgclasses import ConfigClass, arg, optional
+from cfgclasses import arg, optional, parse_args
 from pathlib import Path
 from typing import Optional
 
 @dataclasses.dataclass
-class Config(ConfigClass):
+class Config:
     # Simple options are required on the CLI
     intopt: int = arg("A simple integer field")
     inpath: Path = arg("A required Path field")
 
     # Optional fields default to None when not specified
     outpath: Optional[Path] = optional("An optional Path field")
 
@@ -55,15 +70,15 @@
     # This is entirely optional, and main() methods that take in the Config
     # object as their only arg is a perfectly sensible alternative.
     def run(self) -> None:
         """Main entry point of this script."""
         ...
 
 if __name__ == '__main__':
-    config = Config.parse_args(sys.argv[1:], prog="example")
+    config = parse_args(Config, sys.argv[1:], prog="example")
     config.run()
 ```
 
 The `-h` output from this script is:
 
 ```txt
 usage: example [-h] --intopt INTOPT --inpath INPATH [--outpath OUTPATH] [--stropt STROPT]
```

### Comparing `cfgclasses-2.1.1/pyproject.toml` & `cfgclasses-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 [project]
 name = "cfgclasses"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
   { name="Olli Johnson", email="ollijohnson93@gmail.com" },
 ]
 description = "Strongly typed tool configuration classes for argument parsing."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = []
+
+[project.optional-dependencies]
+dev-dependencies = [
+#  "black>=24.4.0",
+#  "coverage>=6.4.1",
+#  "isort>=5.10.1",
+#  "mypy>=1.5.1",
+#  "pylint>=3.1.0",
+#  "pytest>=7.1.2",
+#  "pytest-mypy-testing==0.1.1",
+#  "sphinx-autodoc-typehints==1.24.0",
+#  "sphinxcontrib-mermaid==0.9.2",
+#  "pytest-mypy-testing @ git+https://github.com/ollij93/pytest-mypy-testing.git",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/ollij93/cfgclasses"
 "Bug Tracker" = "https://github.com/ollij93/cfgclasses/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "cfgclasses/**/*.py",
   "cfgclasses/py.typed",
 ]
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 # ==============================================================================
 # DEV TOOLS
 # ==============================================================================
 [tool.black]
 line-length = 79
 
 [tool.isort]
@@ -74,15 +93,15 @@
 
 [tool.pylint.basic]
 
 [tool.pylint.classes]
 
 [tool.pylint.design]
 # Maximum number of arguments for function / method.
-max-args = 5
+max-args = 8 # Required for dataclass field wrappers
 
 # Maximum number of attributes for a class (see R0902).
 max-attributes = 7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr = 5
 
@@ -136,15 +155,17 @@
 # multiple times (only on the command line, not in the configuration file where
 # it should appear only once). You can also use "--disable=all" to disable
 # everything first and then re-enable specific checks. For example, if you want
 # to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
-disable = []
+disable = [
+  "invalid-field-call", # Unusual use of field due to the nature of our design
+]
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where it
 # should appear only once). See also the "--disable" option for examples.
 enable = ["all"]
 
@@ -179,8 +200,7 @@
 [tool.pylint.variables]
 # Tells whether unused global variables should be treated as a violation.
 # NOTE: Would enable this, but there's no way to add exceptions for things like
 # __all__.
 allow-global-unused-variables = true
 
 #===============================================================================
-
```

### Comparing `cfgclasses-2.1.1/PKG-INFO` & `cfgclasses-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,20 @@
-Metadata-Version: 2.1
-Name: cfgclasses
-Version: 2.1.1
-Summary: Strongly typed tool configuration classes for argument parsing.
-Project-URL: Homepage, https://github.com/ollij93/cfgclasses
-Project-URL: Bug Tracker, https://github.com/ollij93/cfgclasses/issues
-Author-email: Olli Johnson <ollijohnson93@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Config Classes (cfgclasses)
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/ollij93/cfgclasses/actions/workflows/python.yml/badge.svg)](https://github.com/ollij93/cfgclasses/actions/workflows/python.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/cfgclasses.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/cfgclasses/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/cfgclasses.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/cfgclasses/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cfgclasses.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/cfgclasses/) |
 | Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![linting - pylint](https://img.shields.io/badge/lint-pylint-blue.svg)](https://github.com/pylint-dev/pylint) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
 
 -----
 
 Strongly typed tool configuration classes for argument parsing.
 
-ConfigClasses are representations of a python tools CLI configuration options built on [dataclasses](https://docs.python.org/3/library/dataclasses.html). This allows individual tools to focus on specifying their configuration structure without the overhead of interacting with argparse and the typeless Namespace it returns.
+Config classes are representations of a python tools CLI configuration options built on [dataclasses](https://docs.python.org/3/library/dataclasses.html). This allows individual tools to focus on specifying their configuration structure without the overhead of interacting with argparse and the typeless Namespace it returns.
 
 See the [documnentation](https://ollij93.github.io/cfgclasses/) for full user guides and API references.
 
 ## Installation
 
 ```sh
 pip install cfgclasses
@@ -40,25 +26,25 @@
 * Nested config and tool submodes reduce code repetition
 * Mutually exclusive groups support
 * Validation functions for reliable verification of config
 * Argument transformations reducing repetition of common patterns (e.g. reading contents of a file)
 
 ## Example Usage
 
-The following shows a simple script setup using a Config Class.
+The following shows a simple script setup using a Config class.
 
 ```python3
 import dataclasses
 import sys
-from cfgclasses import ConfigClass, arg, optional
+from cfgclasses import arg, optional, parse_args
 from pathlib import Path
 from typing import Optional
 
 @dataclasses.dataclass
-class Config(ConfigClass):
+class Config:
     # Simple options are required on the CLI
     intopt: int = arg("A simple integer field")
     inpath: Path = arg("A required Path field")
 
     # Optional fields default to None when not specified
     outpath: Optional[Path] = optional("An optional Path field")
 
@@ -69,15 +55,15 @@
     # This is entirely optional, and main() methods that take in the Config
     # object as their only arg is a perfectly sensible alternative.
     def run(self) -> None:
         """Main entry point of this script."""
         ...
 
 if __name__ == '__main__':
-    config = Config.parse_args(sys.argv[1:], prog="example")
+    config = parse_args(Config, sys.argv[1:], prog="example")
     config.run()
 ```
 
 The `-h` output from this script is:
 
 ```txt
 usage: example [-h] --intopt INTOPT --inpath INPATH [--outpath OUTPATH] [--stropt STROPT]
```

