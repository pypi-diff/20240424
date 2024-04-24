# Comparing `tmp/tkz-1.0.3.tar.gz` & `tmp/tkz-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkz-1.0.3.tar", last modified: Mon Apr 22 23:00:54 2024, max compression
+gzip compressed data, was "tkz-1.0.4.tar", last modified: Wed Apr 24 18:35:02 2024, max compression
```

## Comparing `tkz-1.0.3.tar` & `tkz-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 23:00:54.099663 tkz-1.0.3/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.3/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 23:00:54.099589 tkz-1.0.3/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    14676 2024-04-22 22:41:20.000000 tkz-1.0.3/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.3/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-22 23:00:54.099887 tkz-1.0.3/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 23:00:54.097908 tkz-1.0.3/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 23:00:54.098605 tkz-1.0.3/src/tkz/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.3/src/tkz/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    85875 2024-04-22 23:00:26.000000 tkz-1.0.3/src/tkz/tkz.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 23:00:54.099399 tkz-1.0.3/src/tkz.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 23:00:54.000000 tkz-1.0.3/src/tkz.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-22 23:00:54.000000 tkz-1.0.3/src/tkz.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-22 23:00:54.000000 tkz-1.0.3/src/tkz.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-22 23:00:54.000000 tkz-1.0.3/src/tkz.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-22 23:00:54.000000 tkz-1.0.3/src/tkz.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.420924 tkz-1.0.4/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.4/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15717 2024-04-24 18:35:02.420838 tkz-1.0.4/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15271 2024-04-24 18:34:35.000000 tkz-1.0.4/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.4/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-24 18:35:02.421147 tkz-1.0.4/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.418508 tkz-1.0.4/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.419864 tkz-1.0.4/src/tkz/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.4/src/tkz/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    86161 2024-04-24 18:34:14.000000 tkz-1.0.4/src/tkz/tkz.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.420641 tkz-1.0.4/src/tkz.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15717 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/top_level.txt
```

### Comparing `tkz-1.0.3/LICENSE.txt` & `tkz-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkz-1.0.3/PKG-INFO` & `tkz-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkz
-Version: 1.0.3
+Version: 1.0.4
 Summary: TikZ Figure Generator
 Home-page: https://gitlab.com/davidwoodburn/tkz
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -94,24 +94,33 @@
 
 ```python
 tkz.config.<option> = <value>
 ```
 
 There are some options you can set for all figures in your file:
 
-| Option      | Description                                 | Default Value |
-| :---------- | :------------------------------------------ | ------------- |
-| `skip`      | flag to skip all subsequent plotting        | `False`       |
-| `silent`    | flag to silence most of the pdflatex output | `True`        |
-| `directory` | directory of the generated figure files     | `None`        |
+| Option       | Description                                 | Default Value |
+| :----------- | :------------------------------------------ | ------------- |
+| `skip`       | flag to skip all subsequent plotting        | `False`       |
+| `silent`     | flag to silence most of the pdflatex output | `True`        |
+| `directory`  | directory of the generated figure files     | `None`        |
+| `standalone` | flag to create standalone LaTeX file        | `True`        |
+| `savepng`    | flag to output png version too              | `False`       |
 
 The `silent` option silences most of the pdflatex output messages, but not all.
 This is turned on by default. If you want to see all the messages, set this
 option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory.
+generated in the current working directory. If the `standalone` flag is `True`,
+this library will attempt to call the `pdflatex` command line program to compile
+the `.tex` file and produce a pdf image. Because you may need a rasterized
+version of your figure after all (see Microsoft Office's lack of support for pdf
+vector images), the `savepng` option will produce a png version of the image
+from the pdf version. This requires the program `pdftoppm` from the `poppler`
+command line utilities package, and that the `standalone` option be set to
+`True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
 
@@ -145,15 +154,14 @@
 | `ytick`       | flag to show y ticks                   | `True`            |
 | `ticksize`    | size of tick marks (cm)                | 0.1 cm            |
 | `xout`        | flag to put x-axis ticks outside       | `False`           |
 | `yout`        | flag to put y-axis ticks outside       | `False`           |
 | `rowmajor`    | flag to layout legend row major        | `False`           |
 | `columns`     | number of legend columns               | `None`            |
 | `preamble`    | added string of LaTeX code in preamble | `None`            |
-| `standalone`  | flag to create standalone LaTeX file   | `True`            |
 
 If either the `width` or `height` is specified, but not both, the other
 dimension will be calculated based on an aspect ratio equal to the golden ratio.
 
 Setting `equal` to `True` is equivalent to `plt.axis('equal')` in MatPlotLib.
 
 ## Data Set Options
```

### Comparing `tkz-1.0.3/README.md` & `tkz-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,24 +79,33 @@
 
 ```python
 tkz.config.<option> = <value>
 ```
 
 There are some options you can set for all figures in your file:
 
-| Option      | Description                                 | Default Value |
-| :---------- | :------------------------------------------ | ------------- |
-| `skip`      | flag to skip all subsequent plotting        | `False`       |
-| `silent`    | flag to silence most of the pdflatex output | `True`        |
-| `directory` | directory of the generated figure files     | `None`        |
+| Option       | Description                                 | Default Value |
+| :----------- | :------------------------------------------ | ------------- |
+| `skip`       | flag to skip all subsequent plotting        | `False`       |
+| `silent`     | flag to silence most of the pdflatex output | `True`        |
+| `directory`  | directory of the generated figure files     | `None`        |
+| `standalone` | flag to create standalone LaTeX file        | `True`        |
+| `savepng`    | flag to output png version too              | `False`       |
 
 The `silent` option silences most of the pdflatex output messages, but not all.
 This is turned on by default. If you want to see all the messages, set this
 option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory.
+generated in the current working directory. If the `standalone` flag is `True`,
+this library will attempt to call the `pdflatex` command line program to compile
+the `.tex` file and produce a pdf image. Because you may need a rasterized
+version of your figure after all (see Microsoft Office's lack of support for pdf
+vector images), the `savepng` option will produce a png version of the image
+from the pdf version. This requires the program `pdftoppm` from the `poppler`
+command line utilities package, and that the `standalone` option be set to
+`True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
 
@@ -130,15 +139,14 @@
 | `ytick`       | flag to show y ticks                   | `True`            |
 | `ticksize`    | size of tick marks (cm)                | 0.1 cm            |
 | `xout`        | flag to put x-axis ticks outside       | `False`           |
 | `yout`        | flag to put y-axis ticks outside       | `False`           |
 | `rowmajor`    | flag to layout legend row major        | `False`           |
 | `columns`     | number of legend columns               | `None`            |
 | `preamble`    | added string of LaTeX code in preamble | `None`            |
-| `standalone`  | flag to create standalone LaTeX file   | `True`            |
 
 If either the `width` or `height` is specified, but not both, the other
 dimension will be calculated based on an aspect ratio equal to the golden ratio.
 
 Setting `equal` to `True` is equivalent to `plt.axis('equal')` in MatPlotLib.
 
 ## Data Set Options
```

### Comparing `tkz-1.0.3/setup.cfg` & `tkz-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tkz
-version = 1.0.3
+version = 1.0.4
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = TikZ Figure Generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/tkz
 classifiers =
```

### Comparing `tkz-1.0.3/src/tkz/tkz.py` & `tkz-1.0.4/src/tkz/tkz.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 names of line styles (e.g., "dashdotted"). However, it is meant to also be
 flexible enough for the user who is familiar with the options of the TikZ
 package. This is enabled through the "fmt" parameter.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-04-22"
+__date__ = "2024-04-24"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
 import warnings
 import math                         # 5-10x faster than NumPy for scalars
@@ -96,14 +96,16 @@
 
 # Library-wide attributes
 class config:
     skip = False                    # flag to skip plotting
     silent = True                   # flag to silence pdflatex output
     directory = None                # directory for figure files
     colormap = MAP_WHEEL            # main color map
+    standalone = True               # flag to create standalone LaTeX file
+    savepng = False                 # flag to send call to `pdftoppm`
 
 
 class GraphLayout:
     """ Settings for the layout of the graph. """
     def __init__(self): # These are the internal, calculated settings.
         self.width = 0.0            # width of figure (cm)
         self.height = 0.0           # height of figure (cm)
@@ -186,16 +188,15 @@
     def __init__(self, filename='fig', width=None, height=None,
             xmin=None, xmax=None, ymin=None, ymax=None,
             xpad=False, ypad=True, xlog=False, ylog=False,
             equal=False, fontsize=9, xlabel=None, ylabel=None,
             xaxis=True, yaxis=True, xgrid=True, ygrid=True,
             xsubgrid=True, ysubgrid=True, xtick=True, ytick=True,
             ticksize=TICK_SIZE, xout=False, yout=False,
-            rowmajor=False, columns=None, preamble=None,
-            standalone=True):
+            rowmajor=False, columns=None, preamble=None):
         # Assign the settings. These are the user-facing options.
         self.filename = filename    # string of file without extension
         self.width = width          # width of pdf image in centimeters
         self.height = height        # height of pdf image in centimeters
         self.xmin = xmin            # x-axis minimum
         self.xmax = xmax            # x-axis maximum
         self.ymin = ymin            # y-axis minimum
@@ -218,15 +219,14 @@
         self.ytick = ytick          # flag to show y ticks
         self.ticksize = ticksize    # size of tick marks (cm)
         self.xout = xout            # flag to put x-axis ticks outside
         self.yout = yout            # flag to put y-axis ticks outside
         self.rowmajor = rowmajor    # flag to layout legend row major
         self.columns = columns      # number of legend columns
         self.preamble = preamble    # added string of LaTeX code in preamble
-        self.standalone = standalone# flag to create standalone LaTeX file
         self.sets = []              # list of set objects
 
     def plot(self, x, y=None, color=None, opacity=1.0, width=THICK,
             pattern=None, label=None, simp=True, fmt=None):
         fmt = append_to_fmt(fmt, opacity, width, pattern)
         p = Set(x=x, y=y, color=color,
                 func=plot_set, label=label, simp=simp, fmt=fmt)
@@ -353,15 +353,15 @@
 
         # Open the output file.
         filepath = "" if config.directory is None else config.directory + "/"
         filepath += self.filename + ".tex"
         fid = open(filepath, "w")
 
         # Open the standalone TikZ script.
-        if self.standalone:
+        if config.standalone:
             write_open(fid, self.preamble)
         elif self.preamble is not None:
             print("Because this plot is not standalone, "
                     + "the additional preamble cannot be used.")
 
         # Define the font size.
         write_textstyle(fid, lay.font_size_name)
@@ -557,39 +557,50 @@
                 else:
                     col += 1
                     if col >= lay.legend_cols:
                         row += 1
                         col = 0
 
         # Close the standalone TikZ script.
-        if self.standalone:
+        if config.standalone:
             write_close(fid)
 
         # Close the output file.
         fid.close()
 
         # -----------------
         # Compile the file.
         # -----------------
 
         # Compile the LaTeX file.
-        if self.standalone:
+        if config.standalone:
+            # Build the pdf compile command.
             cmd = 'pdflatex'
             if config.silent:
                 cmd = cmd + ' --interaction=batchmode'
-            if config.directory is None:
-                os.system(f'{cmd} {self.filename}.tex')
-                os.system(f'rm {self.filename}.aux')
-                os.system(f'rm {self.filename}.log')
-            else:
+
+            # Get the file name.
+            filename = self.filename
+
+            # Append to the command and file name if a directory is specified.
+            if config.directory is not None:
                 pwd = os.getcwd()
                 cmd = f'{cmd} -output-directory="{pwd}/{config.directory}"'
-                os.system(f'{cmd} "{config.directory}/{self.filename}.tex"')
-                os.system(f'rm {config.directory}/{self.filename}.aux')
-                os.system(f'rm {config.directory}/{self.filename}.log')
+                filename = config.directory + '/' + filename
+
+            # Compile the image to pdf.
+            os.system(f'{cmd} "{filename}.tex"')
+            os.system(f'rm "{filename}.aux"')
+            os.system(f'rm "{filename}.log"')
+
+            # Compile the image to png.
+            if config.savepng:
+                os.system(f'pdftoppm "{filename}.pdf" '
+                        + f'"{filename}" -png -r 600 -singlefile')
+
 
 # ---------------------
 # Calculation Functions
 # ---------------------
 
 def check_shapes(sets):
     # Cycle through each data set.
@@ -826,15 +837,15 @@
     # Force fontsize to be a standard value.
     font_sizes = np.array([5, 7, 8, 9, 10, 12, 14.4, 17.28, 20.74, 24.88])
     font_size_names = ["tiny", "scriptsize", "footnotesize", "small",
             "normalsize", "large", "Large", "LARGE", "huge", "Huge"]
     n = (np.abs(font_sizes - fig.fontsize)).argmin() # best-fit index
     if math.fabs(fig.fontsize - font_sizes[n]) > 0.01:
         print("The requested font size is adjusted to a standard value: "
-                + f"{font_size[n]} pt.")
+                + f"{font_sizes[n]} pt.")
     lay.font_size = font_sizes[n]
     lay.font_size_name = font_size_names[n]
 
     # Define text-based lengths.
     lay.L_text = 1.3*lay.font_size/PT_PER_CM # (cm)
 
     # Get the tick shift.
```

### Comparing `tkz-1.0.3/src/tkz.egg-info/PKG-INFO` & `tkz-1.0.4/src/tkz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkz
-Version: 1.0.3
+Version: 1.0.4
 Summary: TikZ Figure Generator
 Home-page: https://gitlab.com/davidwoodburn/tkz
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -94,24 +94,33 @@
 
 ```python
 tkz.config.<option> = <value>
 ```
 
 There are some options you can set for all figures in your file:
 
-| Option      | Description                                 | Default Value |
-| :---------- | :------------------------------------------ | ------------- |
-| `skip`      | flag to skip all subsequent plotting        | `False`       |
-| `silent`    | flag to silence most of the pdflatex output | `True`        |
-| `directory` | directory of the generated figure files     | `None`        |
+| Option       | Description                                 | Default Value |
+| :----------- | :------------------------------------------ | ------------- |
+| `skip`       | flag to skip all subsequent plotting        | `False`       |
+| `silent`     | flag to silence most of the pdflatex output | `True`        |
+| `directory`  | directory of the generated figure files     | `None`        |
+| `standalone` | flag to create standalone LaTeX file        | `True`        |
+| `savepng`    | flag to output png version too              | `False`       |
 
 The `silent` option silences most of the pdflatex output messages, but not all.
 This is turned on by default. If you want to see all the messages, set this
 option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory.
+generated in the current working directory. If the `standalone` flag is `True`,
+this library will attempt to call the `pdflatex` command line program to compile
+the `.tex` file and produce a pdf image. Because you may need a rasterized
+version of your figure after all (see Microsoft Office's lack of support for pdf
+vector images), the `savepng` option will produce a png version of the image
+from the pdf version. This requires the program `pdftoppm` from the `poppler`
+command line utilities package, and that the `standalone` option be set to
+`True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
 
@@ -145,15 +154,14 @@
 | `ytick`       | flag to show y ticks                   | `True`            |
 | `ticksize`    | size of tick marks (cm)                | 0.1 cm            |
 | `xout`        | flag to put x-axis ticks outside       | `False`           |
 | `yout`        | flag to put y-axis ticks outside       | `False`           |
 | `rowmajor`    | flag to layout legend row major        | `False`           |
 | `columns`     | number of legend columns               | `None`            |
 | `preamble`    | added string of LaTeX code in preamble | `None`            |
-| `standalone`  | flag to create standalone LaTeX file   | `True`            |
 
 If either the `width` or `height` is specified, but not both, the other
 dimension will be calculated based on an aspect ratio equal to the golden ratio.
 
 Setting `equal` to `True` is equivalent to `plt.axis('equal')` in MatPlotLib.
 
 ## Data Set Options
```

