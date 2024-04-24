# Comparing `tmp/linalgebralib-0.0.3.tar.gz` & `tmp/linalgebralib-0.0.31.tar.gz`

## Comparing `linalgebralib-0.0.3.tar` & `linalgebralib-0.0.31.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/src/test.py
--rw-r--r--   0        0        0    19602 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/src/linalgebralib/LinAlgebraLib.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/src/linalgebralib/__init__.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/tests/test_linalgebralib.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/LICENSE
--rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    13608 2020-02-02 00:00:00.000000 linalgebralib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/src/test.py
+-rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/src/linalgebralib/LinAlgebraLib.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/src/linalgebralib/__init__.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/tests/test_linalgebralib.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/LICENSE
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 linalgebralib-0.0.31/PKG-INFO
```

### Comparing `linalgebralib-0.0.3/src/test.py` & `linalgebralib-0.0.31/src/test.py`

 * *Files identical despite different names*

### Comparing `linalgebralib-0.0.3/src/linalgebralib/LinAlgebraLib.py` & `linalgebralib-0.0.31/src/linalgebralib/LinAlgebraLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         else:
             if (size[0] == 0 and size[1] != 0) or (size[1] == 0 and size[0] != 0):
                 raise ValueError("Cannot have a matrix with rows and no columns, or columns and no rows.")
             self.contents = []
             self.rows = size[0]
             self.columns = size[1]
             for i in range(self.rows):
-                self.contents.append(rowVector(size=self.columns).contents)
+                self.contents.append([0 for i in range(self.columns)])
 
     def __repr__(self):
         #Respresents the matrix as rows on new lines.
         if self.contents == []:
             return "[]"
         result = []
         for row in self.contents:
```

### Comparing `linalgebralib-0.0.3/tests/test_linalgebralib.py` & `linalgebralib-0.0.31/tests/test_linalgebralib.py`

 * *Files identical despite different names*

### Comparing `linalgebralib-0.0.3/LICENSE` & `linalgebralib-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `linalgebralib-0.0.3/README.md` & `linalgebralib-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `linalgebralib-0.0.3/pyproject.toml` & `linalgebralib-0.0.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "linalgebralib"
-version = "0.0.3"
+version = "0.0.31"
 authors = [
   { name="Adam Authur", email="aauthur@tamu.edu" },
 ]
 description = "This package contains a library of methods and classes relating to Linear Algebra."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `linalgebralib-0.0.3/PKG-INFO` & `linalgebralib-0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: linalgebralib
-Version: 0.0.3
+Version: 0.0.31
 Summary: This package contains a library of methods and classes relating to Linear Algebra.
 Project-URL: Homepage, https://github.com/aauthur/LinAlgebraLib
 Author-email: Adam Authur <aauthur@tamu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

