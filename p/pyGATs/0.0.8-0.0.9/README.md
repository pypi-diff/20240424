# Comparing `tmp/pyGATs-0.0.8.tar.gz` & `tmp/pyGATs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGATs-0.0.8.tar", last modified: Tue Sep 26 10:29:22 2023, max compression
+gzip compressed data, was "pyGATs-0.0.9.tar", last modified: Mon Jan 22 12:48:45 2024, max compression
```

## Comparing `pyGATs-0.0.8.tar` & `pyGATs-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 10:29:22.899644 pyGATs-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-09-26 10:29:11.000000 pyGATs-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-09-26 10:29:22.899644 pyGATs-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-26 10:29:11.000000 pyGATs-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-09-26 10:29:11.000000 pyGATs-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 10:29:22.899644 pyGATs-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 10:29:22.895643 pyGATs-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 10:29:22.895643 pyGATs-0.0.8/src/pyGATs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-09-26 10:29:22.000000 pyGATs-0.0.8/src/pyGATs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-09-26 10:29:22.000000 pyGATs-0.0.8/src/pyGATs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 10:29:22.000000 pyGATs-0.0.8/src/pyGATs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-26 10:29:22.000000 pyGATs-0.0.8/src/pyGATs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 10:29:22.000000 pyGATs-0.0.8/src/pyGATs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 10:29:22.899644 pyGATs-0.0.8/src/pygats/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-09-26 10:29:11.000000 pyGATs-0.0.8/src/pygats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-09-26 10:29:11.000000 pyGATs-0.0.8/src/pygats/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-09-26 10:29:11.000000 pyGATs-0.0.8/src/pygats/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23831 2023-09-26 10:29:11.000000 pyGATs-0.0.8/src/pygats/pygats.py
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2023-09-26 10:29:11.000000 pyGATs-0.0.8/src/pygats/recog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 10:29:22.899644 pyGATs-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-09-26 10:29:11.000000 pyGATs-0.0.8/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-09-26 10:29:11.000000 pyGATs-0.0.8/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-09-26 10:29:11.000000 pyGATs-0.0.8/tests/test_pygats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:48:45.059673 pyGATs-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-22 12:48:34.000000 pyGATs-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-22 12:48:45.059673 pyGATs-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-22 12:48:34.000000 pyGATs-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-01-22 12:48:34.000000 pyGATs-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 12:48:45.059673 pyGATs-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:48:45.055673 pyGATs-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:48:45.059673 pyGATs-0.0.9/src/pyGATs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-22 12:48:45.000000 pyGATs-0.0.9/src/pyGATs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-22 12:48:45.000000 pyGATs-0.0.9/src/pyGATs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 12:48:45.000000 pyGATs-0.0.9/src/pyGATs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-22 12:48:45.000000 pyGATs-0.0.9/src/pyGATs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-22 12:48:45.000000 pyGATs-0.0.9/src/pyGATs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:48:45.055673 pyGATs-0.0.9/src/pygats/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/pygats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/qat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-01-22 12:48:34.000000 pyGATs-0.0.9/src/pygats/recog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:48:45.059673 pyGATs-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-01-22 12:48:34.000000 pyGATs-0.0.9/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-22 12:48:34.000000 pyGATs-0.0.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-22 12:48:34.000000 pyGATs-0.0.9/tests/test_pygats.py
```

### Comparing `pyGATs-0.0.8/LICENSE` & `pyGATs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/PKG-INFO` & `pyGATs-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,15 @@
 License-File: LICENSE
 Requires-Dist: pyautogui
 Requires-Dist: Pillow
 Requires-Dist: pytesseract
 Requires-Dist: Levenshtein
 Requires-Dist: opencv-python
 Requires-Dist: numpy
+Requires-Dist: mss
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 
 # pyGATs
 
 [![Pylint](https://github.com/IntegraSDL/pygats/actions/workflows/pylint.yml/badge.svg)](https://github.com/IntegraSDL/pygats/actions/workflows/pylint.yml)
 [![Python package](https://github.com/IntegraSDL/pygats/actions/workflows/python-package.yml/badge.svg)](https://github.com/IntegraSDL/pygats/actions/workflows/python-package.yml)
```

### Comparing `pyGATs-0.0.8/README.md` & `pyGATs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/pyproject.toml` & `pyGATs-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyGATs"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="vsysoev" },
 ]
 description = "Automate end-to-end and exploratory testing"
 keywords = ["gui", "testing", "automatic"]
 readme = "README.md"
 requires-python = ">=3.7"
@@ -18,15 +18,16 @@
 ]
 dependencies = [
     'pyautogui',
     'Pillow',
     'pytesseract',
     'Levenshtein',
     'opencv-python',
-    'numpy'
+    'numpy',
+    'mss'
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 repository = "https://github.com/IntegraSDL/pymagic-autogui.git"
 
 [project.optional-dependencies]
```

### Comparing `pyGATs-0.0.8/src/pyGATs.egg-info/PKG-INFO` & `pyGATs-0.0.9/src/pyGATs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,15 @@
 License-File: LICENSE
 Requires-Dist: pyautogui
 Requires-Dist: Pillow
 Requires-Dist: pytesseract
 Requires-Dist: Levenshtein
 Requires-Dist: opencv-python
 Requires-Dist: numpy
+Requires-Dist: mss
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 
 # pyGATs
 
 [![Pylint](https://github.com/IntegraSDL/pygats/actions/workflows/pylint.yml/badge.svg)](https://github.com/IntegraSDL/pygats/actions/workflows/pylint.yml)
 [![Python package](https://github.com/IntegraSDL/pygats/actions/workflows/python-package.yml/badge.svg)](https://github.com/IntegraSDL/pygats/actions/workflows/python-package.yml)
```

### Comparing `pyGATs-0.0.8/src/pygats/formatters.py` & `pyGATs-0.0.9/src/pygats/formatters.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/src/pygats/misc.py` & `pyGATs-0.0.9/src/pygats/misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/src/pygats/pygats.py` & `pyGATs-0.0.9/src/pygats/pygats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
 pyGATs is python3 library which combines power of pyautogui, opencv,
 tesseract, markdown and other staff to automate end-to-end and exploratory
 testing.
 """
 import time
 import sys
-import os
 import string
 import random
 import inspect
+import pathlib
 from typing import Optional, List
 import pyautogui
 import pyperclip
 from PIL import Image, ImageChops
 import cv2 as cv
 import numpy as np
+import mss
 
 from pygats.formatters import print_color_text
 
-PLATFORM = ''
 TESTS_PASSED = []
 TESTS_FAILED = []
 STEP_INDEX = 0
 SCREENSHOTS_ON = True
 SCREENSHOT_INDEX = 0
-OUTPUT_PATH = 'output'
-SNAPSHOT_PATH = ''
+OUTPUT_PATH = pathlib.Path('output')
+SNAPSHOT_PATH = None
 SNAPSHOT_INDEX = 0
 SUITE_NAME = ''
 
 
 class Context:  # pylint: disable=too-few-public-methods
     """
     Context stores information about
@@ -38,63 +38,31 @@
 
     def __init__(self, formatter):
         self.formatter = formatter
 
 
 class TestException(Exception):
     """
-    Test exception class stores msg and screenshot when error occurs
+    Test exception class stores msg when error occurs
     """
-    def __init__(self, img, msg):
-        self.image = img
+    def __init__(self, msg):
         self.message = msg
 
 
-def platform_specific_image(image_path: str) -> str:
-    """
-    function returns platform specific path to the image. If screenshot has
-    platform specifics it should be separated in different images. Name of
-    image contains platform name picName.PLATFORM.ext
-
-    Args:
-        image_path (str): path to image
-
-    Returns:
-        str: path to image
-    """
-    if PLATFORM == '':
-        return image_path
-
-    path_parts = image_path.split('.')
-    if len(path_parts) == 2:
-        specific_image_path = path_parts[0] + '.' + PLATFORM + '.' + path_parts[1]
-        if os.path.exists(specific_image_path):
-            return specific_image_path
-
-    return image_path
-
-
 def begin_test(ctx: Context, msg: str):
     """
     Begin of test. Dump msg as name of the test
 
     Args:
         ctx (Context): context of test execution
         msg (str): message to print at the beginning of test case
     """
     global STEP_INDEX
     ctx.formatter.print_header(3, msg)
     STEP_INDEX = 0
-    # img_path = os.path.join(OUTPUT_PATH, 'initial-state.png')
-    # pyautogui.screenshot(img_path)
-    # relative_path = img_path.split(os.path.sep)
-    # tmp_path = os.path.join('', *relative_path[1:])
-    # print('Начальное состояние')
-    # print()
-    # print(f'![Начальное состояние]({tmp_path})')
 
 
 def check(ctx: Context, msg: str, func=None):
     """
     Prints message as check block
 
     Args:
@@ -161,88 +129,90 @@
     Returns:
         PIL.Image: The screenshot as a PIL.Image object.
 
     Notes:
         The screenshot is also stored in the output path as `screenshotIndex`.
     """
     global SCREENSHOT_INDEX
-    img_path = os.path.join(
+    img_path = pathlib.Path(
         OUTPUT_PATH, f'step-{STEP_INDEX}-{SCREENSHOT_INDEX}-passed.png')
     SCREENSHOT_INDEX += 1
 
     # Take the screenshot and store it on disk
-    img = pyautogui.screenshot(img_path, region=rect)
-    # Get the relative path to the screenshot file
-    relative_path = img_path.split(os.path.sep)
-    tmp_path = os.path.join('', *relative_path[1:])
+    with mss.mss() as sct:
+        if rect is None:
+            img = np.array(sct.grab(sct.monitors[0]))
+        else:
+            monitor = {'left': rect[0], 'top': rect[1], 'width': rect[2], 'height': rect[3]}
+            img = np.array(sct.grab(monitor))
+        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+        img = cv.cvtColor(img, cv.COLOR_RGB2BGR)
+        cv.imwrite(str(img_path), img)
     # Display the screenshot
-    ctx.formatter.print_img(tmp_path)
+    ctx.formatter.print_img(img_path)
     return img
 
 
 def take_snapshot(ctx: Context) -> str:
     """Function takes a snapshot to further detect changes on the screen
 
     Args:
         ctx (Context): An object that contains information about the current
                     context.
 
     Returns:
-        tmp_path (str): path to snapshot
+        img_path (PosixPath): path to snapshot
     """
     step(ctx, 'Создание снимка для поиска изменений на экране')
     global SNAPSHOT_PATH
     global SNAPSHOT_INDEX
-    SNAPSHOT_PATH = os.path.join(OUTPUT_PATH, "compare")
-    try:
-        os.makedirs(SNAPSHOT_PATH)
-    except FileExistsError:
-        pass
-    img_path = os.path.join(SNAPSHOT_PATH, f'snapshot-{SNAPSHOT_INDEX}.png')
-    pyautogui.screenshot(img_path)
-    relative_path = img_path.split(os.path.sep)
-    tmp_path = os.path.join('', *relative_path[1:])
+    SNAPSHOT_PATH = pathlib.Path(OUTPUT_PATH, "compare")
+    SNAPSHOT_PATH.mkdir(exist_ok=True)
+    img_path = pathlib.Path(SNAPSHOT_PATH, f'snapshot-{SNAPSHOT_INDEX}.png')
+    with mss.mss() as sct:
+        img = np.array(sct.grab(sct.monitors[0]))
+        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+        img = cv.cvtColor(img, cv.COLOR_RGB2BGR)
+        cv.imwrite(str(img_path), img)
     SNAPSHOT_INDEX += 1
     print()
-    print(f'![Снимок экрана]({tmp_path})')
+    print(f'![Снимок экрана]({img_path})')
     print()
-    return tmp_path
+    return img_path
 
 
-def compare_snapshots(ctx: Context, first_image: str, second_image: str) -> tuple or None:
+def compare_snapshots(ctx: Context, first_img: str, second_img: str) -> tuple or None:
     """Function for comparing two images
 
     Args:
         ctx (Context): An object that contains information about the current
                     context.
-        first_image (str): path to first snapshot for compare
-        second_image (str): path to second snapshot for compare
+        first_img (str): path to first snapshot for compare
+        second_img (str): path to second snapshot for compare
 
     Returns:
         tupple or None: coordinates of the change detection area
     """
     step(ctx, 'Поиск изменений между снимками ...')
     print()
-    print(f'![Первый снимок]({first_image})')
+    print(f'![Первый снимок]({first_img})')
     print()
-    print(f'![Второй снимок]({second_image})')
+    print(f'![Второй снимок]({second_img})')
     print()
-    first = Image.open(os.path.join('./output', first_image))
-    second = Image.open(os.path.join('./output', second_image))
+    first = Image.open(first_img)
+    second = Image.open(second_img)
     result = ImageChops.difference(first, second)
     if result.getbbox() is not None:
-        relative_path = first_image.split('-')
+        relative_path = first_img.split('-')
         first_index = relative_path[len(relative_path) - 1].split('.')[0]
-        relative_path = second_image.split('-')
+        relative_path = second_img.split('-')
         second_index = relative_path[len(relative_path) - 1].split('.')[0]
-        result_path = os.path.join(SNAPSHOT_PATH, f'result-{first_index}-{second_index}.png')
+        result_path = pathlib.Path(SNAPSHOT_PATH, f'result-{first_index}-{second_index}.png')
         result.save(result_path)
-        relative_path = result_path.split(os.path.sep)
-        tmp_path = os.path.join('', *relative_path[1:])
-        print(f'![Найдены изменения]({tmp_path})')
+        print(f'![Найдены изменения]({result_path})')
         print()
         print('**Найдены изменения**')
         print()
         return result.getbbox()
     print()
     print('**Изменения не найдены**')
     print()
@@ -259,90 +229,85 @@
         msg (str, optional): description of the screenshot.
         Defaults to 'Снимок экрана'.  # noqa: DAR003
 
     Returns:
         PIL.Image: input image
     """
     global SCREENSHOT_INDEX
-    image_path = os.path.join(
+    img_path = pathlib.Path(
         OUTPUT_PATH, f'step-{STEP_INDEX}-{SCREENSHOT_INDEX}-passed.png')
     SCREENSHOT_INDEX += 1
-    img.save(image_path)
-    relative_path = image_path.split(os.path.sep)
-    tmp_path = os.path.join('', *relative_path[1:])
-    print(f'![{msg}]({tmp_path})')
+    img.save(img_path)
+    print(f'![{msg}]({img_path})')
     print()
     return img
 
 
 def passed():
     """
     function prints passed information after test case
     """
     if SCREENSHOTS_ON:
-        image_path = os.path.join(OUTPUT_PATH, f'step-{STEP_INDEX}-passed.png')
-        pyautogui.screenshot(image_path)
-        relative_path = image_path.split(os.path.sep)
-        tmp_path = os.path.join('', *relative_path[1:])
-        print(f'![Успешно]({tmp_path})')
+        img_path = pathlib.Path(OUTPUT_PATH, f'step-{STEP_INDEX}-passed.png')
+        with mss.mss() as sct:
+            img = np.array(sct.grab(sct.monitors[0]))
+            img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+            img = cv.cvtColor(img, cv.COLOR_RGB2BGR)
+            cv.imwrite(str(img_path), img)
+        print(f'![Успешно]({img_path})')
     print()
     print('**Успешно**')
     print()
 
 
-def failed(img=pyautogui.screenshot(), msg: Optional[str] = 'Тест не успешен'):
+def failed(msg: Optional[str] = 'Тест не успешен'):
     """
     function generates exception while error occurs
 
     Args:
-        img (PIL.Image, optional): image or screenshot
         msg (Optional[str]): failed text
 
     Raises:
         TestException: raise exception in case of test failed
     """
-    raise TestException(img, msg)
+    raise TestException(msg)
 
 
 def check_image(ctx: Context, img_path: str, timeout: Optional[int] = 1):
     """Check if image is located on screen. Timeout in second waiting image
     to occurs
 
     Args:
         ctx (Context): context
         img_path (str): path to image for check on screen
         timeout (Optional[int]): timeout in seconds to check if image occurs
     """
-    img_path = platform_specific_image(img_path)
     step(ctx, f'Проверка отображения {img_path} ...')
-    # try:
     while timeout > 0:
         if locate_on_screen(img_path) is not None:
             passed()
             return
         timeout -= 1
         time.sleep(1)
-    # except:  # pylint: disable=bare-except
-    #     print('Exception')
-    #     failed(img_path, 'Изображение не найдено')
-    # failed(img_path, 'Изображение не найдено')
 
 
 def locate_on_screen(img_path: str):
     """Function return coord of path to image located on screen.
     If not found returns None
 
     Args:
         img_path (str): path to image to find
 
     Returns:
         (x,y): coordinates path for image on screen
     """
-    img_path = platform_specific_image(img_path)
-    coord = pyautogui.locateOnScreen(img_path, confidence=0.5)
+    try:
+        coord = pyautogui.locateOnScreen(img_path, confidence=0.5)
+    except pyautogui.ImageNotFoundException:
+        failed(msg='Изображение не найдено')
     print(f'Изображение найдено в координатах {coord}')
     return coord
 
 
 def move_to_coord(ctx: Context, x: int, y: int):
     """Function moves mouse to coord x,y
 
@@ -360,19 +325,21 @@
     """Function move mouse to img_path
 
     Args:
         ctx (Context): context
         img_path (str): path to image for move to
 
     """
-    img_path = platform_specific_image(img_path)
     step(ctx, f'Переместить указатель мыши на изображение {img_path} ...')
-    center = pyautogui.locateCenterOnScreen(img_path, confidence=0.8)
+    try:
+        center = pyautogui.locateCenterOnScreen(img_path, confidence=0.8)
+    except pyautogui.ImageNotFoundException:
+        failed(msg='Изображение не найдено')
     if center is None:
-        failed(img_path, 'Изображение не найдено')
+        failed('Изображение не найдено')
     if sys.platform == 'darwin':
         pyautogui.moveTo(center.x / 2, center.y / 2)
     else:
         pyautogui.moveTo(center.x, center.y)
     print(f'Текущая позиция указателя мыши {pyautogui.position()}')
     passed()
 
@@ -406,35 +373,42 @@
     """function clicks button in area
 
     Args:
         ctx (Context): context
         button_path (str): path to button image to press
         area (Optional[str]): path to area of image to print
     """
-    button_path = platform_specific_image(button_path)
-    area = platform_specific_image(area)
     fail_message = 'Изображение не найдено'
     step(ctx, f'Нажать кнопку мыши {button_path} ...')
     if area == '':
-        center = pyautogui.locateCenterOnScreen(button_path, confidence=0.8)
+        try:
+            center = pyautogui.locateCenterOnScreen(button_path, confidence=0.8)
+        except pyautogui.ImageNotFoundException:
+            failed(msg='Изображение не найдено')
         print(f'Кнопка найдена с центром в координатах {center}')
     else:
         print(" area " + area)
-        area_location = pyautogui.locateOnScreen(area, confidence=0.9)
+        try:
+            area_location = pyautogui.locateOnScreen(area, confidence=0.9)
+        except pyautogui.ImageNotFoundException:
+            failed(msg='Изображение не найдено')
         if area_location is None:
-            failed(area, fail_message)
-        box = pyautogui.locate(button_path, area, confidence=0.8)
+            failed(fail_message)
+        try:
+            box = pyautogui.locate(button_path, area, confidence=0.8)
+        except pyautogui.ImageNotFoundException:
+            failed(msg='Изображение не найдено')
         if box is None:
-            failed(area, fail_message)
+            failed(fail_message)
 
         x = area_location.left + box.left + box.width / 2
         y = area_location.top + box.top + box.height / 2
         center = pyautogui.Point(x, y)
     if center is None:
-        failed(button_path, fail_message)
+        failed(fail_message)
 
     print(f'Перемещаем указатель мыши в координаты {center}')
     if sys.platform == 'darwin':
         pyautogui.moveTo(center.x / 2, center.y / 2)
     else:
         pyautogui.moveTo(center.x, center.y)
     # pyautogui.dragTo()
@@ -622,59 +596,59 @@
 
     cnts = list(filter(rect_filter, map(approx, cnts)))
     cnts = sorted(cnts, key=lambda x: abs(x.item(4) - x.item(0)) * abs
                   (x.item(5) - x.item(1)), reverse=True)
     return cnts
 
 
-def find_contours(ctx: Context, image_path: str, fltr=repeater):
+def find_contours(ctx: Context, img_path: str, fltr=repeater):
     """
     Function finds contours by cv and filter them with filter
 
     Args:
         ctx (Context): context of test run
-        image_path (str): path to image where contours will be searched
+        img_path (str): path to image where contours will be searched
         fltr (function, optional): filter which will be used on contours
         results  # noqa: DAR003
 
     Returns:
         list of points: list of points filtered
     """
     step(ctx, 'Поиск контуров с применением селектора')
-    image = cv.imread(image_path)
-    image_gray = cv.cvtColor(image, cv.COLOR_BGR2GRAY)
-    edges = cv.Canny(image_gray, 50, 100)
+    img = cv.imread(img_path)
+    img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
+    edges = cv.Canny(img_gray, 50, 100)
     kernel = cv.getStructuringElement(cv.MORPH_RECT, (2, 2))
     edges = cv.dilate(edges, kernel, iterations=1)
     contours, _ = cv.findContours(
         image=edges, mode=cv.RETR_TREE, method=cv.CHAIN_APPROX_NONE)
     return fltr(contours)
 
 
-def draw_contours(image: Image, cnts: List[np.ndarray]) -> Image:
+def draw_contours(img: Image, cnts: List[np.ndarray]) -> Image:
     """
     Draw contours on a PIL.Image instance.
 
     Args:
-        image (Image): Input image on which to draw the contours.
+        img (Image): Input image on which to draw the contours.
         cnts (List[np.ndarray]): List of contours, represented
         as Numpy arrays.  # noqa: DAR003
 
     Returns:
         Image: Output image with contours drawn.
 
     Raises:
         TypeError: If `img` is not a `PIL.Image` instance.
         ValueError: If `cnts` is not a list of Numpy arrays.
     """
-    if not isinstance(image, Image.Image):
+    if not isinstance(img, Image.Image):
         raise TypeError("img must be a PIL.Image instance")
     if not all(isinstance(cnt, np.ndarray) for cnt in cnts):
         raise ValueError("cnts must be a list of Numpy arrays")
-    np_img = cv.cvtColor(np.array(image), cv.COLOR_RGB2BGR)
+    np_img = cv.cvtColor(np.array(img), cv.COLOR_RGB2BGR)
     cv.drawContours(np_img, cnts, -1, (0, 255, 0), lineType=cv.LINE_AA)
     return Image.fromarray(cv.cvtColor(np_img, cv.COLOR_BGR2RGB))
 
 
 def random_string(string_length: int, character_set: Optional[str] = None):
     """Generate a randomized string of characters.
 
@@ -714,43 +688,44 @@
         counter (Optional[int]): amount to time test cases to be executed
         output (Optional[str]): path to store test results
         screenshots_on (Optional[bool]): create screenshots while running tests
     """
     global OUTPUT_PATH
     global SCREENSHOTS_ON
     SCREENSHOTS_ON = screenshots_on
-    try:
-        os.makedirs(output)
-    except FileExistsError:
-        pass
+    p = pathlib.Path(output)
+    p.mkdir(exist_ok=True)
     for _ in range(counter):
         for f in funcs:
             test_name = f.__name__
+            if SCREENSHOTS_ON:
+                p = pathlib.Path(output, SUITE_NAME, test_name)
+                p.mkdir(parents=True, exist_ok=True)
             try:
-                os.makedirs(os.path.join(output, SUITE_NAME, test_name))
-            except FileExistsError:
-                pass
-            try:
-                OUTPUT_PATH = os.path.join(output, SUITE_NAME, test_name)
+                OUTPUT_PATH = pathlib.Path(output, SUITE_NAME, test_name)
                 f()
-                TESTS_PASSED.append(os.path.join(SUITE_NAME, test_name))
+                TESTS_PASSED.append(str(pathlib.Path(SUITE_NAME, test_name)))
                 if SCREENSHOTS_ON:
-                    img_path = os.path.join(
+                    img_path = pathlib.Path(
                         output, SUITE_NAME, test_name, 'test-passed.png')
-                    pyautogui.screenshot(img_path)
-                    relative_path = img_path.split(os.path.sep)
-                    tmp_path = os.path.join('', *relative_path[1:])
-                    print(f'![Тест пройден]({tmp_path})')
+                    with mss.mss() as sct:
+                        img = np.array(sct.grab(sct.monitors[0]))
+                        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+                        img = cv.cvtColor(img, cv.COLOR_RGB2BGR)
+                        cv.imwrite(str(img_path), img)
+                    print(f'![Тест пройден]({img_path})')
                 print_color_text('\n**Тест пройден**', 'green')
             except TestException as e:
                 if SCREENSHOTS_ON:
-                    img_path = os.path.join(
+                    img_path = pathlib.Path(
                         output, SUITE_NAME, test_name, 'test-failed.png')
-                    pyautogui.screenshot(img_path)
-                    relative_path = img_path.split(os.path.sep)
-                    tmp_path = os.path.join('', *relative_path[1:])
-                    print(f'![Тест не пройден]({tmp_path})')
+                    with mss.mss() as sct:
+                        img = np.array(sct.grab(sct.monitors[0]))
+                        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+                        img = cv.cvtColor(img, cv.COLOR_RGB2BGR)
+                        cv.imwrite(str(img_path), img)
+                    print(f'![Тест не пройден]({img_path})')
                 print_color_text('\n> Error : ' + e.message + '\n', 'red')
                 print_color_text('**Тест не пройден**', 'red')
-                TESTS_FAILED.append(os.path.join(SUITE_NAME, test_name))
+                TESTS_FAILED.append(str(pathlib.Path(SUITE_NAME, test_name)))
 
     print_test_summary(TESTS_PASSED, TESTS_FAILED)
```

### Comparing `pyGATs-0.0.8/src/pygats/recog.py` & `pyGATs-0.0.9/src/pygats/recog.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 """
 
 from dataclasses import dataclass
 import re
 from typing import Optional
 import pyautogui
 import pytesseract
+import mss
+import numpy as np
+import cv2 as cv
 from Levenshtein import ratio
 from PIL import Image
 from pygats.pygats import step, passed, failed
 
 
 @dataclass
 class SearchedText:
@@ -90,15 +93,18 @@
 
     Returns:
         (roi, found):
             roi(ROI): region of interest
             found (bool): whether the text is found in the image
     """
     step(ctx, f'Поиск текста {txt.content} на экране ...')
-    img = pyautogui.screenshot()
+    with mss.mss() as sct:
+        img = np.array(sct.grab(sct.monitors[0]))
+        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+        img = Image.fromarray(img)
     roi, found = find_text(img, txt, skip, False, one_word)
     if found:
         return roi, found
     return find_text(img, txt, skip, True, one_word)
 
 
 def check_text(ctx, img: Image, txt):
@@ -112,32 +118,35 @@
     """
     step(ctx,
          f'Проверка отображения текста {txt.content} на изображении {img}...')
     _, found = find_text(img, txt)
     if not found:
         _, found = find_text(img, txt, extend=True)
         if not found:
-            failed(img, f'{txt.content} не найден на изображении')
+            failed(f'{txt.content} не найден на изображении')
     passed()
 
 
 def check_text_on_screen(ctx, txt):
     """Checks if text (txt) exists on the screen
 
     Args:
         ctx (Context): context
         txt (pygats.recog.SearchedText): text to search on screenshot
     """
     step(ctx, f'Проверка отображения текста {txt.content} на экране ...')
-    img = pyautogui.screenshot()
+    with mss.mss() as sct:
+        img = np.array(sct.grab(sct.monitors[0]))
+        img = cv.cvtColor(img, cv.COLOR_BGR2RGB)
+        img = Image.fromarray(img)
     _, found = find_text(img, txt)
     if not found:
         _, found = find_text(img, txt, extend=True)
         if not found:
-            failed(img, f'{txt.content} не найден на экране')
+            failed(f'{txt.content} не найден на экране')
     passed()
 
 
 def move_to_text(ctx, txt, skip=0):
     """Finds text on the screen and moves the cursor to it
 
     Args:
@@ -244,59 +253,66 @@
     Args:
         img (Image): The input image to crop.
         width (int, optional): The multiplier to determine the beginning of the crop area by width.
         height (int, optional): The multiplier to determine the beginning of the crop area by height
         extend (bool, optional): Whether to extend the crop area by a factor of 2.
 
     Returns:
-        Image: The cropped image area.
+        (x_offset, y_offset, img_crop):
+            x_offset (int), y_offset (int): offset by x and y coordinates
+            img_crop (Image): The cropped image area
     """
     img_width, img_height = img.size
     factor = 1
     if extend:
         crop_width = img_width // 4
         crop_height = img_height // 4
         factor = 2
     else:
         crop_width = img_width // 3
         crop_height = img_height // 3
     crop_coord = (crop_width * width,
                   crop_height * height,
                   crop_width * width + crop_width * factor,
                   crop_height * height + crop_height * factor)
+    x_offset = crop_coord[0]
+    y_offset = crop_coord[1]
     img_crop = img.crop(crop_coord)
-    return img_crop
+    return x_offset, y_offset, img_crop
 
 
 def find_crop_image(img: Image, crop_area: Optional[str] = 'all',
                     extend: Optional[bool] = False) -> Image:
     """
     Detects the crop area for the input image and crops the image based on the specified crop area.
 
     Args:
         img (Image): The input image to crop.
         crop_area (str, optional): The crop area to use. Defaults to 'all'. # noqa: DAR003
         extend (bool, optional): Whether to extend the crop area by a factor of 2.
         Defaults to False.
 
     Returns:
-        Image: The cropped image area.
+        (x_offset, y_offset, img_crop):
+            x_offset (int), y_offset (int): offset by x and y coordinates
+            img_crop (Image): The cropped image area
     """
     crop_area_params = {
         'center': (img, 1, 1, extend),
         'top-left': (img, 0, 0, extend),
         'left': (img, 0, 1, extend),
         'bottom-left': (img, 0, 2, extend),
         'top': (img, 1, 0, extend),
         'bottom': (img, 1, 2, extend),
         'top-right': (img, 2, 0, extend),
         'right': (img, 2, 1, extend),
         'bottom-right': (img, 2, 2, extend)
     }
-    return crop_image(*crop_area_params.get(crop_area)) if crop_area_params.get(crop_area) else img
+    return crop_image(*crop_area_params.get(crop_area)) if crop_area_params.get(crop_area)\
+        else (0, 0, img)
 
 
 def find_text(img: Image, txt, skip=0, extend=False, one_word=False):
     """Function finds text in image with Tesseract
 
     Args:
         img (Image): image where text will be recognized
@@ -306,22 +322,23 @@
         one_word (bool, optional): one word to search
 
     Returns:
         (roi,found):
             roi(ROI): region of interest
             found (bool): whether the text is found in the image
     """
-    img = find_crop_image(img, txt.area, extend=extend)
+    x_offset, y_offset, img = find_crop_image(img, txt.area, extend=extend)
     recognized = pytesseract.image_to_data(img, txt.lang).split('\n')
     lines = combine_lines(recognized, one_word)
     roi, found = ROI(-1, -1, -1, -1), False
     for pos, content in lines[1:]:
         if content.find(txt.content) != -1:
             print("Найден текст " + content)
-            roi, found = pos, True
+            roi = ROI(pos.x + x_offset, pos.y + y_offset, pos.w, pos.h)
+            found = True
             if skip <= 0:
                 break
             skip -= 1
         else:
             if pos.x + pos.y != 0:
                 cropped = img.crop(
                     (pos.x, pos.y,
```

### Comparing `pyGATs-0.0.8/tests/test_formatters.py` & `pyGATs-0.0.9/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/tests/test_misc.py` & `pyGATs-0.0.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.8/tests/test_pygats.py` & `pyGATs-0.0.9/tests/test_pygats.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 def test_screenshot(formatter, capsys):
     """test screenshot"""
     ctx = Context(formatter)
     assert ctx
     screenshot(ctx)
     cptrd = capsys.readouterr()
     print(cptrd.out)
-    assert cptrd.out == '![Screenshot](step-2-0-passed.png)\n\n'
+    assert cptrd.out == '![Screenshot](output/step-2-0-passed.png)\n\n'
```

