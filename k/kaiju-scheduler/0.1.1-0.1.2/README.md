# Comparing `tmp/kaiju_scheduler-0.1.1-py3-none-any.whl.zip` & `tmp/kaiju_scheduler-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 8642 bytes, number of entries: 9
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-19 10:55 kaiju_scheduler/__init__.py
--rw-r--r--  2.0 unx      267 b- defN 24-Apr-19 10:55 kaiju_scheduler/interfaces.py
--rw-r--r--  2.0 unx    10859 b- defN 24-Apr-19 10:55 kaiju_scheduler/scheduler.py
--rw-r--r--  2.0 unx     2721 b- defN 24-Apr-19 10:55 kaiju_scheduler/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-19 10:55 kaiju_scheduler-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4638 b- defN 24-Apr-19 10:55 kaiju_scheduler-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 10:55 kaiju_scheduler-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-19 10:55 kaiju_scheduler-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      761 b- defN 24-Apr-19 10:55 kaiju_scheduler-0.1.1.dist-info/RECORD
-9 files, 20659 bytes uncompressed, 7322 bytes compressed:  64.6%
+Zip file size: 8794 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      236 b- defN 24-Apr-24 18:52 kaiju_scheduler/__init__.py
+-rw-r--r--  2.0 unx      267 b- defN 24-Apr-24 18:52 kaiju_scheduler/interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 18:52 kaiju_scheduler/py.typed
+-rw-r--r--  2.0 unx    10734 b- defN 24-Apr-24 18:52 kaiju_scheduler/scheduler.py
+-rw-r--r--  2.0 unx     2721 b- defN 24-Apr-24 18:52 kaiju_scheduler/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4680 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      839 b- defN 24-Apr-24 18:52 kaiju_scheduler-0.1.2.dist-info/RECORD
+10 files, 20654 bytes uncompressed, 7350 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: kaiju_scheduler/__init__.py
 Comment: 
 
 Filename: kaiju_scheduler/interfaces.py
 Comment: 
 
+Filename: kaiju_scheduler/py.typed
+Comment: 
+
 Filename: kaiju_scheduler/scheduler.py
 Comment: 
 
 Filename: kaiju_scheduler/utils.py
 Comment: 
 
-Filename: kaiju_scheduler-0.1.1.dist-info/LICENSE
+Filename: kaiju_scheduler-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_scheduler-0.1.1.dist-info/METADATA
+Filename: kaiju_scheduler-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_scheduler-0.1.1.dist-info/WHEEL
+Filename: kaiju_scheduler-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_scheduler-0.1.1.dist-info/top_level.txt
+Filename: kaiju_scheduler-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_scheduler-0.1.1.dist-info/RECORD
+Filename: kaiju_scheduler-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_scheduler/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 from kaiju_scheduler.scheduler import *
 from kaiju_scheduler.utils import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## kaiju_scheduler/scheduler.py

```diff
@@ -1,38 +1,26 @@
 """Scheduler classes."""
 
 import asyncio
 import traceback
 from dataclasses import dataclass, field
 from enum import Enum
 from types import MappingProxyType
-from typing import Any, Awaitable, Callable, ClassVar, Dict, List, Mapping, Optional, TypedDict, final
+from typing import Any, Awaitable, Callable, ClassVar, Dict, List, Mapping, Optional, final
 from weakref import proxy
 
 from kaiju_scheduler.interfaces import Logger
 from kaiju_scheduler.utils import retry, timeout
 
 __all__ = ["ExecPolicy", "ScheduledTask", "Scheduler"]
 
 _AsyncCallable = Callable[..., Awaitable[Any]]
 _Sentinel = ...
 
 
-class _TaskInfo(TypedDict):
-    name: str
-    enabled: bool
-    interval_s: float
-    policy: str
-    retries: int
-    retry_interval_s: float
-    max_timeout_s: float
-    started: bool
-    called_at: float
-
-
 @final
 class ExecPolicy(Enum):
     """Function execution policy for a scheduled task."""
 
     CANCEL = "CANCEL"
     """Cancel the previous call immediately if it's still going and restart strictly on interval_s."""
 
@@ -58,15 +46,15 @@
     """
 
 
 @final
 class ScheduledTask:
     """Scheduled task."""
 
-    class _TaskDisableCtx:
+    class _TaskSuspendCtx:
         __slots__ = ("__weakref__", "_task")
 
         def __init__(self, task: "ScheduledTask", /):
             self._task = proxy(task)
 
         async def __aenter__(self):
             self._task.disable()
@@ -134,36 +122,37 @@
     def disable(self) -> None:
         """Disable the task for future execution.
 
         This will not cancel the current execution if it's already running.
         """
         self._enabled = False
 
-    def suspend(self) -> _TaskDisableCtx:
+    def suspend(self) -> _TaskSuspendCtx:
         """Temporarily suspend execution of a task within a context block."""
-        return self._TaskDisableCtx(self)
+        return self._TaskSuspendCtx(self)
 
     async def wait(self) -> None:
         """Wait until the current run has finished."""
         await self._idle.wait()
 
     def json_repr(self) -> Dict[str, Any]:
+        """Get JSON compatible object state info."""
         return {
             "cls": "Task",
-            "data": _TaskInfo(
-                name=self.name,
-                policy=self._policy.value,
-                enabled=self._enabled,
-                started=not self._idle.is_set(),
-                interval_s=self.interval_s,
-                max_timeout_s=self.max_timeout_s,
-                retries=self.retries,
-                retry_interval_s=self.retry_interval_s,
-                called_at=self._called_at,
-            ),
+            "data": {
+                "name": self.name,
+                "policy": self._policy.value,
+                "enabled": self._enabled,
+                "started": not self._idle.is_set(),
+                "interval_s": self.interval_s,
+                "max_timeout_s": self.max_timeout_s,
+                "retries": self.retries,
+                "retry_interval_s": self.retry_interval_s,
+                "called_at": self._called_at,
+            },
         }
 
     def run(self) -> None:
         self._executed_task = self._scheduler.loop.create_task(self._run(), name=self.name)
 
     def _logger(self, msg: str, /):
         if self._scheduler.logger is not None:
@@ -204,15 +193,14 @@
 
 
 @dataclass
 class Scheduler:
     """Schedule and execute local asynchronous functions periodically."""
 
     ExecPolicy: ClassVar = ExecPolicy
-    """Alias to scheduled task exec policy enum."""
 
     min_refresh_rate: ClassVar[float] = 0.1
     """Minimum allowed refresh rate between cycles in seconds, limits `refresh_rate` value."""
 
     wait_task_timeout_safe_mod: ClassVar[float] = 4.0
     """Timeout modifier for WAIT tasks (to prevent them waiting forever)."""
 
@@ -291,17 +279,19 @@
             task.disable()
             executed_task = task._executed_task
             if executed_task and not executed_task.done():
                 if task._policy is not ExecPolicy.SHIELD:
                     executed_task.cancel()
                 _tasks.append(executed_task)
 
-        await asyncio.wait(_tasks)
+        if _tasks:
+            await asyncio.wait(_tasks)
 
     def json_repr(self) -> Dict[str, Any]:
+        """Get JSON compatible object state info."""
         return {
             "cls": "Scheduler",
             "data": {
                 "started": self._started,
                 "time": self.loop.time(),
                 "refresh_rate": self.refresh_rate,
                 "tasks": [task.json_repr() for task in self.tasks],
```

## Comparing `kaiju_scheduler-0.1.1.dist-info/LICENSE` & `kaiju_scheduler-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_scheduler-0.1.1.dist-info/METADATA` & `kaiju_scheduler-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-scheduler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous tasks scheduler and executor
 Home-page: https://github.com/violet-black/kaiju-scheduler
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: scheduler,asyncio,tasks
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,15 @@
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Requires-Dist: m2r2 ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
+Requires-Dist: coverage ; extra == 'test'
 
 [![pypi](https://img.shields.io/pypi/v/kaiju-scheduler.svg)](https://pypi.python.org/pypi/kaiju-scheduler/)
 [![docs](https://readthedocs.org/projects/kaiju-scheduler/badge/?version=latest&style=flat)](https://kaiju-scheduler.readthedocs.io)
 [![codecov](https://codecov.io/gh/violet-black/kaiju-scheduler/graph/badge.svg?token=FEUUMQELFX)](https://codecov.io/gh/violet-black/kaiju-scheduler)
 [![tests](https://github.com/violet-black/kaiju-scheduler/actions/workflows/tests.yaml/badge.svg)](https://github.com/violet-black/kaiju-scheduler/actions/workflows/tests.yaml)
 [![mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

## Comparing `kaiju_scheduler-0.1.1.dist-info/RECORD` & `kaiju_scheduler-0.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-kaiju_scheduler/__init__.py,sha256=9rryZg7sauoa5XDOOY3wTMGMUYPO7bD5kVNrEQFDkPs,236
+kaiju_scheduler/__init__.py,sha256=P7Uyc3MMpEBOtUT95LG2hFePkh0puLWT3GjZMkZfhZ4,236
 kaiju_scheduler/interfaces.py,sha256=b1ypQmToIoj3dT2ImOI5eMUErjxFmf-8aOLi2T__R6U,267
-kaiju_scheduler/scheduler.py,sha256=dBARuye82HE5aIAKpeEIUEsTRn7TtK158slT2GVJQiQ,10859
+kaiju_scheduler/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kaiju_scheduler/scheduler.py,sha256=Hp3RQ1Xyxmz3m4B4r8USrJgoIfOnHGW91lJoJMAYmoY,10734
 kaiju_scheduler/utils.py,sha256=p0u1AcvClFq22zkLTj19rEupkJFn0o_L3Vsl_r6ndTA,2721
-kaiju_scheduler-0.1.1.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-kaiju_scheduler-0.1.1.dist-info/METADATA,sha256=3kYUyqYn4JFLfjxGUHtKwaAkPvFVv69ZvZwoSlA3zj0,4638
-kaiju_scheduler-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kaiju_scheduler-0.1.1.dist-info/top_level.txt,sha256=dAaiI_8l8YBLxltHPsGLRPu62cY-4wr3m0seucrUXZY,16
-kaiju_scheduler-0.1.1.dist-info/RECORD,,
+kaiju_scheduler-0.1.2.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+kaiju_scheduler-0.1.2.dist-info/METADATA,sha256=Z0N50t9oKAsVdTD9eZe0GoIxT3LMy4wvRqdpWY7Lu-8,4680
+kaiju_scheduler-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kaiju_scheduler-0.1.2.dist-info/top_level.txt,sha256=dAaiI_8l8YBLxltHPsGLRPu62cY-4wr3m0seucrUXZY,16
+kaiju_scheduler-0.1.2.dist-info/RECORD,,
```

