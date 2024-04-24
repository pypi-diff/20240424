# Comparing `tmp/pop_cli-4.3.0.tar.gz` & `tmp/pop_cli-4.3.1.tar.gz`

## Comparing `pop_cli-4.3.0.tar` & `pop_cli-4.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-4.3.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/__main__.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/config.yaml
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/config.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/console.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/init.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.3.0/src/hub/state.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.3.0/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.3.0/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.3.0/README.rst
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pop_cli-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-4.3.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1087 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/__main__.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/config.yaml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/config.py
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/console.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/init.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/state.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.3.1/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.3.1/README.rst
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pop_cli-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-4.3.1/PKG-INFO
```

### Comparing `pop_cli-4.3.0/.pre-commit-config.yaml` & `pop_cli-4.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/src/__main__.py` & `pop_cli-4.3.1/src/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,24 @@
 
 
 async def amain(loop):
     async with cpop.hub.Hub(cli="cli") as hub:
         await hub.log.debug("Initialized the hub")
 
         # Start the hub cli
-        holder = asyncio.create_task(hub._holder())
+        task = asyncio.create_task(hub._holder())
 
         try:
             await hub.cli.init.run()
         except KeyboardInterrupt:
             await hub.log.error("Caught keyboard interrupt.  Cancelling...")
         except SystemExit:
             ...
         finally:
             await hub.log.debug("Cleaning up")
             await hub._tasks.put(cpop.hub.SHUTDOWN_SIGNAL)
-            await holder
+            await task
             await loop.shutdown_asyncgens()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pop_cli-4.3.0/src/config.yaml` & `pop_cli-4.3.1/src/config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/src/hub/cli.py` & `pop_cli-4.3.1/src/hub/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return value
     if any(
         (
             hub.lib.re.match(r'^f".*"$', value),
             hub.lib.re.match(r"^hub[\.\w]+(?:\(.*\))?$", value),
         )
     ):
-        value = hub.lib.ast.literal_eval(value, {"hub": hub})
+        value = eval(value, {"hub": hub})
         if hub.lib.asyncio.iscoroutine(value):
             value = await value
 
         return await hub.cli.cli.parse_value(value)
 
     try:
         return hub.lib.json.loads(value)
```

### Comparing `pop_cli-4.3.0/src/hub/config.py` & `pop_cli-4.3.1/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/src/hub/console.py` & `pop_cli-4.3.1/src/hub/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,18 @@
 
                 result = local_namespace.pop("__result__", None)
                 post = {k: v for k, v in local_namespace.items() if k != "hub"}
 
                 # The locals didn't change, this wasn't a variable assignment
                 if previous == post:
                     # If an async function was called without being assigned to a variable then await it
-                    if hub.lib.asyncio.iscoroutine(result) and result not in local_namespace.values():
+                    if (
+                        hub.lib.asyncio.iscoroutine(result)
+                        and result not in local_namespace.values()
+                    ):
                         result = await result
 
                     # If the result wasn't assigned to a variable then print it out
                     if result is not None:
                         await hub.lib.aioconsole.aprint(result)
 
         except EOFError:
@@ -103,15 +106,17 @@
                         continue
                     try:
                         finder = getattr(finder, p)
                     except AttributeError:
                         try:
                             finder = finder.__getitem__(p)
                         except TypeError:
-                            if p.isdigit() and isinstance(finder, hub.lib.typing.Iterable):
+                            if p.isdigit() and isinstance(
+                                finder, hub.lib.typing.Iterable
+                            ):
                                 try:
                                     finder = tuple(finder).__getitem__(int(p))
                                 except Exception:
                                     # No completions if the path is invalid
                                     return
                             else:
                                 # No completions if the path is invalid
@@ -147,18 +152,22 @@
                                 display=display,
                             )
                     except Exception:
                         continue
 
     completer = HubCompleter()
     # Create a completer for local variables
-    local_completer = hub.lib.prompt_toolkit.completion.WordCompleter(list(kwargs.keys()), ignore_case=True)
+    local_completer = hub.lib.prompt_toolkit.completion.WordCompleter(
+        list(kwargs.keys()), ignore_case=True
+    )
 
     # Create a completer for built-in functions
     builtins = [*list(dir(hub.lib.builtins)), "await", "hub"]
-    builtins_completer = hub.lib.prompt_toolkit.completion.WordCompleter(builtins, ignore_case=True)
+    builtins_completer = hub.lib.prompt_toolkit.completion.WordCompleter(
+        builtins, ignore_case=True
+    )
 
     # Combine the hub, local, and built-in completers
     combined_completer = hub.lib.prompt_toolkit.completion.merge_completers(
         [completer, local_completer, builtins_completer]
     )
     return combined_completer
```

### Comparing `pop_cli-4.3.0/src/hub/init.py` & `pop_cli-4.3.1/src/hub/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 
     # Try to restore the hub state
     hub_state_file = await hub.cli.state.restore(opt)
 
     call_help = False
     if (opt.cli.cli != cli) and (
         opt.cli.cli
-        or ((cli in hub._dynamic.config.cli_config) and (cli not in opt.get("pop", {}).get("global_clis", ())))
+        or (
+            (cli in hub._dynamic.config.cli_config)
+            and (cli not in opt.get("pop", {}).get("global_clis", ()))
+        )
     ):
         await hub.log.debug(f"Loading cli: {cli}")
         # Reload hub.OPT with the cli arguments not consumed by the initial hub
         await hub.cli.config.override(cli, opt)
         args = []
         kwargs = {}
     else:
```

### Comparing `pop_cli-4.3.0/src/hub/ref.py` & `pop_cli-4.3.1/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/src/hub/state.py` & `pop_cli-4.3.1/src/hub/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/conftest.py` & `pop_cli-4.3.1/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import aiopath
 import cpop.hub
 import pytest
 
 
 @pytest.fixture(name="hub")
 async def testing_hub():
-    async with cpop.hub.Hub() as hub:
+    async with cpop.hub.Hub(
+        logs=False,
+    ) as hub:
         yield hub
 
 
 @pytest.fixture(autouse=True, scope="session")
 async def tpath():
     code_dir = await aiopath.AsyncPath(__file__).parent.parent.absolute()
     assert await code_dir.exists()
```

### Comparing `pop_cli-4.3.0/tests/integration/test_cli.py` & `pop_cli-4.3.1/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/integration/test_config.py` & `pop_cli-4.3.1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/integration/test_console.py` & `pop_cli-4.3.1/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/integration/test_init.py` & `pop_cli-4.3.1/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/integration/test_ref.py` & `pop_cli-4.3.1/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/tests/integration/test_state.py` & `pop_cli-4.3.1/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/.gitignore` & `pop_cli-4.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/README.rst` & `pop_cli-4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.0/pyproject.toml` & `pop_cli-4.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "4.3.0"
+version = "4.3.1"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
     "aiopath",
-    "cPop>=35.0.0",
+    "cPop>=35.0.6",
     "aioconsole",
     "prompt-toolkit",
 ]
 
 
 [project.optional-dependencies]
 test = [
@@ -154,15 +154,14 @@
   "ISC001",
   # Don't require logging exceptions
   "S112",
   # Ignore 'too many branches'
   "PLR0912",
   # Mutltiple isinstance calls
   "UP038",
-
 ]
 
 [tool.ruff.lint.isort]
 known-first-party = ["cpop"]
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
```

### Comparing `pop_cli-4.3.0/PKG-INFO` & `pop_cli-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 4.3.0
+Version: 4.3.1
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiopath
-Requires-Dist: cpop>=35.0.0
+Requires-Dist: cpop>=35.0.6
 Requires-Dist: prompt-toolkit
 Provides-Extra: test
 Requires-Dist: cpop[test]; extra == 'test'
 Requires-Dist: pexpect; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
```

