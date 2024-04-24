# Comparing `tmp/jplephem-2.8.tar.gz` & `tmp/jplephem-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jplephem-2.8.tar", last modified: Sun Jul 22 20:17:40 2018, max compression
+gzip compressed data, was "dist/jplephem-2.9.tar", last modified: Fri Jan  4 04:35:00 2019, max compression
```

## Comparing `jplephem-2.8.tar` & `jplephem-2.9.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-07-22 20:17:40.000000 jplephem-2.8/
--rw-r-----   0 brandon   (1000) brandon   (1000)    20203 2018-07-22 20:17:40.000000 jplephem-2.8/PKG-INFO
--rw-r-----   0 brandon   (1000) brandon   (1000)     1097 2018-07-22 20:14:40.000000 jplephem-2.8/setup.py
-drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2018-07-22 20:17:40.000000 jplephem-2.8/jplephem/
--rw-r-----   0 brandon   (1000) brandon   (1000)    15425 2016-11-14 22:04:21.000000 jplephem-2.8/jplephem/names.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     1578 2016-11-14 22:04:21.000000 jplephem-2.8/jplephem/ascii.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    10129 2018-07-22 20:13:01.000000 jplephem-2.8/jplephem/daf.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     2429 2018-02-11 18:47:55.000000 jplephem-2.8/jplephem/excerpter.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     7919 2018-02-11 18:12:45.000000 jplephem-2.8/jplephem/spk.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     7987 2018-02-03 20:10:31.000000 jplephem-2.8/jplephem/ephem.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3389 2018-02-11 18:31:21.000000 jplephem-2.8/jplephem/commandline.py
--rw-r-----   0 brandon   (1000) brandon   (1000)     3812 2016-11-14 22:04:21.000000 jplephem-2.8/jplephem/jpltest.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    16398 2018-07-22 20:16:31.000000 jplephem-2.8/jplephem/__init__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)       90 2018-02-11 17:05:05.000000 jplephem-2.8/jplephem/__main__.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    15965 2018-02-11 16:59:37.000000 jplephem-2.8/jplephem/test.py
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2019-01-04 04:35:00.000000 jplephem-2.9/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1084 2019-01-04 03:57:52.000000 jplephem-2.9/LICENSE.txt
+-rw-r-----   0 brandon   (1000) brandon   (1000)    20634 2019-01-04 04:35:00.000000 jplephem-2.9/PKG-INFO
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1092 2018-02-03 17:27:37.000000 jplephem-2.9/README.md
+drwxr-x---   0 brandon   (1000) brandon   (1000)        0 2019-01-04 04:35:00.000000 jplephem-2.9/jplephem/
+-rw-r-----   0 brandon   (1000) brandon   (1000)    16749 2019-01-04 04:34:01.000000 jplephem-2.9/jplephem/__init__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)       90 2018-02-11 17:05:05.000000 jplephem-2.9/jplephem/__main__.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1578 2016-11-14 22:04:21.000000 jplephem-2.9/jplephem/ascii.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     6611 2018-10-01 12:53:48.000000 jplephem-2.9/jplephem/binary_pck.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3389 2018-02-11 18:31:21.000000 jplephem-2.9/jplephem/commandline.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    10129 2018-07-22 20:13:01.000000 jplephem-2.9/jplephem/daf.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     7987 2018-02-03 20:10:31.000000 jplephem-2.9/jplephem/ephem.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     2429 2018-02-11 18:47:55.000000 jplephem-2.9/jplephem/excerpter.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     3812 2016-11-14 22:04:21.000000 jplephem-2.9/jplephem/jpltest.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    15425 2016-11-14 22:04:21.000000 jplephem-2.9/jplephem/names.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8199 2019-01-04 04:15:39.000000 jplephem-2.9/jplephem/spk.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)    16172 2019-01-04 04:21:07.000000 jplephem-2.9/jplephem/test.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)     1097 2019-01-04 04:32:27.000000 jplephem-2.9/setup.py
```

### Comparing `jplephem-2.8/PKG-INFO` & `jplephem-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jplephem
-Version: 2.8
+Version: 2.9
 Summary: Use a JPL ephemeris to predict planet positions.
 Home-page: UNKNOWN
 Author: Brandon Rhodes
 Author-email: brandon@rhodesmill.org
 License: MIT
 Description: 
         This package can load and use a Jet Propulsion Laboratory (JPL)
@@ -196,14 +196,21 @@
            |  segment.target - integer target identifier
            |  segment.frame - integer frame identifier
            |  segment.data_type - integer data type identifier
            |  segment.start_i - index where segment starts
            |  segment.end_i - index where segment ends
           ...
         
+        * If you want to access the raw coefficients, use the segment
+          ``load_array()`` method.  It returns two floats and a NumPy array:
+        
+          >>> initial_epoch, interval_length, coefficients = segment.load_array()
+          >>> print(coefficients.shape)
+          (3, 100448, 13)
+        
         * The square-bracket lookup mechanism ``kernel[3,399]`` is a
           non-standard convenience that returns only the last matching segment
           in the file.  While the SPK standard does say that the last segment
           takes precedence, it also says that earlier segments for a particular
           center-target pair should be fallen back upon for dates that the last
           segment does not cover.  So, if you ever tackle a complicated kernel,
           you will need to implement fallback rules that send some dates to the
@@ -213,15 +220,14 @@
         * If you are accounting for light travel time and require repeated
           computation of the position, but then need the velocity at the end,
           and want to avoid repeating the expensive position calculation, then
           try out the ``segment.generate()`` method - it will let you ask for
           the position, and then only proceed to the velocity once you are sure
           that the light-time error is now small enough.
         
-        
         High-Precision Dates
         --------------------
         
         Since all modern Julian dates are numbers larger than 2.4 million, a
         standard 64-bit Python or NumPy float necessarily leaves only a limited
         number of bits available for the fractional part.  *Technical Note
         2011-02* from the United States Naval Observatory's Astronomical
@@ -299,14 +305,18 @@
         
         https://github.com/brandon-rhodes/python-jplephem/
         
         
         Changelog
         ---------
         
+        **2019 January 3 — Version 2.9**
+        
+        * Added the ``load_array()`` method to the segment class.
+        
         **2018 July 22 — Version 2.8**
         
         * Switched to a making a single memory map of the entire file, to avoid
           running out of file descriptors when users load an ephemeris with
           hundreds of segments.
         
         **2018 February 11 — Version 2.7**
```

### Comparing `jplephem-2.8/setup.py` & `jplephem-2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 sys.modules['numpy'] = sys.modules['sys']
 
 import jplephem
 description, long_description = jplephem.__doc__.split('\n', 1)
 
 setup(name = 'jplephem',
-      version = '2.8',
+      version = '2.9',
       description = description,
       long_description = long_description,
       license = 'MIT',
       author = 'Brandon Rhodes',
       author_email = 'brandon@rhodesmill.org',
       classifiers = [
         'Development Status :: 5 - Production/Stable',
```

### Comparing `jplephem-2.8/jplephem/names.py` & `jplephem-2.9/jplephem/names.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/ascii.py` & `jplephem-2.9/jplephem/ascii.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/daf.py` & `jplephem-2.9/jplephem/daf.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/excerpter.py` & `jplephem-2.9/jplephem/excerpter.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/spk.py` & `jplephem-2.9/jplephem/spk.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         return cls(DAF(open(path, 'rb')))
 
     def close(self):
         """Close this SPK file."""
         self.daf.file.close()
         for segment in self.segments:
             if hasattr(segment, '_data'):
-                del segment._data  # TODO: explicitly close each memory map
+                del segment._data
+        self.daf._array = None
+        self.daf._map = None
 
     def __str__(self):
         daf = self.daf
         d = lambda b: b.decode('latin-1')
         lines = (str(segment) for segment in self.segments)
         return 'File type {0} and format {1} with {2} segments:\n{3}'.format(
             d(daf.locidw), d(daf.locfmt), len(self.segments), '\n'.join(lines))
@@ -61,14 +63,20 @@
         """Given (center, target) integers, return the last matching segment."""
         return self.pairs[key]
 
     def comments(self):
         """Return the file comments, as a string."""
         return self.daf.comments()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
 
 class Segment(object):
     """A single segment of an SPK file.
 
     There are several items of information about each segment that are
     loaded from the underlying SPK file, and made available as object
     attributes:
@@ -137,14 +145,20 @@
 
         coefficients.shape = (int(n), int(rsize))
         coefficients = coefficients[:,2:]  # ignore MID and RADIUS elements
         coefficients.shape = (int(n), component_count, coefficient_count)
         coefficients = rollaxis(coefficients, 1)
         return initial_epoch, interval_length, coefficients
 
+    def load_array(self):
+        data = self._data
+        if data is None:
+            self._data = data = self._load()
+        return data
+
     def generate(self, tdb, tdb2):
         """Generate components and differentials for time `tdb` plus `tdb2`.
 
         Most uses will simply want to call the `compute()` method or the
         `compute_differentials()` method, for convenience.  But in those
         cases (see Skyfield) where you want to compute a position and
         examine it before deciding whether to proceed with the velocity,
```

### Comparing `jplephem-2.8/jplephem/ephem.py` & `jplephem-2.9/jplephem/ephem.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/commandline.py` & `jplephem-2.9/jplephem/commandline.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/jpltest.py` & `jplephem-2.9/jplephem/jpltest.py`

 * *Files identical despite different names*

### Comparing `jplephem-2.8/jplephem/__init__.py` & `jplephem-2.9/jplephem/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,14 +191,21 @@
    |  segment.target - integer target identifier
    |  segment.frame - integer frame identifier
    |  segment.data_type - integer data type identifier
    |  segment.start_i - index where segment starts
    |  segment.end_i - index where segment ends
   ...
 
+* If you want to access the raw coefficients, use the segment
+  ``load_array()`` method.  It returns two floats and a NumPy array:
+
+  >>> initial_epoch, interval_length, coefficients = segment.load_array()
+  >>> print(coefficients.shape)
+  (3, 100448, 13)
+
 * The square-bracket lookup mechanism ``kernel[3,399]`` is a
   non-standard convenience that returns only the last matching segment
   in the file.  While the SPK standard does say that the last segment
   takes precedence, it also says that earlier segments for a particular
   center-target pair should be fallen back upon for dates that the last
   segment does not cover.  So, if you ever tackle a complicated kernel,
   you will need to implement fallback rules that send some dates to the
@@ -208,15 +215,14 @@
 * If you are accounting for light travel time and require repeated
   computation of the position, but then need the velocity at the end,
   and want to avoid repeating the expensive position calculation, then
   try out the ``segment.generate()`` method - it will let you ask for
   the position, and then only proceed to the velocity once you are sure
   that the light-time error is now small enough.
 
-
 High-Precision Dates
 --------------------
 
 Since all modern Julian dates are numbers larger than 2.4 million, a
 standard 64-bit Python or NumPy float necessarily leaves only a limited
 number of bits available for the fractional part.  *Technical Note
 2011-02* from the United States Naval Observatory's Astronomical
@@ -294,14 +300,18 @@
 
 https://github.com/brandon-rhodes/python-jplephem/
 
 
 Changelog
 ---------
 
+**2019 January 3 — Version 2.9**
+
+* Added the ``load_array()`` method to the segment class.
+
 **2018 July 22 — Version 2.8**
 
 * Switched to a making a single memory map of the entire file, to avoid
   running out of file descriptors when users load an ephemeris with
   hundreds of segments.
 
 **2018 February 11 — Version 2.7**
```

### Comparing `jplephem-2.8/jplephem/test.py` & `jplephem-2.9/jplephem/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,14 +318,19 @@
         self.assertEqual(str(segment), segment.describe(verbose=False))
         self.assertEqual(segment.describe(verbose=False),
   '2414864.50..2471184.50  Solar System Barycenter (0) -> Mars Barycenter (4)')
         self.assertEqual(segment.describe(verbose=True),
   '2414864.50..2471184.50  Solar System Barycenter (0) -> Mars Barycenter (4)'
   '\n  frame=1 data_type=2 source=DE-0421LE-0421')
 
+    def test_loading_array(self):
+        segment = self.spk[0,4]
+        initial_epoch, interval_length, coefficients = segment.load_array()
+        self.assertEqual(coefficients.shape, (3, 1760, 11))
+
 
 class LegacyTests(_CommonTests, TestCase):
 
     def setUp(self):
         try:
             import de421
         except ImportError:
@@ -361,21 +366,20 @@
         self.assertAlmostEqual(y, 1.05103857e+08, delta=1.0)
         self.assertAlmostEqual(z, 45550861.44383482, delta=epsilon_m)
 
 
 class NAIF_DAF_Tests(TestCase):
 
     def test_single_position(self):
-        kernel = SPK(NAIF_DAF(open('de405.bsp', 'rb')))
-        x, y, z = kernel[0,4].compute(2457061.5)
-        # Expect rough agreement with a DE430 position from our README:
-        self.assertAlmostEqual(x, 2.05700211e+08, delta=2.0)
-        self.assertAlmostEqual(y, 4.25141646e+07, delta=2.0)
-        self.assertAlmostEqual(z, 1.39379183e+07, delta=2.0)
-        kernel.close()
+        with SPK(NAIF_DAF(open('de405.bsp', 'rb'))) as kernel:
+            x, y, z = kernel[0,4].compute(2457061.5)
+            # Expect rough agreement with a DE430 position from our README:
+            self.assertAlmostEqual(x, 2.05700211e+08, delta=2.0)
+            self.assertAlmostEqual(y, 4.25141646e+07, delta=2.0)
+            self.assertAlmostEqual(z, 1.39379183e+07, delta=2.0)
 
 
 class CommandLineTests(TestCase):
     maxDiff = 9999
 
     def test_comment_command(self):
         output = commandline.main(['comment', 'de405.bsp'])
```

