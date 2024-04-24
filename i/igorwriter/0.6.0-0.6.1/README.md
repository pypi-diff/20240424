# Comparing `tmp/igorwriter-0.6.0.tar.gz` & `tmp/igorwriter-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igorwriter-0.6.0.tar", last modified: Sat Jan 13 08:51:05 2024, max compression
+gzip compressed data, was "igorwriter-0.6.1.tar", last modified: Wed Apr 24 10:57:48 2024, max compression
```

## Comparing `igorwriter-0.6.0.tar` & `igorwriter-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-01-13 08:51:05.280944 igorwriter-0.6.0/
--rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6453 2024-01-13 08:51:05.279945 igorwriter-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5875 2024-01-13 08:08:02.000000 igorwriter-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-13 08:51:05.270943 igorwriter-0.6.0/igorwriter/
--rw-rw-rw-   0        0        0       53 2023-07-04 12:29:43.000000 igorwriter-0.6.0/igorwriter/__init__.py
--rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.6.0/igorwriter/builtin_names.py
-drwxrwxrwx   0        0        0        0 2024-01-13 08:51:05.276944 igorwriter-0.6.0/igorwriter/builtins/
--rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.6.0/igorwriter/builtins/functions.txt
--rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.6.0/igorwriter/builtins/keywords.txt
--rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.6.0/igorwriter/builtins/operations.txt
--rw-rw-rw-   0        0        0      214 2023-07-07 17:00:52.000000 igorwriter-0.6.0/igorwriter/errors.py
--rw-rw-rw-   0        0        0    24283 2024-01-13 08:47:38.000000 igorwriter-0.6.0/igorwriter/igorwave.py
--rw-rw-rw-   0        0        0     1529 2023-07-07 16:02:45.000000 igorwriter-0.6.0/igorwriter/utils.py
--rw-rw-rw-   0        0        0     3012 2023-07-07 16:02:45.000000 igorwriter-0.6.0/igorwriter/validator.py
-drwxrwxrwx   0        0        0        0 2024-01-13 08:51:05.279945 igorwriter-0.6.0/igorwriter.egg-info/
--rw-rw-rw-   0        0        0     6453 2024-01-13 08:51:05.000000 igorwriter-0.6.0/igorwriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-01-13 08:51:05.000000 igorwriter-0.6.0/igorwriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-13 08:51:05.000000 igorwriter-0.6.0/igorwriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-01-13 08:51:05.000000 igorwriter-0.6.0/igorwriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-13 08:51:05.000000 igorwriter-0.6.0/igorwriter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2024-01-13 08:51:05.280944 igorwriter-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1278 2024-01-13 08:49:15.000000 igorwriter-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-13 08:51:05.278943 igorwriter-0.6.0/tests/
--rw-rw-rw-   0        0        0     4113 2023-07-07 16:02:45.000000 igorwriter-0.6.0/tests/test_names.py
--rw-rw-rw-   0        0        0     1102 2023-07-07 16:02:45.000000 igorwriter-0.6.0/tests/test_utils.py
--rw-rw-rw-   0        0        0    19699 2024-01-13 08:47:38.000000 igorwriter-0.6.0/tests/test_wave.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:57:48.817468 igorwriter-0.6.1/
+-rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     6281 2024-04-24 10:57:48.817468 igorwriter-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5640 2024-04-24 10:54:55.000000 igorwriter-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:57:48.808468 igorwriter-0.6.1/igorwriter/
+-rw-rw-rw-   0        0        0       53 2023-07-04 12:29:43.000000 igorwriter-0.6.1/igorwriter/__init__.py
+-rw-rw-rw-   0        0        0      442 2024-01-20 09:55:42.000000 igorwriter-0.6.1/igorwriter/builtin_names.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:57:48.813467 igorwriter-0.6.1/igorwriter/builtins/
+-rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.6.1/igorwriter/builtins/functions.txt
+-rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.6.1/igorwriter/builtins/keywords.txt
+-rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.6.1/igorwriter/builtins/operations.txt
+-rw-rw-rw-   0        0        0      214 2023-07-07 17:00:52.000000 igorwriter-0.6.1/igorwriter/errors.py
+-rw-rw-rw-   0        0        0    23652 2024-03-03 13:53:49.000000 igorwriter-0.6.1/igorwriter/igorwave.py
+-rw-rw-rw-   0        0        0     1529 2023-07-07 16:02:45.000000 igorwriter-0.6.1/igorwriter/utils.py
+-rw-rw-rw-   0        0        0     3155 2024-01-28 05:48:47.000000 igorwriter-0.6.1/igorwriter/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:57:48.816468 igorwriter-0.6.1/igorwriter.egg-info/
+-rw-rw-rw-   0        0        0     6281 2024-04-24 10:57:48.000000 igorwriter-0.6.1/igorwriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2024-04-24 10:57:48.000000 igorwriter-0.6.1/igorwriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:57:48.000000 igorwriter-0.6.1/igorwriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 10:57:48.000000 igorwriter-0.6.1/igorwriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-24 10:57:48.000000 igorwriter-0.6.1/igorwriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2024-04-24 10:57:48.817468 igorwriter-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2024-04-24 10:56:56.000000 igorwriter-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:57:48.815468 igorwriter-0.6.1/tests/
+-rw-rw-rw-   0        0        0     4245 2024-01-28 05:48:47.000000 igorwriter-0.6.1/tests/test_names.py
+-rw-rw-rw-   0        0        0     1102 2023-07-07 16:02:45.000000 igorwriter-0.6.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0    20194 2024-03-03 13:53:49.000000 igorwriter-0.6.1/tests/test_wave.py
```

### Comparing `igorwriter-0.6.0/LICENSE.txt` & `igorwriter-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.6.0/PKG-INFO` & `igorwriter-0.6.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,208 @@
 Metadata-Version: 2.1
 Name: igorwriter
-Version: 0.6.0
+Version: 0.6.1
 Summary: Write IGOR binary (.ibw) or text (.itx) files from numpy array
 Home-page: https://github.com/t-onoz/igorwriter
 Author: t-onoz
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 
-IgorWriter
-==========
+# IgorWriter
 
 Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
 
-Features
---------
-* Compatible with multi-dimensional arrays (up to 4 dimensions)
-* Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
-* Data units (:code:`IgorWave.set_datascale`)
-* Dimension scaling (:code:`IgorWave.set_dimscale`)
-* Dimension labels (:code:`IgorWave.set_dimlabel`)
-* Wave notes (:code:`IgorWave.set_note`)
-* Dependency formula (:code:`IgorWave.set_formula`)
-
-Installation
-------------
-.. code-block:: doscon
+## Features
 
-    $ pip install igorwriter
+-   Compatible with multi-dimensional arrays (up to 4 dimensions)
+-   Supported `numpy` data types: uint, int, float, complex, bool, str,
+    bytes, datetime64
+-   Data units (`IgorWave.set_datascale`)
+-   Dimension scaling (`IgorWave.set_dimscale`)
+-   Dimension labels (`IgorWave.set_dimlabel`)
+-   Wave notes (`IgorWave.set_note`)
+-   Dependency formula (`IgorWave.set_formula`)
+
+## Installation
+
+``` doscon
+$ pip install igorwriter
+```
 
-Usage
------
+## Usage
 
 Basic usage
 
->>> import numpy as np
->>> from igorwriter import IgorWave
->>> array = np.array([1,2,3,4,5,6])
->>> # make IgorWave objects
->>> wave = IgorWave(array, name='mywave')
->>> wave2 = IgorWave(array.astype(np.float32), name='mywave2')
->>> # save data
->>> wave.save('mywave.ibw')
->>> wave.save_itx('mywave.itx')
->>> with open('multi_waves.itx', 'w') as fp:
->>>     # Igor Text files can contain multiples waves per file
->>>     wave.save_itx(fp)
->>>     wave2.save_itx(fp)
+```python
+import numpy as np 
+from igorwriter import IgorWave 
+
+array = np.array([1,2,3,4,5,6]) 
+
+# make IgorWave objects 
+wave = IgorWave(array, name='mywave') 
+wave2 = IgorWave(array.astype(np.float32), name='mywave2') 
+
+# save data
+wave.save('mywave.ibw') 
+wave.save_itx('mywave.itx')
+
+with open('multi_waves.itx', 'w') as fp: 
+    # Igor Text files can contain multiples waves per file 
+    wave.save_itx(fp)
+    wave2.save_itx(fp)
+```
 
 Data units, dimension scaling
 
->>> wave.set_datascale('DataUnit')
->>> wave.set_dimscale('x', 0, 0.01, 's')
+```python
+wave.set_datascale('DataUnit') 
+wave.set_dimscale('x', 0, 0.01, 's')
+```
 
 A two-dimensional array with dimension labels
 
->>> a2 = np.random.random((10, 3))
->>> wave = IgorWave(a2, name='wave2d')
->>> # you may set optional dimension labels
->>> wave.set_dimlabel(0, -1, 'points') # label for entire rows
->>> wave.set_dimlabel(1, -1, 'values') # label for entire columns
->>> wave.set_dimlabel(1, 0, 'ValueA')  # label for column 0
->>> wave.set_dimlabel(1, 1, 'ValueB')  # label for column 1
->>> wave.set_dimlabel(1, 2, 'ValueC')  # label for column 2
->>> wave.save('my2dwave.ibw')
+```python
+a2 = np.random.random((10, 3)) 
+wave = IgorWave(a2, name='wave2d') 
+
+# you may set optional dimension labels 
+wave.set_dimlabel(0, -1, 'points') # label for entire rows 
+wave.set_dimlabel(1, -1, 'values') # label for entire columns 
+wave.set_dimlabel(1, 0, 'ValueA') # label for column 0 
+wave.set_dimlabel(1, 1, 'ValueB') # label for column 1 
+wave.set_dimlabel(1, 2, 'ValueC') # label for column 2 
+wave.save('my2dwave.ibw')
+```
 
 You can append arbitrary Igor commands to Igor Text files.
 
->>> wave = IgorWave([1, 4, 9], name='wave0')
->>> with open('wave0.itx', 'w') as fp:
->>>     wave.save_itx(fp)
->>>     fp.write("X Display 'wave0'\n")
-
-Unicode support
----------------
-From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding.
-If you use Igor Pro 6 or older and want to use non-ascii characters, set :code:`unicode=False` when calling :code:`IgorWave()`.
-It will fall back to system text encoding (Windows-1252, Shift JIS, etc.).
-
-Wave Names
-----------
-There are restrictions on object names in IGOR. From v0.2.0, this package deals with illegal object names.
-
->>> wave = IgorWave(array, name='wave:0', on_errors='fix')  # fix illegal names automatically
-RenameWarning: name 'wave:0' is fixed as 'wave_0' (reason: name must not contain " ' : ; or any control characters.)
->>> wave.name
-'wave_0'
->>> wave = IgorWave(array, name='wave:0', on_errors='raise')  # raise errors
-Traceback (most recent call last):
-...
-InvalidNameError: name must not contain " ' : ; or any control characters.
-
-
-Pint integration
-----------------
-If `Pint <https://github.com/hgrecco/pint>`_ Quantity objects are passed to IgorWave, data units will be set automatically.
-
->>> import pint
->>> ureg = pint.UnitRegistry()
->>> w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
->>> w.save_itx('wave_with_units.itx')
-...
-X SetScale d,0,0,"m / s",'wave_with_units'
-X SetScale /P x,0.0,1.0,"",'wave_with_units'
+```python
+wave = IgorWave([1, 4, 9], name='wave0') 
+with open('wave0.itx', 'w') as fp: 
+    wave.save_itx(fp) 
 
+fp.write("X Display 'wave0'\n")
+```
 
+## Unicode support
+
+From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding. If you
+use Igor Pro 6 or older and want to use non-ascii characters, set
+`unicode=False` when calling `IgorWave()`. It will fall back to system
+text encoding (Windows-1252, Shift JIS, etc.).
+
+## Wave Names
+
+There are restrictions on object names in IGOR. From v0.2.0, this
+package deals with illegal object names.
+
+```python
+# This will issue a RenameWarning, and the name will be automatically changed.
+wave = IgorWave(array, name='wave:0', on_errors='fix')
+print(wave.name)  # wave_0
+
+# This will raise an InvalidNameError.
+wave = IgorWave(array, name='wave:0', on_errors='raise')
+```
+
+## Pint integration
+
+If [Pint](https://github.com/hgrecco/pint) Quantity objects are passed
+to IgorWave, data units will be set automatically.
+
+```python
+import pint 
+ureg = pint.UnitRegistry() 
+w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
+
+w.save_itx('wave_with_units.itx')
+print(open('wave_with_units.itx', 'r').read())
+# ...
+# X SetScale d,0,0,"m / s",'wave_with_units' 
+# X SetScale /P x,0.0,1.0,"",'wave_with_units'
+```
+
+## Pandas integration
 
-Pandas integration
-------------------
 You can easily export DataFrame objects with convenience functions.
 
->>> from igorwriter import utils
->>> utils.dataframe_to_itx(df, 'df.itx')   # all Series are exported in one file
->>> waves = utils.dataframe_to_ibw(df, prefix='df_bin')   # each Series is saved in a separate file, <prefix>_<column>.ibw
->>> waves  # dictionary of generated IgorWaves. You can change wave names, set data units, set dimension scaling, etc.
-{'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
+```python
+from igorwriter import utils 
+utils.dataframe_to_itx(df, 'df.itx') # all Series are exported in one file 
+waves = utils.dataframe_to_ibw(df, prefix='df_bin') # each Series is saved in a separate file, <prefix>_<column>.ibw 
+print(waves) # dictionary of generated IgorWaves
+# {'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
+```
+
+IgorWriter tries to convert index info on `pandas.Series` objects in following manners.
+
+-   If the index is evenly-spaced, wave dimension scaling is set
+    accordingly.
+-   Index names are interpreted as the dimension labels.
+
+## Notes on Image Plots
+
+Image Plot in IGOR and `imshow` in matplotlib use different convention
+for x and y axes:
+
+-   Rows as x, columns as y (IGOR)
+-   Columns as x, rows as y (Matplotlib)
 
-IgorWriter tries to convert index info on pandas.Series objects.
+Thus, `image` parameter was introduced in `save()` and `save_itx()`
+methods. If you use e.g.
 
-* If the index is evenly-spaced, wave dimension scaling is set accordingly.
-* Index names are interpreted as the dimension labels.
 
-Notes on Image Plots
---------------------
-Image Plot in IGOR and :code:`imshow` in matplotlib use different convention for x and y axes:
+wave.save('path.ibw', image=True)
 
-- Rows as x, columns as y (IGOR)
-- Columns as x, rows as y (Matplotlib)
+`plt.imshow` and Image Plot will give the same results.
 
-Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods.
-If you use e.g. 
+The `image=True` option transposes rows and columns of the underlying
+array, but does not swap data units, dimension scaling, etc. (You need to
+change them manually).
 
->>> wave.save('path.ibw', image=True)
-    
-:code:`plt.imshow` and Image Plot will give the same results.
+# Changelog
 
+## v0.6.0 (2024-01-13)
 
-Changelog
-=========
+-   Wave note support
+-   Dependency formula support
 
-v0.6.0 (2024-01-13)
--------------------
-- Wave note support
-- Dependency formula support
+## v0.5.0 (2023-07-08)
 
-v0.5.0 (2023-07-08)
--------------------
-- UTF-8 as default encoding. You can instead use system text encoding by setting :code:`unicode=False` to IgorWave().
-- Automatic conversion from pandas index to dimension scaling.
-- Exporting 64-bit integer waves (requires Igor Pro 7 or later).
-- BUG FIX: Igor Text files created from np.bool\_ arrays were broken.
+-   UTF-8 as default encoding. You can instead use system text encoding
+    by setting `unicode=False` to IgorWave().
+-   Automatic conversion from pandas index to dimension scaling.
+-   Exporting 64-bit integer waves (requires Igor Pro 7 or later).
+-   BUG FIX: Igor Text files created from `np.bool_` arrays were broken.
 
+## v0.4.1 (2023-07-02)
 
-v0.4.1 (2023-07-02)
--------------------
-- Added support for np.str\_, np.bytes\_ arrays.
-- Automatic type conversion for np.object\_ arrays.
-- Added support for dimension scaling (:code:`IgorWave.set_simlabel`).
+-   Added support for `np.str_` and `np.bytes_` arrays.
+-   Automatic type conversion for `np.object_` arrays.
+-   Added support for dimension scaling (`IgorWave.set_simlabel`).
 
+## v0.3.0 (2019-11-16)
 
-v0.3.0 (2019-11-16)
--------------------
-- Added :code:`utils.dict_to_{ibw, itx}` 
-- Set datascale automatically for pint Quantity object.
-- Added support for np.datetime64 array.
+-   Added `utils.dict_to_{ibw, itx}`
+-   Set datascale automatically for pint Quantity object.
+-   Added support for np.datetime64 array.
 
+## v0.2.3 (2019-11-09)
 
-v0.2.3 (2019-11-09)
--------------------
-- Added support for 64-bit integers (by automatically casting onto 32-bit integers on save). 
+-   Added support for 64-bit integers (by automatically casting onto
+    32-bit integers on save).
 
+## v0.2.0 (2019-11-08)
 
-v0.2.0 (2019-11-08)
--------------------
-- Added utilities for pandas (:code:`utils.dataframe_to_{ibw, itx}` ).
-- Added unittest scripts. 
-- Added wave name validator. 
-- BUG FIX: long (> 3 bytes) units for dimension scaling were ignored in
-  save_itx() 
-- IgorWriter now uses system locale encoding rather than ASCII (the default behavior of
-  IGOR Pro prior to ver. 7.00) 
+-   Added utilities for pandas (`utils.dataframe_to_{ibw, itx}` ).
+-   Added unittest scripts.
+-   Added wave name validator.
+-   BUG FIX: long (\> 3 bytes) units for dimension scaling were ignored
+    in save_itx()
+-   IgorWriter now uses system locale encoding rather than ASCII (the
+    default behavior of IGOR Pro prior to ver. 7.00)
```

### Comparing `igorwriter-0.6.0/README.rst` & `igorwriter-0.6.1/igorwriter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,172 +1,208 @@
-IgorWriter
-==========
-
-Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
-
-Features
---------
-* Compatible with multi-dimensional arrays (up to 4 dimensions)
-* Supported :code:`numpy` data types: uint, int, float, complex, bool, str, bytes, datetime64
-* Data units (:code:`IgorWave.set_datascale`)
-* Dimension scaling (:code:`IgorWave.set_dimscale`)
-* Dimension labels (:code:`IgorWave.set_dimlabel`)
-* Wave notes (:code:`IgorWave.set_note`)
-* Dependency formula (:code:`IgorWave.set_formula`)
-
-Installation
-------------
-.. code-block:: doscon
-
-    $ pip install igorwriter
-
-Usage
------
-
-Basic usage
-
->>> import numpy as np
->>> from igorwriter import IgorWave
->>> array = np.array([1,2,3,4,5,6])
->>> # make IgorWave objects
->>> wave = IgorWave(array, name='mywave')
->>> wave2 = IgorWave(array.astype(np.float32), name='mywave2')
->>> # save data
->>> wave.save('mywave.ibw')
->>> wave.save_itx('mywave.itx')
->>> with open('multi_waves.itx', 'w') as fp:
->>>     # Igor Text files can contain multiples waves per file
->>>     wave.save_itx(fp)
->>>     wave2.save_itx(fp)
-
-Data units, dimension scaling
-
->>> wave.set_datascale('DataUnit')
->>> wave.set_dimscale('x', 0, 0.01, 's')
-
-A two-dimensional array with dimension labels
-
->>> a2 = np.random.random((10, 3))
->>> wave = IgorWave(a2, name='wave2d')
->>> # you may set optional dimension labels
->>> wave.set_dimlabel(0, -1, 'points') # label for entire rows
->>> wave.set_dimlabel(1, -1, 'values') # label for entire columns
->>> wave.set_dimlabel(1, 0, 'ValueA')  # label for column 0
->>> wave.set_dimlabel(1, 1, 'ValueB')  # label for column 1
->>> wave.set_dimlabel(1, 2, 'ValueC')  # label for column 2
->>> wave.save('my2dwave.ibw')
-
-You can append arbitrary Igor commands to Igor Text files.
-
->>> wave = IgorWave([1, 4, 9], name='wave0')
->>> with open('wave0.itx', 'w') as fp:
->>>     wave.save_itx(fp)
->>>     fp.write("X Display 'wave0'\n")
-
-Unicode support
----------------
-From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding.
-If you use Igor Pro 6 or older and want to use non-ascii characters, set :code:`unicode=False` when calling :code:`IgorWave()`.
-It will fall back to system text encoding (Windows-1252, Shift JIS, etc.).
-
-Wave Names
-----------
-There are restrictions on object names in IGOR. From v0.2.0, this package deals with illegal object names.
-
->>> wave = IgorWave(array, name='wave:0', on_errors='fix')  # fix illegal names automatically
-RenameWarning: name 'wave:0' is fixed as 'wave_0' (reason: name must not contain " ' : ; or any control characters.)
->>> wave.name
-'wave_0'
->>> wave = IgorWave(array, name='wave:0', on_errors='raise')  # raise errors
-Traceback (most recent call last):
-...
-InvalidNameError: name must not contain " ' : ; or any control characters.
-
-
-Pint integration
-----------------
-If `Pint <https://github.com/hgrecco/pint>`_ Quantity objects are passed to IgorWave, data units will be set automatically.
-
->>> import pint
->>> ureg = pint.UnitRegistry()
->>> w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
->>> w.save_itx('wave_with_units.itx')
-...
-X SetScale d,0,0,"m / s",'wave_with_units'
-X SetScale /P x,0.0,1.0,"",'wave_with_units'
-
-
-
-Pandas integration
-------------------
-You can easily export DataFrame objects with convenience functions.
-
->>> from igorwriter import utils
->>> utils.dataframe_to_itx(df, 'df.itx')   # all Series are exported in one file
->>> waves = utils.dataframe_to_ibw(df, prefix='df_bin')   # each Series is saved in a separate file, <prefix>_<column>.ibw
->>> waves  # dictionary of generated IgorWaves. You can change wave names, set data units, set dimension scaling, etc.
-{'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
-
-IgorWriter tries to convert index info on pandas.Series objects.
-
-* If the index is evenly-spaced, wave dimension scaling is set accordingly.
-* Index names are interpreted as the dimension labels.
-
-Notes on Image Plots
---------------------
-Image Plot in IGOR and :code:`imshow` in matplotlib use different convention for x and y axes:
-
-- Rows as x, columns as y (IGOR)
-- Columns as x, rows as y (Matplotlib)
-
-Thus, :code:`image` parameter was introduced in :code:`save()` and :code:`save_itx()` methods.
-If you use e.g. 
-
->>> wave.save('path.ibw', image=True)
-    
-:code:`plt.imshow` and Image Plot will give the same results.
-
-
-Changelog
-=========
-
-v0.6.0 (2024-01-13)
--------------------
-- Wave note support
-- Dependency formula support
-
-v0.5.0 (2023-07-08)
--------------------
-- UTF-8 as default encoding. You can instead use system text encoding by setting :code:`unicode=False` to IgorWave().
-- Automatic conversion from pandas index to dimension scaling.
-- Exporting 64-bit integer waves (requires Igor Pro 7 or later).
-- BUG FIX: Igor Text files created from np.bool\_ arrays were broken.
-
-
-v0.4.1 (2023-07-02)
--------------------
-- Added support for np.str\_, np.bytes\_ arrays.
-- Automatic type conversion for np.object\_ arrays.
-- Added support for dimension scaling (:code:`IgorWave.set_simlabel`).
-
-
-v0.3.0 (2019-11-16)
--------------------
-- Added :code:`utils.dict_to_{ibw, itx}` 
-- Set datascale automatically for pint Quantity object.
-- Added support for np.datetime64 array.
-
-
-v0.2.3 (2019-11-09)
--------------------
-- Added support for 64-bit integers (by automatically casting onto 32-bit integers on save). 
-
-
-v0.2.0 (2019-11-08)
--------------------
-- Added utilities for pandas (:code:`utils.dataframe_to_{ibw, itx}` ).
-- Added unittest scripts. 
-- Added wave name validator. 
-- BUG FIX: long (> 3 bytes) units for dimension scaling were ignored in
-  save_itx() 
-- IgorWriter now uses system locale encoding rather than ASCII (the default behavior of
-  IGOR Pro prior to ver. 7.00) 
+Metadata-Version: 2.1
+Name: igorwriter
+Version: 0.6.1
+Summary: Write IGOR binary (.ibw) or text (.itx) files from numpy array
+Home-page: https://github.com/t-onoz/igorwriter
+Author: t-onoz
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+
+# IgorWriter
+
+Write Igor Binary Wave (.ibw) or Igor Text (.itx) files from numpy array
+
+## Features
+
+-   Compatible with multi-dimensional arrays (up to 4 dimensions)
+-   Supported `numpy` data types: uint, int, float, complex, bool, str,
+    bytes, datetime64
+-   Data units (`IgorWave.set_datascale`)
+-   Dimension scaling (`IgorWave.set_dimscale`)
+-   Dimension labels (`IgorWave.set_dimlabel`)
+-   Wave notes (`IgorWave.set_note`)
+-   Dependency formula (`IgorWave.set_formula`)
+
+## Installation
+
+``` doscon
+$ pip install igorwriter
+```
+
+## Usage
+
+Basic usage
+
+```python
+import numpy as np 
+from igorwriter import IgorWave 
+
+array = np.array([1,2,3,4,5,6]) 
+
+# make IgorWave objects 
+wave = IgorWave(array, name='mywave') 
+wave2 = IgorWave(array.astype(np.float32), name='mywave2') 
+
+# save data
+wave.save('mywave.ibw') 
+wave.save_itx('mywave.itx')
+
+with open('multi_waves.itx', 'w') as fp: 
+    # Igor Text files can contain multiples waves per file 
+    wave.save_itx(fp)
+    wave2.save_itx(fp)
+```
+
+Data units, dimension scaling
+
+```python
+wave.set_datascale('DataUnit') 
+wave.set_dimscale('x', 0, 0.01, 's')
+```
+
+A two-dimensional array with dimension labels
+
+```python
+a2 = np.random.random((10, 3)) 
+wave = IgorWave(a2, name='wave2d') 
+
+# you may set optional dimension labels 
+wave.set_dimlabel(0, -1, 'points') # label for entire rows 
+wave.set_dimlabel(1, -1, 'values') # label for entire columns 
+wave.set_dimlabel(1, 0, 'ValueA') # label for column 0 
+wave.set_dimlabel(1, 1, 'ValueB') # label for column 1 
+wave.set_dimlabel(1, 2, 'ValueC') # label for column 2 
+wave.save('my2dwave.ibw')
+```
+
+You can append arbitrary Igor commands to Igor Text files.
+
+```python
+wave = IgorWave([1, 4, 9], name='wave0') 
+with open('wave0.itx', 'w') as fp: 
+    wave.save_itx(fp) 
+
+fp.write("X Display 'wave0'\n")
+```
+
+## Unicode support
+
+From igorwriter 0.5.0, IgorWave stores texts with utf-8 encoding. If you
+use Igor Pro 6 or older and want to use non-ascii characters, set
+`unicode=False` when calling `IgorWave()`. It will fall back to system
+text encoding (Windows-1252, Shift JIS, etc.).
+
+## Wave Names
+
+There are restrictions on object names in IGOR. From v0.2.0, this
+package deals with illegal object names.
+
+```python
+# This will issue a RenameWarning, and the name will be automatically changed.
+wave = IgorWave(array, name='wave:0', on_errors='fix')
+print(wave.name)  # wave_0
+
+# This will raise an InvalidNameError.
+wave = IgorWave(array, name='wave:0', on_errors='raise')
+```
+
+## Pint integration
+
+If [Pint](https://github.com/hgrecco/pint) Quantity objects are passed
+to IgorWave, data units will be set automatically.
+
+```python
+import pint 
+ureg = pint.UnitRegistry() 
+w = IgorWave([3, 4] * ureg.meter / ureg.second, name='wave_with_units')
+
+w.save_itx('wave_with_units.itx')
+print(open('wave_with_units.itx', 'r').read())
+# ...
+# X SetScale d,0,0,"m / s",'wave_with_units' 
+# X SetScale /P x,0.0,1.0,"",'wave_with_units'
+```
+
+## Pandas integration
+
+You can easily export DataFrame objects with convenience functions.
+
+```python
+from igorwriter import utils 
+utils.dataframe_to_itx(df, 'df.itx') # all Series are exported in one file 
+waves = utils.dataframe_to_ibw(df, prefix='df_bin') # each Series is saved in a separate file, <prefix>_<column>.ibw 
+print(waves) # dictionary of generated IgorWaves
+# {'col1': <IgorWave 'col1' at 0x...>, 'col2': ...}
+```
+
+IgorWriter tries to convert index info on `pandas.Series` objects in following manners.
+
+-   If the index is evenly-spaced, wave dimension scaling is set
+    accordingly.
+-   Index names are interpreted as the dimension labels.
+
+## Notes on Image Plots
+
+Image Plot in IGOR and `imshow` in matplotlib use different convention
+for x and y axes:
+
+-   Rows as x, columns as y (IGOR)
+-   Columns as x, rows as y (Matplotlib)
+
+Thus, `image` parameter was introduced in `save()` and `save_itx()`
+methods. If you use e.g.
+
+
+wave.save('path.ibw', image=True)
+
+`plt.imshow` and Image Plot will give the same results.
+
+The `image=True` option transposes rows and columns of the underlying
+array, but does not swap data units, dimension scaling, etc. (You need to
+change them manually).
+
+# Changelog
+
+## v0.6.0 (2024-01-13)
+
+-   Wave note support
+-   Dependency formula support
+
+## v0.5.0 (2023-07-08)
+
+-   UTF-8 as default encoding. You can instead use system text encoding
+    by setting `unicode=False` to IgorWave().
+-   Automatic conversion from pandas index to dimension scaling.
+-   Exporting 64-bit integer waves (requires Igor Pro 7 or later).
+-   BUG FIX: Igor Text files created from `np.bool_` arrays were broken.
+
+## v0.4.1 (2023-07-02)
+
+-   Added support for `np.str_` and `np.bytes_` arrays.
+-   Automatic type conversion for `np.object_` arrays.
+-   Added support for dimension scaling (`IgorWave.set_simlabel`).
+
+## v0.3.0 (2019-11-16)
+
+-   Added `utils.dict_to_{ibw, itx}`
+-   Set datascale automatically for pint Quantity object.
+-   Added support for np.datetime64 array.
+
+## v0.2.3 (2019-11-09)
+
+-   Added support for 64-bit integers (by automatically casting onto
+    32-bit integers on save).
+
+## v0.2.0 (2019-11-08)
+
+-   Added utilities for pandas (`utils.dataframe_to_{ibw, itx}` ).
+-   Added unittest scripts.
+-   Added wave name validator.
+-   BUG FIX: long (\> 3 bytes) units for dimension scaling were ignored
+    in save_itx()
+-   IgorWriter now uses system locale encoding rather than ASCII (the
+    default behavior of IGOR Pro prior to ver. 7.00)
```

### Comparing `igorwriter-0.6.0/igorwriter/builtins/functions.txt` & `igorwriter-0.6.1/igorwriter/builtins/functions.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.6.0/igorwriter/builtins/operations.txt` & `igorwriter-0.6.1/igorwriter/builtins/operations.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.6.0/igorwriter/igorwave.py` & `igorwriter-0.6.1/igorwriter/igorwave.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         ('private', ctypes.c_byte * 28),
 
         # ('wData', ctypes.c_float * 1),  # The start of the array of data. Must be 64 bit aligned.
     ]
 
     def __init__(self):
         super(WaveHeader5, self).__init__()
-        self.sfA = (1,) * MAXDIMS
+        self.sfA[:] = (1,) * MAXDIMS
         self.whVersion = 1
 
 
 class IgorWave5(object):
     def __init__(self, array, name='wave0', on_errors='fix', unicode=True, int64_support=False):
         """
 
@@ -161,18 +161,18 @@
             self._wave_header.textWaveContentEncoding = 1
             self._encoding = 'utf-8'
         else:
             self._encoding = _getpreferredencoding()
         self._int64_support = int64_support
         self.rename(name, on_errors)
         self._note = b''
-        self._formula_with_trailing_null = b''
+        self._formula = b''
         self._extended_data_units = b''
         self._extended_dimension_units = [b'', b'', b'', b'']
-        self._dimension_labels = [dict(), dict(), dict(), dict()]
+        self._dimension_labels = (dict(), dict(), dict(), dict())
 
         if isinstance(array, Series):
             self.array = self._parse_Series(array)
         elif isinstance(array, Quantity):
             self.array = self._parse_Pint(array)
         else:
             self.array = np.asarray(array)
@@ -234,35 +234,24 @@
             self._extended_data_units = bunits
 
     def set_dimlabel(self, dimNumber: int, dimIndex: int, label: str):
         """Set dimension labels.
 
         :param dimNumber: 0 (rows), 1 (columns), 2 (layers), or 3 (chunks)
         :param dimIndex: if -1, sets the label for the entire dimension, if >= 0, sets the label for that element of the dimension.
-        :param label: label string (up to 31 characters)
+        :param label: label string (up to 31 characters). Clears the label if empty ('').
         """
         if dimNumber not in [0, 1, 2, 3]:
             raise ValueError('dimNumber must be 0, 1, 2, or 3.')
 
-        # Dimension labels cannot contain illegal characters (", ', :, ; and control characters),
-        # but they can conflict with built-in names.
-        for s in validator.NG_LETTERS:
-            if s in label:
-                raise igorwriter.errors.InvalidNameError(
-                    'thelabel contains illegal characters (", \', :, ;, and control characters)'
-                )
-        blabel = label.encode(self._encoding)
-        if len(blabel) > 31:
-            raise ValueError('Dimension labels cannot be longer than 31 bytes.')
-
-        if label == '':
-            # if label is empty, remove the label.
-            self._dimension_labels[dimNumber].pop(dimIndex, None)
+        if label:
+            blabel = validator.check_and_encode(label, liberal=True, long=False, allow_builtins=True)
+            self._dimension_labels[dimNumber][dimIndex] = blabel + b'\x00' * (32 - len(blabel))
         else:
-            self._dimension_labels[dimNumber][dimIndex] = blabel
+            self._dimension_labels[dimNumber].pop(dimIndex, None)
 
         # calculate new dimLabelsSize
         if self._dimension_labels[dimNumber]:
             # Each dimension has max(dimIndex) + 2 (-1, 0, .. max(dimIndex)) labels, and each of them contains 32 bytes
             dimLabelsSize = 32 * (max(self._dimension_labels[dimNumber]) + 2)
         else:
             dimLabelsSize = 0
@@ -276,18 +265,17 @@
         self._note = note.encode(self._encoding)
         self._bin_header.noteSize = len(self._note)
 
     def set_formula(self, formula):
         """set wave dependency formula.
 
         :param formula: a string that represents the dependency formula. Clears the formula if empty (formula='')."""
-        self._formula_with_trailing_null = formula.encode(self._encoding)
-        if self._formula_with_trailing_null:
-            self._formula_with_trailing_null += b'\x00'
-        self._bin_header.formulaSize = len(self._formula_with_trailing_null)
+        bformula = formula.encode(self._encoding) + b'\x00' if formula else b''
+        self._formula = bformula
+        self._bin_header.formulaSize = len(bformula)
 
     set_wavenote = set_note
 
     def save(self, file, image=False):
         """save data as igor binary wave (.ibw) format.
 
         :param file: file name or binary-file object.
@@ -326,30 +314,29 @@
             # wave data
             if TYPES[a.dtype.type] == 0:  # text waves
                 fp.write(b''.join(a.ravel(order='F')))
             else:
                 fp.write(a.tobytes(order='F'))
 
             # dependency formula
-            fp.write(self._formula_with_trailing_null)
+            fp.write(self._formula)
 
             # wave note
             fp.write(self._note)
 
             # extended data units, dimension units
             fp.write(self._extended_data_units)
             for u in self._extended_dimension_units:
                 fp.write(u)
 
             # dimension labels
             for dimlabeldict in self._dimension_labels:
                 if dimlabeldict:
                     for i in range(-1, max(dimlabeldict)+1):
-                        b = dimlabeldict.get(i, b'\x00')
-                        b += b'\x00' * (32-len(b))
+                        b = dimlabeldict.get(i, b'\x00'*32)
                         assert len(b) == 32
                         fp.write(b)
 
             # string indices if this is a text wave.
             if TYPES[a.dtype.type] == 0:
                 sindices = np.zeros(a.size, dtype=np.int32)
                 pos = 0
@@ -403,20 +390,20 @@
                 start = self._wave_header.sfB[idx]
                 delta = self._wave_header.sfA[idx]
                 fp.write(f'X SetScale /P {dim},{start},{delta},"{dimUnits}",\'{name}\'\n')
 
             # dimension labels
             for dimNumber, dimlabeldict in enumerate(self._dimension_labels):
                 for dimIndex, blabel in dimlabeldict.items():
-                    label = blabel.decode(self._encoding)
+                    label = blabel.rstrip(b'\x00').decode(self._encoding)
                     fp.write(f'X SetDimLabel {dimNumber},{dimIndex},\'{label}\',\'{name}\'\n')
 
             # dependency formula
-            if self._formula_with_trailing_null:
-                formula = self._formula_with_trailing_null[:-1].decode(self._encoding)
+            if self._formula:
+                formula = self._formula.rstrip(b'\x00').decode(self._encoding)
                 fp.write(f'X SetFormula \'{name}\', "{formula}"\n')
 
             # wave note
             if self._note:
                 note = self._escape_specials(self._note.decode(self._encoding))
                 fp.write(f'X Note \'{name}\', "{note}"\n')
         finally:
```

### Comparing `igorwriter-0.6.0/igorwriter/utils.py` & `igorwriter-0.6.1/igorwriter/utils.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.6.0/igorwriter/validator.py` & `igorwriter-0.6.1/igorwriter/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,20 +49,21 @@
 
 def _fix_conflicts(name):
     if name.lower() in (builtin_names.operations + builtin_names.functions + builtin_names.keywords + builtin_names.variables):
         name = name + '_'
     return name, 'name must not conflict with built-in operations, functions, etc.'
 
 
-def check_and_encode(name, liberal=True, long=False, on_errors='raise', encoding=None):
+def check_and_encode(name, liberal=True, long=False, allow_builtins=False,  on_errors='raise', encoding=None):
     """
 
     :param name: name of an object
     :param liberal: whether Liberal Object Names are allowed or not
     :param long: whether Long Object Names (introduced in Igor 8.00) are allowed or not
+    :param allow_builtins: whether conflicts with builtin names are allowed or not
     :param on_errors: If 'raise', raises InvalidNameError when name is invalid, otherwise tries to fix errors.
     :param encoding: text encoding. If None, it is set with getpreferredencoding()
     :return:
     """
     if encoding is None:
         encoding = _getpreferredencoding()
     MAX_BYTES = 255 if long else 31
@@ -70,10 +71,11 @@
     name_after = None
     while name_before != name_after:
         name_before = name
         name = _fix_or_raise(_fix_length, on_errors=on_errors)(name_before, MAX_BYTES, encoding=encoding)
         name = _fix_or_raise(_fix_ng_letters, on_errors=on_errors)(name)
         if not liberal:
             name = _fix_or_raise(_fix_standard, on_errors=on_errors)(name)
-        name = _fix_or_raise(_fix_conflicts, on_errors=on_errors)(name)
+        if not allow_builtins:
+            name = _fix_or_raise(_fix_conflicts, on_errors=on_errors)(name)
         name_after = name
     return name.encode(encoding)
```

### Comparing `igorwriter-0.6.0/setup.py` & `igorwriter-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='igorwriter',
-    version='0.6.0',
+    version='0.6.1',
     description='Write IGOR binary (.ibw) or text (.itx) files from numpy array',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/t-onoz/igorwriter',
     author='t-onoz',
     license='MIT',
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
```

### Comparing `igorwriter-0.6.0/tests/test_names.py` & `igorwriter-0.6.1/tests/test_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,16 +68,17 @@
     def test_conflicts(self):
         names = (
             'append', 'APPEND',  # operations
             'abs', 'ABS',  # functions
             'do', 'DO',  # keywords
             'k1', 'K1',  # variables
         )
-        for name, liberal, long in product(names, (True, False), (True, False)):
-            self.assertRaises(igorwriter.errors.InvalidNameError, v.check_and_encode, name, liberal, long)
-            bname = v.check_and_encode(name, liberal, long, on_errors='fix')
-            desired = (name + '_').encode(encoding)
+        for name, liberal, long, allow_builtins in product(names, (True, False), (True, False), (True, False)):
+            if not allow_builtins:
+                self.assertRaises(igorwriter.errors.InvalidNameError, v.check_and_encode, name, liberal, long)
+            bname = v.check_and_encode(name, liberal, long, allow_builtins, on_errors='fix')
+            desired = name.encode(encoding) if allow_builtins else (name + '_').encode(encoding)
             self.assertEqual(bname, desired)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `igorwriter-0.6.0/tests/test_utils.py` & `igorwriter-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.6.0/tests/test_wave.py` & `igorwriter-0.6.1/tests/test_wave.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,17 @@
             fp.seek(0)
             content = fp.read()
             self.assertRegex(content, com)
 
     def test_dimscale(self):
         array = np.random.randint(0, 100, 10, dtype=np.int32)
         wave = IgorWave(array)
-        wave.set_dimscale('x', 0, 0.01, 's')
+        wave.set_dimscale('x', 1, 0.01, 's')
+        self.assertAlmostEqual(wave._wave_header.sfA[0], 0.01)
+        self.assertAlmostEqual(wave._wave_header.sfB[0], 1.0)
         with open(OUTDIR / 'dimscale.ibw', 'wb') as fp:
             wave.save(fp)
         with open(OUTDIR / 'dimscale.itx', 'w') as fp:
             wave.save_itx(fp)
 
     def test_data_units(self):
         wavename = 'wave0'
@@ -185,19 +187,23 @@
             self.assertIn(com, content)
 
     def test_formula(self):
         wavename = 'sinwave'
         formula = 'sin(x)'
         wave = IgorWave(np.zeros(101), name=wavename)
         wave.set_formula(formula)
+        self.assertEqual(wave._bin_header.formulaSize, len(formula)+1)
         wave.set_note('sine wave')
         wave.set_dimscale('x', 0, np.pi*2/100)
         com = 'X SetFormula \'sinwave\', "sin(x)"'
-        with open(OUTDIR / 'formula.ibw', 'wb') as fp:
+        with open(OUTDIR / 'formula.ibw', 'w+b') as fp:
             wave.save(fp)
+            fp.seek(0)
+            content = fp.read()
+            self.assertIn(b'sin(x)\x00sine wave', content)
         with open(OUTDIR / 'formula.itx', 'w+t') as fp:
             wave.save_itx(fp)
             fp.seek(0)
             content = fp.read()
             self.assertIn(com, content)
 
     def test_invalid_name(self):
@@ -223,15 +229,15 @@
     def test_dimlabel(self):
         a = np.random.random(size=(2, 3, 4, 5))
         wavename = 'dimlabeltest'
         with self.subTest('invalid dimlabel'):
             w = IgorWave(a, wavename)
             self.assertRaises(igorwriter.errors.InvalidNameError, w.set_dimlabel, 0, 0, "'")
             w.set_dimlabel(0, 0, "a"*31)
-            self.assertRaises(ValueError, w.set_dimlabel, 0, 0, "a"*32)
+            self.assertRaises(igorwriter.errors.InvalidNameError, w.set_dimlabel, 0, 0, "a"*32)
         with self.subTest('dimlabel for entire row'):
             label = 'rowname'
             w = IgorWave(a, wavename)
             w.set_dimlabel(0, -1, label)
             com = "X SetDimLabel 0,-1,'%s','%s'" % (label, wavename)
             with open(OUTDIR / 'dimlabel_row_entire.itx', 'w+t') as fp:
                 w.save_itx(fp)
@@ -324,16 +330,19 @@
             string = fp.read()
             self.assertTrue('\\t' in string)
             self.assertTrue('\\r' in string)
             self.assertTrue('\\n' in string)
             self.assertTrue('\\\'' in string)
             self.assertTrue('\\"' in string)
             self.assertTrue('\\\\' in string)
-        with open(OUTDIR / 'textwave_spchars.ibw', 'wb') as fp:
+        with open(OUTDIR / 'textwave_spchars.ibw', 'w+b') as fp:
             w.save(fp)
+            fp.seek(0)
+            content = fp.read()
+            self.assertIn(b''.join(e.encode(w._encoding) for e in a), content)
 
     def test_optional_data(self):
         # wave with a lot of optional data
         a = np.array([str(x)*np.random.randint(1, 10) for x in 'abcdefghijklmnop']).reshape((2, 2, 2, 2))
         w = IgorWave(a, 'optDataTest')
         w.set_dimscale('x', 0, 1, 'verylongdimunitX')
         w.set_dimscale('y', 0, 1, 'verylongdimunitY')
@@ -401,15 +410,15 @@
                     w = IgorWave(s)
                 self.assertAlmostEqual(w._wave_header.sfA[0], 0.2)
                 self.assertAlmostEqual(w._wave_header.sfB[0], 1.0)
                 self.assertNotIn(-1, w._dimension_labels[0])
         with self.subTest('Series object with uniform Index with a name'):
             s.index.name = 'myindex'
             w = IgorWave(s, 'series_uniformind')
-            self.assertEqual(w._dimension_labels[0][-1], b'myindex')
+            self.assertEqual(w._dimension_labels[0][-1].rstrip(b'\x00'), b'myindex')
         with self.subTest('Series object with nonuniform Index'):
             s = pd.Series([1, 2, 3])
             s.index = [1, 2, 3.05]
             s.index.name = 'myindex'
             with self.assertWarns(StrippedSeriesIndexWarning):
                 w = IgorWave(s, 'series_nonuniformind')
             # when index is invalid, dimension labels should be empty
```

