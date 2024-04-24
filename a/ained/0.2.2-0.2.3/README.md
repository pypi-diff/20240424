# Comparing `tmp/ained-0.2.2.tar.gz` & `tmp/ained-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ained-0.2.2.tar", max compression
+gzip compressed data, was "ained-0.2.3.tar", max compression
```

## Comparing `ained-0.2.2.tar` & `ained-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,33 @@
--rw-r--r--   0        0        0     3423 2024-04-18 08:40:43.782456 ained-0.2.2/README.md
--rw-r--r--   0        0        0      654 2024-04-18 08:40:43.782456 ained-0.2.2/ained/Data/exampleData.json
--rw-r--r--   0        0        0     1208 2024-04-18 08:40:43.782456 ained-0.2.2/ained/Data/jasonSchema.json
--rw-r--r--   0        0        0    29149 2024-04-18 08:40:43.782456 ained-0.2.2/ained/Samples/Sample1.txt
--rw-r--r--   0        0        0      294 2024-04-18 08:40:43.782456 ained-0.2.2/ained/Samples/Sample2.txt
--rw-r--r--   0        0        0      397 2024-04-18 08:40:43.782456 ained-0.2.2/ained/TauswortheInC/README.md
--rwxr-xr-x   0        0        0    15800 2024-04-18 08:40:43.782456 ained-0.2.2/ained/TauswortheInC/libtausworthe.so
--rw-r--r--   0        0        0      924 2024-04-18 08:40:43.782456 ained-0.2.2/ained/TauswortheInC/tausworthe.c
--rw-r--r--   0        0        0      110 2024-04-18 08:40:43.782456 ained-0.2.2/ained/TauswortheInC/tausworthe_wrapper.c
--rw-r--r--   0        0        0       21 2024-04-19 12:57:03.698188 ained-0.2.2/ained/__init__.py
--rw-r--r--   0        0        0     2622 2024-04-18 08:40:43.786456 ained-0.2.2/ained/board.py
--rw-r--r--   0        0        0     3765 2024-04-18 08:40:43.786456 ained-0.2.2/ained/calculator.py
--rw-r--r--   0        0        0     2293 2024-04-18 08:40:43.786456 ained-0.2.2/ained/dipole.py
--rw-r--r--   0        0        0     5666 2024-04-18 08:40:43.786456 ained-0.2.2/ained/display.py
--rw-r--r--   0        0        0      573 2024-04-18 08:40:43.786456 ained-0.2.2/ained/fixedpoint_config.py
--rw-r--r--   0        0        0     1742 2024-04-18 08:40:43.786456 ained-0.2.2/ained/generator.py
--rw-r--r--   0        0        0     1116 2024-04-18 08:40:43.786456 ained-0.2.2/ained/historymanager.py
--rw-r--r--   0        0        0     2014 2024-04-18 08:40:43.786456 ained-0.2.2/ained/main.py
--rw-r--r--   0        0        0      317 2024-04-18 08:40:43.786456 ained-0.2.2/ained/number_gen.py
--rw-r--r--   0        0        0     2002 2024-04-18 08:40:43.786456 ained-0.2.2/ained/processJson.py
--rw-r--r--   0        0        0       26 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/Test_Data.txt
--rw-r--r--   0        0        0        0 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__init__.py
--rw-r--r--   0        0        0      172 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2217 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3440 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     4674 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1896 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     8390 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1864 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/test_board.py
--rw-r--r--   0        0        0      736 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/test_dipole.py
--rw-r--r--   0        0        0     1309 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/test_fixedpoint.py
--rw-r--r--   0        0        0      856 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/test_generator.py
--rw-r--r--   0        0        0     3299 2024-04-18 08:40:43.786456 ained-0.2.2/ained/test/test_utils.py
--rw-r--r--   0        0        0      484 2024-04-19 12:57:03.690187 ained-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4061 1970-01-01 00:00:00.000000 ained-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6263 2024-04-24 13:49:26.626230 ained-0.2.3/README.md
+-rw-r--r--   0        0        0      654 2024-04-18 08:40:43.782456 ained-0.2.3/ained/Data/exampleData.json
+-rw-r--r--   0        0        0     1208 2024-04-18 08:40:43.782456 ained-0.2.3/ained/Data/jasonSchema.json
+-rw-r--r--   0        0        0      397 2024-04-18 08:40:43.782456 ained-0.2.3/ained/TauswortheInC/README.md
+-rwxr-xr-x   0        0        0    15800 2024-04-18 08:40:43.782456 ained-0.2.3/ained/TauswortheInC/libtausworthe.so
+-rw-r--r--   0        0        0      924 2024-04-18 08:40:43.782456 ained-0.2.3/ained/TauswortheInC/tausworthe.c
+-rw-r--r--   0        0        0      110 2024-04-18 08:40:43.782456 ained-0.2.3/ained/TauswortheInC/tausworthe_wrapper.c
+-rw-r--r--   0        0        0       21 2024-04-24 13:59:36.263348 ained-0.2.3/ained/__init__.py
+-rw-r--r--   0        0        0     2622 2024-04-18 08:40:43.786456 ained-0.2.3/ained/board.py
+-rw-r--r--   0        0        0     3765 2024-04-18 08:40:43.786456 ained-0.2.3/ained/calculator.py
+-rw-r--r--   0        0        0     2293 2024-04-18 08:40:43.786456 ained-0.2.3/ained/dipole.py
+-rw-r--r--   0        0        0     5666 2024-04-18 08:40:43.786456 ained-0.2.3/ained/display.py
+-rw-r--r--   0        0        0      573 2024-04-18 08:40:43.786456 ained-0.2.3/ained/fixedpoint_config.py
+-rw-r--r--   0        0        0     1742 2024-04-18 08:40:43.786456 ained-0.2.3/ained/generator.py
+-rw-r--r--   0        0        0     1116 2024-04-18 08:40:43.786456 ained-0.2.3/ained/historymanager.py
+-rw-r--r--   0        0        0     2014 2024-04-18 08:40:43.786456 ained-0.2.3/ained/main.py
+-rw-r--r--   0        0        0      317 2024-04-18 08:40:43.786456 ained-0.2.3/ained/number_gen.py
+-rw-r--r--   0        0        0     1927 2024-04-24 12:50:43.739370 ained-0.2.3/ained/processJson.py
+-rw-r--r--   0        0        0       26 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/Test_Data.txt
+-rw-r--r--   0        0        0        0 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2217 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3440 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     4674 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1896 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     8390 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1864 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/test_board.py
+-rw-r--r--   0        0        0      736 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/test_dipole.py
+-rw-r--r--   0        0        0     1276 2024-04-24 12:10:09.173744 ained-0.2.3/ained/test/test_fixedpoint.py
+-rw-r--r--   0        0        0      856 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/test_generator.py
+-rw-r--r--   0        0        0     3299 2024-04-18 08:40:43.786456 ained-0.2.3/ained/test/test_utils.py
+-rw-r--r--   0        0        0      484 2024-04-24 13:59:36.255348 ained-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6901 1970-01-01 00:00:00.000000 ained-0.2.3/PKG-INFO
```

### Comparing `ained-0.2.2/ained/Data/exampleData.json` & `ained-0.2.3/ained/Data/exampleData.json`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/Data/jasonSchema.json` & `ained-0.2.3/ained/Data/jasonSchema.json`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/TauswortheInC/libtausworthe.so` & `ained-0.2.3/ained/TauswortheInC/libtausworthe.so`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/TauswortheInC/tausworthe.c` & `ained-0.2.3/ained/TauswortheInC/tausworthe.c`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/board.py` & `ained-0.2.3/ained/board.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/calculator.py` & `ained-0.2.3/ained/calculator.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/dipole.py` & `ained-0.2.3/ained/dipole.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/display.py` & `ained-0.2.3/ained/display.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/fixedpoint_config.py` & `ained-0.2.3/ained/fixedpoint_config.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/generator.py` & `ained-0.2.3/ained/generator.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/historymanager.py` & `ained-0.2.3/ained/historymanager.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/main.py` & `ained-0.2.3/ained/main.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/processJson.py` & `ained-0.2.3/ained/processJson.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     # Build board
     history_manager = HistoryManager()
     board = Board(size_x=rows, size_y=columns, flip_probability=prob, generator=random_generator,
                   initial_states=initial_states)
 
     # Apply changes for each timestep
     for timestep in timesteps:
-        print(f"Time: {timestep['time']}, Changes: {timestep['changes']}")
         for change in timestep['changes']:
             x = change['x']
             y = change['y']
             proposed = change['state']
             current = board.get_dipole(x, y).current_state.value
 
             if proposed == current:
```

### Comparing `ained-0.2.2/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.3/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.3/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.3/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.3/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.3/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/test_board.py` & `ained-0.2.3/ained/test/test_board.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/test_dipole.py` & `ained-0.2.3/ained/test/test_dipole.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/test_fixedpoint.py` & `ained-0.2.3/ained/test/test_fixedpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     y.equal(x1 + x2)
 
     assert (y.dtype == x1.dtype and y.dtype == x2.dtype)
     assert isclose(0.5, y, rel_tol=0.05)
 
 def test_overflow():
     x1 = Fxp(0.8, signed=False, dtype=DTYPE)
-    print(x1.info(verbose=True))
     x2 = Fxp(0.5, signed=False, dtype=DTYPE)
     y = Fxp(None, signed=False, dtype=DTYPE)
     y.equal(x1 + x2)
 
     assert (y.dtype == x1.dtype and y.dtype == x2.dtype)
     assert isclose(1, y, rel_tol=0.05)
```

### Comparing `ained-0.2.2/ained/test/test_generator.py` & `ained-0.2.3/ained/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `ained-0.2.2/ained/test/test_utils.py` & `ained-0.2.3/ained/test/test_utils.py`

 * *Files identical despite different names*

