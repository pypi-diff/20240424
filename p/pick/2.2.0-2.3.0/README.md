# Comparing `tmp/pick-2.2.0.tar.gz` & `tmp/pick-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pick-2.2.0.tar", max compression
+gzip compressed data, was "pick-2.3.0.tar", max compression
```

## Comparing `pick-2.2.0.tar` & `pick-2.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1080 2021-12-06 03:34:40.191887 pick-2.2.0/LICENSE
--rw-r--r--   0        0        0     2288 2022-11-21 06:21:43.491351 pick-2.2.0/README.md
--rw-r--r--   0        0        0      594 2022-11-21 06:26:10.875528 pick-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6275 2022-11-21 06:21:43.491678 pick-2.2.0/src/pick/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 06:20:56.446530 pick-2.2.0/src/pick/py.typed
--rw-r--r--   0        0        0     3083 2022-11-21 06:27:26.481934 pick-2.2.0/setup.py
--rw-r--r--   0        0        0     3012 2022-11-21 06:27:26.482107 pick-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-19 12:28:44.312843 pick-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2463 2024-04-22 10:46:10.505924 pick-2.3.0/README.md
+-rw-r--r--   0        0        0      622 2024-04-22 10:46:10.506294 pick-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7795 2024-04-22 10:45:57.237655 pick-2.3.0/src/pick/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:28:44.315867 pick-2.3.0/src/pick/py.typed
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 pick-2.3.0/PKG-INFO
```

### Comparing `pick-2.2.0/LICENSE` & `pick-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pick-2.2.0/README.md` & `pick-2.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pick
 
-[![image](https://github.com/wong2/pick/actions/workflows/ci.yml/badge.svg)](https://github.com/wong2/pick/actions/workflows/ci.yml)
+[![image](https://github.com/aisk/pick/actions/workflows/ci.yml/badge.svg)](https://github.com/aisk/pick/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/pick.svg)](https://pypi.python.org/pypi/pick)
 [![PyPI](https://img.shields.io/pypi/dm/pick)](https://pypi.python.org/pypi/pick)
 
 **pick** is a small python library to help you create curses based
 interactive selection list in the terminal.
 
 |         Basic          |         Multiselect          |
@@ -53,11 +53,12 @@
 - `default_index`: (optional) set this if the default selected option
   is not the first one
 - `multiselect`: (optional), if set to True its possible to select
   multiple items by hitting SPACE
 - `min_selection_count`: (optional) for multi select feature to
   dictate a minimum of selected items before continuing
 - `screen`: (optional), if you are using `pick` within an existing curses application set this to your existing `screen` object.  It is assumed this has initialised in the standard way (e.g. via `curses.wrapper()`, or `curses.noecho(); curses.cbreak(); screen.kepad(True)`)
+- `position`: (optional), if you are using `pick` within an existing curses application use this to set the first position to write to. e.g., `position=pick.Position(y=1, x=1)`
 
 ## Community Projects
 
 [pickpack](https://github.com/anafvana/pickpack): A fork of `pick` to select tree data.
```

### Comparing `pick-2.2.0/pyproject.toml` & `pick-2.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pick"
-version = "2.2.0"
+version = "2.3.0"
 description = "Pick an option in the terminal with a simple GUI"
-authors = ["wong2 <wonderfuly@gmail.com>"]
+authors = ["wong2 <wonderfuly@gmail.com>", "AN Long <aisk1988@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/wong2/pick"
-homepage = "https://github.com/wong2/pick"
+repository = "https://github.com/aisk/pick"
+homepage = "https://github.com/aisk/pick"
 keywords = ["terminal", "gui"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 windows-curses = {version = "^2.2.0", platform = "win32"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
-mypy = "^0.990"
+pytest = "^7.2.0"
+mypy = "^1.4"
 pre-commit = "^2.20.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pick-2.2.0/src/pick/__init__.py` & `pick-2.3.0/src/pick/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 import curses
+from collections import namedtuple
 from dataclasses import dataclass, field
-from typing import Any, List, Optional, Sequence, Tuple, TypeVar, Union, Generic
+from typing import Any, Generic, List, Optional, Sequence, Tuple, TypeVar, Union
 
 __all__ = ["Picker", "pick", "Option"]
 
 
 @dataclass
 class Option:
     label: str
-    value: Any
+    value: Any = None
+    description: Optional[str] = None
 
 
 KEYS_ENTER = (curses.KEY_ENTER, ord("\n"), ord("\r"))
 KEYS_UP = (curses.KEY_UP, ord("k"))
 KEYS_DOWN = (curses.KEY_DOWN, ord("j"))
 KEYS_SELECT = (curses.KEY_RIGHT, ord(" "))
 
 SYMBOL_CIRCLE_FILLED = "(x)"
 SYMBOL_CIRCLE_EMPTY = "( )"
 
 OPTION_T = TypeVar("OPTION_T", str, Option)
 PICK_RETURN_T = Tuple[OPTION_T, int]
 
+Position = namedtuple('Position', ['y', 'x'])
 
 @dataclass
 class Picker(Generic[OPTION_T]):
     options: Sequence[OPTION_T]
     title: Optional[str] = None
     indicator: str = "*"
     default_index: int = 0
     multiselect: bool = False
     min_selection_count: int = 0
     selected_indexes: List[int] = field(init=False, default_factory=list)
     index: int = field(init=False, default=0)
     screen: Optional["curses._CursesWindow"] = None
+    position: Position = Position(0, 0)
 
     def __post_init__(self) -> None:
         if len(self.options) == 0:
             raise ValueError("options should not be an empty list")
 
         if self.default_index >= len(self.options):
             raise ValueError("default_index should be less than the length of options")
@@ -100,46 +104,80 @@
                 prefix = f"{prefix} {symbol}"
 
             option_as_str = option.label if isinstance(option, Option) else option
             lines.append(f"{prefix} {option_as_str}")
 
         return lines
 
-    def get_lines(self) -> Tuple[List, int]:
+    def get_lines(self) -> Tuple[List[str], int]:
         title_lines = self.get_title_lines()
         option_lines = self.get_option_lines()
         lines = title_lines + option_lines
         current_line = self.index + len(title_lines) + 1
         return lines, current_line
 
+    def get_description_lines(self, description: str, length: int) -> List[str]:
+        description_words = description.split(" ")
+        description_lines: List[str] = []
+
+        line = ""
+        for i, word in enumerate(description_words):
+            if len(line + " " + word) <= length:
+                if i == 0:
+                    line += word
+                else:
+                    line += " " + word
+            else:
+                description_lines.append(line)
+                line = word
+
+        description_lines.append(line)
+
+        return description_lines
+
     def draw(self, screen: "curses._CursesWindow") -> None:
         """draw the curses ui on the screen, handle scroll if needed"""
-        screen.clear()
+        y, x = self.position  # start point
 
-        x, y = 1, 1  # start point
         max_y, max_x = screen.getmaxyx()
         max_rows = max_y - y  # the max rows we can draw
 
         lines, current_line = self.get_lines()
 
         # calculate how many lines we should scroll, relative to the top
         scroll_top = 0
         if current_line > max_rows:
             scroll_top = current_line - max_rows
 
         lines_to_draw = lines[scroll_top : scroll_top + max_rows]
 
+        description_present = False
+        for option in self.options:
+            if isinstance(option, str) or option.description is not None:
+                description_present = True
+                break
+
         for line in lines_to_draw:
-            screen.addnstr(y, x, line, max_x - 2)
+            if description_present:
+                screen.addnstr(y, x, line, max_x // 2 - 2)
+            else:
+                screen.addnstr(y, x, line, max_x - 2)
             y += 1
 
+        option = self.options[self.index]
+        if isinstance(option, Option) and option.description is not None:
+            description_lines = self.get_description_lines(option.description, max_x // 2)
+
+            for i, line in enumerate(description_lines):
+                screen.addnstr(i + 3, max_x // 2, line, 2 * max_x // 2 - 2)
+
         screen.refresh()
 
     def run_loop(
-        self, screen: "curses._CursesWindow"
+        self, screen: "curses._CursesWindow", position: Position
     ) -> Union[List[PICK_RETURN_T], PICK_RETURN_T]:
         while True:
             self.draw(screen)
             c = screen.getch()
             if c in KEYS_UP:
                 self.move_up()
             elif c in KEYS_DOWN:
@@ -162,40 +200,42 @@
             curses.curs_set(0)
         except:
             # Curses failed to initialize color support, eg. when TERM=vt100
             curses.initscr()
 
     def _start(self, screen: "curses._CursesWindow"):
         self.config_curses()
-        return self.run_loop(screen)
+        return self.run_loop(screen, self.position)
 
     def start(self):
         if self.screen:
             # Given an existing screen
             # don't make any lasting changes
             last_cur = curses.curs_set(0)
-            ret = self.run_loop(self.screen)
+            ret = self.run_loop(self.screen, self.position)
             if last_cur:
                 curses.curs_set(last_cur)
             return ret
         return curses.wrapper(self._start)
 
 
 def pick(
     options: Sequence[OPTION_T],
     title: Optional[str] = None,
     indicator: str = "*",
     default_index: int = 0,
     multiselect: bool = False,
     min_selection_count: int = 0,
     screen: Optional["curses._CursesWindow"] = None,
+    position: Position = Position(0, 0)
 ):
     picker: Picker = Picker(
         options,
         title,
         indicator,
         default_index,
         multiselect,
         min_selection_count,
         screen,
+        position,
     )
     return picker.start()
```

### Comparing `pick-2.2.0/setup.py` & `pick-2.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pick
+Version: 2.3.0
+Summary: Pick an option in the terminal with a simple GUI
+Home-page: https://github.com/aisk/pick
+License: MIT
+Keywords: terminal,gui
+Author: wong2
+Author-email: wonderfuly@gmail.com
+Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: windows-curses (>=2.2.0,<3.0.0) ; sys_platform == "win32"
+Project-URL: Repository, https://github.com/aisk/pick
+Description-Content-Type: text/markdown
+
+# pick
+
+[![image](https://github.com/aisk/pick/actions/workflows/ci.yml/badge.svg)](https://github.com/aisk/pick/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/pick.svg)](https://pypi.python.org/pypi/pick)
+[![PyPI](https://img.shields.io/pypi/dm/pick)](https://pypi.python.org/pypi/pick)
+
+**pick** is a small python library to help you create curses based
+interactive selection list in the terminal.
+
+|         Basic          |         Multiselect          |
+| :--------------------: | :--------------------------: |
+| ![](example/basic.gif) | ![](example/multiselect.gif) |
+
+## Installation
+
+    $ pip install pick
+
+## Usage
+
+**pick** comes with a simple api:
+
+    >>> from pick import pick
+
+    >>> title = 'Please choose your favorite programming language: '
+    >>> options = ['Java', 'JavaScript', 'Python', 'PHP', 'C++', 'Erlang', 'Haskell']
+    >>> option, index = pick(options, title)
+    >>> print(option)
+    >>> print(index)
+
+**outputs**:
+
+    >>> C++
+    >>> 4
+
+**pick** multiselect example:
+
+    >>> from pick import pick
+
+    >>> title = 'Please choose your favorite programming language (press SPACE to mark, ENTER to continue): '
+    >>> options = ['Java', 'JavaScript', 'Python', 'PHP', 'C++', 'Erlang', 'Haskell']
+    >>> selected = pick(options, title, multiselect=True, min_selection_count=1)
+    >>> print(selected)
+
+**outputs**:
+
+    >>> [('Java', 0), ('C++', 4)]
+
+## Options
+
+- `options`: a list of options to choose from
+- `title`: (optional) a title above options list
+- `indicator`: (optional) custom the selection indicator, defaults to `*`
+- `default_index`: (optional) set this if the default selected option
+  is not the first one
+- `multiselect`: (optional), if set to True its possible to select
+  multiple items by hitting SPACE
+- `min_selection_count`: (optional) for multi select feature to
+  dictate a minimum of selected items before continuing
+- `screen`: (optional), if you are using `pick` within an existing curses application set this to your existing `screen` object.  It is assumed this has initialised in the standard way (e.g. via `curses.wrapper()`, or `curses.noecho(); curses.cbreak(); screen.kepad(True)`)
+- `position`: (optional), if you are using `pick` within an existing curses application use this to set the first position to write to. e.g., `position=pick.Position(y=1, x=1)`
 
-package_dir = \
-{'': 'src'}
+## Community Projects
 
-packages = \
-['pick']
+[pickpack](https://github.com/anafvana/pickpack): A fork of `pick` to select tree data.
 
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':sys_platform == "win32"': ['windows-curses>=2.2.0,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'pick',
-    'version': '2.2.0',
-    'description': 'Pick an option in the terminal with a simple GUI',
-    'long_description': "# pick\n\n[![image](https://github.com/wong2/pick/actions/workflows/ci.yml/badge.svg)](https://github.com/wong2/pick/actions/workflows/ci.yml)\n[![PyPI](https://img.shields.io/pypi/v/pick.svg)](https://pypi.python.org/pypi/pick)\n[![PyPI](https://img.shields.io/pypi/dm/pick)](https://pypi.python.org/pypi/pick)\n\n**pick** is a small python library to help you create curses based\ninteractive selection list in the terminal.\n\n|         Basic          |         Multiselect          |\n| :--------------------: | :--------------------------: |\n| ![](example/basic.gif) | ![](example/multiselect.gif) |\n\n## Installation\n\n    $ pip install pick\n\n## Usage\n\n**pick** comes with a simple api:\n\n    >>> from pick import pick\n\n    >>> title = 'Please choose your favorite programming language: '\n    >>> options = ['Java', 'JavaScript', 'Python', 'PHP', 'C++', 'Erlang', 'Haskell']\n    >>> option, index = pick(options, title)\n    >>> print(option)\n    >>> print(index)\n\n**outputs**:\n\n    >>> C++\n    >>> 4\n\n**pick** multiselect example:\n\n    >>> from pick import pick\n\n    >>> title = 'Please choose your favorite programming language (press SPACE to mark, ENTER to continue): '\n    >>> options = ['Java', 'JavaScript', 'Python', 'PHP', 'C++', 'Erlang', 'Haskell']\n    >>> selected = pick(options, title, multiselect=True, min_selection_count=1)\n    >>> print(selected)\n\n**outputs**:\n\n    >>> [('Java', 0), ('C++', 4)]\n\n## Options\n\n- `options`: a list of options to choose from\n- `title`: (optional) a title above options list\n- `indicator`: (optional) custom the selection indicator, defaults to `*`\n- `default_index`: (optional) set this if the default selected option\n  is not the first one\n- `multiselect`: (optional), if set to True its possible to select\n  multiple items by hitting SPACE\n- `min_selection_count`: (optional) for multi select feature to\n  dictate a minimum of selected items before continuing\n- `screen`: (optional), if you are using `pick` within an existing curses application set this to your existing `screen` object.  It is assumed this has initialised in the standard way (e.g. via `curses.wrapper()`, or `curses.noecho(); curses.cbreak(); screen.kepad(True)`)\n\n## Community Projects\n\n[pickpack](https://github.com/anafvana/pickpack): A fork of `pick` to select tree data.\n",
-    'author': 'wong2',
-    'author_email': 'wonderfuly@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wong2/pick',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7',
-}
-
-
-setup(**setup_kwargs)
```

