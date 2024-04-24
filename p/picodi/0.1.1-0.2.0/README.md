# Comparing `tmp/picodi-0.1.1.tar.gz` & `tmp/picodi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.1.1.tar", max compression
+gzip compressed data, was "picodi-0.2.0.tar", max compression
```

## Comparing `picodi-0.1.1.tar` & `picodi-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 21:55:04.108390 picodi-0.1.1/LICENSE
--rw-r--r--   0        0        0     1151 2024-04-23 21:55:04.108390 picodi-0.1.1/README.md
--rw-r--r--   0        0        0      173 2024-04-23 21:55:04.108390 picodi-0.1.1/picodi/__init__.py
--rw-r--r--   0        0        0     9211 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/py.typed
--rw-r--r--   0        0        0      747 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/scopes.py
--rw-r--r--   0        0        0     2583 2024-04-23 21:55:04.112390 picodi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 picodi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 00:17:43.986736 picodi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1151 2024-04-24 00:17:43.986736 picodi-0.2.0/README.md
+-rw-r--r--   0        0        0      173 2024-04-24 00:17:43.986736 picodi-0.2.0/picodi/__init__.py
+-rw-r--r--   0        0        0     8894 2024-04-24 00:17:43.986736 picodi-0.2.0/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:17:43.986736 picodi-0.2.0/picodi/py.typed
+-rw-r--r--   0        0        0      747 2024-04-24 00:17:43.986736 picodi-0.2.0/picodi/scopes.py
+-rw-r--r--   0        0        0     2583 2024-04-24 00:17:43.986736 picodi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 picodi-0.2.0/PKG-INFO
```

### Comparing `picodi-0.1.1/LICENSE` & `picodi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.1.1/README.md` & `picodi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `picodi-0.1.1/picodi/picodi.py` & `picodi-0.2.0/picodi/picodi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import inspect
 import threading
 from collections.abc import Awaitable, Callable, Coroutine, Generator
-from contextlib import (
-    AsyncExitStack,
-    ExitStack,
-    asynccontextmanager,
-    contextmanager,
-    nullcontext,
-)
+from contextlib import AsyncExitStack, ExitStack, asynccontextmanager, contextmanager
 from dataclasses import dataclass, field
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     ContextManager,
     ParamSpec,
@@ -39,15 +33,15 @@
 _lock = threading.RLock()
 _scopes: dict[str, Scope] = {
     "null": NullScope(),
     "singleton": SingletonScope(),
 }
 
 
-def Provide(dependency: Dependency, /, use_cache: bool = True) -> Any:  # noqa: N802
+def Provide(dependency: Dependency, /) -> Any:  # noqa: N802
     """
     Declare a provider.
     It takes a single "dependency" callable (like a function).
     Don't call it directly, picodi will call it for you.
     Dependency can be a regular function or a generator with one yield.
     If the dependency is a generator, it will be used as a context manager.
     Any generator that is valid for `contextlib.contextmanager`
@@ -71,15 +65,15 @@
     def my_service(db=Provide(get_db), settings=Provide(get_settings)):
         assert db == "db connection"
         assert isinstance(settings, Settings)
     ```
     """
     if not getattr(dependency, "_scope_", None):
         dependency._scope_ = "null"  # type: ignore[attr-defined] # noqa: SF01
-    return Depends.from_dependency(dependency, use_cache)
+    return Depends.from_dependency(dependency)
 
 
 def inject(fn: Callable[P, T]) -> Callable[P, T | Coroutine[Any, Any, T]]:
     """
     Decorator to inject dependencies into a function.
     Use it in combination with `Provide` to declare dependencies.
 
@@ -96,42 +90,34 @@
     if inspect.iscoroutinefunction(fn):
 
         @functools.wraps(fn)
         async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             bound = signature.bind(*args, **kwargs)
             bound.apply_defaults()
             exit_stack = AsyncExitStack()
-            for depends, names, get_value in _resolve_depends(
+            for names, get_value in _arguments_to_getter(
                 bound, exit_stack, is_async=True
             ):
-                if depends.use_cache:
-                    value = await get_value()
-                    bound.arguments.update({name: value for name in names})
-                else:
-                    bound.arguments.update({name: await get_value() for name in names})
+                bound.arguments.update({name: await get_value() for name in names})
 
             async with exit_stack:
                 result = await fn(*bound.args, **bound.kwargs)
             return result
 
     else:
 
         @functools.wraps(fn)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             bound = signature.bind(*args, **kwargs)
             bound.apply_defaults()
             exit_stack = ExitStack()
-            for depends, names, get_value in _resolve_depends(
+            for names, get_value in _arguments_to_getter(
                 bound, exit_stack, is_async=False
             ):
-                if depends.use_cache:
-                    value = get_value()
-                    bound.arguments.update({name: value for name in names})
-                else:
-                    bound.arguments.update({name: get_value() for name in names})
+                bound.arguments.update({name: get_value() for name in names})
 
             with exit_stack:
                 result = fn(*bound.args, **bound.kwargs)
             return result
 
     return wrapper
 
@@ -155,15 +141,15 @@
         print("closing db connection")
     ```
     """
     if not inspect.isgeneratorfunction(fn) and not inspect.isasyncgenfunction(fn):
         raise TypeError("Resource should be a generator function")
     fn._scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
     with _lock:
-        _resources.append(Depends.from_dependency(fn, use_cache=True))
+        _resources.append(Depends.from_dependency(fn))
     return fn
 
 
 def init_resources() -> Awaitable | None:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
@@ -195,103 +181,109 @@
 
 CallableManager = Callable[..., AsyncContextManager | ContextManager]
 
 
 @dataclass(frozen=True)
 class Depends:
     dependency: Dependency
-    use_cache: bool
     context_manager: CallableManager | None = field(compare=False)
     is_async: bool = field(compare=False)
 
     def get_scope_name(self) -> str:
         return self.dependency._scope_  # type: ignore[attr-defined] # noqa: SF01
 
-    def value_as_context_manager(self) -> Any:
-        if self.context_manager:
-            return self.context_manager()
-        return nullcontext(self.dependency())
-
     @classmethod
-    def from_dependency(cls, dependency: Dependency, use_cache: bool) -> Depends:
+    def from_dependency(cls, dependency: Dependency) -> Depends:
         context_manager: Callable | None = None
-        is_async = False
+        is_async = inspect.iscoroutinefunction(dependency)
         if inspect.isasyncgenfunction(dependency):
             context_manager = asynccontextmanager(dependency)
             is_async = True
         elif inspect.isgeneratorfunction(dependency):
             context_manager = contextmanager(dependency)
 
-        return cls(dependency, use_cache, context_manager, is_async)
+        return cls(dependency, context_manager, is_async)
 
 
-def _resolve_depends(
+def _arguments_to_getter(
     bound: BoundArguments, exit_stack: AsyncExitStack | ExitStack, is_async: bool
-) -> Generator[tuple[Depends, list[str], Callable[[], Any]], None, None]:
+) -> Generator[tuple[list[str], Callable[[], Any]], None, None]:
     dependencies: dict[Depends, list[str]] = {}
     for name, value in bound.arguments.items():
         if isinstance(value, Depends):
             dependencies.setdefault(value, []).append(name)
 
     get_val = _get_value_from_depends_async if is_async else _get_value_from_depends
 
     for depends, names in dependencies.items():
         get_value = functools.partial(get_val, depends, exit_stack)  # type: ignore
-        yield depends, names, get_value
+        yield names, get_value
 
 
 def _get_value_from_depends(
     depends: Depends,
     local_exit_stack: ExitStack,
 ) -> Any:
     scope_name = depends.get_scope_name()
     scope = _scopes[scope_name]
     try:
         value = scope.get(depends.dependency)
     except KeyError:
-        context_manager = depends.value_as_context_manager()
         exit_stack = local_exit_stack
         if scope_name == "singleton":
             exit_stack = _exit_stack
         if depends.is_async:
-            value = depends.dependency
+            value = depends.dependency()
         else:
             with _lock:
                 try:
                     value = scope.get(depends.dependency)
                 except KeyError:
-                    value = exit_stack.enter_context(context_manager)
+                    value = _call_value(depends, exit_stack)
                     scope.set(depends.dependency, value)
     return value
 
 
 async def _get_value_from_depends_async(
     depends: Depends,
     local_exit_stack: AsyncExitStack,
 ) -> Any:
     scope_name = depends.get_scope_name()
     scope = _scopes[scope_name]
     try:
         value = scope.get(depends.dependency)
     except KeyError:
-        context_manager = depends.value_as_context_manager()
         exit_stack = local_exit_stack
         if scope_name == "singleton":
             exit_stack = _async_exit_stack
         with _lock:
             try:
                 value = scope.get(depends.dependency)
             except KeyError:
+                value = _call_value(depends, exit_stack)
                 if depends.is_async:
-                    value = await exit_stack.enter_async_context(context_manager)
-                else:
-                    value = exit_stack.enter_context(context_manager)
+                    value = await value
                 scope.set(depends.dependency, value)
     return value
 
 
+def _call_value(depends: Depends, exit_stack: ExitStack | AsyncExitStack) -> Any:
+    if depends.is_async:
+        if depends.context_manager:
+            return exit_stack.enter_async_context(  # type: ignore[union-attr]
+                depends.context_manager()  # type: ignore[arg-type]
+            )
+        return depends.dependency()
+    else:
+        if depends.context_manager:
+            return exit_stack.enter_context(
+                depends.context_manager()  # type: ignore[arg-type]
+            )
+        return depends.dependency()
+
+
 def _is_async_environment() -> bool:
     try:
         asyncio.get_running_loop()
     except RuntimeError:
         return False
     return True
```

### Comparing `picodi-0.1.1/picodi/scopes.py` & `picodi-0.2.0/picodi/scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.1.1/pyproject.toml` & `picodi-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.1.1"
+version = "0.2.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.1.1/PKG-INFO` & `picodi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

