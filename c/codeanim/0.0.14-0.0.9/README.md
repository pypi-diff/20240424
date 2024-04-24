# Comparing `tmp/codeanim-0.0.14.tar.gz` & `tmp/codeanim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeanim-0.0.14.tar", max compression
+gzip compressed data, was "codeanim-0.0.9.tar", max compression
```

## Comparing `codeanim-0.0.14.tar` & `codeanim-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-04-24 00:50:20.117986 codeanim-0.0.14/LICENSE
--rw-r--r--   0        0        0     2263 2024-04-24 00:50:20.117986 codeanim-0.0.14/README.md
--rw-r--r--   0        0        0      408 2024-04-24 00:50:20.121986 codeanim-0.0.14/pyproject.toml
--rwxr-xr-x   0        0        0     2055 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/__init__.py
--rw-r--r--   0        0        0     1719 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/chrome.py
--rw-r--r--   0        0        0     2264 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/core.py
--rw-r--r--   0        0        0     1152 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/delayer.py
--rw-r--r--   0        0        0     1759 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/interpolators.py
--rw-r--r--   0        0        0     1770 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/keyboard.py
--rw-r--r--   0        0        0     1338 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/markdown.py
--rw-r--r--   0        0        0      737 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/mouse.py
--rw-r--r--   0        0        0     1058 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/shell.py
--rw-r--r--   0        0        0     3018 2024-04-24 00:50:20.121986 codeanim-0.0.14/src/codeanim/vscode.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 codeanim-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-02-03 20:12:45.447570 codeanim-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3222 2024-03-03 05:35:42.985531 codeanim-0.0.9/README.md
+-rw-r--r--   0        0        0      407 2024-03-03 22:14:09.461599 codeanim-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1917 2024-03-03 21:47:24.662461 codeanim-0.0.9/src/codeanim/__init__.py
+-rw-r--r--   0        0        0     1745 2024-03-03 21:47:24.662778 codeanim-0.0.9/src/codeanim/chrome.py
+-rw-r--r--   0        0        0     1933 2024-03-03 21:47:24.662996 codeanim-0.0.9/src/codeanim/core.py
+-rw-r--r--   0        0        0     1152 2024-03-03 21:47:24.663275 codeanim-0.0.9/src/codeanim/delayer.py
+-rw-r--r--   0        0        0     1776 2024-03-03 21:48:41.342963 codeanim-0.0.9/src/codeanim/keyboard.py
+-rw-r--r--   0        0        0     1338 2024-03-03 01:51:34.373628 codeanim-0.0.9/src/codeanim/markdown.py
+-rw-r--r--   0        0        0     1058 2024-03-03 21:47:24.663704 codeanim-0.0.9/src/codeanim/shell.py
+-rw-r--r--   0        0        0     3047 2024-03-03 21:47:24.663985 codeanim-0.0.9/src/codeanim/vscode.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 codeanim-0.0.9/PKG-INFO
```

### Comparing `codeanim-0.0.14/LICENSE` & `codeanim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.14/src/codeanim/__init__.py` & `codeanim-0.0.9/src/codeanim/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #!/usr/bin/env python3
 import argparse
 import os
 
-from pynput.keyboard import Key  # noqa: F401
-from pynput.mouse import Button  # noqa: F401
-
-from . import chrome, core, interpolators, markdown, vscode  # noqa: F401
+from . import chrome, core, markdown, vscode  # noqa: F401
 from .core import codeanim
-from .mouse import click, move  # noqa: F401
 
 # Public API
+Key = core.Key
 backspace = codeanim.backspace
 delay = codeanim.delay
 pause = codeanim.delay.pause
 paste = codeanim.paste
 tap = codeanim.tap
 wait = codeanim.wait
 write = codeanim.write
```

### Comparing `codeanim-0.0.14/src/codeanim/chrome.py` & `codeanim-0.0.9/src/codeanim/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 def resize(ca: CodeAnim, position: tuple[int, int], size: tuple[int, int]):
     ca.shell.resize(APP_NAME, position, size)
 
 
 @CodeAnim.cmd
 def navigate(ca: CodeAnim, url: str):
     ca.tap("l", modifiers=[Key.cmd])
-    ca.write(url)
+    with ca.delay(0):
+        ca.write(url)
     ca.tap(Key.enter)
 
 
 @CodeAnim.cmd
 def back(ca: CodeAnim):
     ca.tap(Key.left, modifiers=[Key.cmd])
```

### Comparing `codeanim-0.0.14/src/codeanim/core.py` & `codeanim-0.0.9/src/codeanim/keyboard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,66 @@
 import time
-from typing import Callable, Concatenate, ParamSpec, TypeVar
+from threading import Event
 
-import pyperclip
-from pynput.keyboard import Key
-from pynput.mouse import Controller
+from pynput.keyboard import Controller, Key, KeyCode, Listener
 
-from . import shell
-from .delayer import Delayer
-from .keyboard import Keyboard
 
-R = TypeVar("R")
-P = ParamSpec("P")
-
-
-class CodeAnim:
+class Keyboard:
     def __init__(self):
-        self.delay = Delayer()
-        self.keyboard = Keyboard()
-        self.mouse = Controller()
-        self.backspace = backspace
-
-        self.paste = paste
-        self.shell = shell
-        self.tap = tap
-        self.write = write
-
-        self._call_stack = []
+        self.keyboard = Controller()
+        self.press = Event()
+        self.released: Key | KeyCode | None = None
+        self.listener: Listener | None = None
+
+    def handle_press(self, key: Key | KeyCode | None):
+        pass
+
+    def handle_release(self, key: Key | KeyCode | None):
+        self.released = key
+        self.press.set()
 
     def __enter__(self):
         self.start()
         return self
 
     def start(self):
-        self.keyboard.start()
+        self.listener = Listener(
+            on_press=self.handle_press,
+            on_release=self.handle_release,
+        )
+        self.listener.start()
+        return self
 
     def __exit__(self, *args):
         self.stop()
 
     def stop(self):
-        self.keyboard.stop()
-
-    @staticmethod
-    def cmd(func: Callable[Concatenate["CodeAnim", P], R]) -> Callable[P, R]:
-        def codeanim_func(
-            *args: P.args,
-            **kwargs: P.kwargs,
-        ) -> R:
-            codeanim._call_stack.append(func.__name__)
-            result = func(codeanim, *args, **kwargs)
-            codeanim._call_stack.pop()
-            if len(codeanim._call_stack) == 0:
-                codeanim.delay.pause()
-            return result
-
-        return codeanim_func
+        if self.listener is not None:
+            self.listener.stop()
+            self.listener.join()
+            self.listener = None
+
+    def tap(
+        self,
+        key: str | Key,
+        *,
+        modifiers: list[str | Key] = [],
+        repeat: int = 1,
+        delay: float = 0,
+    ):
+        for modifier in modifiers:
+            self.keyboard.press(modifier)
+        for _ in range(repeat):
+            self.keyboard.tap(key)
+            time.sleep(delay)
+        for modifier in modifiers:
+            self.keyboard.release(modifier)
 
     def wait(self, key: Key = Key.shift):
-        self.keyboard.wait(key)
-
-
-@CodeAnim.cmd
-def paste(ca: CodeAnim, text: str, *, paste_delay: float = 0.5):
-    pyperclip.copy(text)
-    ca.tap("v", modifiers=[Key.cmd])
-    time.sleep(paste_delay)  # Need to wait for the paste to finish
-
-
-@CodeAnim.cmd
-def tap(ca: CodeAnim, key: str | Key, *, modifiers: list[Key] = [], repeat: int = 1):
-    ca.keyboard.tap(
-        key,
-        modifiers=modifiers,
-        repeat=repeat,
-        delay=ca.delay.keys.get(key, ca.delay.tap),
-    )
-
-
-@CodeAnim.cmd
-def write(ca: CodeAnim, text: str):
-    for char in text:
-        if char == "\n":
-            ca.tap(Key.enter)
-        elif char == "\t":
-            ca.tap(Key.tab)
-        elif len(char.encode("utf-8")) != 1:
-            ca.paste(char)
-        else:
-            ca.tap(char)
-
-
-@CodeAnim.cmd
-def backspace(ca: CodeAnim, num: int = 1):
-    for _ in range(num):
-        ca.tap(Key.backspace)
-
-
-codeanim = CodeAnim()
+        if self.listener is None or not self.listener.is_alive():
+            raise RuntimeError("KeyMonitor is not running.")
+        time.sleep(0.01)  # Flush previous tap events
+        self.released = None
+        print(f"Tap {key.name} to continue")
+        while key != self.released:
+            self.press.wait()
+            self.press.clear()
```

### Comparing `codeanim-0.0.14/src/codeanim/delayer.py` & `codeanim-0.0.9/src/codeanim/delayer.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.14/src/codeanim/keyboard.py` & `codeanim-0.0.9/src/codeanim/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,78 @@
 import time
-from threading import Event
+from typing import Callable, Concatenate, ParamSpec, TypeVar
 
-from pynput.keyboard import Controller, Key, KeyCode, Listener
+import pyperclip
+from pynput.keyboard import Key
 
+from . import shell
+from .delayer import Delayer
+from .keyboard import Keyboard
 
-class Keyboard:
+R = TypeVar("R")
+P = ParamSpec("P")
+
+
+class CodeAnim:
     def __init__(self):
-        self.keyboard = Controller()
-        self.press = Event()
-        self.released: Key | KeyCode | None = None
-        self.listener: Listener | None = None
-
-    def handle_press(self, key: Key | KeyCode | None):
-        pass
-
-    def handle_release(self, key: Key | KeyCode | None):
-        self.released = key
-        self.press.set()
+        self.delay = Delayer()
+        self.keyboard = Keyboard()
+        self.shell = shell
 
     def __enter__(self):
         self.start()
         return self
 
     def start(self):
-        self.listener = Listener(
-            on_press=self.handle_press,
-            on_release=self.handle_release,
-        )
-        self.listener.start()
-        return self
+        self.keyboard.start()
 
     def __exit__(self, *args):
         self.stop()
 
     def stop(self):
-        if self.listener is not None:
-            self.listener.stop()
-            self.listener.join()
-            self.listener = None
-
-    def tap(
-        self,
-        key: str | Key,
-        *,
-        modifiers: list[Key] = [],
-        repeat: int = 1,
-        delay: float = 0,
-    ):
-        for modifier in modifiers:
-            self.keyboard.press(modifier)
-        for _ in range(repeat):
-            self.keyboard.tap(key)
-            time.sleep(delay)
-        for modifier in modifiers:
-            self.keyboard.release(modifier)
+        self.keyboard.stop()
+
+    @staticmethod
+    def cmd(func: Callable[Concatenate["CodeAnim", P], R]) -> Callable[P, R]:
+        def codeanim_func(
+            *args: P.args,
+            **kwargs: P.kwargs,
+        ) -> R:
+            result = func(codeanim, *args, **kwargs)
+            codeanim.delay.pause()
+            return result
+
+        return codeanim_func
+
+    def tap(self, key: str | Key, *, modifiers: list[str | Key] = [], repeat: int = 1):
+        self.keyboard.tap(
+            key,
+            modifiers=modifiers,
+            repeat=repeat,
+            delay=self.delay.keys.get(key, self.delay.tap),
+        )
 
     def wait(self, key: Key = Key.shift):
-        if self.listener is None or not self.listener.is_alive():
-            raise RuntimeError("KeyMonitor is not running.")
-        time.sleep(0.01)  # Flush previous tap events
-        self.released = None
-        print(f"Tap {key.name} to continue")
-        while key != self.released:
-            self.press.wait()
-            self.press.clear()
+        self.keyboard.wait(key)
+
+    def paste(self, text: str, *, paste_delay: float = 0.5):
+        pyperclip.copy(text)
+        self.tap("v", modifiers=[Key.cmd])
+        time.sleep(paste_delay)  # Need to wait for the paste to finish
+
+    def write(self, text: str):
+        for char in text:
+            if char == "\n":
+                self.tap(Key.enter)
+            elif char == "\t":
+                self.tap(Key.tab)
+            elif len(char.encode("utf-8")) != 1:
+                self.paste(char)
+            else:
+                self.tap(char)
+
+    def backspace(self, num: int = 1):
+        for _ in range(num):
+            self.tap(Key.backspace)
+
+
+codeanim = CodeAnim()
```

### Comparing `codeanim-0.0.14/src/codeanim/markdown.py` & `codeanim-0.0.9/src/codeanim/markdown.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.14/src/codeanim/shell.py` & `codeanim-0.0.9/src/codeanim/shell.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.14/src/codeanim/vscode.py` & `codeanim-0.0.9/src/codeanim/vscode.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     ca.write(cmd)
     ca.tap(Key.enter)
 
 
 @CodeAnim.cmd
 def newline(ca: CodeAnim, line: int = 0, *, above: bool = False):
     if line > 0:
-        jump(line)
+        with ca.delay(0):
+            jump(line)
         ca.tap(Key.enter, modifiers=[Key.cmd, Key.shift])
     else:
         ca.tap(Key.enter, modifiers=[Key.cmd, Key.shift] if above else [Key.cmd])
 
 
 @CodeAnim.cmd
 def jump(ca: CodeAnim, line: int, col: int = 1):
@@ -69,15 +70,15 @@
 
 @CodeAnim.cmd
 def bottom(ca: CodeAnim, *, select: bool = False):
     ca.tap(Key.down, modifiers=[Key.cmd, Key.shift] if select else [Key.cmd])
 
 
 @CodeAnim.cmd
-def new_file(ca: CodeAnim):
+def newfile(ca: CodeAnim):
     ca.tap("n", modifiers=[Key.cmd])
 
 
 @CodeAnim.cmd
 def save(ca: CodeAnim, file: str | None = None):
     if file is None:
         ca.tap("s", modifiers=[Key.cmd])
```

### Comparing `codeanim-0.0.14/PKG-INFO` & `codeanim-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeanim
-Version: 0.0.14
+Version: 0.0.9
 Summary: A tool that automates presentation of software demos.
 Author: Shad Sharma
 Author-email: shadanan@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
@@ -13,27 +13,47 @@
 
 # CodeAnim
 
 CodeAnim is a tool to help you animate VS Code. It provides methods that enable you to type, move the cursor, and send commands to VS Code. It works by sending keystrokes using the pynput library.
 
 ## Installation
 
-We recommend install CodeAnim using [pipx](https://pipx.pypa.io/).
+Create a venv and then pip install CodeAnim from the GitHub repo:
 
 ```shell
-pipx install codeanim
+python3 -m venv .venv
+. .venv/bin/activate
+pip install git+https://github.com/shadanan/codeanim
+```
+
+The run command uses a custom keybinding. Please add this to your `keybindings.json` file in VS Code:
+
+```json
+[
+  {
+    "key": "ctrl+shift+alt+cmd+enter",
+    "command": "python.execInTerminal"
+  }
+]
 ```
 
 ## Usage
 
-CodeAnim runs commands from Markdown files where codeanim commands are enclosed in a `python codeanim` fence.
+There are two ways to use CodeAnim:
+
+- As commands in a Markdown file
+- Imported as a library and executed in a Python script
+
+### Usage of CodeAnim CLI
 
-### Example
+Create a Markdown file and enclose codeanim commands in a `python codeanim` fence.
 
-Create a Markdown file called `codeanim-markdown-demo.md` with the following contents:
+#### Example
+
+Add this to `codeanim-markdown-demo.md`:
 
 ````markdown
 # A Markdown Header
 
 Some text to be read.
 
 ```python codeanim
@@ -53,27 +73,59 @@
 
 To execute the CodeAnim commands in the Markdown file:
 
 ```shell
 codeanim codeanim-markdown-demo.md
 ```
 
-### Flags
+#### Flags
 
 - Set `-v` or `--verbose` to enable verbose mode. Commands will be printed out as they are executed.
 - Set `--live` to enable presentation mode. In this mode, a wait() will be injected after every codeanim fence.
 
+### Usage of CodeAnim Library
+
+Import CodeAnim, and call the functions.
+
+#### Example
+
+Add this to `codeanim_script_demo.py`:
+
+```python
+#!/usr/bin/env python3
+from codeanim import *
+
+# Bring VS Code to the front
+vscode.activate()
+
+# Open myfile.py
+vscode.focus("myfile.py")
+
+# Insert print("Hello, World!") into myfile.py
+write('print("Hello, World!")\n')
+
+# Execute the script
+vscode.run()
+```
+
+Execute your Python script:
+
+```sh
+./codeanim_script_demo.py
+```
+
 ## Development
 
-We use Poetry for development.
+Clone the repo, create a venv, and install dependencies:
 
 ```shell
 git clone https://github.com/shadanan/codeanim.git
 cd codeanim
-poetry install
+python3 -m venv .venv
+pip install .
 ```
 
 ### Formatting
 
 This project adopts the Ruff formatter and is enforced by a GitHub action.
 
 ### VS Code
@@ -84,22 +136,28 @@
 - [Ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 
 ## Tests
 
 There aren't any unit tests yet. In the tests folder, there is an end-to-end test that uses CodeAnim to open the `scratch.py` file, types out some code, and executes it. To run the test:
 
 ```sh
-./e2e-test.sh
+PYTHONPATH=src codeanim tests/e2e.md -v
 ```
 
 Then, validate that it worked by observing that the animation runs, types out:
 
 ```python
 print("Hello, World!")
 ```
 
 And executes the script.
 
+### VS Code Tests
+
+```sh
+PYTHONPATH=src tests/vscode.py
+```
+
 ## Limitations
 
 CodeAnim currently only works on MacOS because of a dependency on AppleScript, which is used to switch to the VS Code window. Also, many of the commands send Mac specific keystrokes. With some effort, CodeAnim can be made to work on other platforms.
```

