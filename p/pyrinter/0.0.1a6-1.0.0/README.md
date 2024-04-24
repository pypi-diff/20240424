# Comparing `tmp/pyrinter-0.0.1a6.tar.gz` & `tmp/pyrinter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrinter-0.0.1a6.tar", last modified: Sun Apr 21 21:18:31 2024, max compression
+gzip compressed data, was "pyrinter-1.0.0.tar", last modified: Wed Apr 24 17:45:46 2024, max compression
```

## Comparing `pyrinter-0.0.1a6.tar` & `pyrinter-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:18:31.144549 pyrinter-0.0.1a6/
--rw-rw-rw-   0        0        0     1086 2022-10-21 07:49:12.000000 pyrinter-0.0.1a6/LICENSE
--rw-rw-rw-   0        0        0     1634 2024-04-21 21:18:31.143549 pyrinter-0.0.1a6/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 21:18:31.122548 pyrinter-0.0.1a6/pyrinter/
--rw-rw-rw-   0        0        0      189 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/__init__.py
--rw-rw-rw-   0        0        0     5795 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/document.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:18:31.139550 pyrinter-0.0.1a6/pyrinter/printers/
--rw-rw-rw-   0        0        0      234 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/printers/__init__.py
--rw-rw-rw-   0        0        0     1023 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/printers/abs_printer.py
--rw-rw-rw-   0        0        0      385 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/printers/sphinx_printer.py
--rw-rw-rw-   0        0        0     2722 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/printers/win_printer.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:18:31.141570 pyrinter-0.0.1a6/pyrinter/utils/
--rw-rw-rw-   0        0        0      250 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/utils/__init__.py
--rw-rw-rw-   0        0        0      313 2024-04-21 20:58:12.000000 pyrinter-0.0.1a6/pyrinter/utils/sphinx_utils.py
--rw-rw-rw-   0        0        0      343 2022-10-21 07:49:12.000000 pyrinter-0.0.1a6/pyrinter/utils/win_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:18:31.142552 pyrinter-0.0.1a6/pyrinter.egg-info/
--rw-rw-rw-   0        0        0     1634 2024-04-21 21:18:31.000000 pyrinter-0.0.1a6/pyrinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-04-21 21:18:31.000000 pyrinter-0.0.1a6/pyrinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:18:31.000000 pyrinter-0.0.1a6/pyrinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-21 21:18:31.000000 pyrinter-0.0.1a6/pyrinter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 21:18:31.000000 pyrinter-0.0.1a6/pyrinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 21:18:31.144549 pyrinter-0.0.1a6/setup.cfg
--rw-rw-rw-   0        0        0      733 2024-04-21 21:16:16.000000 pyrinter-0.0.1a6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.843387 pyrinter-1.0.0/
+-rw-rw-rw-   0        0        0     1086 2022-10-21 07:49:12.000000 pyrinter-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1632 2024-04-24 17:45:46.841386 pyrinter-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-04-21 20:58:12.000000 pyrinter-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.818788 pyrinter-1.0.0/pyrinter/
+-rw-rw-rw-   0        0        0      187 2024-04-24 17:43:37.000000 pyrinter-1.0.0/pyrinter/__init__.py
+-rw-rw-rw-   0        0        0     7535 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/document.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.832386 pyrinter-1.0.0/pyrinter/printers/
+-rw-rw-rw-   0        0        0      234 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/printers/__init__.py
+-rw-rw-rw-   0        0        0     1023 2024-04-21 20:58:12.000000 pyrinter-1.0.0/pyrinter/printers/abs_printer.py
+-rw-rw-rw-   0        0        0      385 2024-04-21 20:58:12.000000 pyrinter-1.0.0/pyrinter/printers/sphinx_printer.py
+-rw-rw-rw-   0        0        0     3260 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/printers/win_printer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.840386 pyrinter-1.0.0/pyrinter/utils/
+-rw-rw-rw-   0        0        0      250 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/utils/__init__.py
+-rw-rw-rw-   0        0        0      315 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/utils/sphinx_utils.py
+-rw-rw-rw-   0        0        0      343 2022-10-21 07:49:12.000000 pyrinter-1.0.0/pyrinter/utils/win_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.841386 pyrinter-1.0.0/pyrinter.egg-info/
+-rw-rw-rw-   0        0        0     1632 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:45:46.843387 pyrinter-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-24 17:44:13.000000 pyrinter-1.0.0/setup.py
```

### Comparing `pyrinter-0.0.1a6/LICENSE` & `pyrinter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrinter-0.0.1a6/PKG-INFO` & `pyrinter-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrinter
-Version: 0.0.1a6
+Version: 1.0.0
 Summary: python printer package
 Author: Hod Vaknin
 License: MIT
 Project-URL: Source, https://github.com/hodvak/py-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyrinter-0.0.1a6/README.md` & `pyrinter-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrinter-0.0.1a6/pyrinter/document.py` & `pyrinter-1.0.0/pyrinter/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from enum import Enum
 from tkinter import Tk
 from tkinter.font import Font as TkFont
 from collections import namedtuple
 from typing import Tuple, Generator, Optional, Union
+from PIL import Image
 
 
 class Font(namedtuple("Font", ("font_name", "height"))):
     """
     class to represent font properties (font name and height)
     """
 
 
 class Align(Enum):
     """
     Alignment for text
     """
+
     RIGHT = 0
     LEFT = 1
 
 
 class PaperSize(Enum):
     """
     Common paper sizes
     """
+
     LETTER = (8.5, 11)
     A4 = (8.3, 11.7)
 
 
 class Document:
     """
     document that can be printed with Printer
     """
 
     def __init__(
-            self,
-            name: str = "My Document",
-            page_size: Union[PaperSize, Tuple[float, float]] = PaperSize.A4,
+        self,
+        name: str = "My Document",
+        page_size: Union[PaperSize, Tuple[float, float]] = PaperSize.A4,
     ):
         """
         create document with name and
 
         :param name: the name of the document (default "My Document")
         :param page_size: the size of the document (default A4)
         """
@@ -48,21 +51,21 @@
 
         if isinstance(page_size, PaperSize):
             page_size = page_size.value
         self.page_size = page_size
         self.name = name
 
     def add_text(
-            self,
-            text: str,
-            font: Font = Font(font_name="Arial", height=12),
-            page: Optional[int] = None,
-            rect: Optional[Tuple[float, float, float, float]] = None,
-            align: Align = Align.LEFT,
-            color: int = 0x000000,
+        self,
+        text: str,
+        font: Font = Font(font_name="Arial", height=12),
+        page: Optional[int] = None,
+        rect: Optional[Tuple[float, float, float, float]] = None,
+        align: Align = Align.LEFT,
+        color: int = 0x000000,
     ):
         """
         add text to the document
 
         :param text: the text to print
         :param font: the font to use
         :param page: specific page to print on, None for new page. Negative indexing is supported. Default None
@@ -90,16 +93,16 @@
 
         new_lines = []
         for line in text.split("\n"):
             new_lines.append("")
             for word in line.split(" "):
                 if new_lines[-1]:
                     if (
-                            Document.__get_text_size(new_lines[-1] + " " + word, font)
-                            < rect[2] - rect[0]
+                        Document.__get_text_size(new_lines[-1] + " " + word, font)
+                        < rect[2] - rect[0]
                     ):
                         new_lines[-1] += " " + word
                     else:
                         new_lines.append(word)
                 else:
                     new_lines[-1] = word
 
@@ -116,34 +119,34 @@
                     "align": align,
                     "color": color,
                 },
             }
         )
 
     def add_frame_rect(
-            self,
-            rect: Optional[Tuple[float, float, float, float]] = None,
-            width: float = 0.01,
-            color: int = 0x000000,
-            page: Optional[int] = None,
+        self,
+        rect: Optional[Tuple[float, float, float, float]] = None,
+        width: float = 0.01,
+        color: int = 0x000000,
+        page: Optional[int] = None,
     ):
         """
         add frame rectangle to the document
 
         :param rect: the rectangle to draw
         :param width: the width of the frame (inch)
         :param color: the color of the frame
         :param page: specific page to print on, None for the last page
         :return: None
         """
         if page is None:
             page = self.pages
 
         if page < 0:
-            page += self.page_size
+            page += self.pages
 
         if page >= self.pages:
             self.pages = page + 1
 
         if page < 0:
             raise IndexError(
                 f"Page index out of range, must be above or equal to {-self.pages} (the number of pages)"
@@ -156,14 +159,66 @@
             {
                 "type": "frame_rect",
                 "page": page,
                 "data": {"rect": rect, "color": color, "width": width},
             }
         )
 
+    def add_image(
+        self,
+        image: Union[str, Image.Image],
+        rect: Optional[Tuple[int, int, int, int]] = None,
+        page: Optional[int] = None,
+    ):
+        """
+        | add image to the document.
+        | on windows: transparent will become white background
+
+        :param image: the image to add, an PIL Image instance or a path to an image
+        :param rect: the rectangle to draw on (inches), None to draw on the whole page
+        :param page: the page to draw on, None for new page. Negative indexing is supported. Default None
+        """
+        if page is None:
+            page = self.pages
+
+        if page < 0:
+            page += self.pages
+
+        if page >= self.pages:
+            self.pages = page + 1
+
+        if page < 0:
+            raise IndexError(
+                f"Page index out of range, must be above or equal to {-self.pages} (the number of pages)"
+            )
+
+        if isinstance(image, str):
+            image = Image.open(image)
+
+        image_width, image_height = image.size
+        if rect is None:
+            scale = min(
+                (self.page_size[0] - 0.75 * 2) / image_width,
+                (self.page_size[1] - 0.75 * 2) / image_height,
+            )
+            new_width = int(image_width * scale)
+            new_height = int(image_height * scale)
+            center = (self.page_size[0] / 2, self.page_size[1] / 2)
+
+            rect = (
+                center[0] - new_width / 2,
+                center[1] - new_height / 2,
+                center[0] + new_width / 2,
+                center[1] + new_height / 2,
+            )
+
+        self.data.append(
+            {"type": "image", "page": page, "data": {"image": image, "rect": rect}}
+        )
+
     @staticmethod
     def __get_text_size(text: str, font: Font) -> float:
         """
         get the text size of a text (width) by the given font
 
         :param text: the text to print
         :param font: the font to use
```

### Comparing `pyrinter-0.0.1a6/pyrinter/printers/abs_printer.py` & `pyrinter-1.0.0/pyrinter/printers/abs_printer.py`

 * *Files identical despite different names*

### Comparing `pyrinter-0.0.1a6/pyrinter/printers/win_printer.py` & `pyrinter-1.0.0/pyrinter/printers/win_printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from PIL import ImageWin, Image
+
 from pyrinter import Document
 from .abs_printer import AbsPrinter
 import win32ui
 import win32con
 
 from ..document import Align
 
@@ -16,14 +18,15 @@
         doc.CreatePrinterDC(self.name)
         doc.StartDoc(document.name)
         doc.SetMapMode(win32con.MM_HIENGLISH)
 
         type_to_command = {
             "text": Printer.__add_text,
             "frame_rect": Printer.__add_frame_rect,
+            "image": Printer.__add_image,
         }
 
         for page in document:
             doc.StartPage()
             for to_print in page:
                 type_to_command[to_print["type"]](doc, to_print["data"])
             doc.EndPage()
@@ -60,14 +63,26 @@
         doc.MoveTo((rect[0], rect[1]))
         doc.LineTo((rect[0], rect[3]))
         doc.LineTo((rect[2], rect[3]))
         doc.LineTo((rect[2], rect[1]))
         doc.LineTo((rect[0], rect[1]))
 
     @staticmethod
+    def __add_image(doc, data):
+        image = data["image"]
+        if image.mode == "RGBA":
+            # Create a white background image
+            white_bg = Image.new("RGBA", image.size, (255, 255, 255, 255))
+            image = Image.alpha_composite(white_bg, image)
+
+        image = image.convert("RGB")
+        dip = ImageWin.Dib(image)
+        dip.draw(doc.GetHandleOutput(), Printer.__get_printer_rect(data["rect"]))
+
+    @staticmethod
     def __get_printer_rect(rect):
         return (
             int(Printer.__inch_to_printer_size(rect[0])),
             -int(Printer.__inch_to_printer_size(rect[1])),
             int(Printer.__inch_to_printer_size(rect[2])),
             -int(Printer.__inch_to_printer_size(rect[3])),
         )
```

### Comparing `pyrinter-0.0.1a6/pyrinter.egg-info/PKG-INFO` & `pyrinter-1.0.0/pyrinter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrinter
-Version: 0.0.1a6
+Version: 1.0.0
 Summary: python printer package
 Author: Hod Vaknin
 License: MIT
 Project-URL: Source, https://github.com/hodvak/py-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyrinter-0.0.1a6/setup.py` & `pyrinter-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyrinter",
-    version="0.0.1a6",
+    version="1.0.0",
     packages=find_packages(include=["pyrinter", "pyrinter.*"]),
     author="Hod Vaknin",
     license="MIT",
     description="python printer package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={"Source": "https://github.com/hodvak/py-printer"},
```

