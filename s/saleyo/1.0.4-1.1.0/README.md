# Comparing `tmp/saleyo-1.0.4.tar.gz` & `tmp/saleyo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saleyo-1.0.4.tar", last modified: Wed Apr 24 03:41:34 2024, max compression
+gzip compressed data, was "saleyo-1.1.0.tar", last modified: Wed Apr 24 12:14:43 2024, max compression
```

## Comparing `saleyo-1.0.4.tar` & `saleyo-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2024-04-24 03:41:20.490147 saleyo-1.0.4/LICENSE
--rw-r--r--   0        0        0     2540 2024-04-24 03:41:20.490147 saleyo-1.0.4/README.md
--rw-r--r--   0        0        0      581 2024-04-24 03:41:34.850283 saleyo-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1324 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/__init__.py
--rw-r--r--   0        0        0      103 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/__init__.py
--rw-r--r--   0        0        0      875 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/template.py
--rw-r--r--   0        0        0     3999 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/toolchain.py
--rw-r--r--   0        0        0      568 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/base/typing.py
--rw-r--r--   0        0        0     4733 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/mixin.py
--rw-r--r--   0        0        0      424 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/__init__.py
--rw-r--r--   0        0        0     1575 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/accessor.py
--rw-r--r--   0        0        0     1179 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/ancestor.py
--rw-r--r--   0        0        0     3162 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/hook.py
--rw-r--r--   0        0        0     1856 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/intercept.py
--rw-r--r--   0        0        0     1558 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/modify.py
--rw-r--r--   0        0        0     1283 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/overwrite.py
--rw-r--r--   0        0        0     2730 2024-04-24 03:41:20.490147 saleyo-1.0.4/src/saleyo/operation/processor.py
--rw-r--r--   0        0        0      100 2024-04-24 03:41:20.490147 saleyo-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0      244 2024-04-24 03:41:20.490147 saleyo-1.0.4/tests/custom.py
--rw-r--r--   0        0        0     1168 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/demo.py
--rw-r--r--   0        0        0      396 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/gc_test.py
--rw-r--r--   0        0        0      528 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/intercept.py
--rw-r--r--   0        0        0      301 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/misc_test.py
--rw-r--r--   0        0        0      201 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/modify_test.py
--rw-r--r--   0        0        0       37 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/test_module_a.py
--rw-r--r--   0        0        0      239 2024-04-24 03:41:20.494147 saleyo-1.0.4/tests/test_module_b.py
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 saleyo-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 12:14:23.333796 saleyo-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2537 2024-04-24 12:14:23.333796 saleyo-1.1.0/README.md
+-rw-r--r--   0        0        0      581 2024-04-24 12:14:43.001987 saleyo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1324 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/base/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/base/template.py
+-rw-r--r--   0        0        0     4000 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/base/toolchain.py
+-rw-r--r--   0        0        0      541 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/base/typing.py
+-rw-r--r--   0        0        0     4917 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/mixin.py
+-rw-r--r--   0        0        0      424 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/operation/__init__.py
+-rw-r--r--   0        0        0     2968 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/operation/accessor.py
+-rw-r--r--   0        0        0     1168 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/operation/ancestor.py
+-rw-r--r--   0        0        0     3156 2024-04-24 12:14:23.333796 saleyo-1.1.0/src/saleyo/operation/hook.py
+-rw-r--r--   0        0        0     1847 2024-04-24 12:14:23.337796 saleyo-1.1.0/src/saleyo/operation/intercept.py
+-rw-r--r--   0        0        0     1543 2024-04-24 12:14:23.337796 saleyo-1.1.0/src/saleyo/operation/modify.py
+-rw-r--r--   0        0        0     1280 2024-04-24 12:14:23.337796 saleyo-1.1.0/src/saleyo/operation/overwrite.py
+-rw-r--r--   0        0        0     2727 2024-04-24 12:14:23.337796 saleyo-1.1.0/src/saleyo/operation/processor.py
+-rw-r--r--   0        0        0      100 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/custom.py
+-rw-r--r--   0        0        0     1168 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/demo.py
+-rw-r--r--   0        0        0      396 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/gc_test.py
+-rw-r--r--   0        0        0      528 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/intercept.py
+-rw-r--r--   0        0        0      711 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/misc_test.py
+-rw-r--r--   0        0        0      216 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/modify_test.py
+-rw-r--r--   0        0        0       37 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/test_module_a.py
+-rw-r--r--   0        0        0      239 2024-04-24 12:14:23.337796 saleyo-1.1.0/tests/test_module_b.py
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 saleyo-1.1.0/PKG-INFO
```

### Comparing `saleyo-1.0.4/LICENSE` & `saleyo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.4/README.md` & `saleyo-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,12 +110,12 @@
 The default operations can't satify you? Why not try define a operation yourself!
 
 ```python
 from typing import Any
 from saleyo import MixinOperation, ToolChain
 from saleyo.base.typing import M
 
-class MyOperation(MixinOperation[Any, M]):
+class MyOperation(MixinOperation[Any]):
     def mixin(self, target: M, toolchain: ToolChain = ...) -> None:
         ...
 ```
```

### Comparing `saleyo-1.0.4/pyproject.toml` & `saleyo-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saleyo"
-version = "1.0.4"
+version = "1.1.0"
 description = "Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate."
 authors = [
     { name = "H2Sxxa", email = "h2sxxa0w0@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `saleyo-1.0.4/src/saleyo/__init__.py` & `saleyo-1.1.0/src/saleyo/__init__.py`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.4/src/saleyo/base/template.py` & `saleyo-1.1.0/src/saleyo/base/template.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC
 from typing import Any, Generic
 
 from .toolchain import ToolChain
 from .typing import T, M
 
 
-class MixinOperation(Generic[T, M], ABC):
+class MixinOperation(Generic[T], ABC):
     """
     The MixinOperation is the base of All Operation.
 
     The generic `MixinOperation` is the type of argument.
 
     `level` will affect to the mixin order, default `1`.
```

### Comparing `saleyo-1.0.4/src/saleyo/base/toolchain.py` & `saleyo-1.1.0/src/saleyo/base/toolchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self.args = args
         self.kwargs = kwargs
 
     def __str__(self) -> str:
-        return f"Arugument(positional: {self.args}, keyword: {self.kwargs} )"
+        return f"Arugument( positional: {self.args}, keyword: {self.kwargs} )"
 
 
 class InvokeEvent(Generic[P, RT]):
     """
     A `InvokeEvent` includes the target function and the arguments to call this functions.
     """
```

### Comparing `saleyo-1.0.4/src/saleyo/mixin.py` & `saleyo-1.1.0/src/saleyo/mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 class Mixin(Generic[M]):
     """
     A `Mixin` Decorator is used to invoke all the `MixinOperation` in Mixin Class.
 
     If the target is a special class, you should custom the toolchain yourself.
 
+    It is recommend to use `assert isinstance(self, <target>)` at the head of operation functions, although there may be some performance cost, but it is worth it in most conditions.
+
     Allow to have more than one target, but that's not recommended.
     """
 
     target: Iterable[M]
     toolchain: ToolChain
     reverse_level: bool
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/accessor.py` & `saleyo-1.1.0/src/saleyo/operation/accessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,89 @@
-from typing import Generic, Optional
+from typing import Callable, Generic, Optional
 
 from ..base.toolchain import ToolChain
-from ..base.typing import T, M
+from ..base.typing import P, T, M
 from ..base.template import MixinOperation
 
 
-class Accessor(Generic[T, M], MixinOperation[str, M]):
+class Accessor(Generic[T], MixinOperation[str]):
     """
-    Want to access and modify some private varibles or methods? Try use `Accessor`!
-
-    The Generic is the type of target varible.
+    The Generic `T` is the type of target varible, if you want to visit a private function, try to use `FunctionAccessor`.
 
     Notice: The value only available after invoking the `mixin` method.
 
-    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix to argument.
+    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix to argument, if the target is complex, you can set `private` to `False` and provide the true name by yourself.
 
     If you use `@Mixin` and have more than one target classes, the `value` will always be the varible of latest target.
     """
 
     _inner: Optional[T]
     _private: bool
 
     def __init__(self, argument: str, level=1, private=True) -> None:
         super().__init__(argument, level)
         self._inner = None
         self._private = private
 
-    @staticmethod
-    def configure(level: int = 1):
-        return lambda argument: Accessor(
-            argument=argument,
-            level=level,
-            private=True,
-        )
-
     def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         self._inner = toolchain.tool_getattr(
             target,
             f"_{target.__name__}{self.argument}" if self._private else self.argument,
         )
         return toolchain.tool_setattr(
             target,
             self.argument,
             self._inner,
         )
 
     @property
-    def value(self) -> Optional[T]:
+    def value(self) -> T:
         """
-        Will be None Call Before The `mixin` method call.
+        Don't use until The `mixin` method call.
         """
+        assert self._inner
         return self._inner
+
+    @value.setter
+    def value(self, value: T):
+        self._inner = value
+
+    @value.deleter
+    def value(self):
+        # may cause some problems
+        del self.value
+
+    def __str__(self) -> str:
+        return f"Accessor {{ value: {self._inner} ({id(self._inner)}) }}"
+
+
+class FunctionAccessor(Generic[P, T], MixinOperation[str]):
+    """
+    `FunctionAccessor` can be call directly.
+
+    It's recommend to provide the Generic `P` and `T`, it can be useful in `__call__`.
+
+    If the `private` is `True`, will add target class name (like `_Foo`) to the prefix to argument, if the target is complex, you can set `private` to `False` and provide the true name by yourself.
+
+    If you just call in operation functions, you can just use a variable with `Callable[P, T]` type.
+
+    ```python
+    something: FunctionAccessor[[str], None] = FunctionAccessor("something")
+    ```
+    """
+
+    _inner: Optional[Callable[P, T]] = None
+    _private: bool
+
+    def __init__(self, argument: str, level=1, private=True) -> None:
+        super().__init__(argument, level)
+        self._private = private
+
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
+        self._inner = toolchain.tool_getattr(
+            target,
+            f"_{target.__name__}{self.argument}" if self._private else self.argument,
+        )
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
+        assert self._inner
+        return self._inner(*args, **kwargs)
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/ancestor.py` & `saleyo-1.1.0/src/saleyo/operation/ancestor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Type
 from saleyo.base.template import MixinOperation
 from saleyo.base.toolchain import ToolChain
 from saleyo.base.typing import M
 
 
-class Ancestor(MixinOperation[Type[Any], M]):
+class Ancestor(MixinOperation[Type[Any]]):
     """
     Ancestor will add the `argument` to `target.__bases__`.
 
     If `reverse`, the `argument` will add to the head of `target.__bases__`.
 
     Don't try to use it with external code and `module`, it may crash.
     """
@@ -26,15 +26,15 @@
     ):
         return lambda argument: Ancestor(
             argument,
             level=level,
             reverse=reverse,
         )
 
-    def mixin(self, target: Type[Any], toolchain: ToolChain = ToolChain()) -> None:
+    def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_setattr(
             target,
             "__bases__",
             (self.argument, *toolchain.tool_getattr(target, "__bases__"))
             if self.reverse
             else (*toolchain.tool_getattr(target, "__bases__"), self.argument),
         )
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/hook.py` & `saleyo-1.1.0/src/saleyo/operation/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Optional, Union
 
 from ..base.typing import M, P, RT, T
 from ..base.toolchain import ToolChain, Arguments
 from ..base.template import MixinOperation
 
 
-class Post(MixinOperation[Callable[[T], Optional[RT]], M]):
+class Post(MixinOperation[Callable[[T], Optional[RT]]]):
     """
     `Post` will call after the target method, and the callable should be decorated as `@staticmethod` and have one argument to receive the result of target method.
 
     If the `post` function return value is not `None`, it will replace the original result.
     """
 
     target_name: Optional[str]
@@ -46,15 +46,15 @@
             if post_result is not None:
                 return post_result
             return result
 
         return toolchain.tool_setattr(target, target_name, post)
 
 
-class Pre(MixinOperation[Callable[P, Optional[Arguments[P]]], M]):
+class Pre(MixinOperation[Callable[P, Optional[Arguments[P]]]]):
     """
     `Pre` will call before the target method, and the callable should be decorated as `@staticmethod` and have `*args,**kwargs` to receive the arguments of target method.
 
     If the `pre` function return value is a `Aruguments`(not `None`), it will replace the original arguments.
     """
 
     target_name: Optional[str]
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/intercept.py` & `saleyo-1.1.0/src/saleyo/operation/intercept.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 _PA = ParamSpec("_PA")
 _PB = ParamSpec("_PB")
 _A = InvokeEvent[_PA, Any]
 _B = InvokeEvent[_PB, Any]
 
 
-class Intercept(Generic[_PA, _PB, M], MixinOperation[Callable[[_A[_PA]], _B[_PB]], M]):
+class Intercept(Generic[_PA, _PB], MixinOperation[Callable[[_A[_PA]], _B[_PB]]]):
     """
     The `Intercept` allow you to intercept the arguments before invoking target method.
 
     Then, you can handle these arguments in your own function and make a redirect to another function.
 
     If you just want to modify the arguments or the result, please see `Pre` and `Post`.
     """
@@ -30,15 +30,15 @@
         super().__init__(argument, level)
         self.target_name = target_name
 
     @staticmethod
     def configure(
         level: int = 1,
         target_name: Optional[str] = None,
-    ) -> Callable[[Callable[[_A[_PA]], _B[_PB]]], "Intercept[_PA, _PB, M]"]:
+    ) -> Callable[[Callable[[_A[_PA]], _B[_PB]]], "Intercept[_PA, _PB]"]:
         return lambda argument: Intercept(
             argument=argument,
             level=level,
             target_name=target_name,
         )
 
     def mixin(
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/modify.py` & `saleyo-1.1.0/src/saleyo/operation/modify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 
 from ..base.typing import M
 from ..base.toolchain import ToolChain
 from ..base.template import MixinOperation
 
 
-class ReName(MixinOperation[str, Any]):
+class ReName(MixinOperation[str]):
     """
     Rename the target name.
     """
 
     new: str
 
     def __init__(self, old: str, new: str, level=1) -> None:
@@ -18,37 +18,36 @@
 
     def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         old = toolchain.tool_getattr(target, self.argument)
         toolchain.tool_delattr(target, self.argument)
         return toolchain.tool_setattr(target, self.new, old)
 
 
-class Del(MixinOperation[str, M]):
+class Del(MixinOperation[str]):
     """
     Delete something named `argument` this from target
     """
 
     def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_delattr(target, self.argument)
 
 
-class Alias(MixinOperation[str, M]):
+class Alias(MixinOperation[str]):
     """will copy the `argument` attribute to `alias`"""
 
     alias: str
 
     def __init__(self, argument: str, alias: str, level=1) -> None:
         super().__init__(argument, level)
         self.alias = alias
 
     def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_setattr(
             target, self.alias, toolchain.tool_getattr(target, self.argument)
         )
 
 
-class Insert(MixinOperation[Any, M]):
+class Insert(MixinOperation[Any]):
     """Will cover target when target exists."""
 
     def mixin(self, target: M, toolchain: ToolChain = ToolChain()) -> None:
         return toolchain.tool_setattr(target, self.argument.__name__, self.argument)
-
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/overwrite.py` & `saleyo-1.1.0/src/saleyo/operation/overwrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Optional
 
 from ..base.typing import M
 from ..base.toolchain import ToolChain
 from ..base.template import MixinOperation
 
 
-class OverWrite(MixinOperation[Callable, M]):
+class OverWrite(MixinOperation[Callable]):
     """
     OverWrite is rude and it will cover the target method.
 
     If the target method doesn't exist, overwrite will add overwrite method to target class.
 
     Try avoid using `OverWrite` with other `OverWrite`.
     """
```

### Comparing `saleyo-1.0.4/src/saleyo/operation/processor.py` & `saleyo-1.1.0/src/saleyo/operation/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional
 
 from ..base.typing import M, NameSpace
 from ..base.toolchain import Container, ToolChain
 from ..base.template import MixinOperation
 
 
-class Processor(MixinOperation[Callable[[str], str], M]):
+class Processor(MixinOperation[Callable[[str], str]]):
     """
     If you want to get the soure code of a method and use `split` and `replace` to modify and redefine it,Try `Processor`.
 
     When you try to use this, please make sure you configure the correct module of your target, or you can use `extra_namespace` to supplement the missing things.
 
     Don't try to use it with external code, like the code of cpython, it will crash.
     """
```

### Comparing `saleyo-1.0.4/tests/demo.py` & `saleyo-1.1.0/tests/demo.py`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.4/tests/intercept.py` & `saleyo-1.1.0/tests/intercept.py`

 * *Files identical despite different names*

### Comparing `saleyo-1.0.4/PKG-INFO` & `saleyo-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saleyo
-Version: 1.0.4
+Version: 1.1.0
 Summary: Saleyo is a lightwight scalable Python AOP framework, easy to use and integrate.
 Author-Email: H2Sxxa <h2sxxa0w0@gmail.com>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/saleyo/
 Project-URL: Repository, https://github.com/H2Sxxa/saleyo
 Project-URL: Issues, https://github.com/H2Sxxa/saleyo/issues
 Requires-Python: >=3.8
@@ -122,12 +122,12 @@
 The default operations can't satify you? Why not try define a operation yourself!
 
 ```python
 from typing import Any
 from saleyo import MixinOperation, ToolChain
 from saleyo.base.typing import M
 
-class MyOperation(MixinOperation[Any, M]):
+class MyOperation(MixinOperation[Any]):
     def mixin(self, target: M, toolchain: ToolChain = ...) -> None:
         ...
 ```
```

