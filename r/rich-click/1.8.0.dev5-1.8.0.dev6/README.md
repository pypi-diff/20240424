# Comparing `tmp/rich_click-1.8.0.dev5.tar.gz` & `tmp/rich_click-1.8.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_click-1.8.0.dev5.tar", last modified: Sat Apr 13 22:29:55 2024, max compression
+gzip compressed data, was "rich_click-1.8.0.dev6.tar", last modified: Sun Apr 14 16:03:03 2024, max compression
```

## Comparing `rich_click-1.8.0.dev5.tar` & `rich_click-1.8.0.dev6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.410796 rich_click-1.8.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.414796 rich_click-1.8.0.dev5/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29574 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.844164 rich_click-1.8.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.848163 rich_click-1.8.0.dev6/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31100 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.848163 rich_click-1.8.0.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_rich_click_cli.py
```

### Comparing `rich_click-1.8.0.dev5/LICENSE` & `rich_click-1.8.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/PKG-INFO` & `rich_click-1.8.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev5
+Version: 1.8.0.dev6
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich_click-1.8.0.dev5/README.md` & `rich_click-1.8.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/pyproject.toml` & `rich_click-1.8.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/__init__.py` & `rich_click-1.8.0.dev6/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev5"
+__version__ = "1.8.0dev6"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click/_compat_click.py` & `rich_click-1.8.0.dev6/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/cli.py` & `rich_click-1.8.0.dev6/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/decorators.py` & `rich_click-1.8.0.dev6/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/patch.py` & `rich_click-1.8.0.dev6/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_click.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_click.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from rich_click.rich_help_configuration import force_terminal_default, terminal_width_default
 from rich_click.utils import CommandGroupDict, OptionGroupDict
 
 
 if TYPE_CHECKING:
     import rich.align
+    import rich.box
     import rich.padding
     import rich.style
 
 
 # Default styles
 STYLE_OPTION: "rich.style.StyleType" = "bold cyan"
 STYLE_ARGUMENT: "rich.style.StyleType" = "bold cyan"
@@ -30,33 +31,36 @@
 STYLE_HELPTEXT: "rich.style.StyleType" = "dim"
 STYLE_OPTION_HELP: "rich.style.StyleType" = ""
 STYLE_OPTION_DEFAULT: "rich.style.StyleType" = "dim"
 STYLE_OPTION_ENVVAR: "rich.style.StyleType" = "dim yellow"
 STYLE_REQUIRED_SHORT: "rich.style.StyleType" = "red"
 STYLE_REQUIRED_LONG: "rich.style.StyleType" = "dim red"
 STYLE_OPTIONS_PANEL_BORDER: "rich.style.StyleType" = "dim"
+STYLE_OPTIONS_PANEL_BOX: Optional[Union[str, "rich.box.Box"]] = "ROUNDED"
 ALIGN_OPTIONS_PANEL: "rich.align.AlignMethod" = "left"
 STYLE_OPTIONS_TABLE_SHOW_LINES: bool = False
 STYLE_OPTIONS_TABLE_LEADING: int = 0
 STYLE_OPTIONS_TABLE_PAD_EDGE: bool = False
 STYLE_OPTIONS_TABLE_PADDING: "rich.padding.PaddingDimensions" = (0, 1)
-STYLE_OPTIONS_TABLE_BOX: "rich.style.StyleType" = ""
+STYLE_OPTIONS_TABLE_BOX: Optional[Union[str, "rich.box.Box"]] = ""
 STYLE_OPTIONS_TABLE_ROW_STYLES: Optional[List["rich.style.StyleType"]] = None
 STYLE_OPTIONS_TABLE_BORDER_STYLE: Optional["rich.style.StyleType"] = None
 STYLE_COMMANDS_PANEL_BORDER: "rich.style.StyleType" = "dim"
+STYLE_COMMANDS_PANEL_BOX: Optional[Union[str, "rich.box.Box"]] = "ROUNDED"
 ALIGN_COMMANDS_PANEL: "rich.align.AlignMethod" = "left"
 STYLE_COMMANDS_TABLE_SHOW_LINES: bool = False
 STYLE_COMMANDS_TABLE_LEADING: int = 0
 STYLE_COMMANDS_TABLE_PAD_EDGE: bool = False
 STYLE_COMMANDS_TABLE_PADDING: "rich.padding.PaddingDimensions" = (0, 1)
-STYLE_COMMANDS_TABLE_BOX: "rich.style.StyleType" = ""
+STYLE_COMMANDS_TABLE_BOX: Optional[Union[str, "rich.box.Box"]] = ""
 STYLE_COMMANDS_TABLE_ROW_STYLES: Optional[List["rich.style.StyleType"]] = None
 STYLE_COMMANDS_TABLE_BORDER_STYLE: Optional["rich.style.StyleType"] = None
 STYLE_COMMANDS_TABLE_COLUMN_WIDTH_RATIO: Optional[Union[Tuple[None, None], Tuple[int, int]]] = (None, None)
 STYLE_ERRORS_PANEL_BORDER: "rich.style.StyleType" = "red"
+STYLE_ERRORS_PANEL_BOX: Optional[Union[str, "rich.box.Box"]] = "ROUNDED"
 ALIGN_ERRORS_PANEL: "rich.align.AlignMethod" = "left"
 STYLE_ERRORS_SUGGESTION: "rich.style.StyleType" = "dim"
 STYLE_ERRORS_SUGGESTION_COMMAND: "rich.style.StyleType" = "blue"
 STYLE_ABORTED: "rich.style.StyleType" = "red"
 WIDTH: Optional[int] = terminal_width_default()
 MAX_WIDTH: Optional[int] = terminal_width_default()
 COLOR_SYSTEM: Optional[Literal["auto", "standard", "256", "truecolor", "windows"]] = (
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_command.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_context.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_help_configuration.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_help_configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing_extensions import Literal
 
 from rich_click.utils import CommandGroupDict, OptionGroupDict, truthy
 
 
 if TYPE_CHECKING:
     import rich.align
+    import rich.box
     import rich.highlighter
     import rich.padding
     import rich.style
 
 
 T = TypeVar("T", bound="RichHelpConfiguration")
 
@@ -76,35 +77,38 @@
     style_helptext: "rich.style.StyleType" = field(default="dim")
     style_option_help: "rich.style.StyleType" = field(default="")
     style_option_default: "rich.style.StyleType" = field(default="dim")
     style_option_envvar: "rich.style.StyleType" = field(default="dim yellow")
     style_required_short: "rich.style.StyleType" = field(default="red")
     style_required_long: "rich.style.StyleType" = field(default="dim red")
     style_options_panel_border: "rich.style.StyleType" = field(default="dim")
+    style_options_panel_box: Optional[Union[str, "rich.box.Box"]] = field(default="ROUNDED")
     align_options_panel: "rich.align.AlignMethod" = field(default="left")
     style_options_table_show_lines: bool = field(default=False)
     style_options_table_leading: int = field(default=0)
     style_options_table_pad_edge: bool = field(default=False)
     style_options_table_padding: "rich.padding.PaddingDimensions" = field(default_factory=lambda: (0, 1))
-    style_options_table_box: "rich.style.StyleType" = field(default="")
+    style_options_table_box: Optional[Union[str, "rich.box.Box"]] = field(default="")
     style_options_table_row_styles: Optional[List["rich.style.StyleType"]] = field(default=None)
     style_options_table_border_style: Optional["rich.style.StyleType"] = field(default=None)
     style_commands_panel_border: "rich.style.StyleType" = field(default="dim")
+    style_commands_panel_box: Optional[Union[str, "rich.box.Box"]] = field(default="ROUNDED")
     align_commands_panel: "rich.align.AlignMethod" = field(default="left")
     style_commands_table_show_lines: bool = field(default=False)
     style_commands_table_leading: int = field(default=0)
     style_commands_table_pad_edge: bool = field(default=False)
     style_commands_table_padding: "rich.padding.PaddingDimensions" = field(default_factory=lambda: (0, 1))
-    style_commands_table_box: "rich.style.StyleType" = field(default="")
+    style_commands_table_box: Optional[Union[str, "rich.box.Box"]] = field(default="")
     style_commands_table_row_styles: Optional[List["rich.style.StyleType"]] = field(default=None)
     style_commands_table_border_style: Optional["rich.style.StyleType"] = field(default=None)
     style_commands_table_column_width_ratio: Optional[Union[Tuple[None, None], Tuple[int, int]]] = field(
         default_factory=lambda: (None, None)
     )
     style_errors_panel_border: "rich.style.StyleType" = field(default="red")
+    style_errors_panel_box: Optional[Union[str, "rich.box.Box"]] = field(default="ROUNDED")
     align_errors_panel: "rich.align.AlignMethod" = field(default="left")
     style_errors_suggestion: "rich.style.StyleType" = field(default="dim")
     style_errors_suggestion_command: "rich.style.StyleType" = field(default="blue")
     style_aborted: "rich.style.StyleType" = field(default="red")
     width: Optional[int] = field(default_factory=terminal_width_default)
     max_width: Optional[int] = field(default_factory=terminal_width_default)
     color_system: Optional[Literal["auto", "standard", "256", "truecolor", "windows"]] = field(default="auto")
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_help_formatter.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/src/rich_click/rich_help_rendering.py` & `rich_click-1.8.0.dev6/src/rich_click/rich_help_rendering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import re
 from fnmatch import fnmatch
-from typing import TYPE_CHECKING, Dict, Iterable, List, Optional, Tuple, TypeVar, Union, overload
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, TypeVar, Union, overload
 
 import click
 
 # Due to how rich_click.cli.patch() works, it is safer to import Command types directly
 # rather than use the click module e.g. click.Command
 from click import Command, Group
 from rich import box
@@ -422,37 +422,43 @@
 
         # Skip if option is hidden
         if getattr(param, "hidden", False):
             continue
 
         # Already mentioned in a config option group
         for option_group in option_groups:
-            if any([opt in option_group.get("options", []) for opt in param.opts]):
+            if any([opt in (option_group.get("options") or []) for opt in param.opts]):
                 break
 
         # No break, no mention - add to the default group
         else:
             if isinstance(param, click.core.Argument) and not formatter.config.group_arguments_options:
                 argument_group_options.append(param.opts[0])
             else:
                 list_of_option_groups = option_groups[-1]["options"]
                 list_of_option_groups.append(param.opts[0])
 
     # If we're not grouping arguments and we got some, prepend before default options
     if len(argument_group_options) > 0:
-        extra_option_group: OptionGroupDict = {
-            "name": formatter.config.arguments_panel_title,
-            "options": argument_group_options,
-        }
+        for grp in option_groups:
+            if grp.get("name", "") == formatter.config.arguments_panel_title and not grp.get("options"):
+                extra_option_group = grp.copy()
+                extra_option_group["options"] = argument_group_options
+                break
+        else:
+            extra_option_group: OptionGroupDict = {  # type: ignore[no-redef]
+                "name": formatter.config.arguments_panel_title,
+                "options": argument_group_options,
+            }
         option_groups.insert(len(option_groups) - 1, extra_option_group)
 
     # Print each option group panel
     for option_group in option_groups:
         options_rows = []
-        for opt in option_group.get("options", []):
+        for opt in option_group.get("options") or []:
             # Get the param
             for param in obj.get_params(ctx):
                 if any([opt in param.opts]):
                     break
             # Skip if option is not listed in this group
             else:
                 continue
@@ -541,37 +547,47 @@
                 "leading": formatter.config.style_options_table_leading,
                 "box": formatter.config.style_options_table_box,
                 "border_style": formatter.config.style_options_table_border_style,
                 "row_styles": formatter.config.style_options_table_row_styles,
                 "pad_edge": formatter.config.style_options_table_pad_edge,
                 "padding": formatter.config.style_options_table_padding,
             }
+            if isinstance(formatter.config.style_options_table_box, str):
+                t_styles["box"] = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
             t_styles.update(option_group.get("table_styles", {}))
-            box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
 
             options_table = Table(
                 highlight=True,
                 show_header=False,
                 expand=True,
-                box=box_style,
                 **t_styles,  # type: ignore[arg-type]
             )
             # Strip the required column if none are required
             if all([x[0] == "" for x in options_rows]):
                 options_rows = [x[1:] for x in options_rows]
             for row in options_rows:
                 options_table.add_row(*row)
-            formatter.write(
-                Panel(
-                    options_table,
-                    border_style=formatter.config.style_options_panel_border,
-                    title=option_group.get("name", formatter.config.options_panel_title),
-                    title_align=formatter.config.align_options_panel,
-                )
-            )
+
+            kw: Dict[str, Any] = {
+                "border_style": formatter.config.style_options_panel_border,
+                "title": option_group.get("name", formatter.config.options_panel_title),
+                "title_align": formatter.config.align_options_panel,
+            }
+
+            if isinstance(formatter.config.style_options_panel_box, str):
+                box_style = getattr(box, formatter.config.style_options_panel_box, None)
+            else:
+                box_style = formatter.config.style_options_panel_box
+
+            if box_style:
+                kw["box"] = box_style
+
+            kw.update(option_group.get("panel_styles", {}))
+
+            formatter.write(Panel(options_table, **kw))
 
 
 def get_rich_commands(
     obj: MultiCommand,
     ctx: click.Context,
     formatter: RichHelpFormatter,
 ) -> None:
@@ -597,22 +613,22 @@
             "leading": formatter.config.style_commands_table_leading,
             "box": formatter.config.style_commands_table_box,
             "border_style": formatter.config.style_commands_table_border_style,
             "row_styles": formatter.config.style_commands_table_row_styles,
             "pad_edge": formatter.config.style_commands_table_pad_edge,
             "padding": formatter.config.style_commands_table_padding,
         }
+        if isinstance(formatter.config.style_commands_table_box, str):
+            t_styles["box"] = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
         t_styles.update(cmd_group.get("table_styles", {}))
-        box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
 
         commands_table = Table(
             highlight=False,
             show_header=False,
             expand=True,
-            box=box_style,
             **t_styles,  # type: ignore[arg-type]
         )
         # Define formatting in first column, as commands don't match highlighter regex
         # and set column ratio for first and second column, if a ratio has been set
         if formatter.config.style_commands_table_column_width_ratio is None:
             table_column_width_ratio: Union[Tuple[None, None], Tuple[int, int]] = (None, None)
         else:
@@ -636,22 +652,31 @@
             if formatter.config.use_click_short_help:
                 helptext = cmd.get_short_help_str()
             else:
                 # Use short_help function argument if used, or the full help
                 helptext = cmd.short_help or cmd.help or ""
             commands_table.add_row(command, _make_command_help(helptext, formatter, is_deprecated=cmd.deprecated))
         if commands_table.row_count > 0:
-            formatter.write(
-                Panel(
-                    commands_table,
-                    border_style=formatter.config.style_commands_panel_border,
-                    title=cmd_group.get("name", formatter.config.commands_panel_title),
-                    title_align=formatter.config.align_commands_panel,
-                )
-            )
+
+            kw: Dict[str, Any] = {
+                "border_style": formatter.config.style_commands_panel_border,
+                "title": cmd_group.get("name", formatter.config.commands_panel_title),
+                "title_align": formatter.config.align_commands_panel,
+            }
+
+            if isinstance(formatter.config.style_commands_panel_box, str):
+                box_style = getattr(box, formatter.config.style_commands_panel_box, None)
+            else:
+                box_style = formatter.config.style_commands_panel_box
+
+            if box_style:
+                kw["box"] = box_style
+
+            kw.update(cmd_group.get("panel_styles", {}))
+            formatter.write(Panel(commands_table, **kw))
 
 
 def get_rich_epilog(
     self: Command,
     ctx: click.Context,
     formatter: RichHelpFormatter,
 ) -> None:
@@ -722,21 +747,33 @@
         )
 
     # A major Python library using click (dbt-core) has its own exception
     # logic that subclasses ClickException, but does not use the message
     # attribute. Checking for the 'message' attribute works to make the
     # rich-click CLI compatible.
     if hasattr(self, "message"):
+
+        kw: Dict[str, Any] = {}
+
+        if isinstance(formatter.config.style_errors_panel_box, str):
+            box_style = getattr(box, formatter.config.style_errors_panel_box, None)
+        else:
+            box_style = formatter.config.style_errors_panel_box
+
+        if box_style:
+            kw["box"] = box_style
+
         formatter.write(
             Padding(
                 Panel(
                     formatter.highlighter(self.format_message()),
                     border_style=config.style_errors_panel_border,
                     title=config.errors_panel_title,
                     title_align=config.align_errors_panel,
+                    **kw,
                 ),
                 (0, 0, 1, 0),
             )
         )
     if config.errors_epilogue:
         formatter.write(Padding(config.errors_epilogue, (0, 1, 1, 1)))
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click/utils.py` & `rich_click-1.8.0.dev6/src/rich_click/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
 class CommandGroupDict(TypedDict):
     """Specification for command groups."""
 
     name: NotRequired[str]
     commands: List[str]
     table_styles: NotRequired[Dict[str, Any]]
+    panel_styles: NotRequired[Dict[str, Any]]
 
 
 class OptionGroupDict(TypedDict):
     """Specification for option groups."""
 
     name: NotRequired[str]
-    options: List[str]
+    options: NotRequired[List[str]]
     table_styles: NotRequired[Dict[str, Any]]
+    panel_styles: NotRequired[Dict[str, Any]]
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click.egg-info/PKG-INFO` & `rich_click-1.8.0.dev6/src/rich_click.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev5
+Version: 1.8.0.dev6
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich_click-1.8.0.dev5/src/rich_click.egg-info/SOURCES.txt` & `rich_click-1.8.0.dev6/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/tests/test_config.py` & `rich_click-1.8.0.dev6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/tests/test_exit_code.py` & `rich_click-1.8.0.dev6/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/tests/test_help.py` & `rich_click-1.8.0.dev6/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev5/tests/test_rich_click_cli.py` & `rich_click-1.8.0.dev6/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

