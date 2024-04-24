# Comparing `tmp/ruleopt-1.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/ruleopt-1.0.1-cp39-cp39-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,39 @@
-Zip file size: 311655 bytes, number of entries: 28
--rw-rw-rw-  2.0 fat      257 b- defN 24-Apr-17 14:21 ruleopt/__init__.py
--rw-rw-rw-  2.0 fat       96 b- defN 24-Apr-17 14:21 ruleopt/aux_classes/__init__.py
--rw-rw-rw-  2.0 fat  1415904 b- defN 24-Apr-17 14:22 ruleopt/aux_classes/aux_classes.c
--rw-rw-rw-  2.0 fat   217600 b- defN 24-Apr-17 14:23 ruleopt/aux_classes/aux_classes.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      280 b- defN 24-Apr-17 14:21 ruleopt/estimator/__init__.py
--rw-rw-rw-  2.0 fat    25006 b- defN 24-Apr-17 14:21 ruleopt/estimator/base.py
--rw-rw-rw-  2.0 fat    12875 b- defN 24-Apr-17 14:21 ruleopt/estimator/lightgbm_.py
--rw-rw-rw-  2.0 fat    11723 b- defN 24-Apr-17 14:21 ruleopt/estimator/xgboost_.py
--rw-rw-rw-  2.0 fat      126 b- defN 24-Apr-17 14:21 ruleopt/estimator/sklearn_/__init__.py
--rw-rw-rw-  2.0 fat     7694 b- defN 24-Apr-17 14:21 ruleopt/estimator/sklearn_/base_sklearn.py
--rw-rw-rw-  2.0 fat    13679 b- defN 24-Apr-17 14:21 ruleopt/estimator/sklearn_/rug.py
--rw-rw-rw-  2.0 fat     5864 b- defN 24-Apr-17 14:21 ruleopt/estimator/sklearn_/rux.py
--rw-rw-rw-  2.0 fat       68 b- defN 24-Apr-17 14:21 ruleopt/explainer/__init__.py
--rw-rw-rw-  2.0 fat     9875 b- defN 24-Apr-17 14:21 ruleopt/explainer/explainer.py
--rw-rw-rw-  2.0 fat      137 b- defN 24-Apr-17 14:21 ruleopt/rule_cost/__init__.py
--rw-rw-rw-  2.0 fat     6681 b- defN 24-Apr-17 14:21 ruleopt/rule_cost/rule_cost.py
--rw-rw-rw-  2.0 fat      247 b- defN 24-Apr-17 14:21 ruleopt/solver/__init__.py
--rw-rw-rw-  2.0 fat     3208 b- defN 24-Apr-17 14:21 ruleopt/solver/base.py
--rw-rw-rw-  2.0 fat     4010 b- defN 24-Apr-17 14:21 ruleopt/solver/cplex_solver.py
--rw-rw-rw-  2.0 fat     3818 b- defN 24-Apr-17 14:21 ruleopt/solver/gurobi_solver.py
--rw-rw-rw-  2.0 fat     4955 b- defN 24-Apr-17 14:21 ruleopt/solver/ortools_solver.py
--rw-rw-rw-  2.0 fat      173 b- defN 24-Apr-17 14:21 ruleopt/utils/__init__.py
--rw-rw-rw-  2.0 fat     1250 b- defN 24-Apr-17 14:21 ruleopt/utils/utils.py
--rw-rw-rw-  2.0 fat     1557 b- defN 24-Apr-17 14:23 ruleopt-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4114 b- defN 24-Apr-17 14:23 ruleopt-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-17 14:23 ruleopt-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-17 14:22 ruleopt-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2394 b- defN 24-Apr-17 14:23 ruleopt-1.0.0.dist-info/RECORD
-28 files, 1753699 bytes uncompressed, 307791 bytes compressed:  82.4%
+Zip file size: 312801 bytes, number of entries: 37
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/estimator/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/solver/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/rule_cost/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/explainer/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/aux_classes/
+-rw-r--r--  2.0 unx      247 b- defN 24-Apr-24 21:26 ruleopt/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 21:27 ruleopt/estimator/sklearn_/
+-rw-r--r--  2.0 unx      271 b- defN 24-Apr-24 21:26 ruleopt/estimator/__init__.py
+-rw-r--r--  2.0 unx    12543 b- defN 24-Apr-24 21:26 ruleopt/estimator/lightgbm_.py
+-rw-r--r--  2.0 unx    11412 b- defN 24-Apr-24 21:26 ruleopt/estimator/xgboost_.py
+-rw-r--r--  2.0 unx    24321 b- defN 24-Apr-24 21:26 ruleopt/estimator/base.py
+-rw-r--r--  2.0 unx     7479 b- defN 24-Apr-24 21:26 ruleopt/estimator/sklearn_/base_sklearn.py
+-rw-r--r--  2.0 unx     5710 b- defN 24-Apr-24 21:26 ruleopt/estimator/sklearn_/rux.py
+-rw-r--r--  2.0 unx      119 b- defN 24-Apr-24 21:26 ruleopt/estimator/sklearn_/__init__.py
+-rw-r--r--  2.0 unx    13325 b- defN 24-Apr-24 21:26 ruleopt/estimator/sklearn_/rug.py
+-rw-r--r--  2.0 unx      168 b- defN 24-Apr-24 21:26 ruleopt/utils/__init__.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-Apr-24 21:26 ruleopt/utils/utils.py
+-rw-r--r--  2.0 unx     4780 b- defN 24-Apr-24 21:26 ruleopt/solver/ortools_solver.py
+-rw-r--r--  2.0 unx      240 b- defN 24-Apr-24 21:26 ruleopt/solver/__init__.py
+-rw-r--r--  2.0 unx     3668 b- defN 24-Apr-24 21:26 ruleopt/solver/gurobi_solver.py
+-rw-r--r--  2.0 unx     3852 b- defN 24-Apr-24 21:26 ruleopt/solver/cplex_solver.py
+-rw-r--r--  2.0 unx     3471 b- defN 24-Apr-24 21:26 ruleopt/solver/base.py
+-rw-r--r--  2.0 unx     6474 b- defN 24-Apr-24 21:26 ruleopt/rule_cost/rule_cost.py
+-rw-r--r--  2.0 unx      134 b- defN 24-Apr-24 21:26 ruleopt/rule_cost/__init__.py
+-rw-r--r--  2.0 unx     9612 b- defN 24-Apr-24 21:26 ruleopt/explainer/explainer.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-24 21:26 ruleopt/explainer/__init__.py
+-rw-r--r--  2.0 unx       91 b- defN 24-Apr-24 21:26 ruleopt/aux_classes/__init__.py
+-rwxr-xr-x  2.0 unx   266240 b- defN 24-Apr-24 21:27 ruleopt/aux_classes/aux_classes.cpython-39-darwin.so
+-rw-r--r--  2.0 unx  1420749 b- defN 24-Apr-24 21:27 ruleopt/aux_classes/aux_classes.c
+-rw-rw-r--  2.0 unx     2424 b- defN 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1530 b- defN 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     4019 b- defN 24-Apr-24 21:27 ruleopt-1.0.1.dist-info/METADATA
+37 files, 1804270 bytes uncompressed, 307925 bytes compressed:  82.9%
```

## zipnote {}

```diff
@@ -1,85 +1,112 @@
-Filename: ruleopt/__init__.py
+Filename: ruleopt/
 Comment: 
 
-Filename: ruleopt/aux_classes/__init__.py
+Filename: ruleopt-1.0.1.dist-info/
 Comment: 
 
-Filename: ruleopt/aux_classes/aux_classes.c
+Filename: ruleopt/estimator/
 Comment: 
 
-Filename: ruleopt/aux_classes/aux_classes.cp39-win_amd64.pyd
+Filename: ruleopt/utils/
 Comment: 
 
-Filename: ruleopt/estimator/__init__.py
+Filename: ruleopt/solver/
 Comment: 
 
-Filename: ruleopt/estimator/base.py
+Filename: ruleopt/rule_cost/
+Comment: 
+
+Filename: ruleopt/explainer/
+Comment: 
+
+Filename: ruleopt/aux_classes/
+Comment: 
+
+Filename: ruleopt/__init__.py
+Comment: 
+
+Filename: ruleopt/estimator/sklearn_/
+Comment: 
+
+Filename: ruleopt/estimator/__init__.py
 Comment: 
 
 Filename: ruleopt/estimator/lightgbm_.py
 Comment: 
 
 Filename: ruleopt/estimator/xgboost_.py
 Comment: 
 
-Filename: ruleopt/estimator/sklearn_/__init__.py
+Filename: ruleopt/estimator/base.py
 Comment: 
 
 Filename: ruleopt/estimator/sklearn_/base_sklearn.py
 Comment: 
 
-Filename: ruleopt/estimator/sklearn_/rug.py
+Filename: ruleopt/estimator/sklearn_/rux.py
 Comment: 
 
-Filename: ruleopt/estimator/sklearn_/rux.py
+Filename: ruleopt/estimator/sklearn_/__init__.py
 Comment: 
 
-Filename: ruleopt/explainer/__init__.py
+Filename: ruleopt/estimator/sklearn_/rug.py
 Comment: 
 
-Filename: ruleopt/explainer/explainer.py
+Filename: ruleopt/utils/__init__.py
 Comment: 
 
-Filename: ruleopt/rule_cost/__init__.py
+Filename: ruleopt/utils/utils.py
 Comment: 
 
-Filename: ruleopt/rule_cost/rule_cost.py
+Filename: ruleopt/solver/ortools_solver.py
 Comment: 
 
 Filename: ruleopt/solver/__init__.py
 Comment: 
 
-Filename: ruleopt/solver/base.py
+Filename: ruleopt/solver/gurobi_solver.py
 Comment: 
 
 Filename: ruleopt/solver/cplex_solver.py
 Comment: 
 
-Filename: ruleopt/solver/gurobi_solver.py
+Filename: ruleopt/solver/base.py
 Comment: 
 
-Filename: ruleopt/solver/ortools_solver.py
+Filename: ruleopt/rule_cost/rule_cost.py
 Comment: 
 
-Filename: ruleopt/utils/__init__.py
+Filename: ruleopt/rule_cost/__init__.py
 Comment: 
 
-Filename: ruleopt/utils/utils.py
+Filename: ruleopt/explainer/explainer.py
+Comment: 
+
+Filename: ruleopt/explainer/__init__.py
+Comment: 
+
+Filename: ruleopt/aux_classes/__init__.py
+Comment: 
+
+Filename: ruleopt/aux_classes/aux_classes.cpython-39-darwin.so
+Comment: 
+
+Filename: ruleopt/aux_classes/aux_classes.c
 Comment: 
 
-Filename: ruleopt-1.0.0.dist-info/LICENSE
+Filename: ruleopt-1.0.1.dist-info/RECORD
 Comment: 
 
-Filename: ruleopt-1.0.0.dist-info/METADATA
+Filename: ruleopt-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: ruleopt-1.0.0.dist-info/WHEEL
+Filename: ruleopt-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: ruleopt-1.0.0.dist-info/top_level.txt
+Filename: ruleopt-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ruleopt-1.0.0.dist-info/RECORD
+Filename: ruleopt-1.0.1.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## ruleopt/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-from .estimator import (RUGClassifier, RUXClassifier, RUXLGBMClassifier, RUXXGBClassifier)
-from .explainer import Explainer
-
-__all__ = [
-    "RUGClassifier",
-    "RUXClassifier",
-    "RUXLGBMClassifier",
-    "RUXXGBClassifier",
-    "Explainer",]
-
+from .estimator import (RUGClassifier, RUXClassifier, RUXLGBMClassifier, RUXXGBClassifier)
+from .explainer import Explainer
+
+__all__ = [
+    "RUGClassifier",
+    "RUXClassifier",
+    "RUXLGBMClassifier",
+    "RUXXGBClassifier",
+    "Explainer",]
+
```

## ruleopt/aux_classes/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from .aux_classes import (Rule, Coefficients)
-
-
-__all__ = [
-    "Rule",
+from .aux_classes import (Rule, Coefficients)
+
+
+__all__ = [
+    "Rule",
     "Coefficients"]
```

## ruleopt/aux_classes/aux_classes.c

```diff
@@ -1,27 +1,26 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
-            "/O2",
-            "/favor:ATOM",
-            "/fp:fast",
+            "-Ofast",
+            "-funroll-loops",
             "-DNPY_NO_DEPRECATED_API=NPY_1_7_API_VERSION"
         ],
         "include_dirs": [
-            "C:\\Users\\runneradmin\\AppData\\Local\\Temp\\pip-build-env-c46otpzo\\overlay\\Lib\\site-packages\\numpy\\core\\include"
+            "/private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "ruleopt.aux_classes.aux_classes",
         "sources": [
             "ruleopt/aux_classes/aux_classes.pyx"
         ]
     },
@@ -1526,18 +1525,18 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "ruleopt\\\\aux_classes\\\\aux_classes.pyx",
+  "ruleopt/aux_classes/aux_classes.pyx",
   "<stringsource>",
   "__init__.cython-30.pxd",
-  "ruleopt\\\\aux_classes\\\\aux_classes.pxd",
+  "ruleopt/aux_classes/aux_classes.pxd",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
@@ -1676,177 +1675,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1908,42 +1907,42 @@
 struct __pyx_obj_7ruleopt_11aux_classes_11aux_classes_Coefficients;
 struct __pyx_obj_7ruleopt_11aux_classes_11aux_classes_Rule;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3545,15 +3544,15 @@
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_Coefficients___reduce_cython[] = "Coefficients.__reduce_cython__";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_Coefficients___setstate_cython[] = "Coefficients.__setstate_cython__";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_ruleopt_aux_classes_aux_classes[] = "ruleopt\\aux_classes\\aux_classes.pyx";
+static const char __pyx_k_ruleopt_aux_classes_aux_classes[] = "ruleopt/aux_classes/aux_classes.pyx";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
@@ -18501,261 +18500,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18764,29 +18763,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18797,15 +18796,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18814,29 +18813,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18847,15 +18846,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18864,29 +18863,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18897,15 +18896,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18914,29 +18913,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18947,15 +18946,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18964,29 +18963,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18997,217 +18996,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19223,15 +19222,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19239,68 +19238,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19308,15 +19307,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19331,15 +19330,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19355,15 +19354,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19371,68 +19370,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19440,15 +19439,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19463,15 +19462,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19487,15 +19486,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19503,68 +19502,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19572,15 +19571,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19595,170 +19594,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -26233,26 +26232,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/pip-build-env-c46otpzo/overlay/Lib/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../private/var/folders/3m/p59k4qdj0f17st0gn2cmj3640000gn/T/pip-build-env-kcwpqpby/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

## ruleopt/estimator/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-from .sklearn_.rug import (RUGClassifier)
-from .sklearn_.rux import (RUXClassifier)
-from .xgboost_ import (RUXXGBClassifier)
-from .lightgbm_ import (RUXLGBMClassifier)
-
-__all__ = [
-    "RUGClassifier",
-    "RUXClassifier",
-    "RUXLGBMClassifier",
+from .sklearn_.rug import (RUGClassifier)
+from .sklearn_.rux import (RUXClassifier)
+from .xgboost_ import (RUXXGBClassifier)
+from .lightgbm_ import (RUXLGBMClassifier)
+
+__all__ = [
+    "RUGClassifier",
+    "RUXClassifier",
+    "RUXLGBMClassifier",
     "RUXXGBClassifier"]
```

## ruleopt/estimator/base.py

 * *Ordering differences only*

```diff
@@ -1,685 +1,685 @@
-from __future__ import annotations
-import warnings
-from typing import Union, Dict
-from abc import abstractmethod
-import numpy as np
-from numpy.typing import ArrayLike
-from sklearn.base import BaseEstimator, ClassifierMixin
-from sklearn.utils.class_weight import compute_sample_weight
-
-from ..aux_classes import Coefficients, Rule
-from ..rule_cost import RuleCost
-from ..utils import check_inputs, check_sample_weight
-from ..solver.base import OptimizationSolver
-
-
-
-class _RUGBASE(BaseEstimator, ClassifierMixin):
-    """
-    The foundational class for all estimators in the ruleopt library. `_RUGBASE` provides
-    the core framework that every model in ruleopt builds upon.
-
-    Parameters
-    ----------
-    solver : OptimizationSolver
-        An instance of a derived class inherits from the 'Optimization Solver' base class.
-        The solver is responsible for optimizing the rule set based on the cost function
-        and constraints.
-
-    rule_cost : RuleCost or int
-        Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-        or a fixed cost
-
-    class_weight: dict, "balanced" or None
-        A dictionary mapping class labels to their respective weights, the string "balanced"
-        to automatically adjust weights inversely proportional to class frequencies,
-        or None for no weights. Used to adjust the model in favor of certain classes.
-
-    threshold : float
-        The minimum weight threshold for including a rule in the final model
-
-    random_state : int or None, default=None
-        Seed for the random number generator to ensure reproducible results.
-    """
-
-    def __init__(
-        self,
-        solver: OptimizationSolver,
-        rule_cost: Union[RuleCost, int],
-        class_weight: Dict[int, float],
-        threshold: float,
-        random_state: Union[None, int],
-    ):
-
-        self._validate_rug_parameters(
-            threshold=threshold,
-            random_state=random_state,
-            rule_cost=rule_cost,
-            solver=solver,
-            class_weight=class_weight,
-        )
-        self.threshold = float(threshold)
-        self.rule_cost = rule_cost
-        self.solver = solver
-        self.random_state = random_state
-        self.class_weight = class_weight
-
-        # Additional initializations
-        self._rng = np.random.default_rng(
-            random_state if random_state is not None else None
-        )
-        self.decision_trees_ = {}
-        self.decision_rules_ = {}
-        self.rule_info_ = {}
-        self.coefficients_ = Coefficients()
-
-        self._is_fitted: bool = False
-        self.majority_class_: int = None
-        self.majority_probability_: float = None
-        self.k_: float = None
-        self.classes_: np.array = None
-        self.rule_columns_: np.array = None
-
-    def _cleanup(self) -> None:
-        """
-        Clean up the model by resetting all of its attributes.
-        """
-        # Resetting all dictionaries
-        self.decision_trees_ = {}
-        self.decision_rules_ = {}
-        self.rule_info_ = {}
-
-        # Cleaning up coefficients
-        self.coefficients_.cleanup()
-
-        # Resetting the random number generator
-        self._rng = np.random.default_rng(self.random_state)
-
-    @abstractmethod
-    def _get_rule(self, *arg, **kwargs) -> Rule: ...
-
-    @abstractmethod
-    def _get_matrix(self, *arg, **kwargs) -> None: ...
-
-    def _get_class_infos(self, y: np.ndarray) -> None:
-        """
-        Computes and stores information about the classes in the dataset.
-
-        This method calculates the majority class, its probability, the total number
-        of unique classes, and stores an array of unique class labels.
-
-        Parameters
-        ----------
-        y : np.ndarray
-            The target values, expected to be a 1D numpy array of class labels.
-
-        Sets Attributes
-        ---------------
-        majority_class_ : int
-            The class label with the highest frequency in `y`.
-        majority_probability_ : float
-            The proportion of samples in `y` belonging to the majority class,
-            calculated as the count of the majority class divided by the total number of samples.
-        k_ : float
-            The total number of unique classes in `y`.
-        classes_ : np.array
-            An array of the unique class labels present in the dataset.
-        """
-        classes, class_counts = np.unique(y, return_counts=True)
-
-        self.majority_class_ = classes[np.argmax(class_counts)]
-        self.majority_probability_ = class_counts / np.sum(class_counts)
-
-        self.k_ = classes.shape[0]
-        self.classes_ = classes
-
-    def _preprocess(self, y: np.ndarray) -> np.ndarray:
-        """
-        Transforms the target values into a vector. If the target
-        class is k and there are K classes, then all components but
-        the kth are set to -1/(K-1) and the kth component is set to 1.
-
-        Parameters
-        ----------
-        y : np.ndarray
-            The target values as a 1D numpy array of class labels.
-
-        Returns
-        -------
-        np.ndarray
-            The preprocessed target values in a one-hot-encoded format, adjusted for the model's
-            optimization process.
-        """
-
-        # Convert the labels into kth unit vector
-        vec_y = np.eye(self.k_)[y]
-
-        # Replace 0s with -1/(K-1)
-        vec_y[vec_y == 0] = -1 / (self.k_ - 1)
-
-        return vec_y
-
-    def _get_rule_cost(
-        self, temp_rule: Rule, covers: np.ndarray, counts: np.ndarray, y: np.ndarray
-    ) -> float:
-        """
-        Calculates the cost of a rule.
-
-        Depending on the `rule_cost` attribute, this method either calls a custom cost
-        function defined in a `RuleCost` instance or returns a fixed cost for the rule.
-
-        Parameters
-        ----------
-        temp_rule : Rule
-            The rule for which the cost is being calculated.
-        covers : np.ndarray
-            An array indicating whether each instance in the dataset is covered by the rule.
-        counts : np.ndarray
-            An array indicating the count of instances covered by the rule, segmented by class.
-        y : np.ndarray
-            The target array, containing the actual class labels of the instances.
-
-        Returns
-        -------
-        float
-            The calculated cost of the rule.
-        """
-
-        if isinstance(self.rule_cost, RuleCost):
-            return self.rule_cost(
-                temp_rule=temp_rule, covers=covers, counts=counts, y=y
-            )
-        elif isinstance(self.rule_cost, (int, float)):
-            return self.rule_cost
-        else:
-            raise TypeError(
-                f"Unsupported type for `rule_cost`: {type(self.rule_cost)}.",
-                "Expected a RuleCost instance or an int.",
-            )
-
-    def _fill_rules(self, weights: np.ndarray) -> None:
-        """
-        Selects and stores rules based on their weights and a predefined threshold.
-
-        Parameters
-        ----------
-        weights : np.ndarray
-            An array containing the weights of each rule.
-
-        Modifies
-        --------
-        rule_columns_ : np.ndarray
-            Updated to include indices of the selected rules, ordered by their weight.
-        decision_rules_ : Dict[int, Rule]
-            Populated with the selected and ordered rules, keyed by their new indices.
-        """
-        # Scale the weights
-        max_weight = np.max(weights)
-        if max_weight != 1 and max_weight > 1.0e-6:
-            weights = np.divide(weights, max_weight)
-
-        # Select columns where weights are above the threshold
-        selected_columns = np.where(weights > self.threshold)[0]
-
-        # Order the selected columns by their weights
-        weight_order = np.argsort(-weights[selected_columns])
-        ordered_columns = selected_columns[weight_order]
-
-        # Assign the ordered columns to the class attribute
-        self.rule_columns_ = ordered_columns
-
-        # Iterate over the columns and fill the rules dictionary
-        for i, col in enumerate(ordered_columns):
-            treeno, leafno, label, sdist = self.rule_info_[col]
-            fit_tree = self.decision_trees_[treeno]
-            rule = self._get_rule(fit_tree, leafno)
-            if len(rule) > 0:
-                rule.label = label
-                rule.weight = weights[col]
-                rule.sdist = sdist
-                self.decision_rules_[i] = rule
-
-    def _predict_base(
-        self,
-        x: np.ndarray,
-        indices: list = None,
-        threshold: float = 0,
-        *,
-        predict_info=False,
-    ) -> np.ndarray:
-        """
-        Calculates the base class weights for each instance based on selected rules.
-        Optionally returns additional prediction info.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The feature matrix for the instances to predict.
-        indices : list, optional
-            Specific indices of rules to use for prediction. If None, all rules
-            are used.
-        threshold : float, default=0
-            The threshold for selecting rules based on their weights.
-        predict_info : bool, default=False
-            If True, returns additional information about the prediction process
-            including indices of samples with missed values, number of rules
-            applied per sample, and average rule length per sample. Otherwise,
-            returns only the array of raw class weights.
-
-        Returns
-        -------
-        np.ndarray
-            An array of raw class weights for each instance, used as the basis for final
-            prediction.
-            If predict_info is True, also returns arrays containing indices of samples
-            with missed values, number of rules applied per sample, and average rule
-            length per sample.
-        """
-
-        # Check if the model has been fitted
-        if indices is None:
-            indices = []
-
-        if not self._is_fitted:
-            raise ValueError("You need to fit the RUG model first")
-
-        # If no specific indices are provided, use all rule indices
-        if len(indices) == 0:
-            indices = list(self.decision_rules_.keys())
-
-        # If provided indices exceed the available rules, return a warning
-        elif np.max(indices) > len(self.decision_rules_):
-            raise ValueError(f"There are only {len(self.decision_rules_)} rules")
-
-        selected_rules = []
-        for rule_index in indices:
-            rule = self.decision_rules_[rule_index]
-            if rule.weight >= threshold:
-                selected_rules.append(rule)
-
-        rule_matrix = np.zeros((x.shape[0], len(selected_rules)), dtype=np.int8)
-        rule_weights = np.zeros(len(selected_rules), dtype=np.float32)
-        rule_lengths = np.zeros(len(selected_rules), dtype=np.uint8)
-        rule_labels = np.zeros(len(selected_rules), dtype=np.uint8)
-
-        for rule_index, rule in enumerate(selected_rules):
-            rule_weights[rule_index] = rule.weight
-            rule_lengths[rule_index] = len(rule)
-            rule_labels[rule_index] = rule.label
-            rule_matrix[:, rule_index] = rule.check_rule(x)
-
-        sum_class_weights_arr = np.zeros(shape=(x.shape[0], self.k_), dtype=np.float32)
-
-        weights_matrix = rule_matrix * rule_weights
-        for rule_label in range(self.k_):
-            selected_rules_indexs = np.where(rule_labels == rule_label)[0]
-            sum_class_weights_arr[:, rule_label] = np.sum(
-                weights_matrix[:, selected_rules_indexs], axis=1
-            )
-
-        # Return the array of class weights
-        if predict_info:
-            warnings.warn(
-                "Enabling 'predict_info' will return additional prediction "
-                "details, including indices of samples with missed values, "
-                "number of rules applied per sample, and average rule length "
-                "per sample. While this information is useful for in-depth "
-                "analysis, it may increase computational overhead and complexity "
-                "of result interpretation. Use this feature judiciously."
-            )
-            rules_per_sample_ = np.sum(rule_matrix, axis=1)
-            missed_values_index_ = np.where(rules_per_sample_ == 0)[0]
-
-            non_zero_mask = rule_matrix != 0
-            applied_rule_lengts = np.sum(
-                rule_matrix * rule_lengths, axis=1, where=non_zero_mask
-            )
-            applied_rule_number = np.sum(non_zero_mask, axis=1, dtype=np.float32)
-
-            rule_length_per_sample_ = np.divide(
-                applied_rule_lengts,
-                applied_rule_number,
-                where=applied_rule_number != 0,
-                out=np.zeros_like(applied_rule_number, dtype=np.float32),
-            )
-
-            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
-
-        else:
-            return sum_class_weights_arr
-
-    def predict(
-        self,
-        x: ArrayLike,
-        indices: list | None = None,
-        threshold: float = 0.0,
-        *,
-        predict_info: bool = False,
-    ) -> np.ndarray:
-        """
-        Predicts class labels for the given data, optionally returning
-        additional prediction info.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        indices : list or None, default=None
-            Specific indices of rules to use for prediction. If None,
-            all rules are used.
-        threshold : float, default=0
-            The threshold for selecting rules based on their weights.
-        predict_info : bool, default=False
-            If True, returns additional information about the prediction
-            process including indices of samples with missed values, number
-            of rules applied per sample, and average rule length per sample.
-            Otherwise, returns only the predicted class labels.
-
-        Returns
-        -------
-        np.ndarray
-            An array of predicted class labels for each instance in `x`.
-            If predict_info is True, also returns arrays containing indices
-            of samples with missed values, number of rules applied per sample,
-            and average rule length per sample.
-        """
-
-        if indices is None:
-            indices = []
-
-        x = check_inputs(x)
-
-        if predict_info:
-            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
-                self._predict_base(x, indices, threshold, predict_info=predict_info)
-            )
-            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
-
-        else:
-            sum_class_weights_arr = self._predict_base(
-                x, indices, threshold, predict_info=predict_info
-            )
-
-            near_zero_mask = np.sum(sum_class_weights_arr, axis=1) <= 1e-6
-            predictions = np.argmax(sum_class_weights_arr, axis=1)
-            predictions[near_zero_mask] = self.majority_class_
-
-            return predictions
-
-    def predict_proba(
-        self,
-        x: ArrayLike,
-        indices: list | None = None,
-        threshold: float = 0.0,
-        *,
-        predict_info: bool = False,
-    ):
-        """
-        Predicts class probabilities for the given data, optionally
-        returning additional prediction info.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        indices : list or None, default=None
-            Specific indices of rules to use for calculating probabilities.
-            If None, all rules are used.
-        threshold : float, default=0
-            The threshold for selecting rules based on their weights.
-        predict_info : bool, default=False
-            If True, returns additional information about the prediction process
-            including indices of samples with missed values, number of rules applied
-            per sample, and average rule length per sample. Otherwise, returns only
-            the probabilities of each class for each sample.
-
-        Returns
-        -------
-        np.ndarray
-            An array where each row corresponds to a sample in `x` and each column
-            to a class, containing the probability of each class for each sample.
-            If predict_info is True, also returns arrays containing indices of samples
-            with missed values, number of rules applied per sample, and average rule
-            length per sample.
-        """
-
-        if indices is None:
-            indices = []
-
-        x = check_inputs(x)
-
-        if predict_info:
-            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
-                self._predict_base(x, indices, threshold, predict_info=predict_info)
-            )
-            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
-
-        else:
-            sum_class_weights_arr = self._predict_base(
-                x, indices, threshold, predict_info=predict_info
-            )
-
-            total_weights = np.sum(sum_class_weights_arr, axis=1)
-            near_zero_total_weight = total_weights <= 1e-6
-            predictions = np.divide(sum_class_weights_arr, total_weights.reshape(-1, 1))
-            predictions[near_zero_total_weight, :] = self.majority_probability_
-
-            return predictions
-
-    def _get_sample_weight(self, sample_weight, y):
-        """
-        Calculates the final sample weights based on initial sample weights, class weights and
-        target values.
-
-        Parameters
-        ----------
-        sample_weight : array-like, shape (n_samples,) or None
-            Initial weights of samples. If None, all samples are assumed to have weight one.
-        class_weight : dict, "balanced" or None
-            Weights associated with classes in the form {class_label: weight}. Can be "balanced"
-            to automatically adjust weights inversely proportional to class frequencies in the input data
-            or None for equal weights.
-        y : array-like, shape (n_samples,)
-            Array of target values (class labels).
-
-        Returns
-        -------
-        final_sample_weights : array-like, shape (n_samples,) or None
-            The computed array of weights for each sample in the dataset. Returns None if all computed
-            weights are equal to one, indicating no weighting is necessary.
-        """
-        final_sample_weights = np.ones_like(y, dtype=np.float32)
-
-        if sample_weight is not None:
-            sample_weight = check_sample_weight(sample_weight)
-            if (
-                sample_weight.shape != y.shape
-                or sample_weight.min() < 0
-            ):
-                raise ValueError(
-                    "sample_weight must be a non-negative numpy array of the same shape as y."
-                )
-
-
-            final_sample_weights *= sample_weight
-
-        if self.class_weight is not None:
-            if isinstance(self.class_weight, dict):
-                if len(self.class_weight.keys()) != np.unique(y).size:
-                    raise ValueError(
-                        "The class_weight dictionary must have a key for each unique value in y."
-                    )
-
-            final_sample_weights *= compute_sample_weight(self.class_weight, y)
-
-        return final_sample_weights
-
-    def _validate_rug_parameters(
-        self,
-        threshold: float,
-        solver: OptimizationSolver,
-        class_weight: Dict[int:float],
-        random_state: int | None,
-        rule_cost,
-    ):
-        if not isinstance(threshold, (float, int)) or threshold < 0:
-            raise TypeError("threshold must be a non-negative float or integer.")
-
-        if not isinstance(solver, (OptimizationSolver)):
-            raise TypeError("solver should be inherited from OptimizationSolver.")
-
-        if not (isinstance(random_state, int) or random_state is None):
-            raise TypeError("random_state must be an integer or None.")
-
-        if not isinstance(rule_cost, (int, RuleCost)):
-            raise TypeError("rule_cost must be an instance of RuleCost or an integer.")
-
-        if isinstance(rule_cost, int) and rule_cost < 0:
-            raise ValueError("If rule_cost is an integer, it must be non-negative.")
-
-        # class_weight check
-        if not isinstance(class_weight, (dict, str, type(None))) or (
-            (type(class_weight) == str) and (class_weight != "balanced")
-        ):
-            raise ValueError("class_weight must be a dictionary, 'balanced', or None.")
-
-        if isinstance(class_weight, dict):
-            if not all(isinstance(k, int) for k in class_weight.keys()):
-                raise ValueError("class_weight keys must be integer.")
-            if not all(isinstance(v, (int, float)) for v in class_weight.values()):
-                raise ValueError("class_weight values must be integer or float.")
-            if any(v < 0 for v in class_weight.values()):
-                raise ValueError("class_weight values must be non-negative.")
-
-    @property
-    def is_fitted(self):
-        """
-        Indicates whether the model is fitted.
-
-        Returns
-        -------
-        bool
-            True if the model is fitted, False otherwise.
-        """
-
-        return self._is_fitted
-
-    @property
-    def decision_rules(self):
-        """
-        Returns the rules extracted from the decision trees, after optimization.
-
-        Returns
-        -------
-        Dict[int, Rule]
-            A dictionary where keys are rule indices and values are Rule objects.
-        """
-
-        return self.decision_rules_
-
-    @property
-    def decision_trees(self):
-        """
-        Returns dictionary that stores the decision tree models.
-
-        Returns
-        -------
-        Dict[int, Any]
-            A dictionary containing decision tree models, with identifiers as keys
-            and decision
-            tree instances as values.
-        """
-        return self.decision_trees_
-
-    @property
-    def rule_info(self):
-        """
-        Returns information about each rule.
-
-        Returns
-        -------
-        Dict[int, Tuple[int, int, int, np.ndarray]]
-            A dictionary with rule indices as keys and tuples containing information about
-            each rule as values. The tuple structure is (rule_id, feature_index, threshold,
-            values_array).
-        """
-
-        return self.rule_info_
-
-    @property
-    def coefficients(self):
-        """
-        Stores coefficients associated with the rules during optimization.
-
-        Returns
-        -------
-        Coefficients
-            An object or array-like structure storing coefficients related to each rule.
-        """
-
-        return self.coefficients_
-
-    @property
-    def majority_class(self):
-        """
-        Returns the class label of the majority class in the dataset.
-
-        Returns
-        -------
-        int
-            The label of the majority class.
-        """
-
-        return self.majority_class_
-
-    @property
-    def majority_probability(self):
-        """
-        Returns the probability of the majority class in the dataset.
-
-        Returns
-        -------
-        float
-            The probability of encountering the majority class in the dataset.
-        """
-
-        return self.majority_probability_
-
-    @property
-    def k(self):
-        """
-        Returns the total number of unique classes in the dataset.
-
-        Returns
-        -------
-        float
-            The total number of unique classes.
-        """
-
-        return self.k_
-
-    @property
-    def classes(self):
-        """
-        Returns unique class labels in the dataset.
-
-        Returns
-        -------
-        np.ndarray
-            An array containing the unique class labels of the dataset.
-        """
-
-        return self.classes_
-
-    @property
-    def rule_columns(self):
-        """
-        Returns indices of rules selected as part of the model.
-
-        Returns
-        -------
-        np.ndarray
-            An array of indices corresponding to the rules included in the model.
-        """
-
-        return self.rule_columns_
+from __future__ import annotations
+import warnings
+from typing import Union, Dict
+from abc import abstractmethod
+import numpy as np
+from numpy.typing import ArrayLike
+from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn.utils.class_weight import compute_sample_weight
+
+from ..aux_classes import Coefficients, Rule
+from ..rule_cost import RuleCost
+from ..utils import check_inputs, check_sample_weight
+from ..solver.base import OptimizationSolver
+
+
+
+class _RUGBASE(BaseEstimator, ClassifierMixin):
+    """
+    The foundational class for all estimators in the ruleopt library. `_RUGBASE` provides
+    the core framework that every model in ruleopt builds upon.
+
+    Parameters
+    ----------
+    solver : OptimizationSolver
+        An instance of a derived class inherits from the 'Optimization Solver' base class.
+        The solver is responsible for optimizing the rule set based on the cost function
+        and constraints.
+
+    rule_cost : RuleCost or int
+        Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+        or a fixed cost
+
+    class_weight: dict, "balanced" or None
+        A dictionary mapping class labels to their respective weights, the string "balanced"
+        to automatically adjust weights inversely proportional to class frequencies,
+        or None for no weights. Used to adjust the model in favor of certain classes.
+
+    threshold : float
+        The minimum weight threshold for including a rule in the final model
+
+    random_state : int or None, default=None
+        Seed for the random number generator to ensure reproducible results.
+    """
+
+    def __init__(
+        self,
+        solver: OptimizationSolver,
+        rule_cost: Union[RuleCost, int],
+        class_weight: Dict[int, float],
+        threshold: float,
+        random_state: Union[None, int],
+    ):
+
+        self._validate_rug_parameters(
+            threshold=threshold,
+            random_state=random_state,
+            rule_cost=rule_cost,
+            solver=solver,
+            class_weight=class_weight,
+        )
+        self.threshold = float(threshold)
+        self.rule_cost = rule_cost
+        self.solver = solver
+        self.random_state = random_state
+        self.class_weight = class_weight
+
+        # Additional initializations
+        self._rng = np.random.default_rng(
+            random_state if random_state is not None else None
+        )
+        self.decision_trees_ = {}
+        self.decision_rules_ = {}
+        self.rule_info_ = {}
+        self.coefficients_ = Coefficients()
+
+        self._is_fitted: bool = False
+        self.majority_class_: int = None
+        self.majority_probability_: float = None
+        self.k_: float = None
+        self.classes_: np.array = None
+        self.rule_columns_: np.array = None
+
+    def _cleanup(self) -> None:
+        """
+        Clean up the model by resetting all of its attributes.
+        """
+        # Resetting all dictionaries
+        self.decision_trees_ = {}
+        self.decision_rules_ = {}
+        self.rule_info_ = {}
+
+        # Cleaning up coefficients
+        self.coefficients_.cleanup()
+
+        # Resetting the random number generator
+        self._rng = np.random.default_rng(self.random_state)
+
+    @abstractmethod
+    def _get_rule(self, *arg, **kwargs) -> Rule: ...
+
+    @abstractmethod
+    def _get_matrix(self, *arg, **kwargs) -> None: ...
+
+    def _get_class_infos(self, y: np.ndarray) -> None:
+        """
+        Computes and stores information about the classes in the dataset.
+
+        This method calculates the majority class, its probability, the total number
+        of unique classes, and stores an array of unique class labels.
+
+        Parameters
+        ----------
+        y : np.ndarray
+            The target values, expected to be a 1D numpy array of class labels.
+
+        Sets Attributes
+        ---------------
+        majority_class_ : int
+            The class label with the highest frequency in `y`.
+        majority_probability_ : float
+            The proportion of samples in `y` belonging to the majority class,
+            calculated as the count of the majority class divided by the total number of samples.
+        k_ : float
+            The total number of unique classes in `y`.
+        classes_ : np.array
+            An array of the unique class labels present in the dataset.
+        """
+        classes, class_counts = np.unique(y, return_counts=True)
+
+        self.majority_class_ = classes[np.argmax(class_counts)]
+        self.majority_probability_ = class_counts / np.sum(class_counts)
+
+        self.k_ = classes.shape[0]
+        self.classes_ = classes
+
+    def _preprocess(self, y: np.ndarray) -> np.ndarray:
+        """
+        Transforms the target values into a vector. If the target
+        class is k and there are K classes, then all components but
+        the kth are set to -1/(K-1) and the kth component is set to 1.
+
+        Parameters
+        ----------
+        y : np.ndarray
+            The target values as a 1D numpy array of class labels.
+
+        Returns
+        -------
+        np.ndarray
+            The preprocessed target values in a one-hot-encoded format, adjusted for the model's
+            optimization process.
+        """
+
+        # Convert the labels into kth unit vector
+        vec_y = np.eye(self.k_)[y]
+
+        # Replace 0s with -1/(K-1)
+        vec_y[vec_y == 0] = -1 / (self.k_ - 1)
+
+        return vec_y
+
+    def _get_rule_cost(
+        self, temp_rule: Rule, covers: np.ndarray, counts: np.ndarray, y: np.ndarray
+    ) -> float:
+        """
+        Calculates the cost of a rule.
+
+        Depending on the `rule_cost` attribute, this method either calls a custom cost
+        function defined in a `RuleCost` instance or returns a fixed cost for the rule.
+
+        Parameters
+        ----------
+        temp_rule : Rule
+            The rule for which the cost is being calculated.
+        covers : np.ndarray
+            An array indicating whether each instance in the dataset is covered by the rule.
+        counts : np.ndarray
+            An array indicating the count of instances covered by the rule, segmented by class.
+        y : np.ndarray
+            The target array, containing the actual class labels of the instances.
+
+        Returns
+        -------
+        float
+            The calculated cost of the rule.
+        """
+
+        if isinstance(self.rule_cost, RuleCost):
+            return self.rule_cost(
+                temp_rule=temp_rule, covers=covers, counts=counts, y=y
+            )
+        elif isinstance(self.rule_cost, (int, float)):
+            return self.rule_cost
+        else:
+            raise TypeError(
+                f"Unsupported type for `rule_cost`: {type(self.rule_cost)}.",
+                "Expected a RuleCost instance or an int.",
+            )
+
+    def _fill_rules(self, weights: np.ndarray) -> None:
+        """
+        Selects and stores rules based on their weights and a predefined threshold.
+
+        Parameters
+        ----------
+        weights : np.ndarray
+            An array containing the weights of each rule.
+
+        Modifies
+        --------
+        rule_columns_ : np.ndarray
+            Updated to include indices of the selected rules, ordered by their weight.
+        decision_rules_ : Dict[int, Rule]
+            Populated with the selected and ordered rules, keyed by their new indices.
+        """
+        # Scale the weights
+        max_weight = np.max(weights)
+        if max_weight != 1 and max_weight > 1.0e-6:
+            weights = np.divide(weights, max_weight)
+
+        # Select columns where weights are above the threshold
+        selected_columns = np.where(weights > self.threshold)[0]
+
+        # Order the selected columns by their weights
+        weight_order = np.argsort(-weights[selected_columns])
+        ordered_columns = selected_columns[weight_order]
+
+        # Assign the ordered columns to the class attribute
+        self.rule_columns_ = ordered_columns
+
+        # Iterate over the columns and fill the rules dictionary
+        for i, col in enumerate(ordered_columns):
+            treeno, leafno, label, sdist = self.rule_info_[col]
+            fit_tree = self.decision_trees_[treeno]
+            rule = self._get_rule(fit_tree, leafno)
+            if len(rule) > 0:
+                rule.label = label
+                rule.weight = weights[col]
+                rule.sdist = sdist
+                self.decision_rules_[i] = rule
+
+    def _predict_base(
+        self,
+        x: np.ndarray,
+        indices: list = None,
+        threshold: float = 0,
+        *,
+        predict_info=False,
+    ) -> np.ndarray:
+        """
+        Calculates the base class weights for each instance based on selected rules.
+        Optionally returns additional prediction info.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The feature matrix for the instances to predict.
+        indices : list, optional
+            Specific indices of rules to use for prediction. If None, all rules
+            are used.
+        threshold : float, default=0
+            The threshold for selecting rules based on their weights.
+        predict_info : bool, default=False
+            If True, returns additional information about the prediction process
+            including indices of samples with missed values, number of rules
+            applied per sample, and average rule length per sample. Otherwise,
+            returns only the array of raw class weights.
+
+        Returns
+        -------
+        np.ndarray
+            An array of raw class weights for each instance, used as the basis for final
+            prediction.
+            If predict_info is True, also returns arrays containing indices of samples
+            with missed values, number of rules applied per sample, and average rule
+            length per sample.
+        """
+
+        # Check if the model has been fitted
+        if indices is None:
+            indices = []
+
+        if not self._is_fitted:
+            raise ValueError("You need to fit the RUG model first")
+
+        # If no specific indices are provided, use all rule indices
+        if len(indices) == 0:
+            indices = list(self.decision_rules_.keys())
+
+        # If provided indices exceed the available rules, return a warning
+        elif np.max(indices) > len(self.decision_rules_):
+            raise ValueError(f"There are only {len(self.decision_rules_)} rules")
+
+        selected_rules = []
+        for rule_index in indices:
+            rule = self.decision_rules_[rule_index]
+            if rule.weight >= threshold:
+                selected_rules.append(rule)
+
+        rule_matrix = np.zeros((x.shape[0], len(selected_rules)), dtype=np.int8)
+        rule_weights = np.zeros(len(selected_rules), dtype=np.float32)
+        rule_lengths = np.zeros(len(selected_rules), dtype=np.uint8)
+        rule_labels = np.zeros(len(selected_rules), dtype=np.uint8)
+
+        for rule_index, rule in enumerate(selected_rules):
+            rule_weights[rule_index] = rule.weight
+            rule_lengths[rule_index] = len(rule)
+            rule_labels[rule_index] = rule.label
+            rule_matrix[:, rule_index] = rule.check_rule(x)
+
+        sum_class_weights_arr = np.zeros(shape=(x.shape[0], self.k_), dtype=np.float32)
+
+        weights_matrix = rule_matrix * rule_weights
+        for rule_label in range(self.k_):
+            selected_rules_indexs = np.where(rule_labels == rule_label)[0]
+            sum_class_weights_arr[:, rule_label] = np.sum(
+                weights_matrix[:, selected_rules_indexs], axis=1
+            )
+
+        # Return the array of class weights
+        if predict_info:
+            warnings.warn(
+                "Enabling 'predict_info' will return additional prediction "
+                "details, including indices of samples with missed values, "
+                "number of rules applied per sample, and average rule length "
+                "per sample. While this information is useful for in-depth "
+                "analysis, it may increase computational overhead and complexity "
+                "of result interpretation. Use this feature judiciously."
+            )
+            rules_per_sample_ = np.sum(rule_matrix, axis=1)
+            missed_values_index_ = np.where(rules_per_sample_ == 0)[0]
+
+            non_zero_mask = rule_matrix != 0
+            applied_rule_lengts = np.sum(
+                rule_matrix * rule_lengths, axis=1, where=non_zero_mask
+            )
+            applied_rule_number = np.sum(non_zero_mask, axis=1, dtype=np.float32)
+
+            rule_length_per_sample_ = np.divide(
+                applied_rule_lengts,
+                applied_rule_number,
+                where=applied_rule_number != 0,
+                out=np.zeros_like(applied_rule_number, dtype=np.float32),
+            )
+
+            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
+
+        else:
+            return sum_class_weights_arr
+
+    def predict(
+        self,
+        x: ArrayLike,
+        indices: list | None = None,
+        threshold: float = 0.0,
+        *,
+        predict_info: bool = False,
+    ) -> np.ndarray:
+        """
+        Predicts class labels for the given data, optionally returning
+        additional prediction info.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        indices : list or None, default=None
+            Specific indices of rules to use for prediction. If None,
+            all rules are used.
+        threshold : float, default=0
+            The threshold for selecting rules based on their weights.
+        predict_info : bool, default=False
+            If True, returns additional information about the prediction
+            process including indices of samples with missed values, number
+            of rules applied per sample, and average rule length per sample.
+            Otherwise, returns only the predicted class labels.
+
+        Returns
+        -------
+        np.ndarray
+            An array of predicted class labels for each instance in `x`.
+            If predict_info is True, also returns arrays containing indices
+            of samples with missed values, number of rules applied per sample,
+            and average rule length per sample.
+        """
+
+        if indices is None:
+            indices = []
+
+        x = check_inputs(x)
+
+        if predict_info:
+            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
+                self._predict_base(x, indices, threshold, predict_info=predict_info)
+            )
+            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
+
+        else:
+            sum_class_weights_arr = self._predict_base(
+                x, indices, threshold, predict_info=predict_info
+            )
+
+            near_zero_mask = np.sum(sum_class_weights_arr, axis=1) <= 1e-6
+            predictions = np.argmax(sum_class_weights_arr, axis=1)
+            predictions[near_zero_mask] = self.majority_class_
+
+            return predictions
+
+    def predict_proba(
+        self,
+        x: ArrayLike,
+        indices: list | None = None,
+        threshold: float = 0.0,
+        *,
+        predict_info: bool = False,
+    ):
+        """
+        Predicts class probabilities for the given data, optionally
+        returning additional prediction info.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        indices : list or None, default=None
+            Specific indices of rules to use for calculating probabilities.
+            If None, all rules are used.
+        threshold : float, default=0
+            The threshold for selecting rules based on their weights.
+        predict_info : bool, default=False
+            If True, returns additional information about the prediction process
+            including indices of samples with missed values, number of rules applied
+            per sample, and average rule length per sample. Otherwise, returns only
+            the probabilities of each class for each sample.
+
+        Returns
+        -------
+        np.ndarray
+            An array where each row corresponds to a sample in `x` and each column
+            to a class, containing the probability of each class for each sample.
+            If predict_info is True, also returns arrays containing indices of samples
+            with missed values, number of rules applied per sample, and average rule
+            length per sample.
+        """
+
+        if indices is None:
+            indices = []
+
+        x = check_inputs(x)
+
+        if predict_info:
+            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
+                self._predict_base(x, indices, threshold, predict_info=predict_info)
+            )
+            return missed_values_index_, rules_per_sample_, rule_length_per_sample_
+
+        else:
+            sum_class_weights_arr = self._predict_base(
+                x, indices, threshold, predict_info=predict_info
+            )
+
+            total_weights = np.sum(sum_class_weights_arr, axis=1)
+            near_zero_total_weight = total_weights <= 1e-6
+            predictions = np.divide(sum_class_weights_arr, total_weights.reshape(-1, 1))
+            predictions[near_zero_total_weight, :] = self.majority_probability_
+
+            return predictions
+
+    def _get_sample_weight(self, sample_weight, y):
+        """
+        Calculates the final sample weights based on initial sample weights, class weights and
+        target values.
+
+        Parameters
+        ----------
+        sample_weight : array-like, shape (n_samples,) or None
+            Initial weights of samples. If None, all samples are assumed to have weight one.
+        class_weight : dict, "balanced" or None
+            Weights associated with classes in the form {class_label: weight}. Can be "balanced"
+            to automatically adjust weights inversely proportional to class frequencies in the input data
+            or None for equal weights.
+        y : array-like, shape (n_samples,)
+            Array of target values (class labels).
+
+        Returns
+        -------
+        final_sample_weights : array-like, shape (n_samples,) or None
+            The computed array of weights for each sample in the dataset. Returns None if all computed
+            weights are equal to one, indicating no weighting is necessary.
+        """
+        final_sample_weights = np.ones_like(y, dtype=np.float32)
+
+        if sample_weight is not None:
+            sample_weight = check_sample_weight(sample_weight)
+            if (
+                sample_weight.shape != y.shape
+                or sample_weight.min() < 0
+            ):
+                raise ValueError(
+                    "sample_weight must be a non-negative numpy array of the same shape as y."
+                )
+
+
+            final_sample_weights *= sample_weight
+
+        if self.class_weight is not None:
+            if isinstance(self.class_weight, dict):
+                if len(self.class_weight.keys()) != np.unique(y).size:
+                    raise ValueError(
+                        "The class_weight dictionary must have a key for each unique value in y."
+                    )
+
+            final_sample_weights *= compute_sample_weight(self.class_weight, y)
+
+        return final_sample_weights
+
+    def _validate_rug_parameters(
+        self,
+        threshold: float,
+        solver: OptimizationSolver,
+        class_weight: Dict[int:float],
+        random_state: int | None,
+        rule_cost,
+    ):
+        if not isinstance(threshold, (float, int)) or threshold < 0:
+            raise TypeError("threshold must be a non-negative float or integer.")
+
+        if not isinstance(solver, (OptimizationSolver)):
+            raise TypeError("solver should be inherited from OptimizationSolver.")
+
+        if not (isinstance(random_state, int) or random_state is None):
+            raise TypeError("random_state must be an integer or None.")
+
+        if not isinstance(rule_cost, (int, RuleCost)):
+            raise TypeError("rule_cost must be an instance of RuleCost or an integer.")
+
+        if isinstance(rule_cost, int) and rule_cost < 0:
+            raise ValueError("If rule_cost is an integer, it must be non-negative.")
+
+        # class_weight check
+        if not isinstance(class_weight, (dict, str, type(None))) or (
+            (type(class_weight) == str) and (class_weight != "balanced")
+        ):
+            raise ValueError("class_weight must be a dictionary, 'balanced', or None.")
+
+        if isinstance(class_weight, dict):
+            if not all(isinstance(k, int) for k in class_weight.keys()):
+                raise ValueError("class_weight keys must be integer.")
+            if not all(isinstance(v, (int, float)) for v in class_weight.values()):
+                raise ValueError("class_weight values must be integer or float.")
+            if any(v < 0 for v in class_weight.values()):
+                raise ValueError("class_weight values must be non-negative.")
+
+    @property
+    def is_fitted(self):
+        """
+        Indicates whether the model is fitted.
+
+        Returns
+        -------
+        bool
+            True if the model is fitted, False otherwise.
+        """
+
+        return self._is_fitted
+
+    @property
+    def decision_rules(self):
+        """
+        Returns the rules extracted from the decision trees, after optimization.
+
+        Returns
+        -------
+        Dict[int, Rule]
+            A dictionary where keys are rule indices and values are Rule objects.
+        """
+
+        return self.decision_rules_
+
+    @property
+    def decision_trees(self):
+        """
+        Returns dictionary that stores the decision tree models.
+
+        Returns
+        -------
+        Dict[int, Any]
+            A dictionary containing decision tree models, with identifiers as keys
+            and decision
+            tree instances as values.
+        """
+        return self.decision_trees_
+
+    @property
+    def rule_info(self):
+        """
+        Returns information about each rule.
+
+        Returns
+        -------
+        Dict[int, Tuple[int, int, int, np.ndarray]]
+            A dictionary with rule indices as keys and tuples containing information about
+            each rule as values. The tuple structure is (rule_id, feature_index, threshold,
+            values_array).
+        """
+
+        return self.rule_info_
+
+    @property
+    def coefficients(self):
+        """
+        Stores coefficients associated with the rules during optimization.
+
+        Returns
+        -------
+        Coefficients
+            An object or array-like structure storing coefficients related to each rule.
+        """
+
+        return self.coefficients_
+
+    @property
+    def majority_class(self):
+        """
+        Returns the class label of the majority class in the dataset.
+
+        Returns
+        -------
+        int
+            The label of the majority class.
+        """
+
+        return self.majority_class_
+
+    @property
+    def majority_probability(self):
+        """
+        Returns the probability of the majority class in the dataset.
+
+        Returns
+        -------
+        float
+            The probability of encountering the majority class in the dataset.
+        """
+
+        return self.majority_probability_
+
+    @property
+    def k(self):
+        """
+        Returns the total number of unique classes in the dataset.
+
+        Returns
+        -------
+        float
+            The total number of unique classes.
+        """
+
+        return self.k_
+
+    @property
+    def classes(self):
+        """
+        Returns unique class labels in the dataset.
+
+        Returns
+        -------
+        np.ndarray
+            An array containing the unique class labels of the dataset.
+        """
+
+        return self.classes_
+
+    @property
+    def rule_columns(self):
+        """
+        Returns indices of rules selected as part of the model.
+
+        Returns
+        -------
+        np.ndarray
+            An array of indices corresponding to the rules included in the model.
+        """
+
+        return self.rule_columns_
```

## ruleopt/estimator/lightgbm_.py

 * *Ordering differences only*

```diff
@@ -1,332 +1,332 @@
-from __future__ import annotations
-import numpy as np
-from numpy.typing import ArrayLike
-
-from .base import _RUGBASE
-from ..aux_classes import Rule
-from ..rule_cost import Gini
-from ..utils import check_module_available, check_inputs
-from ..solver import ORToolsSolver
-
-LIGHTGBM_AVAILABLE = check_module_available("lightgbm")
-
-
-class RUXLGBMClassifier(_RUGBASE):
-    """
-    A classifier that extracts and optimizes decision rules from a trained
-    LightGBM ensemble model to create a compact and interpretable model.
-    This process involves translating the ensemble's trees into a set of rules and
-    using optimization to balance model accuracy and interpretability. The complexity
-    of the resulting rule-based model is  controlled through a penalty parameter.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if not LIGHTGBM_AVAILABLE:
-            raise ImportError(
-                "LightGBM is required for this class but is not installed.",
-                "Please install it with 'pip install lightgbm'",
-            )
-        instance = super(RUXLGBMClassifier, cls).__new__(cls)
-        return instance
-
-    def __init__(
-        self,
-        trained_ensemble,
-        *,
-        solver=ORToolsSolver(),
-        rule_cost=Gini(),
-        class_weight: dict | str | None = None,
-        threshold: float = 1.0e-6,
-        random_state: int | None = None,
-    ):
-        """
-        Parameters
-        ----------
-        trained_ensemble : lightgbm.LGBMClassifier or lightgbm.Booster
-            The trained LightGBM ensemble model from which the rules will be extracted.
-
-        solver : OptimizationSolver, default=ORToolsSolver()
-            An instance of a derived class inherits from the 'Optimization Solver' base class.
-            The solver is responsible for optimizing the rule set based on the cost function
-            and constraints.
-
-        rule_cost : RuleCost or int, default=Gini()
-            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-            or a fixed cost
-
-        class_weight: dict, "balanced" or None, default=None
-            A dictionary mapping class labels to their respective weights, the string "balanced"
-            to automatically adjust weights inversely proportional to class frequencies,
-            or None for no weights. Used to adjust the model in favor of certain classes.
-
-        threshold : float, default=1.0e-6
-            The minimum weight threshold for including a rule in the final model.
-
-        random_state : int or None, default=None
-            Seed for the random number generator to ensure reproducible results.
-        """
-        ### LAZY INIT
-        from lightgbm import Booster
-
-        if not isinstance(trained_ensemble, Booster):
-            if hasattr(trained_ensemble, "booster_"):
-                if not isinstance(trained_ensemble.booster_, Booster):
-                    raise TypeError("trained_ensemble is not an instance of LightGBM.")
-                else:
-                    self.trained_ensemble = trained_ensemble.booster_
-            else:
-                raise TypeError("trained_ensemble is not an instance of LightGBM")
-        else:
-            self.trained_ensemble = trained_ensemble
-
-        super().__init__(
-            threshold=threshold,
-            random_state=random_state,
-            rule_cost=rule_cost,
-            solver=solver,
-            class_weight=class_weight,
-        )
-
-    def _find_leaf_index(self, fit_tree: dict, leaf_index: int, path=None) -> list:
-        """
-        Recursively finds the path from the root to the specified leaf node in a LightGBM tree.
-
-        Parameters
-        ----------
-        fit_tree : dict
-            The tree dictionary from a LightGBM model.
-        leaf_index : int
-            The target leaf node's ID.
-        path : list, optional
-            The path taken to reach the current node, used in recursive calls. Defaults to None.
-
-        Returns
-        -------
-        list
-            The path from the root to the leaf node, represented as a list of node IDs.
-        """
-        if path is None:
-            path = []
-        if isinstance(fit_tree, dict):
-            # If the current fit_tree is the leaf node we're looking for
-            if "leaf_index" in fit_tree and fit_tree["leaf_index"] == leaf_index:
-                return path
-            # Recursively look in the items of the fit_tree
-            for key, value in fit_tree.items():
-                result = self._find_leaf_index(value, leaf_index, path + [key])
-                if result:
-                    return result
-
-    def _get_rule(self, fit_tree: dict, nodeid: int) -> Rule:
-        """
-        Constructs a rule corresponding to the path leading to a specific leaf node in
-        a LightGBM tree.
-
-        Parameters
-        ----------
-        fit_tree : dict
-            The tree structure extracted from a LightGBM model, typically in JSON format.
-        nodeid : int
-            The unique identifier of the leaf node for which to construct the rule.
-
-        Returns
-        -------
-        Rule
-            An object representing the decision rule leading to the specified leaf node.
-        """
-        # Get the path to the leaf node
-        leaf_path = self._find_leaf_index(fit_tree, nodeid)
-
-        # Initialize the rule
-        return_rule = Rule()
-
-        # child variable is used to track the last traversed node
-        child = None
-
-        # While there are still nodes in the path to the leaf node
-        while leaf_path:
-            fit_tree_ = fit_tree.copy()
-            for path in leaf_path:
-                fit_tree_ = fit_tree_[path]
-
-            # If the current node is a split node, add a clause to the rule
-            if "split_feature" in fit_tree_.keys():
-                # Check which child node we're coming from
-                is_left = child == "left_child"
-                # Get the threshold for the split
-                threshold = fit_tree_["threshold"]
-                # Get the default path in case of missing values
-                missing = (is_left and fit_tree_["default_left"]) or (
-                    child == "right_child" and not fit_tree_["default_left"]
-                )
-
-                feature = fit_tree_["split_feature"]
-                ub = threshold if is_left else np.inf
-                lb = -np.inf if is_left else threshold
-                na = missing
-
-                return_rule.add_clause(feature, ub, lb, na)
-
-            # Move to the next node in the path
-            child = leaf_path.pop()
-
-        return return_rule
-
-    def _get_matrix(
-        self,
-        y: np.ndarray,
-        vec_y: np.ndarray,
-        fit_tree: dict,
-        treeno: int,
-        y_rules: np.ndarray,
-    ):
-        """
-        Populates the matrices for the optimization problem based on a single LightGBM tree.
-
-        Parameters
-        ----------
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector, suitable for the optimization problem.
-        fit_tree : dict
-            A single decision tree's structure from LightGBM, in dictionary form.
-        treeno : int
-            The index of the current tree within the ensemble.
-        y_rules : np.ndarray
-            The array of leaf indices for each sample in the training data, determined by
-            the current tree.
-        """
-        # If the coefficients matrix is empty, start from the first column
-        if self.coefficients_.cols.shape[0] == 0:
-            col = 0
-        else:
-            # Otherwise, start from the next available column
-            col = np.max(self.coefficients_.cols) + 1
-
-        # Get the leaf node for each sample in x
-        y_rules = y_rules[:, treeno]
-
-        # Iterate over unique leaf nodes
-        for leafno in np.unique(y_rules):
-            # Get the samples in the leaf
-            covers = np.where(y_rules == leafno)[0]
-            leaf_y_vals = y[covers]  # y values of the samples in the leaf
-
-            # Get unique labels in the leaf and their counts
-            unique_labels, counts = np.unique(leaf_y_vals, return_counts=True)
-
-            # Identify the majority class in the leaf
-            label = unique_labels[np.argmax(counts)]
-
-            # Create a vector for this label
-            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
-            label_vector[label] = 1
-
-            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
-            fill_ahat = np.dot(vec_y[covers, :], label_vector)
-
-            # Update the coefficients matrix with the new information
-            self.coefficients_.rows = np.concatenate((self.coefficients_.rows, covers))
-            self.coefficients_.cols = np.concatenate(
-                (self.coefficients_.cols, [col] * covers.shape[0])
-            )
-            self.coefficients_.yvals = np.concatenate(
-                (self.coefficients_.yvals, np.full(covers.shape[0], fill_ahat))
-            )
-
-            cost = self._get_rule_cost(
-                temp_rule=self._get_rule(fit_tree, leafno),
-                covers=covers,
-                counts=counts,
-                y=y,
-            )
-
-            # Append the cost to the costs in the coefficients matrix
-            self.coefficients_.costs = np.concatenate(
-                (self.coefficients_.costs, [cost])
-            )
-
-            # Calculate the distribution of the samples in the leaf across the classess
-            sdist = counts
-            self.rule_info_[col] = (treeno, leafno, label, sdist)
-            col += 1
-
-    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray):
-        """
-        Generates the coefficient matrices for the optimization problem from all
-        trees in the LightGBM ensemble.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The feature matrix of the training data.
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector.
-        """
-        y_rules = self.trained_ensemble.predict(x, pred_leaf=True).astype(np.intp)
-        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
-            self._get_matrix(y, vec_y, fit_tree, treeno, y_rules)
-
-    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
-        """
-        Fits the RUXLGBMClassifier to the training data, optimizing the
-        extracted rules for a balance between accuracy and interpretability.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels) as integers
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, then samples equal weights.
-
-        Returns
-        -------
-        RUXLGBMClassifier
-            The fitted model, ready for making predictions.
-        """
-
-        x, y = check_inputs(x, y)
-
-        sample_weight = self._get_sample_weight(sample_weight, y)
-
-        # If the model has been fitted before, clean it up
-        if self._is_fitted:
-            self._cleanup()
-
-        # Fills the fitted decision trees.
-        tree_infos = self.trained_ensemble.dump_model()["tree_info"]
-        for treeno, fit_tree in enumerate(tree_infos):
-            self.decision_trees_[treeno] = fit_tree
-
-        # Extract and set properties of the target variable
-        self._get_class_infos(y)
-
-        # Preprocess the target values
-        vec_y = self._preprocess(y)
-
-        # Calculate the coefficients and other parameters for the optimization problem
-        self._get_matrices(x=x, y=y, vec_y=vec_y)
-
-        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
-
-        # Solve the optimization problem again with the new rules
-        ws, *_ = self.solver(
-            coefficients=self.coefficients_,
-            k=self.k_,
-            sample_weight=sample_weight,
-            normalization_constant=normalization_constant,
-        )
-
-        # Fill the decision rules based on the weights obtained from the optimization problem
-        self._fill_rules(ws)
-
-        # Mark the model as fitted
-        self._is_fitted = True
-
-        # Return the fitted model
-        return self
+from __future__ import annotations
+import numpy as np
+from numpy.typing import ArrayLike
+
+from .base import _RUGBASE
+from ..aux_classes import Rule
+from ..rule_cost import Gini
+from ..utils import check_module_available, check_inputs
+from ..solver import ORToolsSolver
+
+LIGHTGBM_AVAILABLE = check_module_available("lightgbm")
+
+
+class RUXLGBMClassifier(_RUGBASE):
+    """
+    A classifier that extracts and optimizes decision rules from a trained
+    LightGBM ensemble model to create a compact and interpretable model.
+    This process involves translating the ensemble's trees into a set of rules and
+    using optimization to balance model accuracy and interpretability. The complexity
+    of the resulting rule-based model is  controlled through a penalty parameter.
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if not LIGHTGBM_AVAILABLE:
+            raise ImportError(
+                "LightGBM is required for this class but is not installed.",
+                "Please install it with 'pip install lightgbm'",
+            )
+        instance = super(RUXLGBMClassifier, cls).__new__(cls)
+        return instance
+
+    def __init__(
+        self,
+        trained_ensemble,
+        *,
+        solver=ORToolsSolver(),
+        rule_cost=Gini(),
+        class_weight: dict | str | None = None,
+        threshold: float = 1.0e-6,
+        random_state: int | None = None,
+    ):
+        """
+        Parameters
+        ----------
+        trained_ensemble : lightgbm.LGBMClassifier or lightgbm.Booster
+            The trained LightGBM ensemble model from which the rules will be extracted.
+
+        solver : OptimizationSolver, default=ORToolsSolver()
+            An instance of a derived class inherits from the 'Optimization Solver' base class.
+            The solver is responsible for optimizing the rule set based on the cost function
+            and constraints.
+
+        rule_cost : RuleCost or int, default=Gini()
+            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+            or a fixed cost
+
+        class_weight: dict, "balanced" or None, default=None
+            A dictionary mapping class labels to their respective weights, the string "balanced"
+            to automatically adjust weights inversely proportional to class frequencies,
+            or None for no weights. Used to adjust the model in favor of certain classes.
+
+        threshold : float, default=1.0e-6
+            The minimum weight threshold for including a rule in the final model.
+
+        random_state : int or None, default=None
+            Seed for the random number generator to ensure reproducible results.
+        """
+        ### LAZY INIT
+        from lightgbm import Booster
+
+        if not isinstance(trained_ensemble, Booster):
+            if hasattr(trained_ensemble, "booster_"):
+                if not isinstance(trained_ensemble.booster_, Booster):
+                    raise TypeError("trained_ensemble is not an instance of LightGBM.")
+                else:
+                    self.trained_ensemble = trained_ensemble.booster_
+            else:
+                raise TypeError("trained_ensemble is not an instance of LightGBM")
+        else:
+            self.trained_ensemble = trained_ensemble
+
+        super().__init__(
+            threshold=threshold,
+            random_state=random_state,
+            rule_cost=rule_cost,
+            solver=solver,
+            class_weight=class_weight,
+        )
+
+    def _find_leaf_index(self, fit_tree: dict, leaf_index: int, path=None) -> list:
+        """
+        Recursively finds the path from the root to the specified leaf node in a LightGBM tree.
+
+        Parameters
+        ----------
+        fit_tree : dict
+            The tree dictionary from a LightGBM model.
+        leaf_index : int
+            The target leaf node's ID.
+        path : list, optional
+            The path taken to reach the current node, used in recursive calls. Defaults to None.
+
+        Returns
+        -------
+        list
+            The path from the root to the leaf node, represented as a list of node IDs.
+        """
+        if path is None:
+            path = []
+        if isinstance(fit_tree, dict):
+            # If the current fit_tree is the leaf node we're looking for
+            if "leaf_index" in fit_tree and fit_tree["leaf_index"] == leaf_index:
+                return path
+            # Recursively look in the items of the fit_tree
+            for key, value in fit_tree.items():
+                result = self._find_leaf_index(value, leaf_index, path + [key])
+                if result:
+                    return result
+
+    def _get_rule(self, fit_tree: dict, nodeid: int) -> Rule:
+        """
+        Constructs a rule corresponding to the path leading to a specific leaf node in
+        a LightGBM tree.
+
+        Parameters
+        ----------
+        fit_tree : dict
+            The tree structure extracted from a LightGBM model, typically in JSON format.
+        nodeid : int
+            The unique identifier of the leaf node for which to construct the rule.
+
+        Returns
+        -------
+        Rule
+            An object representing the decision rule leading to the specified leaf node.
+        """
+        # Get the path to the leaf node
+        leaf_path = self._find_leaf_index(fit_tree, nodeid)
+
+        # Initialize the rule
+        return_rule = Rule()
+
+        # child variable is used to track the last traversed node
+        child = None
+
+        # While there are still nodes in the path to the leaf node
+        while leaf_path:
+            fit_tree_ = fit_tree.copy()
+            for path in leaf_path:
+                fit_tree_ = fit_tree_[path]
+
+            # If the current node is a split node, add a clause to the rule
+            if "split_feature" in fit_tree_.keys():
+                # Check which child node we're coming from
+                is_left = child == "left_child"
+                # Get the threshold for the split
+                threshold = fit_tree_["threshold"]
+                # Get the default path in case of missing values
+                missing = (is_left and fit_tree_["default_left"]) or (
+                    child == "right_child" and not fit_tree_["default_left"]
+                )
+
+                feature = fit_tree_["split_feature"]
+                ub = threshold if is_left else np.inf
+                lb = -np.inf if is_left else threshold
+                na = missing
+
+                return_rule.add_clause(feature, ub, lb, na)
+
+            # Move to the next node in the path
+            child = leaf_path.pop()
+
+        return return_rule
+
+    def _get_matrix(
+        self,
+        y: np.ndarray,
+        vec_y: np.ndarray,
+        fit_tree: dict,
+        treeno: int,
+        y_rules: np.ndarray,
+    ):
+        """
+        Populates the matrices for the optimization problem based on a single LightGBM tree.
+
+        Parameters
+        ----------
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector, suitable for the optimization problem.
+        fit_tree : dict
+            A single decision tree's structure from LightGBM, in dictionary form.
+        treeno : int
+            The index of the current tree within the ensemble.
+        y_rules : np.ndarray
+            The array of leaf indices for each sample in the training data, determined by
+            the current tree.
+        """
+        # If the coefficients matrix is empty, start from the first column
+        if self.coefficients_.cols.shape[0] == 0:
+            col = 0
+        else:
+            # Otherwise, start from the next available column
+            col = np.max(self.coefficients_.cols) + 1
+
+        # Get the leaf node for each sample in x
+        y_rules = y_rules[:, treeno]
+
+        # Iterate over unique leaf nodes
+        for leafno in np.unique(y_rules):
+            # Get the samples in the leaf
+            covers = np.where(y_rules == leafno)[0]
+            leaf_y_vals = y[covers]  # y values of the samples in the leaf
+
+            # Get unique labels in the leaf and their counts
+            unique_labels, counts = np.unique(leaf_y_vals, return_counts=True)
+
+            # Identify the majority class in the leaf
+            label = unique_labels[np.argmax(counts)]
+
+            # Create a vector for this label
+            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
+            label_vector[label] = 1
+
+            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
+            fill_ahat = np.dot(vec_y[covers, :], label_vector)
+
+            # Update the coefficients matrix with the new information
+            self.coefficients_.rows = np.concatenate((self.coefficients_.rows, covers))
+            self.coefficients_.cols = np.concatenate(
+                (self.coefficients_.cols, [col] * covers.shape[0])
+            )
+            self.coefficients_.yvals = np.concatenate(
+                (self.coefficients_.yvals, np.full(covers.shape[0], fill_ahat))
+            )
+
+            cost = self._get_rule_cost(
+                temp_rule=self._get_rule(fit_tree, leafno),
+                covers=covers,
+                counts=counts,
+                y=y,
+            )
+
+            # Append the cost to the costs in the coefficients matrix
+            self.coefficients_.costs = np.concatenate(
+                (self.coefficients_.costs, [cost])
+            )
+
+            # Calculate the distribution of the samples in the leaf across the classess
+            sdist = counts
+            self.rule_info_[col] = (treeno, leafno, label, sdist)
+            col += 1
+
+    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray):
+        """
+        Generates the coefficient matrices for the optimization problem from all
+        trees in the LightGBM ensemble.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The feature matrix of the training data.
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector.
+        """
+        y_rules = self.trained_ensemble.predict(x, pred_leaf=True).astype(np.intp)
+        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
+            self._get_matrix(y, vec_y, fit_tree, treeno, y_rules)
+
+    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
+        """
+        Fits the RUXLGBMClassifier to the training data, optimizing the
+        extracted rules for a balance between accuracy and interpretability.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels) as integers
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples equal weights.
+
+        Returns
+        -------
+        RUXLGBMClassifier
+            The fitted model, ready for making predictions.
+        """
+
+        x, y = check_inputs(x, y)
+
+        sample_weight = self._get_sample_weight(sample_weight, y)
+
+        # If the model has been fitted before, clean it up
+        if self._is_fitted:
+            self._cleanup()
+
+        # Fills the fitted decision trees.
+        tree_infos = self.trained_ensemble.dump_model()["tree_info"]
+        for treeno, fit_tree in enumerate(tree_infos):
+            self.decision_trees_[treeno] = fit_tree
+
+        # Extract and set properties of the target variable
+        self._get_class_infos(y)
+
+        # Preprocess the target values
+        vec_y = self._preprocess(y)
+
+        # Calculate the coefficients and other parameters for the optimization problem
+        self._get_matrices(x=x, y=y, vec_y=vec_y)
+
+        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
+
+        # Solve the optimization problem again with the new rules
+        ws, *_ = self.solver(
+            coefficients=self.coefficients_,
+            k=self.k_,
+            sample_weight=sample_weight,
+            normalization_constant=normalization_constant,
+        )
+
+        # Fill the decision rules based on the weights obtained from the optimization problem
+        self._fill_rules(ws)
+
+        # Mark the model as fitted
+        self._is_fitted = True
+
+        # Return the fitted model
+        return self
```

## ruleopt/estimator/xgboost_.py

 * *Ordering differences only*

```diff
@@ -1,311 +1,311 @@
-from __future__ import annotations
-import re
-import numpy as np
-import pandas as pd
-from numpy.typing import ArrayLike
-
-from .base import _RUGBASE
-from ..aux_classes import Rule
-from ..rule_cost import Gini
-from ..utils import check_module_available, check_inputs
-from ..solver import ORToolsSolver
-
-
-XGBOOST_AVAILABLE = check_module_available("xgboost")
-
-
-class RUXXGBClassifier(_RUGBASE):
-    """
-    A classifier that extracts and optimizes decision rules from a trained
-    XGBoost ensemble model to create a compact and interpretable model.
-    This process involves translating the ensemble's trees into a set of rules and
-    using optimization to balance model accuracy and interpretability. The complexity
-    of the resulting rule-based model is  controlled through a penalty parameter.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if not XGBOOST_AVAILABLE:
-            raise ImportError(
-                "XGBoost is required for this class but is not installed.",
-                "Please install it with 'pip install xgboost'",
-            )
-        instance = super(RUXXGBClassifier, cls).__new__(cls)
-        return instance
-
-    def __init__(
-        self,
-        trained_ensemble,
-        *,
-        solver=ORToolsSolver(),
-        rule_cost=Gini(),
-        class_weight: dict | str | None = None,
-        threshold: float = 1.0e-6,
-        random_state: int | None = None,
-    ):
-        """
-        Parameters
-        ----------
-        trained_ensemble : xgboost.XGBClassifier
-            The trained XGBoost ensemble model from which rules will be extracted.
-            The model should already be trained on the dataset.
-
-        solver : OptimizationSolver, default=ORToolsSolver()
-            An instance of a derived class inherits from the 'Optimization Solver' base class.
-            The solver is responsible for optimizing the rule set based on the cost function
-            and constraints.
-
-        rule_cost : RuleCost or int, default=Gini()
-            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-            or a fixed cost
-
-        class_weight: dict, "balanced" or None, default=None
-            A dictionary mapping class labels to their respective weights, the string "balanced"
-            to automatically adjust weights inversely proportional to class frequencies,
-            or None for no weights. Used to adjust the model in favor of certain classes.
-
-        threshold : float, default=1.0e-6
-            The minimum weight threshold for including a rule in the final model
-
-        random_state : int or None, default=None
-            Seed for the random number generator to ensure reproducible results.
-        """
-        ### LAZY IMPORT
-        from xgboost import Booster
-
-        if not isinstance(trained_ensemble, Booster):
-            if hasattr(trained_ensemble, "get_booster"):
-                if not isinstance(trained_ensemble.get_booster(), Booster):
-                    raise TypeError(
-                        "trained_ensemble is not an instance of XGBClassifier."
-                    )
-                else:
-                    self.trained_ensemble = trained_ensemble
-            else:
-                raise TypeError("trained_ensemble is not an instance of XGBoost")
-        else:
-            raise TypeError(
-                "XGBoost Booster instance not supported yet. Use XGBClassifier."
-            )
-
-        super().__init__(
-            threshold=threshold,
-            random_state=random_state,
-            rule_cost=rule_cost,
-            solver=solver,
-            class_weight=class_weight,
-        )
-
-    def _get_rule(self, fit_tree: pd.DataFrame, leaf_index: int) -> Rule:
-        """
-        Extracts a decision rule leading to a specified leaf node from an XGBoost tree.
-
-        Parameters
-        ----------
-        fit_tree : pd.DataFrame
-            The decision trees represented as a DataFrame extracted from the trained XGBoost model.
-        leaf_index : int
-            The ID of the leaf node for which to construct the decision rule.
-
-        Returns
-        -------
-        Rule
-            An object representing the decision rule leading to the specified leaf node,
-            composed of clauses that define the decision path.
-        """
-        # Initialize the rule
-        return_rule = Rule()
-
-        if fit_tree.shape[0] <= 1:
-            return return_rule
-
-        while True:
-            # Find the parent node of the current leaf
-            parent = fit_tree.loc[
-                np.any(fit_tree.loc[:, ["Yes", "No"]] == leaf_index, axis=1), "Node"
-            ].values[0]
-
-            # Extract information about the decision at the parent node
-            feature = int(fit_tree.loc[fit_tree.Node == parent, "Feature"].values[0])
-
-            threshold = fit_tree.loc[fit_tree.Node == parent, "Split"].values[0]
-            is_left = (
-                fit_tree.loc[fit_tree.Node == parent, "Yes"].values[0] == leaf_index
-            )
-            missing = (
-                fit_tree.loc[fit_tree.Node == parent, "Missing"].values[0] == leaf_index
-            )
-
-            ub = threshold if is_left else np.inf
-            lb = -np.inf if is_left else threshold
-            na = missing
-
-            return_rule.add_clause(feature, ub, lb, na)
-
-            # If we reached the root of the tree, break the loop
-            if parent == 0:
-                break
-
-            # Move up the tree
-            leaf_index = parent
-
-        return return_rule
-
-    def _get_matrix(
-        self,
-        y: np.ndarray,
-        vec_y: np.ndarray,
-        fit_tree: pd.DataFrame,
-        treeno: int,
-        y_rules: np.ndarray,
-    ):
-        """
-        Populates the matrices for the optimization problem based on a single XGBoost tree.
-
-        Parameters
-        ----------
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector, suitable for the optimization problem.
-        fit_tree : pd.DataFrame
-            A single decision tree's structure from XGBoost, represented as a DataFrame.
-        treeno : int
-            The index of the current tree within the ensemble.
-        y_rules : np.ndarray
-            The array of leaf indices for each sample in the training data, determined
-            by the current tree.
-        """
-        # If the coefficients matrix is empty, start from the first column
-        if self.coefficients_.cols.shape[0] == 0:
-            col = 0
-        else:
-            # Otherwise, start from the next available column
-            col = np.max(self.coefficients_.cols) + 1
-
-        # Get the leaf node for each sample in x
-        y_rules = y_rules[:, treeno]
-
-        # Iterate over unique leaf nodes
-        for leafno in np.unique(y_rules):
-            # Get the samples in the leaf
-            covers = np.where(y_rules == leafno)[0]
-            leaf_y_vals = y[covers]  # y values of the samples in the leaf
-
-            # Get unique labels in the leaf and their counts
-            unique_labels, counts = np.unique(leaf_y_vals, return_counts=True)
-
-            # Identify the majority class in the leaf
-            label = unique_labels[np.argmax(counts)]
-
-            # Create a vector for this label
-            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
-            label_vector[label] = 1
-
-            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
-            fill_ahat = np.dot(vec_y[covers, :], label_vector)
-
-            # Update the coefficients matrix with the new information
-            self.coefficients_.rows = np.concatenate((self.coefficients_.rows, covers))
-            self.coefficients_.cols = np.concatenate(
-                (self.coefficients_.cols, [col] * covers.shape[0])
-            )
-            self.coefficients_.yvals = np.concatenate(
-                (self.coefficients_.yvals, np.full(covers.shape[0], fill_ahat))
-            )
-
-            cost = self._get_rule_cost(
-                temp_rule=self._get_rule(fit_tree, leafno),
-                covers=covers,
-                counts=counts,
-                y=y,
-            )
-
-            # Append the cost to the costs in the coefficients matrix
-            self.coefficients_.costs = np.concatenate(
-                (self.coefficients_.costs, [cost])
-            )
-
-            # Calculate the distribution of the samples in the leaf across the classes
-            sdist = counts
-            self.rule_info_[col] = (treeno, leafno, label, sdist)
-            col += 1
-
-    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray):
-        """
-        Generates the coefficient matrices for the optimization problem from
-        all trees in the XGBoost ensemble.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The feature matrix of the training data.
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector.
-        """
-        y_rules = self.trained_ensemble.apply(x).astype(np.intp)
-        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
-            self._get_matrix(y, vec_y, fit_tree, treeno, y_rules)
-
-    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
-        """
-        Fits the RUXXGBClassifier to the training data, optimizing
-        the extracted rules for a balance between accuracy and interpretability.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels) as integers
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, then samples get equal weights.
-
-        Returns
-        -------
-        RUXXGBClassifier
-            The fitted model, ready for making predictions.
-        """
-        x, y = check_inputs(x, y)
-
-        sample_weight = self._get_sample_weight(sample_weight, y)
-
-        # If the model has been fitted before, clean it up
-        if self._is_fitted:
-            self._cleanup()
-
-        # Fills the fitted decision trees.
-        out = self.trained_ensemble.get_booster().trees_to_dataframe()
-        pattern = re.compile(r"-(\d+)")
-        columns = ["Yes", "No", "Missing"]
-        out[columns] = out[columns].map(
-            lambda x: (
-                int(pattern.search(x).group(1))
-                if pd.notna(x) and pattern.search(x)
-                else None
-            )
-        )
-        out.Feature = out.Feature.str.lstrip("f")
-        self.decision_trees_ = {
-            treeno: out.loc[out.Tree == treeno] for treeno in out.Tree.unique()
-        }
-
-        self._get_class_infos(y)
-        vec_y = self._preprocess(y)
-
-        self._get_matrices(x=x, y=y, vec_y=vec_y)
-
-        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
-
-        ws, *_ = self.solver(
-            coefficients=self.coefficients_,
-            k=self.k_,
-            sample_weight=sample_weight,
-            normalization_constant=normalization_constant,
-        )
-
-        self._fill_rules(ws)
-        self._is_fitted = True
-
-        return self
+from __future__ import annotations
+import re
+import numpy as np
+import pandas as pd
+from numpy.typing import ArrayLike
+
+from .base import _RUGBASE
+from ..aux_classes import Rule
+from ..rule_cost import Gini
+from ..utils import check_module_available, check_inputs
+from ..solver import ORToolsSolver
+
+
+XGBOOST_AVAILABLE = check_module_available("xgboost")
+
+
+class RUXXGBClassifier(_RUGBASE):
+    """
+    A classifier that extracts and optimizes decision rules from a trained
+    XGBoost ensemble model to create a compact and interpretable model.
+    This process involves translating the ensemble's trees into a set of rules and
+    using optimization to balance model accuracy and interpretability. The complexity
+    of the resulting rule-based model is  controlled through a penalty parameter.
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if not XGBOOST_AVAILABLE:
+            raise ImportError(
+                "XGBoost is required for this class but is not installed.",
+                "Please install it with 'pip install xgboost'",
+            )
+        instance = super(RUXXGBClassifier, cls).__new__(cls)
+        return instance
+
+    def __init__(
+        self,
+        trained_ensemble,
+        *,
+        solver=ORToolsSolver(),
+        rule_cost=Gini(),
+        class_weight: dict | str | None = None,
+        threshold: float = 1.0e-6,
+        random_state: int | None = None,
+    ):
+        """
+        Parameters
+        ----------
+        trained_ensemble : xgboost.XGBClassifier
+            The trained XGBoost ensemble model from which rules will be extracted.
+            The model should already be trained on the dataset.
+
+        solver : OptimizationSolver, default=ORToolsSolver()
+            An instance of a derived class inherits from the 'Optimization Solver' base class.
+            The solver is responsible for optimizing the rule set based on the cost function
+            and constraints.
+
+        rule_cost : RuleCost or int, default=Gini()
+            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+            or a fixed cost
+
+        class_weight: dict, "balanced" or None, default=None
+            A dictionary mapping class labels to their respective weights, the string "balanced"
+            to automatically adjust weights inversely proportional to class frequencies,
+            or None for no weights. Used to adjust the model in favor of certain classes.
+
+        threshold : float, default=1.0e-6
+            The minimum weight threshold for including a rule in the final model
+
+        random_state : int or None, default=None
+            Seed for the random number generator to ensure reproducible results.
+        """
+        ### LAZY IMPORT
+        from xgboost import Booster
+
+        if not isinstance(trained_ensemble, Booster):
+            if hasattr(trained_ensemble, "get_booster"):
+                if not isinstance(trained_ensemble.get_booster(), Booster):
+                    raise TypeError(
+                        "trained_ensemble is not an instance of XGBClassifier."
+                    )
+                else:
+                    self.trained_ensemble = trained_ensemble
+            else:
+                raise TypeError("trained_ensemble is not an instance of XGBoost")
+        else:
+            raise TypeError(
+                "XGBoost Booster instance not supported yet. Use XGBClassifier."
+            )
+
+        super().__init__(
+            threshold=threshold,
+            random_state=random_state,
+            rule_cost=rule_cost,
+            solver=solver,
+            class_weight=class_weight,
+        )
+
+    def _get_rule(self, fit_tree: pd.DataFrame, leaf_index: int) -> Rule:
+        """
+        Extracts a decision rule leading to a specified leaf node from an XGBoost tree.
+
+        Parameters
+        ----------
+        fit_tree : pd.DataFrame
+            The decision trees represented as a DataFrame extracted from the trained XGBoost model.
+        leaf_index : int
+            The ID of the leaf node for which to construct the decision rule.
+
+        Returns
+        -------
+        Rule
+            An object representing the decision rule leading to the specified leaf node,
+            composed of clauses that define the decision path.
+        """
+        # Initialize the rule
+        return_rule = Rule()
+
+        if fit_tree.shape[0] <= 1:
+            return return_rule
+
+        while True:
+            # Find the parent node of the current leaf
+            parent = fit_tree.loc[
+                np.any(fit_tree.loc[:, ["Yes", "No"]] == leaf_index, axis=1), "Node"
+            ].values[0]
+
+            # Extract information about the decision at the parent node
+            feature = int(fit_tree.loc[fit_tree.Node == parent, "Feature"].values[0])
+
+            threshold = fit_tree.loc[fit_tree.Node == parent, "Split"].values[0]
+            is_left = (
+                fit_tree.loc[fit_tree.Node == parent, "Yes"].values[0] == leaf_index
+            )
+            missing = (
+                fit_tree.loc[fit_tree.Node == parent, "Missing"].values[0] == leaf_index
+            )
+
+            ub = threshold if is_left else np.inf
+            lb = -np.inf if is_left else threshold
+            na = missing
+
+            return_rule.add_clause(feature, ub, lb, na)
+
+            # If we reached the root of the tree, break the loop
+            if parent == 0:
+                break
+
+            # Move up the tree
+            leaf_index = parent
+
+        return return_rule
+
+    def _get_matrix(
+        self,
+        y: np.ndarray,
+        vec_y: np.ndarray,
+        fit_tree: pd.DataFrame,
+        treeno: int,
+        y_rules: np.ndarray,
+    ):
+        """
+        Populates the matrices for the optimization problem based on a single XGBoost tree.
+
+        Parameters
+        ----------
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector, suitable for the optimization problem.
+        fit_tree : pd.DataFrame
+            A single decision tree's structure from XGBoost, represented as a DataFrame.
+        treeno : int
+            The index of the current tree within the ensemble.
+        y_rules : np.ndarray
+            The array of leaf indices for each sample in the training data, determined
+            by the current tree.
+        """
+        # If the coefficients matrix is empty, start from the first column
+        if self.coefficients_.cols.shape[0] == 0:
+            col = 0
+        else:
+            # Otherwise, start from the next available column
+            col = np.max(self.coefficients_.cols) + 1
+
+        # Get the leaf node for each sample in x
+        y_rules = y_rules[:, treeno]
+
+        # Iterate over unique leaf nodes
+        for leafno in np.unique(y_rules):
+            # Get the samples in the leaf
+            covers = np.where(y_rules == leafno)[0]
+            leaf_y_vals = y[covers]  # y values of the samples in the leaf
+
+            # Get unique labels in the leaf and their counts
+            unique_labels, counts = np.unique(leaf_y_vals, return_counts=True)
+
+            # Identify the majority class in the leaf
+            label = unique_labels[np.argmax(counts)]
+
+            # Create a vector for this label
+            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
+            label_vector[label] = 1
+
+            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
+            fill_ahat = np.dot(vec_y[covers, :], label_vector)
+
+            # Update the coefficients matrix with the new information
+            self.coefficients_.rows = np.concatenate((self.coefficients_.rows, covers))
+            self.coefficients_.cols = np.concatenate(
+                (self.coefficients_.cols, [col] * covers.shape[0])
+            )
+            self.coefficients_.yvals = np.concatenate(
+                (self.coefficients_.yvals, np.full(covers.shape[0], fill_ahat))
+            )
+
+            cost = self._get_rule_cost(
+                temp_rule=self._get_rule(fit_tree, leafno),
+                covers=covers,
+                counts=counts,
+                y=y,
+            )
+
+            # Append the cost to the costs in the coefficients matrix
+            self.coefficients_.costs = np.concatenate(
+                (self.coefficients_.costs, [cost])
+            )
+
+            # Calculate the distribution of the samples in the leaf across the classes
+            sdist = counts
+            self.rule_info_[col] = (treeno, leafno, label, sdist)
+            col += 1
+
+    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray):
+        """
+        Generates the coefficient matrices for the optimization problem from
+        all trees in the XGBoost ensemble.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The feature matrix of the training data.
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector.
+        """
+        y_rules = self.trained_ensemble.apply(x).astype(np.intp)
+        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
+            self._get_matrix(y, vec_y, fit_tree, treeno, y_rules)
+
+    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
+        """
+        Fits the RUXXGBClassifier to the training data, optimizing
+        the extracted rules for a balance between accuracy and interpretability.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels) as integers
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples get equal weights.
+
+        Returns
+        -------
+        RUXXGBClassifier
+            The fitted model, ready for making predictions.
+        """
+        x, y = check_inputs(x, y)
+
+        sample_weight = self._get_sample_weight(sample_weight, y)
+
+        # If the model has been fitted before, clean it up
+        if self._is_fitted:
+            self._cleanup()
+
+        # Fills the fitted decision trees.
+        out = self.trained_ensemble.get_booster().trees_to_dataframe()
+        pattern = re.compile(r"-(\d+)")
+        columns = ["Yes", "No", "Missing"]
+        out[columns] = out[columns].map(
+            lambda x: (
+                int(pattern.search(x).group(1))
+                if pd.notna(x) and pattern.search(x)
+                else None
+            )
+        )
+        out.Feature = out.Feature.str.lstrip("f")
+        self.decision_trees_ = {
+            treeno: out.loc[out.Tree == treeno] for treeno in out.Tree.unique()
+        }
+
+        self._get_class_infos(y)
+        vec_y = self._preprocess(y)
+
+        self._get_matrices(x=x, y=y, vec_y=vec_y)
+
+        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
+
+        ws, *_ = self.solver(
+            coefficients=self.coefficients_,
+            k=self.k_,
+            sample_weight=sample_weight,
+            normalization_constant=normalization_constant,
+        )
+
+        self._fill_rules(ws)
+        self._is_fitted = True
+
+        return self
```

## ruleopt/estimator/sklearn_/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from .rug import RUGClassifier
-from .rux import RUXClassifier
-
-__all__ = [
-    "RUGClassifier",
-    "RUXClassifier",
-]
+from .rug import RUGClassifier
+from .rux import RUXClassifier
+
+__all__ = [
+    "RUGClassifier",
+    "RUXClassifier",
+]
```

## ruleopt/estimator/sklearn_/base_sklearn.py

```diff
@@ -1,219 +1,219 @@
-from sklearn.tree import DecisionTreeClassifier
-import numpy as np
-from ..base import _RUGBASE
-from ...aux_classes import Rule
-
-
-class _RUGSKLEARN(_RUGBASE):
-    """
-    The base class specialized for use with scikit-learn.
-
-    This subclass implements the rule extraction process specifically for decision trees
-    trained using scikit-learn.
-    """
-
-    def __init__(
-        self,
-        solver,
-        rule_cost,
-        class_weight,
-        threshold,
-        random_state,
-    ):
-        """
-        Parameters
-        ----------
-        solver : OptimizationSolver
-            An instance of a derived class inherits from the 'Optimization Solver' base class.
-            The solver is responsible for optimizing the rule set based on the cost function
-            and constraints.
-
-        rule_cost : RuleCost or int
-            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-            or a fixed cost
-
-        class_weight: dict, "balanced" or None
-            A dictionary mapping class labels to their respective weights, the string "balanced"
-            to automatically adjust weights inversely proportional to class frequencies,
-            or None for no weights. Used to adjust the model in favor of certain classes.
-
-        threshold : floa
-            The minimum weight threshold for including a rule in the final model
-
-        random_state : int or None
-            Seed for the random number generator to ensure reproducible results.
-            Defaults to None.
-        """
-        super().__init__(
-            threshold=threshold,
-            random_state=random_state,
-            rule_cost=rule_cost,
-            solver=solver,
-            class_weight=class_weight,
-        )
-
-    def _get_rule(self, fit_tree: DecisionTreeClassifier, nodeid: int) -> Rule:
-        """
-        Constructs a rule from a given node in a decision tree.
-
-        Parameters
-        ----------
-        fit_tree : DecisionTreeClassifier
-            The fitted decision tree from which to extract the rule.
-        nodeid : int
-            The ID of the node from which the rule is to be extracted.
-
-        Returns
-        -------
-        Rule
-            An object representing the extracted rule.
-        """
-
-        # Initializing the rule to be returned
-        return_rule = Rule()
-
-        # If the first feature of the tree is -2, the rule is empty
-        if fit_tree.tree_.feature[0] == -2:
-            return Rule()
-
-        # Extracting information from the tree
-        tree = fit_tree.tree_
-        left = tree.children_left
-        right = tree.children_right
-        threshold = tree.threshold
-        missing_left = tree.missing_go_to_left
-
-        # Building dictionaries to hold node information
-        node_info = {
-            node_id: (parent, True, bool(missing_left[parent]))
-            for parent, node_id in enumerate(left)
-        }
-        node_info.update(
-            {
-                node_id: (parent, False, not bool(missing_left[parent]))
-                for parent, node_id in enumerate(right)
-            }
-        )
-
-        # Traversing up the tree to build the rule
-        while nodeid != 0:
-            parent, is_left, missing = node_info[nodeid]
-
-            feature = tree.feature[parent]
-            ub = threshold[parent] if is_left else np.inf
-            lb = -np.inf if is_left else threshold[parent]
-            na = missing
-
-            return_rule.add_clause(feature, ub, lb, na)
-            nodeid = parent
-
-        return return_rule
-
-    def _get_matrix(
-        self,
-        x: np.ndarray,
-        y: np.ndarray,
-        vec_y: np.ndarray,
-        fit_tree: DecisionTreeClassifier,
-        treeno: int,
-        betas: np.ndarray = None,
-        normalization_constant: np.ndarray = None
-    ) -> None:
-        """
-        Generates matrices for optimization.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The feature matrix of the training data.
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector, adjusted for optimization.
-        fit_tree : DecisionTreeClassifier
-            A fitted decision tree model from which to extract rules.
-        treeno : int
-            An identifier for the decision tree within an ensemble.
-        """
-        # If the coefficients matrix is empty, start from the first column
-        if self.coefficients_.cols.shape[0] == 0:
-            col = 0
-        else:
-            # Otherwise, start from the next available column
-            col = np.max(self.coefficients_.cols) + 1
-
-        # Get the leaf node for each sample in x
-        y_rules = fit_tree.apply(x)
-        preds = fit_tree.predict(x).astype(np.intp)
-
-        no_improvement = True
-
-        # Iterate over unique leaf nodes
-        for leafno in np.unique(y_rules):
-            temp_rule = self._get_rule(fit_tree, leafno)
-
-            if hasattr(self, "_temp_rules"):
-                if temp_rule in self._temp_rules:
-                    continue
-
-            covers = np.where(y_rules == leafno)[0]
-            leaf_y_vals = y[covers]  # y values of the samples in the leaf
-
-            _, counts = np.unique(leaf_y_vals, return_counts=True)
-
-            # Identify the majority class in the leaf
-            label = preds[covers][0]
-
-            # Create a vector for this label
-            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
-            label_vector[label] = 1
-
-            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
-            fill_ahat = np.dot(vec_y[covers, :], label_vector)
-            
-            cost = self._get_rule_cost(
-                    temp_rule=temp_rule,
-                    covers=covers,
-                    counts=counts,
-                    y=y,
-                )
-
-            if (betas is not None) & (normalization_constant is not None):
-                red_cost = np.dot(
-                    np.multiply(((self.k_ - 1.0) / self.k_), fill_ahat),
-                    betas[
-                        covers
-                    ],  # (betas if sample_weight is None else betas * sample_weight),
-                ) - (cost * self.solver.penalty * normalization_constant)
-
-            else:
-                red_cost = float("inf")
-
-            if red_cost > 0:
-                covers_fill = np.full((covers.shape[0],), fill_ahat, dtype=np.intp)
-                covers_col = np.full((covers.shape[0],), col, dtype=np.intp)
-
-
-                self.coefficients_.rows = np.concatenate(
-                    (self.coefficients_.rows, covers)
-                )
-                self.coefficients_.cols = np.concatenate(
-                    (self.coefficients_.cols, covers_col)
-                )
-                self.coefficients_.yvals = np.concatenate(
-                    (self.coefficients_.yvals, covers_fill)
-                )
-
-                # Append the cost to the costs in the coefficients matrix
-                self.coefficients_.costs = np.concatenate(
-                    (self.coefficients_.costs, [cost])
-                )
-
-                # Calculate the distribution of the samples in the leaf across the classes
-                sdist = counts
-                self.rule_info_[col] = (treeno, leafno, label, sdist)
-                col += 1
-                
-                no_improvement = False
-                
-        return no_improvement
+from sklearn.tree import DecisionTreeClassifier
+import numpy as np
+from ..base import _RUGBASE
+from ...aux_classes import Rule
+
+
+class _RUGSKLEARN(_RUGBASE):
+    """
+    The base class specialized for use with scikit-learn.
+
+    This subclass implements the rule extraction process specifically for decision trees
+    trained using scikit-learn.
+    """
+
+    def __init__(
+        self,
+        solver,
+        rule_cost,
+        class_weight,
+        threshold,
+        random_state,
+    ):
+        """
+        Parameters
+        ----------
+        solver : OptimizationSolver
+            An instance of a derived class inherits from the 'Optimization Solver' base class.
+            The solver is responsible for optimizing the rule set based on the cost function
+            and constraints.
+
+        rule_cost : RuleCost or int
+            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+            or a fixed cost
+
+        class_weight: dict, "balanced" or None
+            A dictionary mapping class labels to their respective weights, the string "balanced"
+            to automatically adjust weights inversely proportional to class frequencies,
+            or None for no weights. Used to adjust the model in favor of certain classes.
+
+        threshold : floa
+            The minimum weight threshold for including a rule in the final model
+
+        random_state : int or None
+            Seed for the random number generator to ensure reproducible results.
+            Defaults to None.
+        """
+        super().__init__(
+            threshold=threshold,
+            random_state=random_state,
+            rule_cost=rule_cost,
+            solver=solver,
+            class_weight=class_weight,
+        )
+
+    def _get_rule(self, fit_tree: DecisionTreeClassifier, nodeid: int) -> Rule:
+        """
+        Constructs a rule from a given node in a decision tree.
+
+        Parameters
+        ----------
+        fit_tree : DecisionTreeClassifier
+            The fitted decision tree from which to extract the rule.
+        nodeid : int
+            The ID of the node from which the rule is to be extracted.
+
+        Returns
+        -------
+        Rule
+            An object representing the extracted rule.
+        """
+
+        # Initializing the rule to be returned
+        return_rule = Rule()
+
+        # If the first feature of the tree is -2, the rule is empty
+        if fit_tree.tree_.feature[0] == -2:
+            return Rule()
+
+        # Extracting information from the tree
+        tree = fit_tree.tree_
+        left = tree.children_left
+        right = tree.children_right
+        threshold = tree.threshold
+        missing_left = tree.missing_go_to_left
+
+        # Building dictionaries to hold node information
+        node_info = {
+            node_id: (parent, True, bool(missing_left[parent]))
+            for parent, node_id in enumerate(left)
+        }
+        node_info.update(
+            {
+                node_id: (parent, False, not bool(missing_left[parent]))
+                for parent, node_id in enumerate(right)
+            }
+        )
+
+        # Traversing up the tree to build the rule
+        while nodeid != 0:
+            parent, is_left, missing = node_info[nodeid]
+
+            feature = tree.feature[parent]
+            ub = threshold[parent] if is_left else np.inf
+            lb = -np.inf if is_left else threshold[parent]
+            na = missing
+
+            return_rule.add_clause(feature, ub, lb, na)
+            nodeid = parent
+
+        return return_rule
+
+    def _get_matrix(
+        self,
+        x: np.ndarray,
+        y: np.ndarray,
+        vec_y: np.ndarray,
+        fit_tree: DecisionTreeClassifier,
+        treeno: int,
+        betas: np.ndarray = None,
+        normalization_constant: np.ndarray = None
+    ) -> None:
+        """
+        Generates matrices for optimization.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The feature matrix of the training data.
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector, adjusted for optimization.
+        fit_tree : DecisionTreeClassifier
+            A fitted decision tree model from which to extract rules.
+        treeno : int
+            An identifier for the decision tree within an ensemble.
+        """
+        # If the coefficients matrix is empty, start from the first column
+        if self.coefficients_.cols.shape[0] == 0:
+            col = 0
+        else:
+            # Otherwise, start from the next available column
+            col = np.max(self.coefficients_.cols) + 1
+
+        # Get the leaf node for each sample in x
+        y_rules = fit_tree.apply(x)
+        preds = fit_tree.predict(x).astype(np.intp)
+
+        no_improvement = True
+
+        # Iterate over unique leaf nodes
+        for leafno in np.unique(y_rules):
+            temp_rule = self._get_rule(fit_tree, leafno)
+
+            if hasattr(self, "_temp_rules"):
+                if temp_rule in self._temp_rules:
+                    continue
+
+            covers = np.where(y_rules == leafno)[0]
+            leaf_y_vals = y[covers]  # y values of the samples in the leaf
+
+            _, counts = np.unique(leaf_y_vals, return_counts=True)
+
+            # Identify the majority class in the leaf
+            label = preds[covers][0]
+
+            # Create a vector for this label
+            label_vector = np.full((self.k_,), -1 / (self.k_ - 1))
+            label_vector[label] = 1
+
+            # Calculate fill_ahat, which will be used to update yvals in the coefficients matrix
+            fill_ahat = np.dot(vec_y[covers, :], label_vector)
+            
+            cost = self._get_rule_cost(
+                    temp_rule=temp_rule,
+                    covers=covers,
+                    counts=counts,
+                    y=y,
+                )
+
+            if (betas is not None) & (normalization_constant is not None):
+                red_cost = np.dot(
+                    np.multiply(((self.k_ - 1.0) / self.k_), fill_ahat),
+                    betas[
+                        covers
+                    ],  # (betas if sample_weight is None else betas * sample_weight),
+                ) - (cost * self.solver.penalty * normalization_constant)
+
+            else:
+                red_cost = float("inf")
+
+            if red_cost > 0:
+                covers_fill = np.full((covers.shape[0],), fill_ahat, dtype=np.float32)
+                covers_col = np.full((covers.shape[0],), col, dtype=np.int32)
+
+
+                self.coefficients_.rows = np.concatenate(
+                    (self.coefficients_.rows, covers)
+                )
+                self.coefficients_.cols = np.concatenate(
+                    (self.coefficients_.cols, covers_col)
+                )
+                self.coefficients_.yvals = np.concatenate(
+                    (self.coefficients_.yvals, covers_fill)
+                )
+
+                # Append the cost to the costs in the coefficients matrix
+                self.coefficients_.costs = np.concatenate(
+                    (self.coefficients_.costs, [cost])
+                )
+
+                # Calculate the distribution of the samples in the leaf across the classes
+                sdist = counts
+                self.rule_info_[col] = (treeno, leafno, label, sdist)
+                col += 1
+                
+                no_improvement = False
+                
+        return no_improvement
```

## ruleopt/estimator/sklearn_/rug.py

 * *Ordering differences only*

```diff
@@ -1,354 +1,354 @@
-from __future__ import annotations
-
-import numpy as np
-from numpy.typing import ArrayLike
-from sklearn.tree import DecisionTreeClassifier
-
-from .base_sklearn import _RUGSKLEARN
-from ...rule_cost import Gini
-from ...utils import check_inputs
-from ...solver import ORToolsSolver
-
-
-class RUGClassifier(_RUGSKLEARN):
-    """
-    Rule Generation algorithm for multi-class classification. This algorithm aims at
-    producing a compact and interpretable model by employing optimization-bsed rule learning.
-    """
-
-    def __init__(
-        self,
-        solver=ORToolsSolver(),
-        rule_cost=Gini(),
-        max_rmp_calls=20,
-        threshold: float = 1.0e-6,
-        random_state: int | None = None,
-        class_weight: dict | str | None = None,
-        criterion: str = "gini",
-        splitter: str = "best",
-        max_depth: int | None = None,
-        min_samples_split: int = 2,
-        min_samples_leaf: int = 1,
-        min_weight_fraction_leaf: float = 0.0,
-        max_features: int | float | str = None,
-        max_leaf_nodes: int | None = None,
-        min_impurity_decrease: float = 0.0,
-        ccp_alpha: float = 0.0,
-        monotonic_cst: ArrayLike | None = None,
-    ):
-        """
-        Parameters
-        ----------
-        solver : OptimizationSolver, default=ORToolsSolver()
-            An instance of a derived class inherits from the 'Optimization Solver' base class.
-            The solver is responsible for optimizing the rule set based on the cost function
-            and constraints.
-
-        rule_cost : RuleCost or int, default=Gini()
-            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-            or a fixed cost
-
-        max_rmp_calls : int, default=20
-            Maximum number of Restricted Master Problem (RMP) iterations allowed during fitting.
-
-        class_weight: dict, "balanced" or None, default=None
-            A dictionary mapping class labels to their respective weights, the string "balanced"
-            to automatically adjust weights inversely proportional to class frequencies,
-            or None for no weights. Used to adjust the model in favor of certain classes.
-
-        threshold : float, default=1.0e-6
-            The minimum weight threshold for including a rule in the final model.
-
-        random_state : int or None, default=None
-            Seed for the random number generator to ensure reproducible results.
-
-        criterion : {"gini", "entropy", "log_loss"}, default="gini"
-            The function to measure the quality of a split. Supported criteria are
-            "gini" for the Gini impurity and "log_loss" and "entropy" both for the
-
-        splitter : {"best", "random"}, default="best"
-            The strategy used to choose the split at each node. Supported
-            strategies are "best" to choose the best split and "random" to choose
-            the best random split.
-
-        max_depth : int, default=None
-            The maximum depth of the tree. If None, then nodes are expanded until
-            all leaves are pure or until all leaves contain less than
-            min_samples_split samples.
-
-        min_samples_split : int or float, default=2
-            The minimum number of samples required to split an internal node:
-
-        min_samples_leaf : int or float, default=1
-            The minimum number of samples required to be at a leaf node.
-            A split point at any depth will only be considered if it leaves at
-            least ``min_samples_leaf`` training samples in each of the left and
-            right branches.  This may have the effect of smoothing the model,
-            especially in regression.
-
-        min_weight_fraction_leaf : float, default=0.0
-            The minimum weighted fraction of the sum total of weights (of all
-            the input samples) required to be at a leaf node. Samples have
-            equal weight when sample_weight is not provided.
-
-        max_features : int, float or {"sqrt", "log2"}, default=None
-            The number of features to consider when looking for the best split:
-
-        max_leaf_nodes : int, default=None
-            Grow a tree with ``max_leaf_nodes`` in best-first fashion.
-            Best nodes are defined as relative reduction in impurity.
-            If None then unlimited number of leaf nodes.
-
-        min_impurity_decrease : float, default=0.0
-            A node will be split if this split induces a decrease of the impurity
-            greater than or equal to this value.
-
-        ccp_alpha : non-negative float, default=0.0
-            Complexity parameter used for Minimal Cost-Complexity Pruning. The
-            subtree with the largest cost complexity that is smaller than
-            ``ccp_alpha`` will be chosen. By default, no pruning is performed.
-
-        monotonic_cst : array-like of int of shape (n_features), default=None
-            Indicates the monotonicity constraint to enforce on each feature.
-            - 1: monotonic increase
-            - 0: no constraint
-            - -1: monotonic decrease
-        """
-        self._validate_parameters(
-            max_rmp_calls,
-            criterion,
-            splitter,
-            max_depth,
-            min_samples_split,
-            min_samples_leaf,
-            min_weight_fraction_leaf,
-            max_features,
-            max_leaf_nodes,
-            min_impurity_decrease,
-            ccp_alpha,
-            monotonic_cst,
-        )
-
-        super().__init__(
-            threshold=threshold,
-            random_state=random_state,
-            solver=solver,
-            rule_cost=rule_cost,
-            class_weight=class_weight,
-        )
-
-        self.max_rmp_calls = int(max_rmp_calls)
-
-        self.criterion = criterion
-        self.splitter = splitter
-        self.max_depth = max_depth
-        self.min_samples_split = min_samples_split
-        self.min_samples_leaf = min_samples_leaf
-        self.min_weight_fraction_leaf = min_weight_fraction_leaf
-        self.max_features = max_features
-        self.max_leaf_nodes = max_leaf_nodes
-        self.min_impurity_decrease = min_impurity_decrease
-        self.ccp_alpha = ccp_alpha
-        self.monotonic_cst = monotonic_cst
-
-        self._temp_rules = []
-
-    def _fit_decision_tree(
-        self, x: np.ndarray, y: np.ndarray, sample_weight: np.ndarray
-    ) -> DecisionTreeClassifier:
-        """
-        Fits a decision tree to the data, taking into account sample weights.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            Feature matrix of the training data.
-        y : np.ndarray
-            Target vector of the training data.
-        sample_weight : np.ndarray
-            Array of weights for the samples.
-
-        Returns
-        -------
-        DecisionTreeClassifier
-            A decision tree classifier fitted to the weighted data.
-        """
-        dt = DecisionTreeClassifier(
-            random_state=self._rng.integers(np.iinfo(np.int16).max),
-            criterion=self.criterion,
-            splitter=self.splitter,
-            class_weight=self.class_weight,
-            max_depth=self.max_depth,
-            min_samples_split=self.min_samples_split,
-            min_samples_leaf=self.min_samples_leaf,
-            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
-            max_features=self.max_features,
-            max_leaf_nodes=self.max_leaf_nodes,
-            min_impurity_decrease=self.min_impurity_decrease,
-            ccp_alpha=self.ccp_alpha,
-            monotonic_cst=self.monotonic_cst,
-        )
-
-        if sample_weight is not None:
-            dt.class_weight = None
-
-        # Fit the decision tree to the data
-        return dt.fit(x, y, sample_weight=sample_weight)
-
-    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
-        """
-        Fits the RUGClassifier model to the training data using a rule generation approach.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels) as integers
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, then samples get equal weights.
-
-        Returns
-        -------
-        RUGClassifier
-            The fitted model, ready for making predictions.
-        """
-        x, y = check_inputs(x, y)
-
-        sample_weight = self._get_sample_weight(sample_weight, y)
-
-        if self._is_fitted:
-            self._cleanup()
-
-        treeno = 0
-        fit_tree = self._fit_decision_tree(x, y, sample_weight=None)
-        self.decision_trees_[treeno] = fit_tree
-
-        self._get_class_infos(y)
-        vec_y = self._preprocess(y)
-        self._get_matrix(x, y, vec_y, fit_tree, treeno)
-
-        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
-
-        ws, betas = self.solver(
-            coefficients=self.coefficients_,
-            k=self.k_,
-            sample_weight=sample_weight,
-            normalization_constant=normalization_constant,
-        )
-
-        # Rule generation
-        for _ in range(self.max_rmp_calls):
-            if np.all(betas <= 1e-6):
-                break
-
-            treeno += 1
-            fit_tree = self._fit_decision_tree(x, y, sample_weight=betas)
-            self.decision_trees_[treeno] = fit_tree
-
-            no_improvement = self._get_matrix(x, y, vec_y, fit_tree, treeno, betas, normalization_constant)
-
-            if no_improvement:
-                break
-
-            ws, betas = self.solver(
-                coefficients=self.coefficients_,
-                k=self.k_,
-                ws0=ws.copy(),
-                normalization_constant=normalization_constant,
-                sample_weight=sample_weight,
-            )
-
-        self._fill_rules(ws)
-        self._is_fitted = True
-
-        return self
-
-    def _validate_parameters(
-        self,
-        max_rmp_calls,
-        criterion,
-        splitter,
-        max_depth,
-        min_samples_split,
-        min_samples_leaf,
-        min_weight_fraction_leaf,
-        max_features,
-        max_leaf_nodes,
-        min_impurity_decrease,
-        ccp_alpha,
-        monotonic_cst,
-    ):
-        # max_rmp_calls check
-        if not isinstance(max_rmp_calls, (float, int)):
-            raise TypeError("max_rmp_calls must be an integer.")
-
-        if max_rmp_calls < 0:
-            raise ValueError("max_rmp_calls must be a non-negative integer.")
-
-        # criterion check
-        if criterion not in {"gini", "entropy", "log_loss"}:
-            raise ValueError(
-                "criterion must be one of 'gini', 'entropy', or 'log_loss'."
-            )
-
-        # splitter check
-        if splitter not in {"best", "random"}:
-            raise ValueError("splitter must be 'best' or 'random'.")
-
-        # max_depth check
-        if max_depth is not None and not isinstance(max_depth, int):
-            raise TypeError("max_depth must be an integer or None.")
-        if isinstance(max_depth, int) and max_depth < 1:
-            raise ValueError("max_depth must be greater than 0.")
-
-        # min_samples_split check
-        if not isinstance(min_samples_split, (int, float)) or min_samples_split < 2:
-            raise ValueError(
-                "min_samples_split must be an integer or float greater than or equal to 2."
-            )
-
-        # min_samples_leaf check
-        if not isinstance(min_samples_leaf, (int, float)) or min_samples_leaf < 1:
-            raise ValueError(
-                "min_samples_leaf must be an integer or float greater than or equal to 1."
-            )
-
-        # min_weight_fraction_leaf check
-        if not isinstance(min_weight_fraction_leaf, float) or not (
-            0.0 <= min_weight_fraction_leaf <= 1.0
-        ):
-            raise ValueError(
-                "min_weight_fraction_leaf must be a float between 0.0 and 1.0."
-            )
-
-        # max_features check
-        if (
-            max_features is not None
-            and not isinstance(max_features, (int, float, str))
-            or (isinstance(max_features, str) and max_features not in {"sqrt", "log2"})
-        ):
-            raise ValueError(
-                "max_features must be an integer, float, 'sqrt', 'log2', or None."
-            )
-
-        # max_leaf_nodes check
-        if max_leaf_nodes is not None and (
-            not isinstance(max_leaf_nodes, int) or max_leaf_nodes < 1
-        ):
-            raise ValueError("max_leaf_nodes must be a positive integer or None.")
-
-        # min_impurity_decrease check
-        if not isinstance(min_impurity_decrease, float) or min_impurity_decrease < 0.0:
-            raise ValueError("min_impurity_decrease must be a non-negative float.")
-
-        # ccp_alpha check
-        if not isinstance(ccp_alpha, float) or ccp_alpha < 0.0:
-            raise ValueError("ccp_alpha must be a non-negative float.")
-
-        # monotonic_cst check
-        if monotonic_cst is not None and (
-            not isinstance(monotonic_cst, (list, tuple))
-            or not all(isinstance(item, int) for item in monotonic_cst)
-        ):
-            raise ValueError("monotonic_cst must be an array-like of integers or None.")
+from __future__ import annotations
+
+import numpy as np
+from numpy.typing import ArrayLike
+from sklearn.tree import DecisionTreeClassifier
+
+from .base_sklearn import _RUGSKLEARN
+from ...rule_cost import Gini
+from ...utils import check_inputs
+from ...solver import ORToolsSolver
+
+
+class RUGClassifier(_RUGSKLEARN):
+    """
+    Rule Generation algorithm for multi-class classification. This algorithm aims at
+    producing a compact and interpretable model by employing optimization-bsed rule learning.
+    """
+
+    def __init__(
+        self,
+        solver=ORToolsSolver(),
+        rule_cost=Gini(),
+        max_rmp_calls=20,
+        threshold: float = 1.0e-6,
+        random_state: int | None = None,
+        class_weight: dict | str | None = None,
+        criterion: str = "gini",
+        splitter: str = "best",
+        max_depth: int | None = None,
+        min_samples_split: int = 2,
+        min_samples_leaf: int = 1,
+        min_weight_fraction_leaf: float = 0.0,
+        max_features: int | float | str = None,
+        max_leaf_nodes: int | None = None,
+        min_impurity_decrease: float = 0.0,
+        ccp_alpha: float = 0.0,
+        monotonic_cst: ArrayLike | None = None,
+    ):
+        """
+        Parameters
+        ----------
+        solver : OptimizationSolver, default=ORToolsSolver()
+            An instance of a derived class inherits from the 'Optimization Solver' base class.
+            The solver is responsible for optimizing the rule set based on the cost function
+            and constraints.
+
+        rule_cost : RuleCost or int, default=Gini()
+            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+            or a fixed cost
+
+        max_rmp_calls : int, default=20
+            Maximum number of Restricted Master Problem (RMP) iterations allowed during fitting.
+
+        class_weight: dict, "balanced" or None, default=None
+            A dictionary mapping class labels to their respective weights, the string "balanced"
+            to automatically adjust weights inversely proportional to class frequencies,
+            or None for no weights. Used to adjust the model in favor of certain classes.
+
+        threshold : float, default=1.0e-6
+            The minimum weight threshold for including a rule in the final model.
+
+        random_state : int or None, default=None
+            Seed for the random number generator to ensure reproducible results.
+
+        criterion : {"gini", "entropy", "log_loss"}, default="gini"
+            The function to measure the quality of a split. Supported criteria are
+            "gini" for the Gini impurity and "log_loss" and "entropy" both for the
+
+        splitter : {"best", "random"}, default="best"
+            The strategy used to choose the split at each node. Supported
+            strategies are "best" to choose the best split and "random" to choose
+            the best random split.
+
+        max_depth : int, default=None
+            The maximum depth of the tree. If None, then nodes are expanded until
+            all leaves are pure or until all leaves contain less than
+            min_samples_split samples.
+
+        min_samples_split : int or float, default=2
+            The minimum number of samples required to split an internal node:
+
+        min_samples_leaf : int or float, default=1
+            The minimum number of samples required to be at a leaf node.
+            A split point at any depth will only be considered if it leaves at
+            least ``min_samples_leaf`` training samples in each of the left and
+            right branches.  This may have the effect of smoothing the model,
+            especially in regression.
+
+        min_weight_fraction_leaf : float, default=0.0
+            The minimum weighted fraction of the sum total of weights (of all
+            the input samples) required to be at a leaf node. Samples have
+            equal weight when sample_weight is not provided.
+
+        max_features : int, float or {"sqrt", "log2"}, default=None
+            The number of features to consider when looking for the best split:
+
+        max_leaf_nodes : int, default=None
+            Grow a tree with ``max_leaf_nodes`` in best-first fashion.
+            Best nodes are defined as relative reduction in impurity.
+            If None then unlimited number of leaf nodes.
+
+        min_impurity_decrease : float, default=0.0
+            A node will be split if this split induces a decrease of the impurity
+            greater than or equal to this value.
+
+        ccp_alpha : non-negative float, default=0.0
+            Complexity parameter used for Minimal Cost-Complexity Pruning. The
+            subtree with the largest cost complexity that is smaller than
+            ``ccp_alpha`` will be chosen. By default, no pruning is performed.
+
+        monotonic_cst : array-like of int of shape (n_features), default=None
+            Indicates the monotonicity constraint to enforce on each feature.
+            - 1: monotonic increase
+            - 0: no constraint
+            - -1: monotonic decrease
+        """
+        self._validate_parameters(
+            max_rmp_calls,
+            criterion,
+            splitter,
+            max_depth,
+            min_samples_split,
+            min_samples_leaf,
+            min_weight_fraction_leaf,
+            max_features,
+            max_leaf_nodes,
+            min_impurity_decrease,
+            ccp_alpha,
+            monotonic_cst,
+        )
+
+        super().__init__(
+            threshold=threshold,
+            random_state=random_state,
+            solver=solver,
+            rule_cost=rule_cost,
+            class_weight=class_weight,
+        )
+
+        self.max_rmp_calls = int(max_rmp_calls)
+
+        self.criterion = criterion
+        self.splitter = splitter
+        self.max_depth = max_depth
+        self.min_samples_split = min_samples_split
+        self.min_samples_leaf = min_samples_leaf
+        self.min_weight_fraction_leaf = min_weight_fraction_leaf
+        self.max_features = max_features
+        self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
+
+        self._temp_rules = []
+
+    def _fit_decision_tree(
+        self, x: np.ndarray, y: np.ndarray, sample_weight: np.ndarray
+    ) -> DecisionTreeClassifier:
+        """
+        Fits a decision tree to the data, taking into account sample weights.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            Feature matrix of the training data.
+        y : np.ndarray
+            Target vector of the training data.
+        sample_weight : np.ndarray
+            Array of weights for the samples.
+
+        Returns
+        -------
+        DecisionTreeClassifier
+            A decision tree classifier fitted to the weighted data.
+        """
+        dt = DecisionTreeClassifier(
+            random_state=self._rng.integers(np.iinfo(np.int16).max),
+            criterion=self.criterion,
+            splitter=self.splitter,
+            class_weight=self.class_weight,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            ccp_alpha=self.ccp_alpha,
+            monotonic_cst=self.monotonic_cst,
+        )
+
+        if sample_weight is not None:
+            dt.class_weight = None
+
+        # Fit the decision tree to the data
+        return dt.fit(x, y, sample_weight=sample_weight)
+
+    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
+        """
+        Fits the RUGClassifier model to the training data using a rule generation approach.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels) as integers
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples get equal weights.
+
+        Returns
+        -------
+        RUGClassifier
+            The fitted model, ready for making predictions.
+        """
+        x, y = check_inputs(x, y)
+
+        sample_weight = self._get_sample_weight(sample_weight, y)
+
+        if self._is_fitted:
+            self._cleanup()
+
+        treeno = 0
+        fit_tree = self._fit_decision_tree(x, y, sample_weight=None)
+        self.decision_trees_[treeno] = fit_tree
+
+        self._get_class_infos(y)
+        vec_y = self._preprocess(y)
+        self._get_matrix(x, y, vec_y, fit_tree, treeno)
+
+        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
+
+        ws, betas = self.solver(
+            coefficients=self.coefficients_,
+            k=self.k_,
+            sample_weight=sample_weight,
+            normalization_constant=normalization_constant,
+        )
+
+        # Rule generation
+        for _ in range(self.max_rmp_calls):
+            if np.all(betas <= 1e-6):
+                break
+
+            treeno += 1
+            fit_tree = self._fit_decision_tree(x, y, sample_weight=betas)
+            self.decision_trees_[treeno] = fit_tree
+
+            no_improvement = self._get_matrix(x, y, vec_y, fit_tree, treeno, betas, normalization_constant)
+
+            if no_improvement:
+                break
+
+            ws, betas = self.solver(
+                coefficients=self.coefficients_,
+                k=self.k_,
+                ws0=ws.copy(),
+                normalization_constant=normalization_constant,
+                sample_weight=sample_weight,
+            )
+
+        self._fill_rules(ws)
+        self._is_fitted = True
+
+        return self
+
+    def _validate_parameters(
+        self,
+        max_rmp_calls,
+        criterion,
+        splitter,
+        max_depth,
+        min_samples_split,
+        min_samples_leaf,
+        min_weight_fraction_leaf,
+        max_features,
+        max_leaf_nodes,
+        min_impurity_decrease,
+        ccp_alpha,
+        monotonic_cst,
+    ):
+        # max_rmp_calls check
+        if not isinstance(max_rmp_calls, (float, int)):
+            raise TypeError("max_rmp_calls must be an integer.")
+
+        if max_rmp_calls < 0:
+            raise ValueError("max_rmp_calls must be a non-negative integer.")
+
+        # criterion check
+        if criterion not in {"gini", "entropy", "log_loss"}:
+            raise ValueError(
+                "criterion must be one of 'gini', 'entropy', or 'log_loss'."
+            )
+
+        # splitter check
+        if splitter not in {"best", "random"}:
+            raise ValueError("splitter must be 'best' or 'random'.")
+
+        # max_depth check
+        if max_depth is not None and not isinstance(max_depth, int):
+            raise TypeError("max_depth must be an integer or None.")
+        if isinstance(max_depth, int) and max_depth < 1:
+            raise ValueError("max_depth must be greater than 0.")
+
+        # min_samples_split check
+        if not isinstance(min_samples_split, (int, float)) or min_samples_split < 2:
+            raise ValueError(
+                "min_samples_split must be an integer or float greater than or equal to 2."
+            )
+
+        # min_samples_leaf check
+        if not isinstance(min_samples_leaf, (int, float)) or min_samples_leaf < 1:
+            raise ValueError(
+                "min_samples_leaf must be an integer or float greater than or equal to 1."
+            )
+
+        # min_weight_fraction_leaf check
+        if not isinstance(min_weight_fraction_leaf, float) or not (
+            0.0 <= min_weight_fraction_leaf <= 1.0
+        ):
+            raise ValueError(
+                "min_weight_fraction_leaf must be a float between 0.0 and 1.0."
+            )
+
+        # max_features check
+        if (
+            max_features is not None
+            and not isinstance(max_features, (int, float, str))
+            or (isinstance(max_features, str) and max_features not in {"sqrt", "log2"})
+        ):
+            raise ValueError(
+                "max_features must be an integer, float, 'sqrt', 'log2', or None."
+            )
+
+        # max_leaf_nodes check
+        if max_leaf_nodes is not None and (
+            not isinstance(max_leaf_nodes, int) or max_leaf_nodes < 1
+        ):
+            raise ValueError("max_leaf_nodes must be a positive integer or None.")
+
+        # min_impurity_decrease check
+        if not isinstance(min_impurity_decrease, float) or min_impurity_decrease < 0.0:
+            raise ValueError("min_impurity_decrease must be a non-negative float.")
+
+        # ccp_alpha check
+        if not isinstance(ccp_alpha, float) or ccp_alpha < 0.0:
+            raise ValueError("ccp_alpha must be a non-negative float.")
+
+        # monotonic_cst check
+        if monotonic_cst is not None and (
+            not isinstance(monotonic_cst, (list, tuple))
+            or not all(isinstance(item, int) for item in monotonic_cst)
+        ):
+            raise ValueError("monotonic_cst must be an array-like of integers or None.")
```

## ruleopt/estimator/sklearn_/rux.py

 * *Ordering differences only*

```diff
@@ -1,154 +1,154 @@
-from __future__ import annotations
-
-import numpy as np
-from sklearn.ensemble._forest import ForestClassifier
-from sklearn.ensemble import GradientBoostingClassifier
-from numpy.typing import ArrayLike
-
-from .base_sklearn import _RUGSKLEARN
-from ...rule_cost import Gini
-from ...utils import check_inputs
-from ...solver import ORToolsSolver
-
-
-class RUXClassifier(_RUGSKLEARN):
-    """
-    RUXClassifier aims to build a compact and interpretable model
-    by employing rule-based learning extracted from a trained scikit-learn
-    ensemble model such as Random Forests, Gradient Boosting Machines, 
-    and Extra-Trees Classifiers. It allows a user to trade off between
-    the complexity of the model (number of rules) and the accuracy of the model.
-    """
-
-    def __init__(
-        self,
-        trained_ensemble,
-        *,
-        solver=ORToolsSolver(),
-        rule_cost=Gini(),
-        class_weight: dict | str | None = None,
-        threshold: float = 1.0e-6,
-        random_state: int | None = None,
-    ):
-        """
-        Parameters
-        ----------
-        trained_ensemble : sklearn.ensemble object
-            The trained scikit-learn ensemble model from which the rules will be
-            extracted.
-
-        solver : OptimizationSolver, default=ORToolsSolver()
-            An instance of a derived class inherits from the 'Optimization Solver' base class.
-            The solver is responsible for optimizing the rule set based on the cost function
-            and constraints.
-
-        rule_cost : RuleCost or int, default=Gini()
-            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
-            or a fixed cost
-
-        class_weight: dict, "balanced" or None, default=None
-            A dictionary mapping class labels to their respective weights, the string "balanced"
-            to automatically adjust weights inversely proportional to class frequencies,
-            or None for no weights. Used to adjust the model in favor of certain classes.
-
-        threshold : float, default=1.0e-6
-            The minimum weight threshold for including a rule in the final model
-
-        random_state : int or None, default=None
-            Seed for the random number generator to ensure reproducible results.
-        """
-        if not (
-            isinstance(trained_ensemble, (GradientBoostingClassifier, ForestClassifier))
-        ):
-            raise TypeError(
-                "trained_ensemble must be an instance of ",
-                "sklearn.ensemble.GradientBoostingClassifier, ",
-                "sklearn.ensemble.RandomForestClassifier, ",
-                "or sklearn.ensemble.ExtraTreesClassifier.",
-            )
-
-        self.trained_ensemble = trained_ensemble
-        super().__init__(
-            threshold=threshold,
-            random_state=random_state,
-            rule_cost=rule_cost,
-            solver=solver,
-            class_weight=class_weight,
-        )
-
-    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray) -> None:
-        """
-        Prepares the optimization problem matrices based on the ensemble of decision trees.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The feature matrix of the training data.
-        y : np.ndarray
-            The target vector of the training data.
-        vec_y : np.ndarray
-            The preprocessed target vector, adjusted for optimization.
-        """
-        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
-            self._get_matrix(x, y, vec_y, fit_tree, treeno)
-
-    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
-        """
-        Fits the RUXClassifier to the training data.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels) as integers
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, then samples get equal weights.
-
-        Returns
-        -------
-        RUXClassifier
-            The fitted model, ready for making predictions.
-        """
-        x, y = check_inputs(x, y)
-
-        sample_weight = self._get_sample_weight(sample_weight, y)
-
-        # If the model has been fitted before, clean it up
-        if self._is_fitted:
-            self._cleanup()
-
-        # Fills the fitted decision trees.
-        tree_infos = self.trained_ensemble.estimators_
-        for treeno, fit_tree in enumerate(tree_infos):
-            self.decision_trees_[treeno] = (
-                fit_tree[0] if isinstance(fit_tree, np.ndarray) else fit_tree
-            )
-
-        # Extract and set properties of the target variable
-        self._get_class_infos(y)
-
-        # Preprocess the target values
-        vec_y = self._preprocess(y)
-
-        # Calculate the coefficients and other parameters for the optimization problem
-        self._get_matrices(x, y, vec_y)
-
-        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
-
-        # Solve the optimization problem again with the new rules
-        ws, *_ = self.solver(
-            coefficients=self.coefficients_,
-            k=self.k_,
-            sample_weight=sample_weight,
-            normalization_constant=normalization_constant,
-        )
-
-        # Fill the decision rules based on the weights obtained from the optimization problem
-        self._fill_rules(ws)
-
-        # Mark the model as fitted
-        self._is_fitted = True
-
-        # Return the fitted model
-        return self
+from __future__ import annotations
+
+import numpy as np
+from sklearn.ensemble._forest import ForestClassifier
+from sklearn.ensemble import GradientBoostingClassifier
+from numpy.typing import ArrayLike
+
+from .base_sklearn import _RUGSKLEARN
+from ...rule_cost import Gini
+from ...utils import check_inputs
+from ...solver import ORToolsSolver
+
+
+class RUXClassifier(_RUGSKLEARN):
+    """
+    RUXClassifier aims to build a compact and interpretable model
+    by employing rule-based learning extracted from a trained scikit-learn
+    ensemble model such as Random Forests, Gradient Boosting Machines, 
+    and Extra-Trees Classifiers. It allows a user to trade off between
+    the complexity of the model (number of rules) and the accuracy of the model.
+    """
+
+    def __init__(
+        self,
+        trained_ensemble,
+        *,
+        solver=ORToolsSolver(),
+        rule_cost=Gini(),
+        class_weight: dict | str | None = None,
+        threshold: float = 1.0e-6,
+        random_state: int | None = None,
+    ):
+        """
+        Parameters
+        ----------
+        trained_ensemble : sklearn.ensemble object
+            The trained scikit-learn ensemble model from which the rules will be
+            extracted.
+
+        solver : OptimizationSolver, default=ORToolsSolver()
+            An instance of a derived class inherits from the 'Optimization Solver' base class.
+            The solver is responsible for optimizing the rule set based on the cost function
+            and constraints.
+
+        rule_cost : RuleCost or int, default=Gini()
+            Defines the cost of rules, either as a specific calculation method (RuleCost instance)
+            or a fixed cost
+
+        class_weight: dict, "balanced" or None, default=None
+            A dictionary mapping class labels to their respective weights, the string "balanced"
+            to automatically adjust weights inversely proportional to class frequencies,
+            or None for no weights. Used to adjust the model in favor of certain classes.
+
+        threshold : float, default=1.0e-6
+            The minimum weight threshold for including a rule in the final model
+
+        random_state : int or None, default=None
+            Seed for the random number generator to ensure reproducible results.
+        """
+        if not (
+            isinstance(trained_ensemble, (GradientBoostingClassifier, ForestClassifier))
+        ):
+            raise TypeError(
+                "trained_ensemble must be an instance of ",
+                "sklearn.ensemble.GradientBoostingClassifier, ",
+                "sklearn.ensemble.RandomForestClassifier, ",
+                "or sklearn.ensemble.ExtraTreesClassifier.",
+            )
+
+        self.trained_ensemble = trained_ensemble
+        super().__init__(
+            threshold=threshold,
+            random_state=random_state,
+            rule_cost=rule_cost,
+            solver=solver,
+            class_weight=class_weight,
+        )
+
+    def _get_matrices(self, x: np.ndarray, y: np.ndarray, vec_y: np.ndarray) -> None:
+        """
+        Prepares the optimization problem matrices based on the ensemble of decision trees.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The feature matrix of the training data.
+        y : np.ndarray
+            The target vector of the training data.
+        vec_y : np.ndarray
+            The preprocessed target vector, adjusted for optimization.
+        """
+        for treeno, fit_tree in enumerate(self.decision_trees_.values()):
+            self._get_matrix(x, y, vec_y, fit_tree, treeno)
+
+    def fit(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike | None = None):
+        """
+        Fits the RUXClassifier to the training data.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels) as integers
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples get equal weights.
+
+        Returns
+        -------
+        RUXClassifier
+            The fitted model, ready for making predictions.
+        """
+        x, y = check_inputs(x, y)
+
+        sample_weight = self._get_sample_weight(sample_weight, y)
+
+        # If the model has been fitted before, clean it up
+        if self._is_fitted:
+            self._cleanup()
+
+        # Fills the fitted decision trees.
+        tree_infos = self.trained_ensemble.estimators_
+        for treeno, fit_tree in enumerate(tree_infos):
+            self.decision_trees_[treeno] = (
+                fit_tree[0] if isinstance(fit_tree, np.ndarray) else fit_tree
+            )
+
+        # Extract and set properties of the target variable
+        self._get_class_infos(y)
+
+        # Preprocess the target values
+        vec_y = self._preprocess(y)
+
+        # Calculate the coefficients and other parameters for the optimization problem
+        self._get_matrices(x, y, vec_y)
+
+        normalization_constant = 1.0 / np.max(self.coefficients_.costs)
+
+        # Solve the optimization problem again with the new rules
+        ws, *_ = self.solver(
+            coefficients=self.coefficients_,
+            k=self.k_,
+            sample_weight=sample_weight,
+            normalization_constant=normalization_constant,
+        )
+
+        # Fill the decision rules based on the weights obtained from the optimization problem
+        self._fill_rules(ws)
+
+        # Mark the model as fitted
+        self._is_fitted = True
+
+        # Return the fitted model
+        return self
```

## ruleopt/explainer/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-from .explainer import (Explainer )
-
-__all__ = [
+from .explainer import (Explainer )
+
+__all__ = [
     "Explainer"]
```

## ruleopt/explainer/explainer.py

 * *Ordering differences only*

```diff
@@ -1,263 +1,263 @@
-from __future__ import annotations
-import warnings
-import numpy as np
-from sklearn.utils import check_array
-from sklearn.utils.validation import check_is_fitted
-from ..estimator.base import _RUGBASE
-
-from numpy.typing import ArrayLike
-
-
-class Explainer:
-    """
-    Initializes the Explainer with a given estimator. The estimator must be fitted and
-    of a type that inherits from _RUGBASE, such as RUGClassifier, RUXClassifier,
-    RUXLGBMClassifier, or RUXXGBClassifier.
-    """
-
-    def __init__(self, estimator: _RUGBASE) -> None:
-        """
-        Parameters
-        ----------
-        estimator : ruleopt.estimator instance
-            A fitted estimator of a type that inherits from _RUGBASE.
-        """
-        if not isinstance(estimator, _RUGBASE):
-            raise TypeError(
-                "Estimator should be an instance of a class inheriting from _RUGBASE, ",
-                f"not {type(estimator)}",
-            )
-
-        check_is_fitted(estimator, attributes=["_is_fitted"])
-
-        self.estimator = estimator
-
-    def retrieve_rule_details(
-        self,
-        feature_names: list | None = None,
-        indices: list | None = None,
-        info: bool = True,
-    ) -> dict:
-        """
-        Retrieves and optionally prints detailed information about the specified rules.
-        If indices are provided, information for those specific rules is returned.
-        Otherwise, information for all rules is returned.
-
-        Parameters
-        ----------
-        feature_names : list or None, default=None
-            List of feature names for more readable rule descriptions. If None, indices are used.
-
-        indices :list or None, default=None
-            Indices of the rules to retrieve. If None, retrieves all rules.
-
-        info : bool, default=True
-            If True, prints the rules' details in a human-readable format.
-
-        Returns
-        -------
-        dict
-            A dictionary mapping each rule index to its details, including label, weight,
-            rule description, and statistical distribution. If a rule has no conditions,
-            it sets the majority class.
-        """
-        rules = self.estimator.decision_rules_
-        if indices is not None:
-            # Validate indices
-            max_index = max(rules.keys())
-            indices = [i for i in indices if i <= max_index]
-            if len(indices) < len(set(indices)):
-                warnings.warn("Some specified indices are out of range.")
-        else:
-            indices = list(rules.keys())
-
-        return_dict = {}
-        for indx in indices:
-            rule = rules.get(indx, None)
-            if rule is None:
-                continue  # Skip if rule does not exist, alternative to raising an error
-            rule_details = {
-                "label": int(rule.label),
-                "weight": float(rule.weight),
-                "rule": (
-                    rule.to_dict(feature_names)
-                    if rule
-                    else "No Rule: Set Majority Class"
-                ),
-                "sdist": rule.sdist.tolist(),
-            }
-            return_dict[indx] = rule_details
-            if info:
-                self._display_rule_info(indx, rule, feature_names)
-
-        return return_dict
-
-    def find_applicable_rules_for_samples(
-        self,
-        x: ArrayLike,
-        threshold: float = 0.0,
-        feature_names: list | None = None,
-        info: bool = True,
-    ) -> list:
-        """
-        Identifies which rules apply to each instance in the provided input data
-        based on a given threshold. Optionally, prints detailed information about
-        each rule that applies to the instances.
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-
-        threshold : float, default=0.0
-            Minimum rule weight threshold for considering a rule as covering an instance.
-
-        feature_names : list or None, default=None
-            List of feature names for more readable rule descriptions. If None, indices are used.
-
-        info : bool, default=True
-            If True, prints the details of the applicable rules for each instance.
-
-        Returns
-        -------
-        List[List[int]]
-            A list of lists, where each inner list contains the indices of rules that cover
-            the corresponding instance in `x`.
-        """
-        x = check_array(np.asarray(x, dtype=np.float32), force_all_finite="allow-nan")
-
-        selected_rules = []
-        rule_indexs = []
-        for rule_index, rule in self.estimator.decision_rules_.items():
-            if rule.weight >= threshold:
-                selected_rules.append(rule)
-                rule_indexs.append(rule_index)
-
-        rule_matrix = np.zeros((x.shape[0], len(selected_rules)), dtype=np.int8)
-
-        for rule_index, rule in enumerate(selected_rules):
-            rule_matrix[:, rule_index] = rule.check_rule(x)
-
-        index_list = [np.where(row > 0)[0].tolist() for row in rule_matrix]
-
-        if info:
-            for i, applied_rules in enumerate(index_list):
-                print(f"Rules for instance {i}")
-
-                if len(applied_rules) > 0:
-                    for rule_id in applied_rules:
-                        self._display_rule_info(
-                            rule_indexs[rule_id], rule, feature_names
-                        )
-
-                else:
-                    print(
-                        f"No rules applicable. Filled with majority class.\nClass: {self.estimator.majority_class_}\n"
-                    )
-
-        return index_list
-
-    def _display_rule_info(self, indx, rule, feature_names=None) -> None:
-        """
-        Prints the details of a specified rule in a human-readable format. This
-        method is designed for internal use to support other public methods that
-        may require detailed rule information to be printed.
-
-        Parameters
-        ----------
-        indx : int
-            Index of the rule being printed.
-
-        rule : Rule object
-            The rule whose details are to be printed.
-
-        feature_names : Optional[List[str]], default=None
-            List of feature names for more readable rule descriptions. If None,
-            feature indices are used.
-        """
-        print(f"RULE {indx}:")
-        rule_description = (
-            rule.to_text(feature_names) if feature_names else rule.to_text()
-        )
-        print(rule_description)
-        print(f"Class: {rule.label}")
-        print(f"Scaled rule weight: {rule.weight:.4f}\n")
-
-    def summarize_rule_metrics(self, info: bool = True) -> dict:
-        """
-        Calculates and optionally prints the total number of rules and the average
-        rule length within the model. 
-        
-        If instance is not covered by any rule, rule length counts as 0. 
-
-        Parameters
-        ----------
-        info : bool, default=True
-            If True, prints the summary information.
-
-        Returns
-        -------
-        dict
-            A dictionary containing 'num_of_rules' (the total number of rules) and
-            'avg_rule_length' (the average length of the rules).
-        """
-        num_of_rules = len(self.estimator.decision_rules_)
-        avg_rule_length = np.mean(
-            [len(rule) for rule in self.estimator.decision_rules_.values()]
-        )
-
-        if info:
-            print(f"Total number of rules: {num_of_rules}")
-            print(f"Average rule length: {avg_rule_length:.2f}")
-
-        return {"num_of_rules": num_of_rules, "avg_rule_length": avg_rule_length}
-
-    def evaluate_rule_coverage_metrics(self, x: ArrayLike, info: bool = True) -> dict:
-        """
-        Calculates metrics including the number of instances not covered by any
-        rule ('num_of_missed'), the average number of rules per sample
-        ('avg_num_rules_per_sample'), and the average rule length per sample
-        ('avg_rule_length_per_sample'). Optionally, prints this information.
-        
-        If instance is not covered by any rule, rule length counts as 0. 
-
-        Parameters
-        ----------
-        x : array-like of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to dtype=np.float32.
-
-        info : bool, default=True
-            If True, prints the calculated metrics.
-
-        Returns
-        -------
-        dict
-            A dictionary with calculated metrics: 'num_of_missed', 'avg_num_rules_per_sample',
-            and 'avg_rule_length_per_sample'.
-        """
-        x = check_array(np.asarray(x, dtype=np.float32), force_all_finite="allow-nan")
-
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
-                self.estimator.predict(x, predict_info=True)
-            )
-
-        results = {
-            "num_of_missed": len(missed_values_index_),
-            "avg_num_rules_per_sample": np.mean(rules_per_sample_),
-            "avg_rule_length_per_sample": np.mean(rule_length_per_sample_),
-        }
-
-        if info:
-            print(
-                f"Number of instances not covered by any rule: {results['num_of_missed']}"
-            )
-            print(
-                f"Average number of rules per sample: {results['avg_num_rules_per_sample']:.2f}"
-            )
-            print(
-                f"Average length of rules per sample: {results['avg_rule_length_per_sample']:.2f}"
-            )
-
-        return results
+from __future__ import annotations
+import warnings
+import numpy as np
+from sklearn.utils import check_array
+from sklearn.utils.validation import check_is_fitted
+from ..estimator.base import _RUGBASE
+
+from numpy.typing import ArrayLike
+
+
+class Explainer:
+    """
+    Initializes the Explainer with a given estimator. The estimator must be fitted and
+    of a type that inherits from _RUGBASE, such as RUGClassifier, RUXClassifier,
+    RUXLGBMClassifier, or RUXXGBClassifier.
+    """
+
+    def __init__(self, estimator: _RUGBASE) -> None:
+        """
+        Parameters
+        ----------
+        estimator : ruleopt.estimator instance
+            A fitted estimator of a type that inherits from _RUGBASE.
+        """
+        if not isinstance(estimator, _RUGBASE):
+            raise TypeError(
+                "Estimator should be an instance of a class inheriting from _RUGBASE, ",
+                f"not {type(estimator)}",
+            )
+
+        check_is_fitted(estimator, attributes=["_is_fitted"])
+
+        self.estimator = estimator
+
+    def retrieve_rule_details(
+        self,
+        feature_names: list | None = None,
+        indices: list | None = None,
+        info: bool = True,
+    ) -> dict:
+        """
+        Retrieves and optionally prints detailed information about the specified rules.
+        If indices are provided, information for those specific rules is returned.
+        Otherwise, information for all rules is returned.
+
+        Parameters
+        ----------
+        feature_names : list or None, default=None
+            List of feature names for more readable rule descriptions. If None, indices are used.
+
+        indices :list or None, default=None
+            Indices of the rules to retrieve. If None, retrieves all rules.
+
+        info : bool, default=True
+            If True, prints the rules' details in a human-readable format.
+
+        Returns
+        -------
+        dict
+            A dictionary mapping each rule index to its details, including label, weight,
+            rule description, and statistical distribution. If a rule has no conditions,
+            it sets the majority class.
+        """
+        rules = self.estimator.decision_rules_
+        if indices is not None:
+            # Validate indices
+            max_index = max(rules.keys())
+            indices = [i for i in indices if i <= max_index]
+            if len(indices) < len(set(indices)):
+                warnings.warn("Some specified indices are out of range.")
+        else:
+            indices = list(rules.keys())
+
+        return_dict = {}
+        for indx in indices:
+            rule = rules.get(indx, None)
+            if rule is None:
+                continue  # Skip if rule does not exist, alternative to raising an error
+            rule_details = {
+                "label": int(rule.label),
+                "weight": float(rule.weight),
+                "rule": (
+                    rule.to_dict(feature_names)
+                    if rule
+                    else "No Rule: Set Majority Class"
+                ),
+                "sdist": rule.sdist.tolist(),
+            }
+            return_dict[indx] = rule_details
+            if info:
+                self._display_rule_info(indx, rule, feature_names)
+
+        return return_dict
+
+    def find_applicable_rules_for_samples(
+        self,
+        x: ArrayLike,
+        threshold: float = 0.0,
+        feature_names: list | None = None,
+        info: bool = True,
+    ) -> list:
+        """
+        Identifies which rules apply to each instance in the provided input data
+        based on a given threshold. Optionally, prints detailed information about
+        each rule that applies to the instances.
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+
+        threshold : float, default=0.0
+            Minimum rule weight threshold for considering a rule as covering an instance.
+
+        feature_names : list or None, default=None
+            List of feature names for more readable rule descriptions. If None, indices are used.
+
+        info : bool, default=True
+            If True, prints the details of the applicable rules for each instance.
+
+        Returns
+        -------
+        List[List[int]]
+            A list of lists, where each inner list contains the indices of rules that cover
+            the corresponding instance in `x`.
+        """
+        x = check_array(np.asarray(x, dtype=np.float32), force_all_finite="allow-nan")
+
+        selected_rules = []
+        rule_indexs = []
+        for rule_index, rule in self.estimator.decision_rules_.items():
+            if rule.weight >= threshold:
+                selected_rules.append(rule)
+                rule_indexs.append(rule_index)
+
+        rule_matrix = np.zeros((x.shape[0], len(selected_rules)), dtype=np.int8)
+
+        for rule_index, rule in enumerate(selected_rules):
+            rule_matrix[:, rule_index] = rule.check_rule(x)
+
+        index_list = [np.where(row > 0)[0].tolist() for row in rule_matrix]
+
+        if info:
+            for i, applied_rules in enumerate(index_list):
+                print(f"Rules for instance {i}")
+
+                if len(applied_rules) > 0:
+                    for rule_id in applied_rules:
+                        self._display_rule_info(
+                            rule_indexs[rule_id], rule, feature_names
+                        )
+
+                else:
+                    print(
+                        f"No rules applicable. Filled with majority class.\nClass: {self.estimator.majority_class_}\n"
+                    )
+
+        return index_list
+
+    def _display_rule_info(self, indx, rule, feature_names=None) -> None:
+        """
+        Prints the details of a specified rule in a human-readable format. This
+        method is designed for internal use to support other public methods that
+        may require detailed rule information to be printed.
+
+        Parameters
+        ----------
+        indx : int
+            Index of the rule being printed.
+
+        rule : Rule object
+            The rule whose details are to be printed.
+
+        feature_names : Optional[List[str]], default=None
+            List of feature names for more readable rule descriptions. If None,
+            feature indices are used.
+        """
+        print(f"RULE {indx}:")
+        rule_description = (
+            rule.to_text(feature_names) if feature_names else rule.to_text()
+        )
+        print(rule_description)
+        print(f"Class: {rule.label}")
+        print(f"Scaled rule weight: {rule.weight:.4f}\n")
+
+    def summarize_rule_metrics(self, info: bool = True) -> dict:
+        """
+        Calculates and optionally prints the total number of rules and the average
+        rule length within the model. 
+        
+        If instance is not covered by any rule, rule length counts as 0. 
+
+        Parameters
+        ----------
+        info : bool, default=True
+            If True, prints the summary information.
+
+        Returns
+        -------
+        dict
+            A dictionary containing 'num_of_rules' (the total number of rules) and
+            'avg_rule_length' (the average length of the rules).
+        """
+        num_of_rules = len(self.estimator.decision_rules_)
+        avg_rule_length = np.mean(
+            [len(rule) for rule in self.estimator.decision_rules_.values()]
+        )
+
+        if info:
+            print(f"Total number of rules: {num_of_rules}")
+            print(f"Average rule length: {avg_rule_length:.2f}")
+
+        return {"num_of_rules": num_of_rules, "avg_rule_length": avg_rule_length}
+
+    def evaluate_rule_coverage_metrics(self, x: ArrayLike, info: bool = True) -> dict:
+        """
+        Calculates metrics including the number of instances not covered by any
+        rule ('num_of_missed'), the average number of rules per sample
+        ('avg_num_rules_per_sample'), and the average rule length per sample
+        ('avg_rule_length_per_sample'). Optionally, prints this information.
+        
+        If instance is not covered by any rule, rule length counts as 0. 
+
+        Parameters
+        ----------
+        x : array-like of shape (n_samples, n_features)
+            The training input samples. Internally, it will be converted to dtype=np.float32.
+
+        info : bool, default=True
+            If True, prints the calculated metrics.
+
+        Returns
+        -------
+        dict
+            A dictionary with calculated metrics: 'num_of_missed', 'avg_num_rules_per_sample',
+            and 'avg_rule_length_per_sample'.
+        """
+        x = check_array(np.asarray(x, dtype=np.float32), force_all_finite="allow-nan")
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            missed_values_index_, rules_per_sample_, rule_length_per_sample_ = (
+                self.estimator.predict(x, predict_info=True)
+            )
+
+        results = {
+            "num_of_missed": len(missed_values_index_),
+            "avg_num_rules_per_sample": np.mean(rules_per_sample_),
+            "avg_rule_length_per_sample": np.mean(rule_length_per_sample_),
+        }
+
+        if info:
+            print(
+                f"Number of instances not covered by any rule: {results['num_of_missed']}"
+            )
+            print(
+                f"Average number of rules per sample: {results['avg_num_rules_per_sample']:.2f}"
+            )
+            print(
+                f"Average length of rules per sample: {results['avg_rule_length_per_sample']:.2f}"
+            )
+
+        return results
```

## ruleopt/rule_cost/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-from .rule_cost import Length, Gini, Mixed, MixedSigmoid, RuleCost
-
-__all__ = ["Length", "Gini", "Mixed", "MixedSigmoid", "RuleCost"]
+from .rule_cost import Length, Gini, Mixed, MixedSigmoid, RuleCost
+
+__all__ = ["Length", "Gini", "Mixed", "MixedSigmoid", "RuleCost"]
```

## ruleopt/rule_cost/rule_cost.py

 * *Ordering differences only*

```diff
@@ -1,207 +1,207 @@
-from abc import abstractmethod, ABC
-import numpy as np
-from ..aux_classes import Rule
-
-
-class RuleCost(ABC):
-    """
-    Abstract base class representing the cost associated with a rule or a set of rules.
-
-    This class is designed to be subclassed by specific cost calculation implementations.
-    Each subclass should provide a specific cost calculation strategy by overriding the
-    `__call__` method. The `__call__` method allows instances of the subclass to be used
-    as if they were functions, directly invoking the cost calculation.
-    """
-
-    @abstractmethod
-    def __call__(self):
-        """
-        Abstract method to be implemented by subclasses to calculate and return the cost.
-
-        This method should take relevant parameters as input (e.g., the rule or set of
-        rules being evaluated) and return a numerical value representing the cost. The
-        exact implementation details and parameters are to be defined in the subclass.
-
-        Returns
-        -------
-        cost : float
-            The calculated cost of the rule or set of rules. This is a numerical value
-            indicating the cost or penalty associated with the rule(s) based on the
-            specific calculation strategy implemented in the subclass.
-        """
-
-
-class Length(RuleCost):
-    """
-    Calculate the cost of a rule based on its length.
-    """
-
-    def __call__(self, temp_rule: Rule, *args, **kwargs) -> int:
-        """
-        Calculate and return the cost of the rule.
-
-        Parameters
-        ----------
-        temp_rule : Rule
-            The rule to calculate the cost for.
-
-        Returns
-        -------
-        int
-            The cost of the rule, defined as its length.
-        """
-        cost = len(temp_rule)
-        return cost
-
-
-class Gini(RuleCost):
-    """
-    Calculate the Gini cost of a split.
-    
-    .. math::
-       Gini = 1 - \\sum_{i=1}^{n}(p_i)^2,
-
-    where
-    
-    - :math:`p_i` is the probability of an object being classified to a particular class.
-
-    """
-
-    def __call__(self, counts: np.ndarray, *args, **kwargs) -> float:
-        """
-        Calculate and return the Gini cost for a node.
-
-        Parameters
-        ----------
-        counts : np.ndarray
-            An array containing the counts of each class in a node.
-
-        Returns
-        -------
-        float
-            The Gini cost for the node.
-        """
-        probs = np.divide(counts, np.sum(counts))
-        cost = 1 - np.sum(np.square(probs))
-        return cost
-
-
-class Mixed(RuleCost):
-    """
-    Calculate the mixed cost, combining class separation and data selection terms with
-    a weighting parameter.
-    
-    The mixed cost for a rule is calculated as follows:
-
-    .. math::
-       Mixed = w \\times class\\_separation\\_term + (1 - w) \\times data\\_selection\\_term,
-
-    where
-
-    - :math:`w` is the weighting parameter to balance class separation and data selection terms,
-    - :math:`class\\_separation\\_term` is :math:`1 - \\left(1 - \\left(\\frac{\\min(covers)}{number\\_of\\_classes}\\right)\\right)`,
-    - :math:`data\\_selection\\_term` is :math:`1 - \\left(\\frac{number\\_of\\_classes}{total\\_samples}\\right)`.
-
-    
-    """
-
-    def __init__(self, w: float = 0.7) -> None:
-        """
-        Initialize the mixed cost calculation with a weighting parameter.
-
-        Parameters
-        ----------
-        w : float, optional, default=0.7
-            Weighting parameter to balance class separation and data selection terms.
-        """
-        self.w = w
-
-    def __call__(self, covers: np.ndarray, y: np.ndarray, *args, **kwargs) -> float:
-        """
-        Calculate and return the mixed cost for a rule.
-
-        Parameters
-        ----------
-        covers : np.ndarray
-            Array of cover sizes for the classes.
-
-        y : np.ndarray
-            The target array.
-
-        Returns
-        -------
-        float
-            The mixed cost for the rule.
-        """
-        class_separation_term = 1 - (1 - (np.min(covers) / covers.shape[0]))
-        data_selection_term = 1 - (covers.shape[0] / y.shape[0])
-        cost = self.w * class_separation_term + (1 - self.w) * data_selection_term
-        return cost
-
-
-class MixedSigmoid(RuleCost):
-    """
-    Calculate the mixed cost with a sigmoid adjustment based on weighting and alpha
-    parameters.
-    
-    The sigmoid-adjusted mixed cost for a rule is calculated as follows:
-
-    .. math::
-       MixedSigmoid = \\frac{1}{1 + e^{-\\alpha (w \\times class\\_separation\\_term + (1 - w) \\times data\\_selection\\_term - 0.5)}},
-
-    where
-
-    - :math:`w` is the weighting parameter to balance class separation and data selection terms,
-    - :math:`\\alpha` is the scaling parameter to adjust the steepness of the sigmoid function,
-    - :math:`class\\_separation\\_term` is :math:`1 - \\left(1 - \\left(\\frac{\\min(covers)}{number\\_of\\_classes}\\right)\\right)`,
-    - :math:`data\\_selection\\_term` is :math:`1 - \\left(\\frac{number\\_of\\_classes}{total\\_samples}\\right)`.    
-
-    """
-
-    def __init__(self, w: float = 0.7, alpha: float = 10) -> None:
-        """
-        Initialize the sigmoid-adjusted mixed cost calculation with weighting and
-        alpha parameters.
-
-        Parameters
-        ----------
-        w : float, optional, default=0.7
-            Weighting parameter to balance class separation and data selection terms.
-
-        alpha : float, optional, default=10
-            Scaling parameter to adjust the steepness of the sigmoid function.
-        """
-        self.w = w
-        self.alpha = alpha
-
-    def __call__(self, covers: np.ndarray, y: np.ndarray, *args, **kwargs) -> float:
-        """
-        Calculate and return the sigmoid-adjusted mixed cost for a rule.
-
-        Parameters
-        ----------
-        covers : np.ndarray
-            Array of cover sizes for the classes.
-
-        y : np.ndarray
-            The target array.
-
-        Returns
-        -------
-        float
-            The sigmoid-adjusted mixed cost for the rule.
-        """
-        class_separation_term = 1 - (1 - (np.min(covers) / covers.shape[0]))
-        data_selection_term = 1 - (covers.shape[0] / y.shape[0])
-        cost = 1 / (
-            1
-            + np.exp(
-                -self.alpha
-                * (
-                    self.w * class_separation_term
-                    + (1 - self.w) * data_selection_term
-                    - 0.5
-                )
-            )
-        )
-        return cost
+from abc import abstractmethod, ABC
+import numpy as np
+from ..aux_classes import Rule
+
+
+class RuleCost(ABC):
+    """
+    Abstract base class representing the cost associated with a rule or a set of rules.
+
+    This class is designed to be subclassed by specific cost calculation implementations.
+    Each subclass should provide a specific cost calculation strategy by overriding the
+    `__call__` method. The `__call__` method allows instances of the subclass to be used
+    as if they were functions, directly invoking the cost calculation.
+    """
+
+    @abstractmethod
+    def __call__(self):
+        """
+        Abstract method to be implemented by subclasses to calculate and return the cost.
+
+        This method should take relevant parameters as input (e.g., the rule or set of
+        rules being evaluated) and return a numerical value representing the cost. The
+        exact implementation details and parameters are to be defined in the subclass.
+
+        Returns
+        -------
+        cost : float
+            The calculated cost of the rule or set of rules. This is a numerical value
+            indicating the cost or penalty associated with the rule(s) based on the
+            specific calculation strategy implemented in the subclass.
+        """
+
+
+class Length(RuleCost):
+    """
+    Calculate the cost of a rule based on its length.
+    """
+
+    def __call__(self, temp_rule: Rule, *args, **kwargs) -> int:
+        """
+        Calculate and return the cost of the rule.
+
+        Parameters
+        ----------
+        temp_rule : Rule
+            The rule to calculate the cost for.
+
+        Returns
+        -------
+        int
+            The cost of the rule, defined as its length.
+        """
+        cost = len(temp_rule)
+        return cost
+
+
+class Gini(RuleCost):
+    """
+    Calculate the Gini cost of a split.
+    
+    .. math::
+       Gini = 1 - \\sum_{i=1}^{n}(p_i)^2,
+
+    where
+    
+    - :math:`p_i` is the probability of an object being classified to a particular class.
+
+    """
+
+    def __call__(self, counts: np.ndarray, *args, **kwargs) -> float:
+        """
+        Calculate and return the Gini cost for a node.
+
+        Parameters
+        ----------
+        counts : np.ndarray
+            An array containing the counts of each class in a node.
+
+        Returns
+        -------
+        float
+            The Gini cost for the node.
+        """
+        probs = np.divide(counts, np.sum(counts))
+        cost = 1 - np.sum(np.square(probs))
+        return cost
+
+
+class Mixed(RuleCost):
+    """
+    Calculate the mixed cost, combining class separation and data selection terms with
+    a weighting parameter.
+    
+    The mixed cost for a rule is calculated as follows:
+
+    .. math::
+       Mixed = w \\times class\\_separation\\_term + (1 - w) \\times data\\_selection\\_term,
+
+    where
+
+    - :math:`w` is the weighting parameter to balance class separation and data selection terms,
+    - :math:`class\\_separation\\_term` is :math:`1 - \\left(1 - \\left(\\frac{\\min(covers)}{number\\_of\\_classes}\\right)\\right)`,
+    - :math:`data\\_selection\\_term` is :math:`1 - \\left(\\frac{number\\_of\\_classes}{total\\_samples}\\right)`.
+
+    
+    """
+
+    def __init__(self, w: float = 0.7) -> None:
+        """
+        Initialize the mixed cost calculation with a weighting parameter.
+
+        Parameters
+        ----------
+        w : float, optional, default=0.7
+            Weighting parameter to balance class separation and data selection terms.
+        """
+        self.w = w
+
+    def __call__(self, covers: np.ndarray, y: np.ndarray, *args, **kwargs) -> float:
+        """
+        Calculate and return the mixed cost for a rule.
+
+        Parameters
+        ----------
+        covers : np.ndarray
+            Array of cover sizes for the classes.
+
+        y : np.ndarray
+            The target array.
+
+        Returns
+        -------
+        float
+            The mixed cost for the rule.
+        """
+        class_separation_term = 1 - (1 - (np.min(covers) / covers.shape[0]))
+        data_selection_term = 1 - (covers.shape[0] / y.shape[0])
+        cost = self.w * class_separation_term + (1 - self.w) * data_selection_term
+        return cost
+
+
+class MixedSigmoid(RuleCost):
+    """
+    Calculate the mixed cost with a sigmoid adjustment based on weighting and alpha
+    parameters.
+    
+    The sigmoid-adjusted mixed cost for a rule is calculated as follows:
+
+    .. math::
+       MixedSigmoid = \\frac{1}{1 + e^{-\\alpha (w \\times class\\_separation\\_term + (1 - w) \\times data\\_selection\\_term - 0.5)}},
+
+    where
+
+    - :math:`w` is the weighting parameter to balance class separation and data selection terms,
+    - :math:`\\alpha` is the scaling parameter to adjust the steepness of the sigmoid function,
+    - :math:`class\\_separation\\_term` is :math:`1 - \\left(1 - \\left(\\frac{\\min(covers)}{number\\_of\\_classes}\\right)\\right)`,
+    - :math:`data\\_selection\\_term` is :math:`1 - \\left(\\frac{number\\_of\\_classes}{total\\_samples}\\right)`.    
+
+    """
+
+    def __init__(self, w: float = 0.7, alpha: float = 10) -> None:
+        """
+        Initialize the sigmoid-adjusted mixed cost calculation with weighting and
+        alpha parameters.
+
+        Parameters
+        ----------
+        w : float, optional, default=0.7
+            Weighting parameter to balance class separation and data selection terms.
+
+        alpha : float, optional, default=10
+            Scaling parameter to adjust the steepness of the sigmoid function.
+        """
+        self.w = w
+        self.alpha = alpha
+
+    def __call__(self, covers: np.ndarray, y: np.ndarray, *args, **kwargs) -> float:
+        """
+        Calculate and return the sigmoid-adjusted mixed cost for a rule.
+
+        Parameters
+        ----------
+        covers : np.ndarray
+            Array of cover sizes for the classes.
+
+        y : np.ndarray
+            The target array.
+
+        Returns
+        -------
+        float
+            The sigmoid-adjusted mixed cost for the rule.
+        """
+        class_separation_term = 1 - (1 - (np.min(covers) / covers.shape[0]))
+        data_selection_term = 1 - (covers.shape[0] / y.shape[0])
+        cost = 1 / (
+            1
+            + np.exp(
+                -self.alpha
+                * (
+                    self.w * class_separation_term
+                    + (1 - self.w) * data_selection_term
+                    - 0.5
+                )
+            )
+        )
+        return cost
```

## ruleopt/solver/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from .ortools_solver import ORToolsSolver
-from .base import OptimizationSolver
-from .gurobi_solver import GurobiSolver
-from .cplex_solver import CPLEXSolver
-
-
-__all__ = ["ORToolsSolver", "GurobiSolver", "CPLEXSolver", "OptimizationSolver"]
+from .ortools_solver import ORToolsSolver
+from .base import OptimizationSolver
+from .gurobi_solver import GurobiSolver
+from .cplex_solver import CPLEXSolver
+
+
+__all__ = ["ORToolsSolver", "GurobiSolver", "CPLEXSolver", "OptimizationSolver"]
```

## ruleopt/solver/base.py

```diff
@@ -1,82 +1,93 @@
-from abc import ABC, abstractmethod
-from typing import Any
-import warnings
-
-
-class OptimizationSolver(ABC):
-    """
-    This abstract base class defines the interface for a generic solver.
-    Implementations of this class must provide the `__call__` method, 
-    allowing the solver to be invoked as if it were a function.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-        if not hasattr(self, "penalty"):
-            raise AttributeError("Subclasses must define 'penalty'")
-        if not hasattr(self, "use_sparse"):
-            raise AttributeError("Subclasses must define 'use_sparse'")
-
-    @abstractmethod
-    def __call__(self, *args: Any, **kwds: Any) -> Any:
-        """
-        Executes the solver using the provided arguments and keyword arguments.
-
-        Parameters:
-            *args (Any): Positional arguments required for solving the problem.
-            **kwds (Any): Keyword arguments required for solving the problem.
-
-        Returns:
-            Any: The result of the solving process.
-        """
-        pass
-
-    def _check_params(self):
-        if not isinstance(self.penalty, (float, int)) or self.penalty <= 0:
-            raise TypeError("penalty must be a positive float.")
-
-        if not isinstance(self.use_sparse, bool):
-            raise TypeError(f"use_sparse must be True or False.")
-
-        if hasattr(self, "solver_type"):
-            valid_solvers = [
-                "CLP",
-                "GLOP",
-                "GUROBI_LP",
-                "CPLEX_LP",
-                "XPRESS_LP",
-                "GLPK_LP",
-                "HiGHS",
-            ]
-            if (
-                not isinstance(self.solver_type, str)
-                or self.solver_type not in valid_solvers
-            ):
-                raise ValueError(f"solver_type must be one of {valid_solvers}.")
-
-        if hasattr(self, "lr"):
-            if not isinstance(self.lr, (float, int)) or self.lr <= 0:
-                raise TypeError("lr must be a positive float.")
-            
-        if hasattr(self, "constraint_cost"):
-            if not isinstance(self.constraint_cost, (float, int)) or self.constraint_cost <= 0:
-                raise TypeError("constraint_cost must be a positive float.")
-
-        if hasattr(self, "weight_decay"):
-            if not isinstance(self.weight_decay, (int, float)) or self.weight_decay < 0:
-                raise TypeError("weight_decay must be a non-negative float.")
-
-        if hasattr(self, "patience"):
-            if not isinstance(self.patience, int) or self.patience <= 0:
-                raise TypeError("patience must be a positive integer.")
-
-        if hasattr(self, "device"):
-            valid_devices = ["cuda", "cpu"]
-            if not isinstance(self.device, str) or self.device not in valid_devices:
-                raise ValueError(f"solver_type must be one of {valid_devices}.")
-
-        if self.use_sparse:
-            warnings.warn(
-                "A sparse data format is being used. If your dataset is not sufficiently "
-                "large, using a sparse format could lead to performance issues.",
-            )
+from abc import ABC, abstractmethod
+from typing import Any
+import warnings
+
+
+class OptimizationSolver(ABC):
+    """
+    This abstract base class defines the interface for a generic solver.
+    Implementations of this class must provide the `__call__` method, 
+    allowing the solver to be invoked as if it were a function.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.penalty: float | int
+        self.use_sparse: bool
+        self.solver_type: str | None
+        self.lr: float | int | None
+        self.constraint_cost: float | int | None
+        self.weight_decay: float | int | None
+        self.patience: int | None
+        self.device: str | None
+        self._check_params()
+
+    @abstractmethod
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        """
+        Executes the solver using the provided arguments and keyword arguments.
+
+        Parameters:
+            *args (Any): Positional arguments required for solving the problem.
+            **kwds (Any): Keyword arguments required for solving the problem.
+
+        Returns:
+            Any: The result of the solving process.
+        """
+        pass
+
+    def _check_params(self):
+        if not hasattr(self, "penalty"):
+            raise AttributeError("Subclasses must define 'penalty'")
+        
+        if not hasattr(self, "use_sparse"):
+            raise AttributeError("Subclasses must define 'use_sparse'")
+        
+        if not isinstance(self.penalty, (float, int)) or self.penalty <= 0:
+            raise TypeError("penalty must be a positive float.")
+
+        if not isinstance(self.use_sparse, bool):
+            raise TypeError(f"use_sparse must be True or False.")
+
+        if hasattr(self, "solver_type"):
+            valid_solvers = [
+                "CLP",
+                "GLOP",
+                "GUROBI_LP",
+                "CPLEX_LP",
+                "XPRESS_LP",
+                "GLPK_LP",
+                "HiGHS",
+            ]
+            if (
+                not isinstance(self.solver_type, str)
+                or self.solver_type not in valid_solvers
+            ):
+                raise ValueError(f"solver_type must be one of {valid_solvers}.")
+
+        if hasattr(self, "lr"):
+            if not isinstance(self.lr, (float, int)) or self.lr <= 0:
+                raise TypeError("lr must be a positive float.")
+            
+        if hasattr(self, "constraint_cost"):
+            if not isinstance(self.constraint_cost, (float, int)) or self.constraint_cost <= 0:
+                raise TypeError("constraint_cost must be a positive float.")
+
+        if hasattr(self, "weight_decay"):
+            if not isinstance(self.weight_decay, (int, float)) or self.weight_decay < 0:
+                raise TypeError("weight_decay must be a non-negative float.")
+
+        if hasattr(self, "patience"):
+            if not isinstance(self.patience, int) or self.patience <= 0:
+                raise TypeError("patience must be a positive integer.")
+
+        if hasattr(self, "device"):
+            valid_devices = ["cuda", "cpu"]
+            if not isinstance(self.device, str) or self.device not in valid_devices:
+                raise ValueError(f"solver_type must be one of {valid_devices}.")
+
+        if self.use_sparse:
+            warnings.warn(
+                "A sparse data format is being used. If your dataset is not sufficiently "
+                "large, using a sparse format could lead to performance issues.",
+            )
```

## ruleopt/solver/cplex_solver.py

```diff
@@ -1,126 +1,125 @@
-from typing import Tuple
-import numpy as np
-from scipy.sparse import csr_matrix
-from ..utils import check_module_available
-from .base import OptimizationSolver
-
-CPLEX_AVAILABLE = check_module_available("docplex")
-
-
-class CPLEXSolver(OptimizationSolver):
-    """
-    A solver wrapper class for linear optimization using the CPLEX solver.
-
-    The solver supports both dense and sparse matrix representations.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if not CPLEX_AVAILABLE:
-            raise ImportError(
-                "CPLEX is required for this class but is not installed.",
-                "Please install it with 'pip install docplex cplex'",
-            )
-        instance = super(CPLEXSolver, cls).__new__(cls)
-        return instance
-
-    def __init__(
-        self,
-        penalty: float = 1.0,
-        use_sparse: bool = False,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        penalty : float, default=2.0
-            Penalty parameter for the cost in the objective function.
-        use_sparse : bool, default=False
-            Determines whether to use a sparse matrix representation for the optimization
-            problem. Using sparse matrices can significantly reduce memory usage and improve
-            performance for large-scale problems with many zeros in the data.
-        """
-        self.penalty = penalty
-        self.use_sparse = use_sparse
-        super().__init__()
-        super()._check_params()
-
-    def __call__(
-        self,
-        coefficients,
-        k: int,
-        sample_weight,
-        normalization_constant,
-        ws0: np.ndarray = None,
-        *args,
-        **kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Parameters
-        ----------
-        coefficients : object
-            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
-            and costs associated with each rule ('costs').
-        k : float
-            A scaling factor for the coefficients.
-        ws0 : array-like, optional
-            Initial weights for the optimization process. If provided, should have the same
-            length as the number of rules. Otherwise, weights are initialized to ones.
-
-        Returns
-        -------
-        ws : numpy.ndarray
-            The optimal weights for each rule.
-        betas : numpy.ndarray
-            The optimal dual solution.
-        """
-        ### LAZY IMPORT
-        from docplex.mp.model import Model
-
-        a_hat = csr_matrix(
-            (
-                coefficients.yvals,
-                (coefficients.rows, coefficients.cols),
-            ),
-            dtype=np.float64,
-        ) * ((k - 1.0) / k)
-
-        if not self.use_sparse:
-            a_hat = a_hat.toarray()
-
-        costs = np.array(coefficients.costs, copy=False)
-
-        n, m = a_hat.shape
-        # Primal Model
-        modprimal = Model("RUXG Primal")
-
-        # Variables
-        vs = modprimal.continuous_var_list(n, name="vs")
-        ws = modprimal.continuous_var_list(m, name="ws")
-
-        # Set initial values
-        initial_values = []
-
-        if ws0 is not None:
-            initial_values += [(ws[i], ws0[i]) for i in range(len(ws0))]
-
-        # Assign initial solution
-        modprimal.start = initial_values
-
-        # Objective
-        modprimal.minimize(
-            modprimal.sum(vs * sample_weight)
-            + modprimal.scal_prod(ws, costs * self.penalty * normalization_constant)
-        )
-        # Constraints
-        for i in range(n):
-            modprimal.add_constraint(
-                modprimal.sum(a_hat[i, j] * ws[j] for j in range(m)) + vs[i] >= 1.0
-            )
-
-        modprimal.solve()
-
-        betas = np.array(
-            [c.dual_value for c in modprimal.iter_constraints()], dtype=np.float64
-        )
-        ws = np.array([v.solution_value for v in ws], dtype=np.float64)
-
-        return ws, betas
+from typing import Tuple
+import numpy as np
+from scipy.sparse import csr_matrix
+from ..utils import check_module_available
+from .base import OptimizationSolver
+
+CPLEX_AVAILABLE = check_module_available("docplex")
+
+
+class CPLEXSolver(OptimizationSolver):
+    """
+    A solver wrapper class for linear optimization using the CPLEX solver.
+
+    The solver supports both dense and sparse matrix representations.
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if not CPLEX_AVAILABLE:
+            raise ImportError(
+                "CPLEX is required for this class but is not installed.",
+                "Please install it with 'pip install docplex cplex'",
+            )
+        instance = super(CPLEXSolver, cls).__new__(cls)
+        return instance
+
+    def __init__(
+        self,
+        penalty: float = 1.0,
+        use_sparse: bool = False,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        penalty : float, default=1.0
+            Penalty parameter for the cost in the objective function.
+        use_sparse : bool, default=False
+            Determines whether to use a sparse matrix representation for the optimization
+            problem. Using sparse matrices can significantly reduce memory usage and improve
+            performance for large-scale problems with many zeros in the data.
+        """
+        self.penalty = penalty
+        self.use_sparse = use_sparse
+        super().__init__()
+
+    def __call__(
+        self,
+        coefficients,
+        k: int,
+        sample_weight,
+        normalization_constant,
+        ws0: np.ndarray = None,
+        *args,
+        **kwargs,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Parameters
+        ----------
+        coefficients : object
+            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
+            and costs associated with each rule ('costs').
+        k : float
+            A scaling factor for the coefficients.
+        ws0 : array-like, optional
+            Initial weights for the optimization process. If provided, should have the same
+            length as the number of rules. Otherwise, weights are initialized to ones.
+
+        Returns
+        -------
+        ws : numpy.ndarray
+            The optimal weights for each rule.
+        betas : numpy.ndarray
+            The optimal dual solution.
+        """
+        ### LAZY IMPORT
+        from docplex.mp.model import Model
+
+        a_hat = csr_matrix(
+            (
+                coefficients.yvals,
+                (coefficients.rows, coefficients.cols),
+            ),
+            dtype=np.float64,
+        ) * ((k - 1.0) / k)
+
+        if not self.use_sparse:
+            a_hat = a_hat.toarray()
+
+        costs = np.array(coefficients.costs, copy=False)
+
+        n, m = a_hat.shape
+        # Primal Model
+        modprimal = Model("RUXG Primal")
+
+        # Variables
+        vs = modprimal.continuous_var_list(n, name="vs")
+        ws = modprimal.continuous_var_list(m, name="ws")
+
+        # Set initial values
+        initial_values = []
+
+        if ws0 is not None:
+            initial_values += [(ws[i], ws0[i]) for i in range(len(ws0))]
+
+        # Assign initial solution
+        modprimal.start = initial_values
+
+        # Objective
+        modprimal.minimize(
+            modprimal.sum(vs * sample_weight)
+            + modprimal.scal_prod(ws, costs * self.penalty * normalization_constant)
+        )
+        # Constraints
+        for i in range(n):
+            modprimal.add_constraint(
+                modprimal.sum(a_hat[i, j] * ws[j] for j in range(m)) + vs[i] >= 1.0
+            )
+
+        modprimal.solve()
+
+        betas = np.array(
+            [c.dual_value for c in modprimal.iter_constraints()], dtype=np.float64
+        )
+        ws = np.array([v.solution_value for v in ws], dtype=np.float64)
+
+        return ws, betas
```

## ruleopt/solver/gurobi_solver.py

```diff
@@ -1,118 +1,117 @@
-from typing import Tuple
-import numpy as np
-from scipy.sparse import csr_matrix
-from ..utils import check_module_available
-from .base import OptimizationSolver
-
-GUROBI_AVAILABLE = check_module_available("gurobipy")
-
-
-class GurobiSolver(OptimizationSolver):
-    """
-    A solver wrapper class for linear optimization using the Gurobi solver.
-
-    The solver supports both dense and sparse matrix representations.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if not GUROBI_AVAILABLE:
-            raise ImportError(
-                "Gurobi is required for this class but is not installed.",
-                "Please install it with 'pip install gurobipy'",
-            )
-        instance = super(GurobiSolver, cls).__new__(cls)
-        return instance
-
-    def __init__(
-        self,
-        penalty: float = 1.0,
-        use_sparse: bool = False,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        penalty : float, default=2.0
-            Penalty parameter for the cost in the objective function.
-
-        use_sparse : bool, default=False
-            Determines whether to use a sparse matrix representation for the optimization
-            problem. Using sparse matrices can significantly reduce memory usage and improve
-            performance for large-scale problems with many zeros in the data.
-        """
-        self.penalty = penalty
-        self.use_sparse = use_sparse
-        super().__init__()
-        super()._check_params()
-
-    def __call__(
-        self,
-        coefficients,
-        k: int,
-        sample_weight,
-        normalization_constant,
-        ws0: np.ndarray = None,
-        *args,
-        **kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Parameters
-        ----------
-        coefficients : object
-            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
-            and costs associated with each rule ('costs').
-        k : float
-            A scaling factor for the coefficients.
-        ws0 : array-like, optional
-            Initial weights for the optimization process. If provided, should have the same
-            length as the number of rules. Otherwise, weights are initialized to ones.
-
-        Returns
-        -------
-        ws : numpy.ndarray
-            The optimized weights for each rule after the optimization process.
-        betas : numpy.ndarray
-            The betas values indicating constraint violations for the optimized solution.
-        """
-        ### LAZY IMPORT
-        from gurobipy import Model, GRB
-
-        a_hat = csr_matrix(
-            (
-                coefficients.yvals,
-                (coefficients.rows, coefficients.cols),
-            ),
-            dtype=np.float64,
-        ) * ((k - 1.0) / k)
-
-        if not self.use_sparse:
-            a_hat = a_hat.toarray()
-
-        costs = np.array(coefficients.costs, copy=False)
-
-        n, m = a_hat.shape
-
-        modprimal = Model("RUG Primal")
-        modprimal.setParam("OutputFlag", False)
-        # Variables
-        vs = modprimal.addMVar(shape=int(n), name="vs")
-        ws = modprimal.addMVar(shape=int(m), name="ws")
-
-        if ws0 is not None:
-            tempws = np.zeros(m)
-            tempws[: len(ws0)] = ws0
-            ws.setAttr("Start", tempws)
-            modprimal.update()
-
-        # Objective
-        modprimal.setObjective(
-            sample_weight @ vs + (costs * self.penalty * normalization_constant) @ ws,
-            GRB.MINIMIZE,
-        )
-        # Constraints
-        modprimal.addConstr(a_hat @ ws + vs >= 1.0, name="a_hat Constraints")
-
-        modprimal.optimize()
-
-        betas = np.array(modprimal.getAttr(GRB.Attr.Pi)[:n])
-
-        return ws.X, betas
+from typing import Tuple
+import numpy as np
+from scipy.sparse import csr_matrix
+from ..utils import check_module_available
+from .base import OptimizationSolver
+
+GUROBI_AVAILABLE = check_module_available("gurobipy")
+
+
+class GurobiSolver(OptimizationSolver):
+    """
+    A solver wrapper class for linear optimization using the Gurobi solver.
+
+    The solver supports both dense and sparse matrix representations.
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if not GUROBI_AVAILABLE:
+            raise ImportError(
+                "Gurobi is required for this class but is not installed.",
+                "Please install it with 'pip install gurobipy'",
+            )
+        instance = super(GurobiSolver, cls).__new__(cls)
+        return instance
+
+    def __init__(
+        self,
+        penalty: float = 1.0,
+        use_sparse: bool = False,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        penalty : float, default=1.0
+            Penalty parameter for the cost in the objective function.
+
+        use_sparse : bool, default=False
+            Determines whether to use a sparse matrix representation for the optimization
+            problem. Using sparse matrices can significantly reduce memory usage and improve
+            performance for large-scale problems with many zeros in the data.
+        """
+        self.penalty = penalty
+        self.use_sparse = use_sparse
+        super().__init__()
+
+    def __call__(
+        self,
+        coefficients,
+        k: int,
+        sample_weight,
+        normalization_constant,
+        ws0: np.ndarray = None,
+        *args,
+        **kwargs,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Parameters
+        ----------
+        coefficients : object
+            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
+            and costs associated with each rule ('costs').
+        k : float
+            A scaling factor for the coefficients.
+        ws0 : array-like, optional
+            Initial weights for the optimization process. If provided, should have the same
+            length as the number of rules. Otherwise, weights are initialized to ones.
+
+        Returns
+        -------
+        ws : numpy.ndarray
+            The optimized weights for each rule after the optimization process.
+        betas : numpy.ndarray
+            The betas values indicating constraint violations for the optimized solution.
+        """
+        ### LAZY IMPORT
+        from gurobipy import Model, GRB
+
+        a_hat = csr_matrix(
+            (
+                coefficients.yvals,
+                (coefficients.rows, coefficients.cols),
+            ),
+            dtype=np.float64,
+        ) * ((k - 1.0) / k)
+
+        if not self.use_sparse:
+            a_hat = a_hat.toarray()
+
+        costs = np.array(coefficients.costs, copy=False)
+
+        n, m = a_hat.shape
+
+        modprimal = Model("RUG Primal")
+        modprimal.setParam("OutputFlag", False)
+        # Variables
+        vs = modprimal.addMVar(shape=int(n), name="vs")
+        ws = modprimal.addMVar(shape=int(m), name="ws")
+
+        if ws0 is not None:
+            tempws = np.zeros(m)
+            tempws[: len(ws0)] = ws0
+            ws.setAttr("Start", tempws)
+            modprimal.update()
+
+        # Objective
+        modprimal.setObjective(
+            sample_weight @ vs + (costs * self.penalty * normalization_constant) @ ws,
+            GRB.MINIMIZE,
+        )
+        # Constraints
+        modprimal.addConstr(a_hat @ ws + vs >= 1.0, name="a_hat Constraints")
+
+        modprimal.optimize()
+
+        betas = np.array(modprimal.getAttr(GRB.Attr.Pi)[:n])
+
+        return ws.X, betas
```

## ruleopt/solver/ortools_solver.py

```diff
@@ -1,143 +1,142 @@
-from typing import Any
-from scipy.sparse import csr_matrix
-import numpy as np
-from ..utils import check_module_available
-from .base import OptimizationSolver
-
-
-ORTOOLS_AVAILABLE = check_module_available("ortools")
-
-
-class ORToolsSolver(OptimizationSolver):
-    """
-    A solver wrapper class for linear optimization using the Google's OR-Tools solver.
-    
-    The solver supports both dense and sparse matrix representations.
-
-    This solver can handle large-scale linear programming problems by interfacing with
-    various backend solvers such as CLP, GLOP, and proprietary solvers like Gurobi and CPLEX.
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if not ORTOOLS_AVAILABLE:
-            raise ImportError(
-                "OR-Tools is required for this class but is not installed.",
-                "Please install it with 'pip install ortools'",
-            )
-        instance = super(ORToolsSolver, cls).__new__(cls)
-        return instance
-
-    def __init__(
-        self,
-        penalty: float = 1.0,
-        solver_type: str = "GLOP",
-        use_sparse: bool = False,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        penalty : float, default=2.0
-            Penalty parameter for the cost in the objective function.
-
-        solver_type : {"CLP", "GLOP", "GUROBI_LP", "CPLEX_LP", "XPRESS_LP", "GLPK_LP", "HiGHS"}, default="GLOP"
-            The type of Linear Programming solver to use.
-
-        use_sparse : bool, default=False
-            Determines whether to use a sparse matrix representation for the optimization
-            problem. Using sparse matrices can significantly reduce memory usage and improve
-            performance for large-scale problems with many zeros in the data.
-        """
-        self.solver_type = solver_type
-        self.penalty = penalty
-        self.use_sparse = use_sparse
-        super().__init__()
-        super()._check_params()
-
-    def __call__(self, coefficients, k, sample_weight, normalization_constant, *args, **kwargs) -> Any:
-        """
-        Solves a linear optimization problem with the given coefficients and penalty.
-
-        Parameters
-        ----------
-        coefficients : object
-            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
-            and costs associated with each rule ('costs').
-        k : float
-            A scaling factor for the coefficients.
-
-        Returns
-        -------
-        ws : numpy.ndarray
-            The optimized weights for each rule after the optimization process.
-        betas : numpy.ndarray
-            The betas values indicating constraint violations for the optimized solution.
-
-        Raises
-        ------
-        ValueError
-            If the specified solver type is not supported or not linked correctly.
-        """
-        ### LAZY IMPORT
-        from ortools.linear_solver.python import model_builder
-        from pandas import Index
-
-        a_hat = csr_matrix(
-            (
-                coefficients.yvals,
-                (coefficients.rows, coefficients.cols),
-            ),
-            dtype=np.float64,
-        ) * ((k - 1.0) / k)
-
-        if not self.use_sparse:
-            a_hat = a_hat.toarray()
-
-        n, m = a_hat.shape
-
-        costs = np.array(coefficients.costs, dtype=np.float32)
-
-        model = model_builder.Model()
-        solver = model_builder.Solver(self.solver_type)
-
-        if not solver.solver_is_supported():
-            raise ValueError(
-                f"Support for {self.solver_type} not linked in, or the license ",
-                "was not found.",
-            )
-
-        # Variables
-        vs = model.new_num_var_series(
-            name="vs", index=Index(np.arange(n)), lower_bounds=0
-        )
-        ws = model.new_num_var_series(
-            name="ws", index=Index(np.arange(m)), lower_bounds=0
-        )
-
-        # Objective
-        model.minimize(vs @ sample_weight + normalization_constant * self.penalty * costs @ ws)
-
-        # Constraints
-        model.add((a_hat @ ws + vs).map(lambda x: x >= 1))
-
-        solver.solve(model)
-
-        ws = solver.values(ws).values
-        betas = solver.dual_values(model._get_linear_constraints()).values
-
-        return ws, betas
-
-    def _validate_parameters(self, solver_type, penalty_parameter):
-        valid_solvers = [
-            "CLP",
-            "GLOP",
-            "GUROBI_LP",
-            "CPLEX_LP",
-            "XPRESS_LP",
-            "GLPK_LP",
-            "HiGHS",
-        ]
-        if not isinstance(solver_type, str) or solver_type not in valid_solvers:
-            raise ValueError(f"solver_type must be one of {valid_solvers}.")
-
-        if not isinstance(penalty_parameter, (float, int)) or penalty_parameter <= 0:
-            raise ValueError("penalty_parameter must be a positive float or integer.")
+from typing import Any
+from scipy.sparse import csr_matrix
+import numpy as np
+from ..utils import check_module_available
+from .base import OptimizationSolver
+
+
+ORTOOLS_AVAILABLE = check_module_available("ortools")
+
+
+class ORToolsSolver(OptimizationSolver):
+    """
+    A solver wrapper class for linear optimization using the Google's OR-Tools solver.
+    
+    The solver supports both dense and sparse matrix representations.
+
+    This solver can handle large-scale linear programming problems by interfacing with
+    various backend solvers such as CLP, GLOP, and proprietary solvers like Gurobi and CPLEX.
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if not ORTOOLS_AVAILABLE:
+            raise ImportError(
+                "OR-Tools is required for this class but is not installed.",
+                "Please install it with 'pip install ortools'",
+            )
+        instance = super(ORToolsSolver, cls).__new__(cls)
+        return instance
+
+    def __init__(
+        self,
+        penalty: float = 1.0,
+        solver_type: str = "GLOP",
+        use_sparse: bool = False,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        penalty : float, default=1.0
+            Penalty parameter for the cost in the objective function.
+
+        solver_type : {"CLP", "GLOP", "GUROBI_LP", "CPLEX_LP", "XPRESS_LP", "GLPK_LP", "HiGHS"}, default="GLOP"
+            The type of Linear Programming solver to use.
+
+        use_sparse : bool, default=False
+            Determines whether to use a sparse matrix representation for the optimization
+            problem. Using sparse matrices can significantly reduce memory usage and improve
+            performance for large-scale problems with many zeros in the data.
+        """
+        self.solver_type = solver_type
+        self.penalty = penalty
+        self.use_sparse = use_sparse
+        super().__init__()
+
+    def __call__(self, coefficients, k, sample_weight, normalization_constant, *args, **kwargs) -> Any:
+        """
+        Solves a linear optimization problem with the given coefficients and penalty.
+
+        Parameters
+        ----------
+        coefficients : object
+            An object containing the sparse matrix coefficients ('yvals', 'rows', 'cols'),
+            and costs associated with each rule ('costs').
+        k : float
+            A scaling factor for the coefficients.
+
+        Returns
+        -------
+        ws : numpy.ndarray
+            The optimized weights for each rule after the optimization process.
+        betas : numpy.ndarray
+            The betas values indicating constraint violations for the optimized solution.
+
+        Raises
+        ------
+        ValueError
+            If the specified solver type is not supported or not linked correctly.
+        """
+        ### LAZY IMPORT
+        from ortools.linear_solver.python import model_builder
+        from pandas import Index
+
+        a_hat = csr_matrix(
+            (
+                coefficients.yvals,
+                (coefficients.rows, coefficients.cols),
+            ),
+            dtype=np.float64,
+        ) * ((k - 1.0) / k)
+
+        if not self.use_sparse:
+            a_hat = a_hat.toarray()
+
+        n, m = a_hat.shape
+
+        costs = np.array(coefficients.costs, dtype=np.float32)
+
+        model = model_builder.Model()
+        solver = model_builder.Solver(self.solver_type)
+
+        if not solver.solver_is_supported():
+            raise ValueError(
+                f"Support for {self.solver_type} not linked in, or the license ",
+                "was not found.",
+            )
+
+        # Variables
+        vs = model.new_num_var_series(
+            name="vs", index=Index(np.arange(n)), lower_bounds=0
+        )
+        ws = model.new_num_var_series(
+            name="ws", index=Index(np.arange(m)), lower_bounds=0
+        )
+
+        # Objective
+        model.minimize(vs @ sample_weight + normalization_constant * self.penalty * costs @ ws)
+
+        # Constraints
+        model.add((a_hat @ ws + vs).map(lambda x: x >= 1))
+
+        solver.solve(model)
+
+        ws = solver.values(ws).values
+        betas = solver.dual_values(model._get_linear_constraints()).values
+
+        return ws, betas
+
+    def _validate_parameters(self, solver_type, penalty_parameter):
+        valid_solvers = [
+            "CLP",
+            "GLOP",
+            "GUROBI_LP",
+            "CPLEX_LP",
+            "XPRESS_LP",
+            "GLPK_LP",
+            "HiGHS",
+        ]
+        if not isinstance(solver_type, str) or solver_type not in valid_solvers:
+            raise ValueError(f"solver_type must be one of {valid_solvers}.")
+
+        if not isinstance(penalty_parameter, (float, int)) or penalty_parameter <= 0:
+            raise ValueError("penalty_parameter must be a positive float or integer.")
```

## ruleopt/utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from .utils import (check_inputs, check_module_available, check_sample_weight)
-
-__all__ = [
-    "check_inputs",
-    "check_module_available",
+from .utils import (check_inputs, check_module_available, check_sample_weight)
+
+__all__ = [
+    "check_inputs",
+    "check_module_available",
     "check_sample_weight"]
```

## ruleopt/utils/utils.py

 * *Ordering differences only*

```diff
@@ -1,40 +1,40 @@
-from typing import Tuple
-from sklearn.utils import check_array
-import numpy as np
-from numpy.typing import ArrayLike
-import importlib.util
-
-
-def check_inputs(x: ArrayLike, y: ArrayLike = None) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Validates and preprocesses input data for the model.
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples, n_features)
-        The training input samples. Internally, it will be converted to dtype=np.float32.
-    y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-        The target values (class labels) as integers
-
-    Returns
-    -------
-    Tuple[np.ndarray, np.ndarray]
-        The validated and preprocessed input matrix `x` and target vector `y`.
-    """
-    x = check_array(x, dtype=np.float32, force_all_finite="allow-nan")
-    if y is not None:
-        y = check_array(y, ensure_2d=False, dtype=np.intp)
-        return x, y
-    return x
-
-
-def check_sample_weight(sample_weight: ArrayLike):
-    return check_array(sample_weight, ensure_2d=False, dtype=np.float32)
-
-
-def check_module_available(module_name):
-    """
-    Checks module is installed.
-    """
-    spec = importlib.util.find_spec(module_name)
-    return spec is not None
+from typing import Tuple
+from sklearn.utils import check_array
+import numpy as np
+from numpy.typing import ArrayLike
+import importlib.util
+
+
+def check_inputs(x: ArrayLike, y: ArrayLike = None) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Validates and preprocesses input data for the model.
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples, n_features)
+        The training input samples. Internally, it will be converted to dtype=np.float32.
+    y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+        The target values (class labels) as integers
+
+    Returns
+    -------
+    Tuple[np.ndarray, np.ndarray]
+        The validated and preprocessed input matrix `x` and target vector `y`.
+    """
+    x = check_array(x, dtype=np.float32, force_all_finite="allow-nan")
+    if y is not None:
+        y = check_array(y, ensure_2d=False, dtype=np.intp)
+        return x, y
+    return x
+
+
+def check_sample_weight(sample_weight: ArrayLike):
+    return check_array(sample_weight, ensure_2d=False, dtype=np.float32)
+
+
+def check_module_available(module_name):
+    """
+    Checks module is installed.
+    """
+    spec = importlib.util.find_spec(module_name)
+    return spec is not None
```

## Comparing `ruleopt-1.0.0.dist-info/LICENSE` & `ruleopt-1.0.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2024 Ilker Birbil, Nursen Aydin, Ozgur Martin, Samet Copur
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+BSD 3-Clause License
+
+Copyright (c) 2024 Ilker Birbil, Nursen Aydin, Ozgur Martin, Samet Copur
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Comparing `ruleopt-1.0.0.dist-info/METADATA` & `ruleopt-1.0.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: ruleopt
-Version: 1.0.0
-Summary: Optimization-Based Rule Learning for Classification
-Author-email: Ilker Birbil <sibirbil@gmail.com>, Nursen Aydin <nursenaydin@gmail.com>, Ozgür Martin <ozgurmartin@gmail.com>, Samet Copur <sametcopur@yahoo.com>
-License: BSD 3-Clause License
-Project-URL: Documentation, https://ruleopt.readthedocs.io/
-Project-URL: Repository, https://github.com/sametcopur/ruleopt
-Project-URL: Tracker, https://github.com/sametcopur/ruleopt/issues
-Keywords: python,data-science,machine-learning,linear-programming,machine-learning-library,explainable-ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scikit-learn >=1.4.1
-Requires-Dist: numpy >=1.25.2
-Requires-Dist: pandas >=2.0.3
-Requires-Dist: scipy >=1.11.4
-Requires-Dist: ortools >=9.9.3963
-
-# RuleOpt
-## Optimization-Based Rule Learning for Classification
-
-RuleOpt is an optimization-based rule learning algorithm designed for classification problems. Focusing on scalability and interpretability, RuleOpt utilizes linear programming for rule generation and extraction. An earlier version of this work is available in [our manuscript](https://arxiv.org/abs/2104.10751).
-
- The Python library `ruleopt` is capable to extract rules from ensemble models, and it also implements a novel rule generation scheme. The library ensures compatibility with existing machine learning pipelines, and it is especially efficient for tackling large-scale problems.
-
-Here are a few highlights of `ruleopt`:
-
-- **Efficient Rule Generation and Extraction**: Leverages linear programming for scalable rule generation (stand-alone machine learning method) and rule extraction from trained random forest and boosting models.
-- **Interpretability**: Prioritizes model transparency by assigning costs to rules in order to achieve a desirable balance with accuracy.
-- **Integration with Machine Learning Libraries**: Facilitates smooth integration with well-known Python libraries `scikit-learn`, `LightGBM`, and `XGBoost`, and existing machine learning pipelines.
-- **Extensive Solver Support**: Supports a wide array of solvers, including _Gurobi_, _CPLEX_ and _OR-Tools_.
-
-### Installation 
-To install `ruleopt`, you can just use the pip command:
-
-```bash
-pip install ruleopt
-```
-### Usage
-
-To use `ruleopt`, you need to initialize the `ruleopt` class with your specific parameters and fit it to your data. Here's a basic example:
-
-
-```python
-from sklearn.model_selection import train_test_split
-from sklearn.datasets import load_iris
-
-from ruleopt import RUGClassifier
-from ruleopt.rule_cost import Gini
-from ruleopt.solver import ORToolsSolver
-
-# Set a random state for reproducibility
-random_state = 42
-
-# Load the Iris dataset
-X, y = load_iris(return_X_y=True)
-
-# Split the dataset into training and testing sets
-X_train, X_test, y_train, y_test = train_test_split(
-    X, y, test_size=0.2, random_state=random_state
-)
-
-# Define tree parameters
-tree_parameters = {"max_depth": 3, "class_weight": "balanced"}
-
-solver = ORToolsSolver()
-rule_cost = Gini()
-
-# Initialize the RUGClassifier with specific parameters
-rug = RUGClassifier(
-    solver=solver,
-    random_state=random_state,
-    max_rmp_calls=20,
-    rule_cost=rule_cost,
-    **tree_parameters,
-)
-
-# Fit the RUGClassifier to the training data
-rug.fit(X_train, y_train)
-
-# Predict the labels of the testing set
-y_pred = rug.predict(X_test)
-```
-### Documentation
-For more detailed information about the API and advanced usage, please refer to the full  [documentation](https://ruleopt.readthedocs.io/en/latest/).
-
-### Contributing
-Contributions are welcome! If you'd like to improve `ruleopt` or suggest new features, feel free to fork the repository and submit a pull request.
-
-### License
-`ruleopt` is released under the BSD 3-Clause License. See the LICENSE file for more details.
+Metadata-Version: 2.1
+Name: ruleopt
+Version: 1.0.1
+Summary: Optimization-Based Rule Learning for Classification
+Author-email: Ilker Birbil <sibirbil@gmail.com>, Nursen Aydin <nursenaydin@gmail.com>, Ozgür Martin <ozgurmartin@gmail.com>, Samet Copur <sametcopur@yahoo.com>
+License: BSD 3-Clause License
+Project-URL: Documentation, https://ruleopt.readthedocs.io/
+Project-URL: Repository, https://github.com/sametcopur/ruleopt
+Project-URL: Tracker, https://github.com/sametcopur/ruleopt/issues
+Keywords: python,data-science,machine-learning,linear-programming,machine-learning-library,explainable-ai
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scikit-learn >=1.4.1
+Requires-Dist: numpy >=1.25.2
+Requires-Dist: pandas >=2.0.3
+Requires-Dist: scipy >=1.11.4
+Requires-Dist: ortools >=9.9.3963
+
+# RuleOpt
+## Optimization-Based Rule Learning for Classification
+
+RuleOpt is an optimization-based rule learning algorithm designed for classification problems. Focusing on scalability and interpretability, RuleOpt utilizes linear programming for rule generation and extraction. An earlier version of this work is available in [our manuscript](https://arxiv.org/abs/2104.10751).
+
+ The Python library `ruleopt` is capable of extracting rules from ensemble models, and it also implements a novel rule generation scheme. The library ensures compatibility with existing machine learning pipelines, and it is especially efficient for tackling large-scale problems.
+
+Here are a few highlights of `ruleopt`:
+
+- **Efficient Rule Generation and Extraction**: Leverages linear programming for scalable rule generation (stand-alone machine learning method) and rule extraction from trained random forest and boosting models.
+- **Interpretability**: Prioritizes model transparency by assigning costs to rules in order to achieve a desirable balance with accuracy.
+- **Integration with Machine Learning Libraries**: Facilitates smooth integration with well-known Python libraries `scikit-learn`, `LightGBM`, and `XGBoost`, and existing machine learning pipelines.
+- **Extensive Solver Support**: Supports a wide array of solvers, including _Gurobi_, _CPLEX_ and _OR-Tools_.
+
+### Installation 
+To install `ruleopt`, use the following pip command:
+
+```bash
+pip install ruleopt
+```
+### Usage
+
+To use `ruleopt`, you need to initialize the `ruleopt` class with your specific parameters and fit it to your data. Here's a basic example:
+
+
+```python
+from sklearn.model_selection import train_test_split
+from sklearn.datasets import load_iris
+
+from ruleopt import RUGClassifier
+from ruleopt.rule_cost import Gini
+from ruleopt.solver import ORToolsSolver
+
+# Set a random state for reproducibility
+random_state = 42
+
+# Load the Iris dataset
+X, y = load_iris(return_X_y=True)
+
+# Split the dataset into training and testing sets
+X_train, X_test, y_train, y_test = train_test_split(
+    X, y, test_size=0.2, random_state=random_state
+)
+
+# Define tree parameters
+tree_parameters = {"max_depth": 3, "class_weight": "balanced"}
+
+solver = ORToolsSolver()
+rule_cost = Gini()
+
+# Initialize the RUGClassifier with specific parameters
+rug = RUGClassifier(
+    solver=solver,
+    random_state=random_state,
+    max_rmp_calls=20,
+    rule_cost=rule_cost,
+    **tree_parameters,
+)
+
+# Fit the RUGClassifier to the training data
+rug.fit(X_train, y_train)
+
+# Predict the labels of the testing set
+y_pred = rug.predict(X_test)
+```
+### Documentation
+For more detailed information about the API and advanced usage, please refer to the full  [documentation](https://ruleopt.readthedocs.io/en/latest/).
+
+### Contributing
+Contributions are welcome! If you'd like to improve `ruleopt` or suggest new features, feel free to fork the repository and submit a pull request.
+
+### License
+`ruleopt` is released under the BSD 3-Clause License. See the LICENSE file for more details.
```

## Comparing `ruleopt-1.0.0.dist-info/RECORD` & `ruleopt-1.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-ruleopt/__init__.py,sha256=4IfJMKA1Ej57JEvfEktQXc0zMXgkqpmWSMDKOe7cfyE,257
-ruleopt/aux_classes/__init__.py,sha256=UGkt4gSK-CxEorj-BOxOVGu36HvPbUfYN5OeZSy2vp4,96
-ruleopt/aux_classes/aux_classes.c,sha256=Xv3QzZzP55stWfDCLkZjucKrSZRtotY5-DLSKbAEHp8,1415904
-ruleopt/aux_classes/aux_classes.cp39-win_amd64.pyd,sha256=cTrkk7EUETSOFNKGgIGg5AuiuN7I1YAHv092GCwmtco,217600
-ruleopt/estimator/__init__.py,sha256=8SIFO2ba0bwOdMUxQjdnwHlbsj_OhnZ0cGipMq8XMV0,280
-ruleopt/estimator/base.py,sha256=Bcfvmzchmc_C6CS1QyTkO5SdkzgxYypcA9tNv3UO-sA,25006
-ruleopt/estimator/lightgbm_.py,sha256=VrTF_dmUgfrBwsXzsmiLR23xYJQ8f6BUIq24iGo_kCs,12875
-ruleopt/estimator/xgboost_.py,sha256=YqvaP6f0iXrm_XIVHu8DHsa5BpCm0L5HBBFE4dS5QCw,11723
-ruleopt/estimator/sklearn_/__init__.py,sha256=vpPehVjHJuFZgWiq2vuI6WADan_84Vqnw2CcmAYXYQQ,126
-ruleopt/estimator/sklearn_/base_sklearn.py,sha256=WYNPR5yt_4GN2Y553g5VINJd5CQInhaE8trAgndnjp8,7694
-ruleopt/estimator/sklearn_/rug.py,sha256=AFYetmzye09kiNloENIQtE29PDDQLyCv7tcyGQAapvU,13679
-ruleopt/estimator/sklearn_/rux.py,sha256=dyzUnxx0VVNhN6vEzNb9PPKX5b38YY_Si3VbHDr9LrE,5864
-ruleopt/explainer/__init__.py,sha256=vYoSUVEeHYFWLjrwXyBSVdu7lhU9nK1KWGyEwidMgvQ,68
-ruleopt/explainer/explainer.py,sha256=udL2-licFi4xNu0YqGep-raKrZvnsGd6WkTPITKAXIQ,9875
-ruleopt/rule_cost/__init__.py,sha256=RyyBoe-0dHNHd_LMMYnEiCotnqQAJgRPhI9PHizvN7g,137
-ruleopt/rule_cost/rule_cost.py,sha256=8b0YCDS-kdcNc8MZGWwAhGeD1bpgb11C6AUXRpR_J50,6681
-ruleopt/solver/__init__.py,sha256=ZHispZQ10cu7KlzSra07SfyfPPy8GF_FXtc9_Hhp8zo,247
-ruleopt/solver/base.py,sha256=9ihPetgGh7YCGiQNL2Oz44i0xuAQT8H-WhDCqQZtdSY,3208
-ruleopt/solver/cplex_solver.py,sha256=aUckQzdavJjFpPnJh5610CcF1b3bQeWKcZWNERx-gwQ,4010
-ruleopt/solver/gurobi_solver.py,sha256=zIE2w9lzFuI6tEbQrIxpkDqeA4dAf-r0XWypNEMu2e0,3818
-ruleopt/solver/ortools_solver.py,sha256=Umh_bh8kjB9zAe7dcv0Dhrgx_BNp2FolutJw214fvW4,4955
-ruleopt/utils/__init__.py,sha256=7KHQaMT3RIeS_Drv7CUYu_bCZXCIsrC4toanI2rFXbY,173
-ruleopt/utils/utils.py,sha256=OnKCRblesWEIdx8dwz_AV5k7PeVhBRMQUTx4854OFQo,1250
-ruleopt-1.0.0.dist-info/LICENSE,sha256=XKfAKwrOVjOOE8e-U2iCArlr02PPATNyq6fv3y_lKu4,1557
-ruleopt-1.0.0.dist-info/METADATA,sha256=4JH5B71VQnWSWbXgnoDB3QGZTgrrZ6R7tirAzfCwXkA,4114
-ruleopt-1.0.0.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-ruleopt-1.0.0.dist-info/top_level.txt,sha256=5eXJDNaihq5rZdf1uSl9UMqGI050yX27S4inqYQMGSA,8
-ruleopt-1.0.0.dist-info/RECORD,,
+ruleopt/__init__.py,sha256=o8AuVrs9jVmDhaQwkVxxw5LJ90cNfXetouaQ2ELc9iw,247
+ruleopt/estimator/__init__.py,sha256=84Fg0ed4aOcTTKXOKx9HGjfrXAud-PuSurZieMmbNCw,271
+ruleopt/estimator/lightgbm_.py,sha256=2dkqn5T_Fxf8yhfOt5slueJja0g43A_q5DUumM4-w04,12543
+ruleopt/estimator/xgboost_.py,sha256=l4gZng-zzulJEZllhv3fuvr-dfJp6Rwsc8BXdvSshBw,11412
+ruleopt/estimator/base.py,sha256=AVuFh-GfZ0uEHjOmSe2-HOYSXnIATtH8rExK5H6BZWI,24321
+ruleopt/estimator/sklearn_/base_sklearn.py,sha256=9cgM3V1In48zpipWd1o-O-8PEdOZcIxON-zyhLy2T2Q,7479
+ruleopt/estimator/sklearn_/rux.py,sha256=TbsGLIcn5Eb2s6-CA6VXGcgHJb8w2sxCKmFUg7hIzeM,5710
+ruleopt/estimator/sklearn_/__init__.py,sha256=3hCiryClpNFIMGTkiTotqQoPjMk8A81o1dV3sjuA2Io,119
+ruleopt/estimator/sklearn_/rug.py,sha256=PNkzd-Za1tKhkPMc-vJQGWypAPyIrlpx3baFvaZQeTM,13325
+ruleopt/utils/__init__.py,sha256=EYtdosgeYDx5QOKw4rYJ2YrMlvK5wYF0HtdNyaQ9OwQ,168
+ruleopt/utils/utils.py,sha256=MBS75YGMXI14Gf24V8BqNvp3i-aE9ihKmzHwFySxXXQ,1210
+ruleopt/solver/ortools_solver.py,sha256=ntHxokipkyx146spIcOC2qZagTo2fAU8HF9lNsuD5sE,4780
+ruleopt/solver/__init__.py,sha256=NINaM9BqcymtXwqkMBp7MMJI8OF4dOtwKSVKakdZ-tg,240
+ruleopt/solver/gurobi_solver.py,sha256=SkJVv3lgS8TUQN8vEAK7MjaaWEGhX_G3HNhoTwV_kWs,3668
+ruleopt/solver/cplex_solver.py,sha256=R_zkboeR200puG9hK1bYTgVDC39CYKfQuy9LFJJzId8,3852
+ruleopt/solver/base.py,sha256=mQOHtO-NbAv8mSLDKnidYwN4S4eSPVXb4gyes0iCsEc,3471
+ruleopt/rule_cost/rule_cost.py,sha256=K_zdRpEZiN4DU45SbQISRK77BzdD8FMIdu5hKCkiwVc,6474
+ruleopt/rule_cost/__init__.py,sha256=umUIFMfNXmHTCdj819rVeO-daVXGGXQSpJAGAZhBVJo,134
+ruleopt/explainer/explainer.py,sha256=NHYHjKdpARUUgmhRy_cht-1FJLeMxz6qzOTGCITadbY,9612
+ruleopt/explainer/__init__.py,sha256=Qj8LYBiKERpljG1l85lDYaSTZCn9ZRCu3cAadAr2fF4,65
+ruleopt/aux_classes/__init__.py,sha256=N-EmTWYG51YSOZJ4Lw7fq2hJNyzBp9eirffgV7CBRUw,91
+ruleopt/aux_classes/aux_classes.cpython-39-darwin.so,sha256=hIW7FBT_jnEH_l6vFXmMH1yTJjwGwW4skngCcZ6ttu0,266240
+ruleopt/aux_classes/aux_classes.c,sha256=IBZXWw37vnIGir1die_OzoEIKMaOLIn9Mie9cko28e0,1420749
+ruleopt-1.0.1.dist-info/RECORD,,
+ruleopt-1.0.1.dist-info/LICENSE,sha256=TqIIvIA84fvxlzbfHTeCarlJ-0iNyL4ZYyvT6Tk6lqs,1530
+ruleopt-1.0.1.dist-info/WHEEL,sha256=t3aNIuHimB-eyeerOmc50nLML0b4_R6yjydcdcJkGHg,108
+ruleopt-1.0.1.dist-info/top_level.txt,sha256=5eXJDNaihq5rZdf1uSl9UMqGI050yX27S4inqYQMGSA,8
+ruleopt-1.0.1.dist-info/METADATA,sha256=vlIacwxyTcpAxLMhtYnC4roFU6oSP-jaFxrWsnhPZr0,4019
```

