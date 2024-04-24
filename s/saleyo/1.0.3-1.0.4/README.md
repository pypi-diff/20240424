# Comparing `tmp/saleyo-1.0.3.tar.gz` & `tmp/saleyo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saleyo-1.0.3.tar", last modified: Thu Mar 28 00:29:58 2024, max compression
+gzip compressed data, was "saleyo-1.0.4.tar", last modified: Wed Apr 24 03:41:34 2024, max compression
```

## Comparing `saleyo-1.0.3.tar` & `saleyo-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1063 2024-03-28 00:29:41.779614 saleyo-1.0.3/LICENSE
--rw-r--r--   0        0        0     2551 2024-03-28 00:29:41.779614 saleyo-1.0.3/README.md
--rw-r--r--   0        0        0      581 2024-03-28 00:29:58.635480 saleyo-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1240 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/__init__.py
--rw-r--r--   0        0        0      103 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/base/__init__.py
--rw-r--r--   0        0        0      707 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/base/template.py
--rw-r--r--   0        0        0     3995 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/base/toolchain.py
--rw-r--r--   0        0        0      537 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/base/typing.py
--rw-r--r--   0        0        0     4719 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/mixin.py
--rw-r--r--   0        0        0      344 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/__init__.py
--rw-r--r--   0        0        0     1585 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/accessor.py
--rw-r--r--   0        0        0     3180 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/hook.py
--rw-r--r--   0        0        0     1863 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/intercept.py
--rw-r--r--   0        0        0     1534 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/modify.py
--rw-r--r--   0        0        0     1296 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/overwrite.py
--rw-r--r--   0        0        0     2743 2024-03-28 00:29:41.779614 saleyo-1.0.3/src/saleyo/operation/processor.py
--rw-r--r--   0        0        0      100 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0      244 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/custom.py
--rw-r--r--   0        0        0     1168 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/demo.py
--rw-r--r--   0        0        0      396 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/gc_test.py
--rw-r--r--   0        0        0      528 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/intercept.py
--rw-r--r--   0        0        0      201 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/modify_test.py
--rw-r--r--   0        0        0       37 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/test_module_a.py
--rw-r--r--   0        0        0      239 2024-03-28 00:29:41.779614 saleyo-1.0.3/tests/test_module_b.py
--rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 saleyo-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 03:41:20.490147 saleyo-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2540 2024-04-24 03:41:20.490147 saleyo-1.0.4/README.md
+-rw-r--r--   0        0        0      581 2024-04-24 03:41:34.850283 saleyo-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1324 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/template.py
+-rw-r--r--   0        0        0     3999 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/toolchain.py
+-rw-r--r--   0        0        0      568 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/typing.py
+-rw-r--r--   0        0        0     4733 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/mixin.py
+-rw-r--r--   0        0        0      424 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/__init__.py
+-rw-r--r--   0        0        0     1575 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/accessor.py
+-rw-r--r--   0        0        0     1179 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/ancestor.py
+-rw-r--r--   0        0        0     3162 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/hook.py
+-rw-r--r--   0        0        0     1856 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/intercept.py
+-rw-r--r--   0        0        0     1558 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/modify.py
+-rw-r--r--   0        0        0     1283 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/overwrite.py
+-rw-r--r--   0        0        0     2730 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/processor.py
+-rw-r--r--   0        0        0      100 2024-04-24 03:41:20.490147 saleyo-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-24 03:41:20.490147 saleyo-1.0.4/tests/custom.py
+-rw-r--r--   0        0        0     1168 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/demo.py
+-rw-r--r--   0        0        0      396 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/gc_test.py
+-rw-r--r--   0        0        0      528 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/intercept.py
+-rw-r--r--   0        0        0      301 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/misc_test.py
+-rw-r--r--   0        0        0      201 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/modify_test.py
+-rw-r--r--   0        0        0       37 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/test_module_a.py
+-rw-r--r--   0        0        0      239 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/test_module_b.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 saleyo-1.0.4/PKG-INFO
```

### Comparing `saleyo-1.0.3/LICENSE` & `saleyo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.3/README.md` & `saleyo-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class Foo:
     __private = "private varible"
 
     def demo(self):
         pass
 
 
-@Mixin(target=Foo)
+@Mixin(target = Foo)
 class MixinFoo:
     # Will add a varible named `__private` to Foo and it has the same address with `_Foo__private`
     private: Accessor[str] = Accessor("__private")
 
     # Will Add the `func` to `Foo`
     @OverWrite
     def func(self):
@@ -108,14 +108,14 @@
 ### Custom Operation
 
 The default operations can't satify you? Why not try define a operation yourself!
 
 ```python
 from typing import Any
 from saleyo import MixinOperation, ToolChain
-from saleyo.base.typing import MixinAble
+from saleyo.base.typing import M
 
-class MyOperation(MixinOperation[Any]):
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ...) -> None:
+class MyOperation(MixinOperation[Any, M]):
+    def mixin(self, target: M, toolchain: ToolChain = ...) -> None:
         ...
 ```
```

### Comparing `saleyo-1.0.3/pyproject.toml` & `saleyo-1.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saleyo"
-version = "1.0.3"
+version = "1.0.4"
 description = "Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate."
 authors = [
     { name = "H2Sxxa", email = "h2sxxa0w0@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `saleyo-1.0.3/src/saleyo/__init__.py` & `saleyo-1.0.4/src/saleyo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from .operation import Intercept as Intercept
 from .operation import OverWrite as OverWrite
 from .operation import Pre as Pre
 from .operation import Post as Post
 from .operation import Del as Del
 from .operation import ReName as ReName
 from .operation import Alias as Alias
+from .operation import Ancestor as Ancestor
+from .operation import Insert as Insert
 from .base.toolchain import ToolChain as ToolChain
 from .base.toolchain import Arguments as Arguments
 from .base.toolchain import InvokeEvent as InvokeEvent
 from .base.toolchain import CPyToolChain as CPyToolChain
 from .base.toolchain import GCToolChain as GCToolChain
 from .base.template import MixinOperation as MixinOperation
```

### Comparing `saleyo-1.0.3/src/saleyo/base/toolchain.py` & `saleyo-1.0.4/src/saleyo/base/toolchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     tool_delattr=lambda _object, _name: _get_referents(_object.__dict__)[0].__delitem__(
         _name
     ),
 )
 """
 GC ToolChain use the `get_referents` functions in `gc` and it can modify some special class.
 
-Notice: There is no guarantee that it can modify any class, and this method is rude and danger, avoid using it in produce environment.
+Notice: There is no guarantee that it can modify any class, and this method is rude and dangerous, avoid using it in produce environment.
 """
 
 
 def _cpy_get_dict(_object: Any) -> Dict[str, Any]:
     return _cast(
         id(_object) + type(_object).__dictoffset__, _POINTER(_py_object)
     ).contents.value
@@ -49,17 +49,17 @@
     tool_hasattr=lambda _object, _name: _name in _cpy_get_dict(_object),
     tool_setattr=lambda _object, _name, _attr: _cpy_get_dict(_object).update(
         {_name: _attr}
     ),
     tool_delattr=lambda _object, _name: _cpy_get_dict(_object).__delitem__(_name),
 )
 """
-`CPyToolChain` use the `ctypes` to modify class, it's danger than other default toolchains.
+`CPyToolChain` use the `ctypes` to modify class, it's dangerous than other default toolchains.
 
-Notice: There is no guarantee that it can modify any class, and this method is rude and danger, avoid using it in produce environment.
+Notice: There is no guarantee that it can modify any class, and this method is rude and dangerous, avoid using it in produce environment.
 """
 
 
 class Container:
     """
     Container is A Class to keep a namespace and use this namespace to define function / variable / ...
     """
@@ -67,15 +67,15 @@
     environment: NameSpace
 
     def __init__(self, *namespace: Optional[NameSpace]) -> None:
         self.environment = {
             k: v for _ in namespace if _ is not None for k, v in _.items()
         }
 
-    def exec(self, source: str) -> Dict[str, Any]:
+    def exec(self, source: str) -> NameSpace:
         exec(source, self.environment)
         return self.environment
 
     def define_function(
         self, function_name: str, source: str, indent: Optional[int] = None
     ) -> FunctionType:
         if indent is None:
```

### Comparing `saleyo-1.0.3/src/saleyo/base/typing.py` & `saleyo-1.0.4/src/saleyo/base/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 `T` means `Type`
 """
 P = ParamSpec("P")
 """
 `P` means `Params`
 """
 
+M = TypeVar("M", Type[Any], ModuleType, Any)
+"""
+These can be the target of mixin.
+
+Not recommend input Any.
+"""
+
+
 # Alias
 
 NameSpace = Dict[str, Any]
 """
 `NameSpace` is the alias of `Dict[str, Any]`
 """
 
 IterableOrSingle = Union[T, Iterable[T]]
 """
 `IterableOrSingle[T]` is the alias of `Union[T, List[T]]` 
 """
-
-MixinAble = Union[Type[Any], ModuleType]
-"""
-These can be the target of mixin.
-"""
```

### Comparing `saleyo-1.0.3/src/saleyo/mixin.py` & `saleyo-1.0.4/src/saleyo/mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Iterable, List
+from typing import Generic, Iterable, List, Union
 
 from .base.template import MixinOperation
 from .base.toolchain import ToolChain
-from .base.typing import T, IterableOrSingle, MixinAble
+from .base.typing import M, T, IterableOrSingle
 
 
-class Mixin:
+class Mixin(Generic[M]):
     """
     A `Mixin` Decorator is used to invoke all the `MixinOperation` in Mixin Class.
 
     If the target is a special class, you should custom the toolchain yourself.
 
     Allow to have more than one target, but that's not recommended.
     """
 
-    target: Iterable[MixinAble]
+    target: Iterable[M]
     toolchain: ToolChain
     reverse_level: bool
 
     def __init__(
         self,
-        target: IterableOrSingle[MixinAble],
+        target: IterableOrSingle[M],
         toolchain: ToolChain = ToolChain(),
         reverse_level: bool = False,
     ) -> None:
         self.target = target if isinstance(target, Iterable) else [target]
         self.toolchain = toolchain
         self.reverse_level = reverse_level
 
@@ -135,9 +135,9 @@
         """
         for operation in (
             operations if isinstance(operations, Iterable) else [operations]
         ):
             for target in self.target:
                 operation.mixin(target=target, toolchain=self.toolchain)
 
-    def __call__(self, mixin: T) -> T:
+    def __call__(self, mixin: T) -> Union[M, T]:
         return self.apply_from_class(mixin=mixin)
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/accessor.py` & `saleyo-1.0.4/src/saleyo/operation/accessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Generic, Optional
 
 from ..base.toolchain import ToolChain
-from ..base.typing import T, MixinAble
+from ..base.typing import T, M
 from ..base.template import MixinOperation
 
 
-class Accessor(Generic[T], MixinOperation[str]):
+class Accessor(Generic[T, M], MixinOperation[str, M]):
     """
     Want to access and modify some private varibles or methods? Try use `Accessor`!
 
     The Generic is the type of target varible.
 
     Notice: The value only available after invoking the `mixin` method.
 
@@ -30,15 +30,15 @@
     def configure(level: int = 1):
         return lambda argument: Accessor(
             argument=argument,
             level=level,
             private=True,
         )
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         self._inner = toolchain.tool_getattr(
             target,
             f"_{target.__name__}{self.argument}" if self._private else self.argument,
         )
         return toolchain.tool_setattr(
             target,
             self.argument,
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/hook.py` & `saleyo-1.0.4/src/saleyo/operation/hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Optional, Union
 
-from ..base.typing import P, RT, T, MixinAble
+from ..base.typing import M, P, RT, T
 from ..base.toolchain import ToolChain, Arguments
 from ..base.template import MixinOperation
 
 
-class Post(MixinOperation[Callable[[T], Optional[RT]]]):
+class Post(MixinOperation[Callable[[T], Optional[RT]], M]):
     """
     `Post` will call after the target method, and the callable should be decorated as `@staticmethod` and have one argument to receive the result of target method.
 
     If the `post` function return value is not `None`, it will replace the original result.
     """
 
     target_name: Optional[str]
@@ -30,15 +30,15 @@
     ):
         return lambda argument: Post(
             argument=argument,
             target_name=target_name,
             level=level,
         )
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
         native_function: Callable[..., T] = toolchain.tool_getattr(target, target_name)
 
         def post(*args, **kwargs) -> Union[T, RT]:
             result = native_function(*args, **kwargs)
@@ -46,15 +46,15 @@
             if post_result is not None:
                 return post_result
             return result
 
         return toolchain.tool_setattr(target, target_name, post)
 
 
-class Pre(MixinOperation[Callable[P, Optional[Arguments[P]]]]):
+class Pre(MixinOperation[Callable[P, Optional[Arguments[P]]], M]):
     """
     `Pre` will call before the target method, and the callable should be decorated as `@staticmethod` and have `*args,**kwargs` to receive the arguments of target method.
 
     If the `pre` function return value is a `Aruguments`(not `None`), it will replace the original arguments.
     """
 
     target_name: Optional[str]
@@ -75,15 +75,15 @@
     ):
         return lambda argument: Pre(
             argument=argument,
             target_name=target_name,
             level=level,
         )
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
         native_function = toolchain.tool_getattr(target, target_name)
 
         def pre(*args: P.args, **kwargs: P.kwargs) -> Any:
             arguments = self.argument(*args, **kwargs)
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/intercept.py` & `saleyo-1.0.4/src/saleyo/operation/intercept.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ..base.typing import MixinAble
+from ..base.typing import M
 from ..base.toolchain import InvokeEvent, ToolChain
 from ..base.template import MixinOperation
 
 from typing import Any, Callable, Generic, Optional, ParamSpec
 
 _PA = ParamSpec("_PA")
 _PB = ParamSpec("_PB")
 _A = InvokeEvent[_PA, Any]
 _B = InvokeEvent[_PB, Any]
 
 
-class Intercept(Generic[_PA, _PB], MixinOperation[Callable[[_A[_PA]], _B[_PB]]]):
+class Intercept(Generic[_PA, _PB, M], MixinOperation[Callable[[_A[_PA]], _B[_PB]], M]):
     """
     The `Intercept` allow you to intercept the arguments before invoking target method.
 
     Then, you can handle these arguments in your own function and make a redirect to another function.
 
     If you just want to modify the arguments or the result, please see `Pre` and `Post`.
     """
@@ -30,24 +30,24 @@
         super().__init__(argument, level)
         self.target_name = target_name
 
     @staticmethod
     def configure(
         level: int = 1,
         target_name: Optional[str] = None,
-    ) -> Callable[[Callable[[_A[_PA]], _B[_PB]]], "Intercept[_PA, _PB]"]:
+    ) -> Callable[[Callable[[_A[_PA]], _B[_PB]]], "Intercept[_PA, _PB, M]"]:
         return lambda argument: Intercept(
             argument=argument,
             level=level,
             target_name=target_name,
         )
 
     def mixin(
         self,
-        target: MixinAble,
+        target: M,
         toolchain: ToolChain = ToolChain(),
     ) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
 
         native_function = toolchain.tool_getattr(
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/modify.py` & `saleyo-1.0.4/src/saleyo/operation/modify.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 from typing import Any
 
-from ..base.typing import MixinAble
+from ..base.typing import M
 from ..base.toolchain import ToolChain
 from ..base.template import MixinOperation
 
 
-class ReName(MixinOperation[str]):
+class ReName(MixinOperation[str, Any]):
     """
     Rename the target name.
     """
 
     new: str
 
     def __init__(self, old: str, new: str, level=1) -> None:
         super().__init__(old, level)
         self.new = new
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         old = toolchain.tool_getattr(target, self.argument)
         toolchain.tool_delattr(target, self.argument)
         return toolchain.tool_setattr(target, self.new, old)
 
 
-class Del(MixinOperation[str]):
+class Del(MixinOperation[str, M]):
     """
     Delete something named `argument` this from target
     """
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_delattr(target, self.argument)
 
 
-class Alias(MixinOperation[str]):
+class Alias(MixinOperation[str, M]):
     """will copy the `argument` attribute to `alias`"""
 
     alias: str
 
     def __init__(self, argument: str, alias: str, level=1) -> None:
         super().__init__(argument, level)
         self.alias = alias
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_setattr(
             target, self.alias, toolchain.tool_getattr(target, self.argument)
         )
 
 
-class Insert(MixinOperation[Any]):
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+class Insert(MixinOperation[Any, M]):
+    """Will cover target when target exists."""
+
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_setattr(target, self.argument.__name__, self.argument)
+
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/overwrite.py` & `saleyo-1.0.4/src/saleyo/operation/overwrite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Optional
 
-from ..base.typing import MixinAble
+from ..base.typing import M
 from ..base.toolchain import ToolChain
 from ..base.template import MixinOperation
 
 
-class OverWrite(MixinOperation[Callable]):
+class OverWrite(MixinOperation[Callable, M]):
     """
     OverWrite is rude and it will cover the target method.
 
     If the target method doesn't exist, overwrite will add overwrite method to target class.
 
     Try avoid using `OverWrite` with other `OverWrite`.
     """
@@ -29,15 +29,15 @@
         target_name: Optional[str] = None,
     ) -> Callable[[Callable], "OverWrite"]:
         return lambda argument: OverWrite(
             argument=argument,
             target_name=target_name,
         )
 
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         target_name = (
             self.argument.__name__ if self.target_name is None else self.target_name
         )
         self.argument.__qualname__ = f"{target.__name__}.{target_name}"
         return toolchain.tool_setattr(
             target,
             target_name,
```

### Comparing `saleyo-1.0.3/src/saleyo/operation/processor.py` & `saleyo-1.0.4/src/saleyo/operation/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from inspect import getsource
 from types import ModuleType
 from typing import Callable, Optional
 
-from ..base.typing import MixinAble, NameSpace
+from ..base.typing import M, NameSpace
 from ..base.toolchain import Container, ToolChain
 from ..base.template import MixinOperation
 
 
-class Processor(MixinOperation[Callable[[str], str]]):
+class Processor(MixinOperation[Callable[[str], str], M]):
     """
     If you want to get the soure code of a method and use `split` and `replace` to modify and redefine it,Try `Processor`.
 
     When you try to use this, please make sure you configure the correct module of your target, or you can use `extra_namespace` to supplement the missing things.
 
     Don't try to use it with external code, like the code of cpython, it will crash.
     """
@@ -51,15 +51,15 @@
             target_name=target_name,
             module=module,
             extra_namespace=extra_namespace,
         )
 
     def mixin(
         self,
-        target: MixinAble,
+        target: M,
         toolchain: ToolChain = ToolChain(),
     ) -> None:
         target_name = (
             self.target_name if self.target_name is not None else self.argument.__name__
         )
 
         return toolchain.tool_setattr(
```

### Comparing `saleyo-1.0.3/tests/demo.py` & `saleyo-1.0.4/tests/demo.py`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.3/tests/intercept.py` & `saleyo-1.0.4/tests/intercept.py`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.3/PKG-INFO` & `saleyo-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saleyo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate.
 Author-Email: H2Sxxa <h2sxxa0w0@gmail.com>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/saleyo/
 Project-URL: Repository, https://github.com/H2Sxxa/saleyo
 Project-URL: Issues, https://github.com/H2Sxxa/saleyo/issues
 Requires-Python: >=3.8
@@ -48,15 +48,15 @@
 class Foo:
     __private = "private varible"
 
     def demo(self):
         pass
 
 
-@Mixin(target=Foo)
+@Mixin(target = Foo)
 class MixinFoo:
     # Will add a varible named `__private` to Foo and it has the same address with `_Foo__private`
     private: Accessor[str] = Accessor("__private")
 
     # Will Add the `func` to `Foo`
     @OverWrite
     def func(self):
@@ -120,14 +120,14 @@
 ### Custom Operation
 
 The default operations can't satify you? Why not try define a operation yourself!
 
 ```python
 from typing import Any
 from saleyo import MixinOperation, ToolChain
-from saleyo.base.typing import MixinAble
+from saleyo.base.typing import M
 
-class MyOperation(MixinOperation[Any]):
-    def mixin(self, target: MixinAble, toolchain: ToolChain = ...) -> None:
+class MyOperation(MixinOperation[Any, M]):
+    def mixin(self, target: M, toolchain: ToolChain = ...) -> None:
         ...
 ```
```

