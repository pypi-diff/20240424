# Comparing `tmp/trm_woodburn-0.1.1.tar.gz` & `tmp/trm_woodburn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.1.1.tar", last modified: Sat Apr 20 02:33:49 2024, max compression
+gzip compressed data, was "trm_woodburn-0.1.2.tar", last modified: Wed Apr 24 12:26:34 2024, max compression
```

## Comparing `trm_woodburn-0.1.1.tar` & `trm_woodburn-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 02:33:49.368734 trm_woodburn-0.1.1/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.1.1/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-20 02:33:49.368683 trm_woodburn-0.1.1/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6392 2024-04-20 01:04:40.000000 trm_woodburn-0.1.1/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.1.1/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-20 02:33:49.368949 trm_woodburn-0.1.1/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 02:33:49.367060 trm_woodburn-0.1.1/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 02:33:49.367750 trm_woodburn-0.1.1/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.1.1/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    24835 2024-04-20 02:32:21.000000 trm_woodburn-0.1.1/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-20 02:33:49.368504 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-20 02:33:49.000000 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-20 02:33:49.000000 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-20 02:33:49.000000 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-20 02:33:49.000000 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-20 02:33:49.000000 trm_woodburn-0.1.1/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.661321 trm_woodburn-0.1.2/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.1.2/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-24 12:26:34.661267 trm_woodburn-0.1.2/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6392 2024-04-24 12:26:17.000000 trm_woodburn-0.1.2/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.1.2/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-24 12:26:34.661546 trm_woodburn-0.1.2/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.659348 trm_woodburn-0.1.2/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.660255 trm_woodburn-0.1.2/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.1.2/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    25274 2024-04-24 12:24:26.000000 trm_woodburn-0.1.2/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.661085 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.1.1/LICENSE.txt` & `trm_woodburn-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.1.1/PKG-INFO` & `trm_woodburn-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -166,9 +166,9 @@
 estimated time remaining to complete the process based on the initial time
 stored in `t_init` will be displayed. When the process is completed, the total
 elapsed time since `t_init` will be displayed. If `cols` is not provided, the
 full width of the current terminal window will be used. If the `fat` input is
 set to `True`, the bars will be thick.
 
 ```
- 44% [/////////////////////----------------------------] -00:00:02.1
+ 44% ======================----------------------------- -00:00:02.1
 ```
```

### Comparing `trm_woodburn-0.1.1/README.md` & `trm_woodburn-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -151,9 +151,9 @@
 estimated time remaining to complete the process based on the initial time
 stored in `t_init` will be displayed. When the process is completed, the total
 elapsed time since `t_init` will be displayed. If `cols` is not provided, the
 full width of the current terminal window will be used. If the `fat` input is
 set to `True`, the bars will be thick.
 
 ```
- 44% [/////////////////////----------------------------] -00:00:02.1
+ 44% ======================----------------------------- -00:00:02.1
 ```
```

### Comparing `trm_woodburn-0.1.1/setup.cfg` & `trm_woodburn-0.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.1.1
+version = 0.1.2
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.1.1/src/trm/trm.py` & `trm_woodburn-0.1.2/src/trm/trm.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-04-19"
+__date__ = "2024-04-24"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
 import time
 import math
@@ -57,15 +57,15 @@
     Parameters
     ----------
     x : (K,) or (J, K) np.ndarray
         Array of x-axis values or matrix of rows of x-axis values.
     y : (K,) or (J, K) np.ndarray, default None
         Array of y-axis values or matrix of rows of y-axis values. If `y` is not
         provided, `x` will be used as the `y` array and `x` will be defined to
-        be an array of indices.
+        be an array of indices (starting at zero).
     label : str, default ''
         Text to place at top of the plot, centered in the border.
     rows : int, default 1
         Desired number of rows if greater than 1 or fraction of existing rows if
         less than 1.
     cols : int, default 1
         Desired number of columns if greater than 1 or fraction of window
@@ -88,17 +88,21 @@
     except: # If getting terminal size fails, use default values.
         term_cols = config.cols
         term_rows = config.rows
         colorize = False
     term_rows -= 1 # Account for the prompt line.
 
     # Convert a fractional canvas size to columns and rows.
-    if cols <= 1:
+    if cols < 0:
+        raise ValueError(f"cols should be positive: {cols}!")
+    elif cols <= 1:
         cols = max(round(term_cols * cols), 3)
-    if rows <= 1:
+    if rows < 0:
+        raise ValueError(f"rows should be positive: {rows}!")
+    elif rows <= 1:
         rows = max(round(term_rows * rows), 3)
 
     # Adjust for the bounding box and ensure integer type.
     rows = int(rows) - 2
     cols = int(cols) - 2
 
     # Define the sub-columns and sub-rows.
@@ -112,19 +116,21 @@
     # If only `x` is provided, copy to `y`
     # and make `x` an array of integers.
     if y is None:
         y = x + 0
         if np.ndim(y) == 0:
             x = 1.0
         elif np.ndim(y) == 1:
-            x = np.arange(len(y)) + 1
+            x = np.arange(len(y))
         elif np.ndim(y) == 2:
             J, K = y.shape
-            x = np.arange(K) + 1
+            x = np.arange(K)
             x = np.outer(np.ones(J), x)
+    if isinstance(y, str):
+        raise ValueError(f"y should not be a string: {y}!")
 
     # Ensure x and y are both 2D arrays.
     x = np.array(x)
     y = np.array(y)
     if np.ndim(x) == 0:
         x = np.array([[x]])
     elif np.ndim(x) == 1:
@@ -523,14 +529,19 @@
             if n_col > 0:
                 row_str += sep
             row_str += fixed_width_string(val, width)
         print(row_str)
 
 
 def sparsity(matrix, label=''):
+    """
+    Print the sparsity of a matrix. Note, if you are using SciPy sparse arrays
+    or matrices, use the method `toarray()` on the input to this function.
+    """
+
     # Convert matrix to zeros and ones.
     M = (np.abs(matrix) > 1e-30).astype(int)
 
     # Convert the large matrix to a smaller matrix of character values.
     C = matrix_to_braille(M) if config.uni else matrix_to_stars(M)
 
     # Create the shape string.
@@ -640,15 +651,15 @@
 
 
 def matrix_to_ascii(M):
     # Pad the matrix with zeros.
     I, J = M.shape
     II = math.ceil(I/3)*3
     MM = np.zeros((II, J), dtype=int)
-    MM[:I, :J] = M
+    MM[:I, :J] = M[:I, :J]
 
     # Convert the matrix of ones and zeros to braille characters.
     glyphs = np.array([ # " `-'.!:|"
         0x20, 0x60, 0x2D, 0x27, 0x2E, 0x21, 0x3A, 0x7C])
     C = glyphs[M[::3] + 2*M[1::3] + 4*M[2::3]]
     return C
```

### Comparing `trm_woodburn-0.1.1/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.1.2/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -166,9 +166,9 @@
 estimated time remaining to complete the process based on the initial time
 stored in `t_init` will be displayed. When the process is completed, the total
 elapsed time since `t_init` will be displayed. If `cols` is not provided, the
 full width of the current terminal window will be used. If the `fat` input is
 set to `True`, the bars will be thick.
 
 ```
- 44% [/////////////////////----------------------------] -00:00:02.1
+ 44% ======================----------------------------- -00:00:02.1
 ```
```

