# Comparing `tmp/ItsPrompt-1.4.tar.gz` & `tmp/itsprompt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ItsPrompt-1.4.tar", last modified: Sat May 27 07:09:38 2023, max compression
+gzip compressed data, was "itsprompt-1.5.tar", last modified: Wed Apr 24 13:18:04 2024, max compression
```

## Comparing `ItsPrompt-1.4.tar` & `itsprompt-1.5.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/keyboard_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/objects/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    21146 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/raw_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 07:09:28.000000 ItsPrompt-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-27 07:09:38.985905 ItsPrompt-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-05-27 07:09:28.000000 ItsPrompt-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-27 07:09:28.000000 ItsPrompt-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 07:09:38.985905 ItsPrompt-1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-27 07:09:28.000000 ItsPrompt-1.4/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.621362 itsprompt-1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.617361 itsprompt-1.5/ItsPrompt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.617361 itsprompt-1.5/ItsPrompt/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/keyboard_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.617361 itsprompt-1.5/ItsPrompt/objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.621362 itsprompt-1.5/ItsPrompt/objects/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/prompts/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/prompts/options_with_separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/prompts/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/prompts/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.621362 itsprompt-1.5/ItsPrompt/objects/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/table/table_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/table/table_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/table/table_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/objects/table/table_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21337 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.621362 itsprompt-1.5/ItsPrompt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/raw_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/prompts/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:55.000000 itsprompt-1.5/ItsPrompt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:04.621362 itsprompt-1.5/ItsPrompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-24 13:18:04.000000 itsprompt-1.5/ItsPrompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 13:18:04.000000 itsprompt-1.5/ItsPrompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:18:04.000000 itsprompt-1.5/ItsPrompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 13:18:04.000000 itsprompt-1.5/ItsPrompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 13:18:04.000000 itsprompt-1.5/ItsPrompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 13:17:55.000000 itsprompt-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-24 13:18:04.621362 itsprompt-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-24 13:17:55.000000 itsprompt-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 13:17:55.000000 itsprompt-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:18:04.621362 itsprompt-1.5/setup.cfg
```

### Comparing `ItsPrompt-1.4/ItsPrompt/data/checkbox.py` & `itsprompt-1.5/ItsPrompt/data/select.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 from dataclasses import dataclass
 
+from ItsPrompt.objects.prompts.option import Option
+from ItsPrompt.objects.prompts.options_with_separator import OptionsWithSeparator
+from ItsPrompt.objects.prompts.separator import Separator
+from ItsPrompt.objects.prompts.type import OptionsList
+
 
 @dataclass
-class CheckboxOption:
+class SelectOption(Option):
     name: str
     id: str
-    is_selected: bool
+    is_disabled: bool
 
 
-def process_data(options: tuple[str | tuple[str, str], ...]) -> list[CheckboxOption]:
+def process_data(options: OptionsList) -> OptionsWithSeparator[SelectOption | Separator]:
     """
     Processes the given `options` and returns the processed list
 
     :param options: A list of options to process
-    :type options: tuple[str  |  tuple[str, str], ...]
+    :type options: tuple[str | OptionWithId | Separator, ...]
     :raises TypeError: If an option is not processable, a `TypeError` will be raised
-    :return: a list of `CheckboxOption`
-    :rtype: list[CheckboxOption]
+    :return: a list of `SelectOptions`
+    :rtype: list[SelectOption]
     """
-    processed_options: list[CheckboxOption] = []
+    processed_options: list[SelectOption | Separator] = []
 
     # process given options
     for option in options:
         if type(option) is str:
-            processed_options.append(CheckboxOption(name=option, id=option, is_selected=False))
+            processed_options.append(SelectOption(name=option, id=option, is_disabled=False))
         elif type(option) is tuple:
-            processed_options.append(CheckboxOption(name=option[0], id=option[1], is_selected=False))
+            processed_options.append(SelectOption(name=option[0], id=option[1], is_disabled=False))
+        elif type(option) is Separator:
+            processed_options.append(option)
         else:
             raise TypeError('Argument is not processable')
 
-    return processed_options
+    return OptionsWithSeparator(*processed_options)
```

### Comparing `ItsPrompt-1.4/ItsPrompt/data/expand.py` & `itsprompt-1.5/ItsPrompt/data/expand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 from dataclasses import dataclass
 
+from ..objects.prompts.option import Option
+from ..objects.prompts.options_with_separator import OptionsWithSeparator
+from ..objects.prompts.separator import Separator
+from ..objects.prompts.type import OptionsList
+
 
 @dataclass
-class ExpandOption:
+class ExpandOption(Option):
     key: str
     name: str
     id: str
+    is_disabled: bool
 
 
-def process_data(options: tuple[str | tuple[str, str, str], ...]) -> list[ExpandOption]:
+def process_data(options: OptionsList) -> OptionsWithSeparator[ExpandOption | Separator]:
     """
     Processes the given `options` and returns the processed list
 
     :param options: A list of options to process
-    :type options: tuple[str  |  tuple[str, str, str], ...]
+    :type options: tuple[str | OptionWithId | Separator, ...]
     :raises ValueError: If the keys are not unique
     :raises ValueError: If the keys are not of length 1
     :raises ValueError: If the keys are not ascii
     :raises ValueError: If the keys are using h
     :raises TypeError: If an option is not processable
     :return: A list of `ExpandOptions`
     :rtype: list[ExpandOption]
     """
     # check if every key is unique, otherwise return error
-    keys = [option[0] for option in options]
+    keys = [option[0] for option in options if type(option) is not Separator]  # type: ignore
     if len(set(keys)) < len(keys):
         raise ValueError('Keys must be unique!')
 
     # check that every key string is only one char long
-    if any([len(option[0]) > 1 or len(option[0]) < 1 for option in options]):
+    if any(
+        [
+            len(option[0]) > 1 or len(option[0]) < 1 for option in options if  # type: ignore
+            type(option) is not Separator
+        ]
+    ):
         raise ValueError('Keys must be of length 1!')
 
     # check that every key is ascii
-    if any([not option[0].isascii() for option in options]):
+    if any([not option[0].isascii() for option in options if type(option) is not Separator]):  # type: ignore
         raise ValueError('Keys must be ascii!')
 
     # check if h is not assigned
-    if any([option[0] == 'h' for option in options]):
+    if any([option[0] == 'h' for option in options if type(option) is not Separator]):  # type: ignore
         raise ValueError('The h-key is not assignable!')
 
     processed_options: list[ExpandOption] = []
 
     # process given options
     for option in options:
         if type(option) is str:
-            # use first letter as key, and str as name and id
-            processed_options.append(ExpandOption(key=option[0], name=option, id=option))
+            # use the first letter as the key, and str as name and id
+            processed_options.append(ExpandOption(key=option[0], name=option, id=option, is_disabled=False))
         elif type(option) is tuple:
-            processed_options.append(ExpandOption(key=option[0], name=option[1], id=option[2]))
+            processed_options.append(
+                ExpandOption(key=option[0], name=option[1], id=option[2], is_disabled=False)  # type: ignore
+            )
+        elif type(option) is Separator:
+            processed_options.append(option)  # type: ignore
         else:
             raise TypeError('Argument is not processable')
 
     # append a help option
-    processed_options.append(ExpandOption(key='h', name='Help Menu, list or hide all options', id=''))
+    processed_options.append(
+        ExpandOption(key='h', name='Help Menu, list or hide all options', id='', is_disabled=False)
+    )
 
-    return processed_options
+    return OptionsWithSeparator(*processed_options)
```

### Comparing `ItsPrompt-1.4/ItsPrompt/data/style.py` & `itsprompt-1.5/ItsPrompt/data/style.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,51 +2,58 @@
 from dataclasses import asdict, dataclass
 
 from prompt_toolkit.styles import Style
 
 
 @dataclass
 class PromptStyle:
-    '''
+    """
     The style object used for styling the prompts.
-    
+
     Empty styles will not be styled, so they appear without any styling.
-    '''
+    """
     question_mark: str = ''
     question: str = ''
     option: str = ''
     selected_option: str = ''
     tooltip: str = ''
     error: str = ''
     text: str = ''
     grayout: str = ''
+    disabled: str = ''
+    separator: str = ''
 
 
 default_style = PromptStyle(
-    question_mark='fg:ansigreen',
-    selected_option='fg:ansicyan',
-    tooltip='fg:ansibrightblue bg:ansiwhite bold',
-    error='fg:ansiwhite bg:ansired bold',
-    grayout='fg:ansibrightblack',
+    question_mark="fg:ansigreen",
+    selected_option="fg:ansicyan",
+    tooltip="fg:ansibrightblue bg:ansiwhite bold",
+    error="fg:ansiwhite bg:ansired bold",
+    grayout="fg:ansibrightblack",
+    disabled="fg:ansibrightblack",
+    separator="fg:ansibrightgreen",
 )
+"""
+The default style for the prompts.
+"""
 
 
-def convert_style(style: PromptStyle) -> Style:
-    '''
+def _convert_style(style: PromptStyle) -> Style:
+    """
     Converts the given `PromptStyle` to a usable `Style` object.
 
     :param style: The style to convert
     :type style: PromptStyle
     :return: The converted `Style` object
     :rtype: Style
-    '''
+    """
     return Style.from_dict(asdict(style))
 
 
 def create_from_default() -> PromptStyle:
-    '''
-    Returns a copy of the default style, which can be edited without changing the default style.
+    """
+    Returns a copy of the :data:`default_style` which can be edited without changing the default style.
 
-    :return: A editable copy of the default style
+    :return: An editable copy of the default style
     :rtype: PromptStyle
-    '''
+    """
     return copy.deepcopy(default_style)
```

### Comparing `ItsPrompt-1.4/ItsPrompt/data/table.py` & `itsprompt-1.5/ItsPrompt/data/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from typing import TYPE_CHECKING, Union
 
+from ..objects.prompts.type import TablePromptDict, TablePromptList
 from ..objects.table.table_base import TableDataBase
 from ..objects.table.table_dict import TableDataFromDict
+from ..objects.table.table_list import TableDataFromList
 
 # only import pandas and TableData if pandas is installed
 try:
     from pandas import DataFrame
 
     from ..objects.table.table_df import TableDataFromDF
 except ModuleNotFoundError:  # pragma: no cover
@@ -15,26 +17,28 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
 
 
 class Table:
 
-    def __init__(self, data: Union["DataFrame", dict[str, list[str]]]) -> None:
+    def __init__(self, data: Union["DataFrame", TablePromptDict, TablePromptList]) -> None:
         """
         Creates a table object for storing the drawable table instance
 
         :param data: the data to display
         :type data: DataFrame
         """
         # change type of all columns to str
         # TODO maybe later support more datatypes
         self.data: TableDataBase
         if type(data) is dict:
             self.data = TableDataFromDict(data)
+        elif type(data) is list:
+            self.data = TableDataFromList(data)
         elif type(data) is DataFrame:
             self.data = TableDataFromDF(data)
 
         # save amount of rows
         self.row_count = self.data.row_count
         self.col_count = self.data.col_count
```

### Comparing `ItsPrompt-1.4/ItsPrompt/keyboard_handler.py` & `itsprompt-1.5/ItsPrompt/keyboard_handler.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.4/ItsPrompt/objects/table/table_base.py` & `itsprompt-1.5/ItsPrompt/objects/table/table_base.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.4/ItsPrompt/objects/table/table_df.py` & `itsprompt-1.5/ItsPrompt/objects/table/table_df.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.4/ItsPrompt/objects/table/table_dict.py` & `itsprompt-1.5/ItsPrompt/objects/table/table_dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Generator
 
 from .table_base import TableDataBase
+from ..prompts.type import TablePromptDict
 
 
 class TableDataFromDict(TableDataBase):
 
-    def __init__(self, data: dict[str, list[str]]) -> None:
+    def __init__(self, data: TablePromptDict) -> None:
         # make sure every list has same length
         lengths = set([len(t) for t in data.values()])
         if len(lengths) != 1:
             raise ValueError("Dictionary columns (lists) must be same length!")
 
         self.data = data
 
@@ -48,9 +49,9 @@
     def del_key(self, row: int, col: int):
         new = self.get_item_at(row, col)[:-1]
         self.set_item_at(row, col, new)
 
     def get_column_location(self, val: str) -> int:
         return self.columns.index(val)
 
-    def get_data(self) -> dict[str, list[str]]:
+    def get_data(self) -> TablePromptDict:
         return self.data
```

### Comparing `ItsPrompt-1.4/ItsPrompt/prompt.py` & `itsprompt-1.5/ItsPrompt/prompt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-# ItsPrompt
+ItsPrompt
+=========
 
 created by ItsNameless
 
 :copyright: (c) 2023-present ItsNameless
 :license: MIT, see LICENSE for more details.
 """
 
@@ -24,17 +25,17 @@
 from prompt_toolkit.layout.controls import BufferControl, FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.layout.menus import (
     CompletionsMenu,
     MultiColumnCompletionsMenu,
 )
 
-from .data.style import PromptStyle, convert_style, default_style
-from .data.type import CompletionDict
+from .data.style import PromptStyle, _convert_style, default_style
 from .keyboard_handler import generate_key_bindings
+from .objects.prompts.type import CompletionDict, TablePromptDict, TablePromptList, OptionsList
 from .prompts.checkbox import CheckboxPrompt
 from .prompts.confirm import ConfirmPrompt
 from .prompts.expand import ExpandPrompt
 from .prompts.input import InputPrompt
 from .prompts.raw_select import RawSelectPrompt
 from .prompts.select import SelectPrompt
 from .prompts.table import TablePrompt
@@ -55,44 +56,42 @@
     ```
     """
 
     @classmethod
     def select(
         cls,
         question: str,
-        options: tuple[str | tuple[str, str], ...],
+        options: OptionsList,
         default: str | None = None,
+        disabled: tuple[str, ...] | None = None,
         style: PromptStyle | None = None,
     ) -> str:
         """
-        Ask the user for selecting ONE of the given `options`.
+        Ask the user for selecting **one** of the given `options`.
 
         This method shows the question alongside the `options` as a nice list. The user has the ability to use the
-        up, down and enter keys to navigate between the options and select the one thats right.
+        up, down and enter keys to navigate between the options and select the one that is right.
 
         The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
         where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
-        :type question: str
         :param options: A list of possible options
-        :type options: tuple[str  |  tuple[str, str], ...]
-        :param default: The id of the default option to select (empty or None if the first should be default),
-        defaults to None
-        :type default: str | None, optional
+        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
+        :param disabled: A list of ids, which should be disabled by default (empty if None)
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
-        :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
         """
         app = SelectPrompt(
             question,
             options,
             default,
+            disabled,
             layout=Layout(
                 HSplit(
                     [
                         Window(FormattedTextControl(), always_hide_cursor=True),
                         Window(
                             FormattedTextControl(HTML('Use UP, DOWN to select, ENTER to submit')),
                             char=' ',
@@ -100,58 +99,55 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(SelectPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def raw_select(
         cls,
         question: str,
-        options: tuple[str | tuple[str, str], ...],
+        options: OptionsList,
         default: str | None = None,
+        disabled: tuple[str, ...] | None = None,
         allow_keyboard: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
         """
-        Ask the user for selection ONE of the given `options`.
+        Ask the user for selecting **one** of the given `options`.
 
         This method shows the question alongside the `options` as a nice list. The user needs to type the index of
         the answer. If `allow_keyboard` is given, the user may use the keyboard as in the `select()` method.
 
         The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
         where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
-        :type question: str
         :param options: A list of possible options
-        :type options: tuple[str  |  tuple[str, str], ...]
-        :param default: The id of the default option to select (empty or None if the first should be default),
-        defaults to None
-        :type default: str | None, optional
+        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
+        :param disabled: A list of ids, which should be disabled by default (empty if None)
         :param allow_keyboard: Whether the user should be able to select the answer with up and down, defaults to False
-        :type allow_keyboard: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
-        :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
         """
         app = RawSelectPrompt(
             question,
             options,
             default,
+            disabled,
             allow_keyboard,
             layout=Layout(
                 HSplit(
                     [
                         Window(FormattedTextControl(), always_hide_cursor=True),
                         Window(
                             FormattedTextControl(HTML('Type the INDEX of your selection, ENTER to submit')),
@@ -160,59 +156,56 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(RawSelectPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
         ans = app.prompt()
-        if ans == None:
+        if ans is None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def expand(
         cls,
         question: str,
-        options: tuple[str | tuple[str, str, str], ...],
+        options: OptionsList,
         default: str | None = None,
+        disabled: tuple[str, ...] | None = None,
         allow_keyboard: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
         """
-        Ask the user for selecting ONE of the given `options`.
+        Ask the user for selecting **one** of the given `options`.
 
         The user needs to type the key of the option. If the user types `h`, all options will be shown.
 
         The `options` are either a string, where `s[0]` will be the key to select and the string will be used as name
         and id, or a tuple[str, str, str] where `t[0]` will be the key, `t[1]` the name and `t[2]` the id of the option.
 
         Every key must be a unique ascii character and of length 1, and there may not be a key assigned to `h`.
 
         :param question: The question to display
-        :type question: str
         :param options: A list of possible options
-        :type options: tuple[str  |  tuple[str, str, str], ...]
-        :param default: The id of the default option to select (empty or None if `h` should be default), defaults to
-        None
-        :type default: str | None, optional
+        :param default: The id of the default option to select (empty or None if `h` should be default), defaults to None
+        :param disabled: A list of ids, which should be disabled by default (empty if None)
         :param allow_keyboard: Whether the user should be able to select the answer with up and down, defaults to False
-        :type allow_keyboard: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
-        :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
         """
         app = ExpandPrompt(
             question,
             options,
             default,
+            disabled,
             allow_keyboard,
             layout=Layout(
                 HSplit(
                     [
                         Window(FormattedTextControl(), always_hide_cursor=True),
                         Window(
                             FormattedTextControl(
@@ -223,62 +216,58 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(ExpandPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
         ans = app.prompt()
-        if ans == None:
+        if ans is None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def checkbox(
         cls,
         question: str,
-        options: tuple[str | tuple[str, str], ...],
+        options: OptionsList,
         pointer_at: int | None = None,
         default_checked: tuple[str, ...] | None = None,
+        disabled: tuple[str, ...] | None = None,
         min_selections: int = 0,
         style: PromptStyle | None = None,
     ) -> list[str]:
         """
-        Ask the user for selecting MULTIPLE of the given `options`.
+        Ask the user for selecting **multiple** of the given `options`.
 
         The `options` will be shown as a nice list. The user may navigate with up and down, select or deselect with
         space and submit with enter.
 
         The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
         where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
-        :type question: str
         :param options: A list of possible options
-        :type options: tuple[str  |  tuple[str, str], ...]
         :param pointer_at: A 0-indexed value, where the pointer should start (0 if None), defaults to None
-        :type pointer_at: int | None, optional
         :param default_checked: A list of ids, which should be checked by default (empty if None)
-        :type default_checked: tuple[str, ...] | None, optional
-        :param min_selections: A minimum amount of options that need to be checked before submitting (prohibits the
-        user of submitting, if not enough are checked; 0 if None)
-        :type min_selections: int, optional
+        :param disabled: A list of ids, which should be disabled by default (empty if None)
+        :param min_selections: A minimum amount of options that need to be checked before submitting (prohibits the user of submitting, if not enough are checked; 0 if None)
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
-        :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The ids of the selected options
         :rtype: list[str]
         """
         app = CheckboxPrompt(
             question,
             options,
             pointer_at,
             default_checked,
+            disabled,
             min_selections,
             layout=Layout(
                 HSplit(
                     [
                         Window(FormattedTextControl(), always_hide_cursor=True),
                         Window(
                             FormattedTextControl(
@@ -289,15 +278,15 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(CheckboxPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
@@ -343,78 +332,84 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(ConfirmPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
 
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def input(
         cls,
         question: str,
         default: str | None = None,
         multiline: bool = False,
         show_symbol: str | None = None,
-        validate: Callable[[str], str | None] | None = None,
+        validate: Callable[[str], str | bool | None] | None = None,
         completions: list[str] | CompletionDict | None = None,
         completer: Completer | None = None,
         completion_show_multicolumn: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
         """
         Ask the user for typing an input.
 
-        If default is given, it will be returned if enter was pressed and no input was given by the user. If the user
-        writes an input, the default will be overwritten.
+        If :data:`default` is given, it will be returned if enter was pressed and no input was given by the user. If the user
+        writes an input, the :data:`default` will be overwritten.
+
+        If :data:`multiline` is activated, enter will not submit, but rather create a newline. Use ``alt+enter`` to submit.
 
-        If multiline is activated, enter will not submit, but rather create a newline. Use `alt+enter` to submit.
+        If :data:`show_symbol` is given, all chars (except newlines) will be replaced with this character in the interface.
+        The result will still be the input the user typed, it just will not appear in the CLI. This is useful for
+        password inputs.
 
-        If show_symbol is given, all chars (except newlines) will be replaced with this character in the interface.
-        The result will still be the input the user typed, it just will not appear in the CLI.
+        :data:`validate` takes a function which receives a :class:`str` (the current input of the user) and may 
+        return :class:`None`, a :class:`str` or simply a boolean value.
 
-        Validate takes a function which receives a `str` (the current input of the user) and may return None or a
-        `str`. If the function returns None, the prompt may assume that the input is valid. If it returns a `str`,
-        this will be the error shown to the user. The user will not be able to submit the input, if validate returns
-        an error.
+        If the function returns :class:`None` (or ``True``), the prompt may assume that the input is
+        valid.
 
-        Completions may be a list of possible completion strings or a nested dictionary where the key is a completion
-        string and the value is a new dict in the same style (more in the README.md).
+        If it returns a :class:`str`, this will be the error shown to the user. If it returns ``False``, the error 
+        shown will simply be a general error statement without additional information. The user will not be able to 
+        submit the input, if :data:`validate` returns an error.
 
-        You can use your own Completer as well (more in the README.md).
+        :data:`completions` may be a list of possible completion strings or a nested dictionary where the key is a 
+        completion string and the value is a new dict in the same style (more in the README.md).
 
-        THESE VALUES ARE MUTUALLY EXCLUSIVE. You may not use both. If you use a completer, you can not use show_symbol!
+        You can use your own :class:`Completer` as well (more in the README.md).
+
+        :data:`completions` **and** :data:`completer` **are mutually exclusive!** You may not use both. If you use a :data:`completer`, you can not use 
+        :data:`show_symbol`!
 
         :param question: The question to display
         :type question: str
         :param default: The default value to fill in, defaults to None
         :type default: str | None, optional
         :param multiline: Whether to allow the user to type multiple lines, defaults to False
         :type multiline: bool, optional
         :param show_symbol: A symbol to show instead of the users input, defaults to None
         :type show_symbol: str | None, optional
         :param validate: A function to check the users input in real-time, defaults to None
-        :type validate: Callable[[str], str | None] | None, optional
+        :type validate: Callable[[str], str | bool | None] | None, optional
         :param completions: The completions to use, defaults to None
         :type completions: list[str] | CompletionDict | None, optional
         :param completer: A completer to use, defaults to None
         :type completer: Completer | None, optional
-        :param completion_show_multicolumn: Whether to show the completions as a scrollable list or as multiple
-        columns, defaults to False
+        :param completion_show_multicolumn: if True, shows completions as multiple columns, defaults to False
         :type completion_show_multicolumn: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
-        :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
+        :raises KeyboardInterrupt: When the user presses ctrl-c, :class:`KeyboardInterrupt` will be raised
         :return: The input of the user
         :rtype: str
         """
 
         # extracting the body, so we can display a floating auto completion field
         body = HSplit(
             [
@@ -457,47 +452,47 @@
                             ycursor=True,
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(InputPrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
 
         ans = app.prompt()
-        if ans == None:
+        if ans is None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def table(
         cls,
         question: str,
-        data: Union["DataFrame", dict[str, list[str]]],
+        data: Union["DataFrame", TablePromptDict, TablePromptList],
         style: PromptStyle | None = None,
-    ) -> Union["DataFrame", dict[str, list[str]]]:
+    ) -> Union["DataFrame", TablePromptDict, TablePromptList]:
         """
         Ask the user for filling out the displayed table.
 
         This method shows the question alongside a table, which the user may navigate with the arrow keys. The user
-        has the ability to use the up, down and enter keys to navigate between the options and change the text in
+        can use the up, down and enter keys to navigate between the options and change the text in
         each cell.
 
-        The `data` is either a pandas DataFrame or a dictionary.
+        The `data` is either a :class:`pandas.DataFrame`, a :class:`list` or a :class:`dict` (more in the README.md).
 
         :param question: The question to display
         :type question: str
         :param data: The data to display
-        :type data: DataFrame | dict[str, list[str]]
+        :type data: DataFrame | TablePromptDict | TablePromptList
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
-        :rtype: str
+        :rtype: DataFrame | TablePromptDict | TablePromptList
         """
         app = TablePrompt(
             question,
             data,
             layout=Layout(
                 HSplit(
                     [
@@ -514,14 +509,14 @@
                             height=1
                         )
                     ]
                 )
             ),
             key_bindings=generate_key_bindings(TablePrompt),
             erase_when_done=True,
-            style=convert_style(style) if style else convert_style(default_style),
+            style=_convert_style(style) if style else _convert_style(default_style),
         )
         ans = app.prompt()
         # if type(ans) is type(None):
         if ans is None:
             raise KeyboardInterrupt()
         return ans  # type: ignore
```

### Comparing `ItsPrompt-1.4/ItsPrompt/prompts/checkbox.py` & `itsprompt-1.5/ItsPrompt/prompts/checkbox.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.checkbox import process_data
+from ..objects.prompts.separator import Separator
+from ..objects.prompts.type import OptionsList
 
 
 class CheckboxPrompt(Application):
     CHECKED_SIGN = '\u25cf'
     UNCHECKED_SIGN = '\u25cb'
 
     def __init__(
         self,
         question: str,
-        options: tuple[str | tuple[str, str], ...],
+        options: OptionsList,
         pointer_at: int | None = None,
         default_checked: tuple[str, ...] | None = None,
+        disabled: tuple[str, ...] | None = None,
         min_selections: int = 0,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
@@ -39,79 +42,111 @@
 
         # save min selections
         self.min_selections = min_selections
 
         # process options
         self.options = process_data(options)
 
-        # set pointer selection
-        self.selection = pointer_at if pointer_at else 0
-
         # default check default option (or none if not given)
         if default_checked is not None:
             was_set = 0  # Keeping track of options which where selected.
             # If was_set is not as big as len(default_checked),
             # then we know that there was an invalid option which could not be checked,
             # so we raise an error.
             for option in self.options:
                 if option.id in default_checked:
                     option.is_selected = True
                     was_set += 1
 
             if was_set != len(default_checked):
                 raise ValueError('At least one of the given default_checked values is invalid.')
 
+        # disable options (or none if not given)
+        if disabled is not None:
+            was_set = 0  # Keeping track of options which where disabled.
+            # If was_set is not as big as len(disabled),
+            # then we know that there was an invalid option which could not be disabled,
+            # so we raise an error.
+            for option in self.options:
+                if option.id in disabled:
+                    option.is_disabled = True
+                    was_set += 1
+
+            if was_set != len(disabled):
+                raise ValueError("At least one of the given disabled values is invalid.")
+
+        # set pointer selection
+        self.selection = pointer_at if pointer_at else 0
+
+        # if the current selection is disabled, we will skip it
+        while self.options[self.selection].is_disabled:
+            self.selection = (self.selection + 1) % len(self.options)
+
     def update(self):
         """update prompt content"""
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:'
 
-        for i, option in enumerate(self.options):
+        for i, option in self.options.with_separators_enumerate():
+
+            if type(option) is Separator:
+                content += f"\n<separator>{option.label}</separator>"
+                continue
+
+            disabled = ("<disabled>", "</disabled>") if option.is_disabled else ("", "")  # type: ignore
+            # Disabled tags will only be inserted if the option is disabled,
+            # otherwise there will only be an empty string inserted.
+            selected = self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN  # type: ignore
+
             if i == self.selection:
-                content += f'\n<selected_option>  > ' \
-                           f'{self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} ' \
-                           f'{option.name}</selected_option>'
+                content += f"\n{disabled[0]}<selected_option>  > {selected} {option.name}</selected_option>{disabled[1]}"  # type: ignore
             else:
-                content += f'\n<option>    ' \
-                           f'{self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} ' \
-                           f' {option.name} </option> '
-
-                self.prompt_content.text = HTML(content)
-
-                # show error, if error should be shown, else show normal prompt
-                if not self.is_error:
-                    # show normal prompt, change style to standard toolbar
-                    self.toolbar_content.text = self.toolbar_content_default_text
-                    self.toolbar_window.style = 'class:tooltip'
-                else:  # pragma: no cover
-                    # show error prompt and error style
-                    # the only error that might occur is that not enough options are selected
-                    self.toolbar_content.text = f'ERROR: a minimum of {self.min_selections} options need to be ' \
-                                                f'selected!'
-                    self.toolbar_window.style = 'class:error'
+                content += f"\n{disabled[0]}<option>    {selected} {option.name} </option>{disabled[1]}"  # type: ignore
+
+        self.prompt_content.text = HTML(content)
+
+        # show error, if error should be shown, else show normal prompt
+        if not self.is_error:
+            # show normal prompt, change style to standard toolbar
+            self.toolbar_content.text = self.toolbar_content_default_text
+            self.toolbar_window.style = 'class:tooltip'
+        else:  # pragma: no cover
+            # show error prompt and error style
+            # the only error that might occur is that not enough options are selected
+            self.toolbar_content.text = f'ERROR: a minimum of {self.min_selections} options need to be ' \
+                                        f'selected!'
+            self.toolbar_window.style = 'class:error'
 
     def prompt(self) -> list[str] | None:
         """start the application, returns the return value"""
         self.update()
         out: list[str] | None = self.run()
 
         return out
 
     def on_up(self):
         """when up is pressed, the previous indexed option will be selected"""
         self.selection = (self.selection - 1) % len(self.options)
 
+        # if the current selection is disabled, we will skip it
+        while self.options[self.selection].is_disabled:
+            self.selection = (self.selection - 1) % len(self.options)
+
         # reset error
         self.is_error = False
 
         self.update()
 
     def on_down(self):
         """when down is pressed, the next indexed option will be selected"""
         self.selection = (self.selection + 1) % len(self.options)
 
+        # if the current selection is disabled, we will skip it
+        while self.options[self.selection].is_disabled:
+            self.selection = (self.selection + 1) % len(self.options)
+
         # reset error
         self.is_error = False
 
         self.update()
 
     def on_space(self):
         """when space is pressed, select or deselect current selection"""
@@ -126,15 +161,15 @@
         # get selected options
         selected_options: list[str] = []
 
         for option in self.options:
             if option.is_selected:
                 selected_options.append(option.id)
 
-        # make sure that enough are selected
+        # make sure that enough options are selected
         if len(selected_options) < self.min_selections:  # pragma: no cover
             # show error
             self.is_error = True
             self.update()
             return
 
         self.exit(result=selected_options)
```

### Comparing `ItsPrompt-1.4/ItsPrompt/prompts/confirm.py` & `itsprompt-1.5/ItsPrompt/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.4/ItsPrompt/prompts/expand.py` & `itsprompt-1.5/ItsPrompt/prompts/select.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,112 @@
 from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.controls import FormattedTextControl
 
-from ..data.expand import process_data
+from ..data.select import process_data
+from ..objects.prompts.separator import Separator
+from ..objects.prompts.type import OptionsList
 
 
-class ExpandPrompt(Application):
+class SelectPrompt(Application):
 
     def __init__(
         self,
         question: str,
-        options: tuple[str | tuple[str, str, str], ...],
+        options: OptionsList,
         default: str | None = None,
-        allow_keyboard: bool = False,
+        disabled: tuple[str, ...] | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
         self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save question
         self.question = question
 
-        # save keyboard option
-        self.allow_keyboard = allow_keyboard
-
-        # save whether view is expanded or not
-        self.is_expanded = False
-
         # process options
         self.options = process_data(options)
 
-        # save a string with all keys
-        self.keys = ''.join([option.key for option in self.options])
+        # disable options
+        if disabled is not None:
+            was_set = 0  # Keeping track of options which where disabled.
+            # If was_set is not as big as len(disabled),
+            # then we know that there was an invalid option which could not be disabled,
+            # so we raise an error.
+            for option in self.options:
+                if option.id in disabled:
+                    option.is_disabled = True
+                    was_set += 1
+
+            if was_set != len(disabled):
+                raise ValueError("At least one of the given disabled values is invalid.")
 
-        # default select default option (or "help" if not given)
+        # default select default option (or first if not given)
         if default is None:
-            self.selection = 'h'
-            return
-
-        for i, option in enumerate(self.options):
-            if option.id == default:
-                self.selection = option.key
-                break
+            for i, option in enumerate(self.options):
+                if not option.is_disabled:
+                    self.selection = i
+                    break
         else:
-            raise ValueError('Default value is not a valid id.')
+            for i, option in enumerate(self.options):
+                if option.id == default:
+                    if option.is_disabled:
+                        raise ValueError("Default value must not be disabled.")
+                    self.selection = i
+                    break
+            else:
+                raise ValueError('Default value is not a valid id.')
 
     def update(self):
         """update prompt content"""
-        # question
-        content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: <text>({self.keys})</text>'
+        content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:'
 
-        # options, show only if it is expanded
-        if self.is_expanded:
-            for option in self.options:
-                if option.key == self.selection:
-                    content += f'\n<selected_option>    {option.key}) {option.name}</selected_option>'
-                else:
-                    content += f'\n<option>    {option.key}) {option.name}</option>'
+        for i, option in self.options.with_separators_enumerate():
 
-        # text
-        content += f'\n<text>    Answer: {self.selection}</text>'
+            if type(option) is Separator:
+                content += f"\n<separator>{option.label}</separator>"
+                continue
+
+            disabled = ("<disabled>", "</disabled>") if option.is_disabled else ("", "")  # type: ignore
+            # Disabled tags will only be inserted if the option is disabled,
+            # otherwise there will only be an empty string inserted.
+            if i == self.selection:
+                content += \
+                    f'\n{disabled[0]}<selected_option>  > {option.name}</selected_option>{disabled[1]}'  # type: ignore
+            else:
+                content += \
+                    f'\n{disabled[0]}<option>    {option.name}</option>{disabled[1]}'  # type: ignore
 
         self.prompt_content.text = HTML(content)
 
     def prompt(self) -> str | None:
         """start the application, returns the return value"""
         self.update()
         out: str | None = self.run()
 
         return out
 
     def on_up(self):
         """when up is pressed, the previous indexed option will be selected"""
-        if not self.allow_keyboard:
-            return
+        self.selection = (self.selection - 1) % len(self.options)
 
-        self.selection = self.keys[(self.keys.index(self.selection) - 1) % len(self.keys)]
+        # if the current selection is disabled, we will skip it
+        while self.options[self.selection].is_disabled:
+            self.selection = (self.selection - 1) % len(self.options)
 
         self.update()
 
     def on_down(self):
         """when down is pressed, the next indexed option will be selected"""
-        if not self.allow_keyboard:
-            return
+        self.selection = (self.selection + 1) % len(self.options)
 
-        self.selection = self.keys[(self.keys.index(self.selection) + 1) % len(self.keys)]
-
-        self.update()
-
-    def on_key(self, key_sequence: list[str]):
-        """when an index is pressed, which is available to select, select this index"""
-        key = key_sequence[0]
-
-        # return if key is not an available key
-        if not key in self.keys:
-            return
-
-        # only expand if h is pressed, otherwise change selection
-        if key == 'h':
-            self.is_expanded = not self.is_expanded
-        else:
-            self.selection = key
+        # if the current selection is disabled, we will skip it
+        while self.options[self.selection].is_disabled:
+            self.selection = (self.selection + 1) % len(self.options)
 
         self.update()
 
     def on_enter(self):
-        # if current selection is h-key, change is_expanded
-        # otherwise return selected id
-        if self.selection == 'h':
-            self.is_expanded = not self.is_expanded
-            self.update()
-            return
-
         # get selected id
-        self.exit(result=self.options[self.keys.index(self.selection)].id)
+        self.exit(result=self.options[self.selection].id)
```

### Comparing `ItsPrompt-1.4/ItsPrompt/prompts/input.py` & `itsprompt-1.5/ItsPrompt/prompts/input.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     FuzzyWordCompleter,
     NestedCompleter,
 )
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.processors import PasswordProcessor
 
-from ..data.type import CompletionDict
+from ..objects.prompts.type import CompletionDict
 
 
 class InputPrompt(Application):
 
     def __init__(
         self,
         question: str,
         default: str | None = None,
         multiline: bool = False,
         show_symbol: str | None = None,
-        validate: Callable[[str], str | None] | None = None,
+        validate: Callable[[str], str | bool | None] | None = None,
         completions: list[str] | CompletionDict | None = None,
         completer: Completer | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
@@ -111,24 +111,33 @@
 
         # run validation and show error, if validation gives error
         if not self.validate:
             return
 
         validation_result = self.validate(self.buffer.text)
 
-        self.is_error = bool(validation_result)
+        if validation_result in (None, True):
+            self.is_error = False
+        else:
+            # validation_result is either a string (which will be the displayed error) or False (if the user used a
+            # lambda statement)
+            self.is_error = True
+
+        # error is either the error returned by the validation function or a default error, if the validation
+        # returned False (in case it is a lambda)
+        error = validation_result if type(validation_result) is str else "Please check your Input!"
 
         # show error, if error should be shown, else show normal prompt
         if not self.is_error:
             # show normal prompt, change style to standard toolbar
             self.toolbar_content.text = self.toolbar_content_default_text
             self.toolbar_window.style = 'class:tooltip'
         else:
             # show error prompt and error style
-            self.toolbar_content.text = validation_result
+            self.toolbar_content.text = error
             self.toolbar_window.style = 'class:error'
 
         # run completion
         # Since we take over control of the buffer and the keyboard, the completion
         # (and all of its commands) need to be run manually every time we press a key.
         # This does not in any way change the user experience,
         # as it does the exact same thing the standard completer does.
```

### Comparing `ItsPrompt-1.4/ItsPrompt/prompts/table.py` & `itsprompt-1.5/ItsPrompt/prompts/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from typing import TYPE_CHECKING, Union
 
 from prompt_toolkit import Application, HTML
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.table import Table
+from ..objects.prompts.type import TablePromptDict, TablePromptList
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame
 
 
 class TablePrompt(Application):
 
     def __init__(
         self,
         question: str,
-        data: Union["DataFrame", dict[str, list[str]]],
+        data: Union["DataFrame", TablePromptDict, TablePromptList],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
         self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
@@ -44,18 +45,18 @@
         # append table
         content += html.escape(
             self.table.get_table_as_str()
         )  # escaping is needed so formatting from PromptToolkit won't destroy the whole table
 
         self.prompt_content.text = HTML(content)
 
-    def prompt(self) -> Union["DataFrame", dict[str, list[str]], None]:
+    def prompt(self) -> Union["DataFrame", TablePromptDict, None]:
         """start the application, returns the return value"""
         self.update()
-        out: Union["DataFrame", dict[str, list[str]], None] = self.run()
+        out: Union["DataFrame", TablePromptDict, None] = self.run()
 
         return out
 
     def on_up(self):
         """when up is pressed, the cell one above will be selected"""
         self.table.on_up()
```

### Comparing `ItsPrompt-1.4/ItsPrompt.egg-info/SOURCES.txt` & `itsprompt-1.5/ItsPrompt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 ItsPrompt/keyboard_handler.py
 ItsPrompt/prompt.py
+ItsPrompt/py.typed
 ItsPrompt.egg-info/PKG-INFO
 ItsPrompt.egg-info/SOURCES.txt
 ItsPrompt.egg-info/dependency_links.txt
 ItsPrompt.egg-info/requires.txt
 ItsPrompt.egg-info/top_level.txt
 ItsPrompt/data/__init__.py
 ItsPrompt/data/checkbox.py
 ItsPrompt/data/expand.py
 ItsPrompt/data/select.py
 ItsPrompt/data/style.py
 ItsPrompt/data/table.py
-ItsPrompt/data/type.py
+ItsPrompt/objects/prompts/option.py
+ItsPrompt/objects/prompts/options_with_separator.py
+ItsPrompt/objects/prompts/separator.py
+ItsPrompt/objects/prompts/type.py
 ItsPrompt/objects/table/table_base.py
 ItsPrompt/objects/table/table_df.py
 ItsPrompt/objects/table/table_dict.py
+ItsPrompt/objects/table/table_list.py
 ItsPrompt/prompts/__init__.py
 ItsPrompt/prompts/checkbox.py
 ItsPrompt/prompts/confirm.py
 ItsPrompt/prompts/expand.py
 ItsPrompt/prompts/input.py
 ItsPrompt/prompts/raw_select.py
 ItsPrompt/prompts/select.py
-ItsPrompt/prompts/table.py
-tests/test_prompt.py
+ItsPrompt/prompts/table.py
```

### Comparing `ItsPrompt-1.4/LICENSE` & `itsprompt-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.4/pyproject.toml` & `itsprompt-1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ItsPrompt"
-version = "1.4"
+version = "1.5"
 authors = [
     { name = "ItsNameless" },
 ]
 description = "Prompting - the fancy way"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -52,7 +52,8 @@
 each_dict_entry_on_separate_line = false
 dedent_closing_brackets = true
 
 [tool.mypy]
 packages = "ItsPrompt"
 explicit_package_bases = true
 check_untyped_defs = true
+exclude = ["docs", "venv"]
```

