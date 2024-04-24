# Comparing `tmp/picodi-0.1.0.tar.gz` & `tmp/picodi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.1.0.tar", max compression
+gzip compressed data, was "picodi-0.1.1.tar", max compression
```

## Comparing `picodi-0.1.0.tar` & `picodi-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-20 22:47:49.315404 picodi-0.1.0/LICENSE
--rw-r--r--   0        0        0     1151 2024-04-23 18:32:32.692046 picodi-0.1.0/README.md
--rw-r--r--   0        0        0      173 2024-04-23 18:32:32.687702 picodi-0.1.0/picodi/__init__.py
--rw-r--r--   0        0        0     8927 2024-04-23 18:32:32.711628 picodi-0.1.0/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-04-20 22:47:49.338206 picodi-0.1.0/picodi/py.typed
--rw-r--r--   0        0        0      747 2024-04-22 18:34:38.779767 picodi-0.1.0/picodi/scopes.py
--rw-r--r--   0        0        0     2583 2024-04-23 18:32:32.671575 picodi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 picodi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 21:55:04.108390 picodi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1151 2024-04-23 21:55:04.108390 picodi-0.1.1/README.md
+-rw-r--r--   0        0        0      173 2024-04-23 21:55:04.108390 picodi-0.1.1/picodi/__init__.py
+-rw-r--r--   0        0        0     9211 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/py.typed
+-rw-r--r--   0        0        0      747 2024-04-23 21:55:04.112390 picodi-0.1.1/picodi/scopes.py
+-rw-r--r--   0        0        0     2583 2024-04-23 21:55:04.112390 picodi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 picodi-0.1.1/PKG-INFO
```

### Comparing `picodi-0.1.0/LICENSE` & `picodi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.1.0/README.md` & `picodi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `picodi-0.1.0/picodi/picodi.py` & `picodi-0.1.1/picodi/picodi.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,64 +159,71 @@
         raise TypeError("Resource should be a generator function")
     fn._scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
     with _lock:
         _resources.append(Depends.from_dependency(fn, use_cache=True))
     return fn
 
 
-def init_resources() -> Awaitable:
+def init_resources() -> Awaitable | None:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
     async_resources = []
     for depends in _resources:
         if depends.is_async:
             async_resources.append(
                 _get_value_from_depends_async(depends, _async_exit_stack)
             )
         else:
             _get_value_from_depends(depends, _exit_stack)
 
-    return asyncio.gather(*async_resources)
+    if _is_async_environment():
+        return asyncio.gather(*async_resources)
+    return None
 
 
-def shutdown_resources() -> Awaitable:
+def shutdown_resources() -> Awaitable | None:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
     _exit_stack.close()
-    return _async_exit_stack.aclose()
+    if _is_async_environment():
+        return _async_exit_stack.aclose()
+    return None
+
+
+CallableManager = Callable[..., AsyncContextManager | ContextManager]
 
 
 @dataclass(frozen=True)
 class Depends:
     dependency: Dependency
     use_cache: bool
-    context_manager: ContextManager | AsyncContextManager | None = field(compare=False)
+    context_manager: CallableManager | None = field(compare=False)
     is_async: bool = field(compare=False)
 
     def get_scope_name(self) -> str:
         return self.dependency._scope_  # type: ignore[attr-defined] # noqa: SF01
 
     def value_as_context_manager(self) -> Any:
         if self.context_manager:
-            return self.context_manager
+            return self.context_manager()
         return nullcontext(self.dependency())
 
     @classmethod
     def from_dependency(cls, dependency: Dependency, use_cache: bool) -> Depends:
-        context_manager: ContextManager | AsyncContextManager | None = None
+        context_manager: Callable | None = None
         is_async = False
         if inspect.isasyncgenfunction(dependency):
-            context_manager = asynccontextmanager(dependency)()
+            context_manager = asynccontextmanager(dependency)
             is_async = True
         elif inspect.isgeneratorfunction(dependency):
-            context_manager = contextmanager(dependency)()
+            context_manager = contextmanager(dependency)
 
         return cls(dependency, use_cache, context_manager, is_async)
 
 
 def _resolve_depends(
     bound: BoundArguments, exit_stack: AsyncExitStack | ExitStack, is_async: bool
 ) -> Generator[tuple[Depends, list[str], Callable[[], Any]], None, None]:
@@ -276,7 +283,15 @@
             except KeyError:
                 if depends.is_async:
                     value = await exit_stack.enter_async_context(context_manager)
                 else:
                     value = exit_stack.enter_context(context_manager)
                 scope.set(depends.dependency, value)
     return value
+
+
+def _is_async_environment() -> bool:
+    try:
+        asyncio.get_running_loop()
+    except RuntimeError:
+        return False
+    return True
```

### Comparing `picodi-0.1.0/picodi/scopes.py` & `picodi-0.1.1/picodi/scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.1.0/pyproject.toml` & `picodi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.1.0"
+version = "0.1.1"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.1.0/PKG-INFO` & `picodi-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/yakimka/picodi
 Description-Content-Type: text/markdown
 
 # picodi
 
 [![Build Status](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml/badge.svg?branch=main&event=push)](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml)
```

