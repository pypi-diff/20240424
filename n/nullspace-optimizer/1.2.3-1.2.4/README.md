# Comparing `tmp/nullspace_optimizer-1.2.3-py3-none-any.whl.zip` & `tmp/nullspace_optimizer-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,37 @@
-Zip file size: 21303 bytes, number of entries: 10
+Zip file size: 63785 bytes, number of entries: 35
 -rw-rw-r--  2.0 unx     1107 b- defN 23-Nov-07 08:38 nullspace_optimizer/__init__.py
 -rw-rw-r--  2.0 unx     6649 b- defN 24-Feb-23 09:54 nullspace_optimizer/inout.py
 -rw-rw-r--  2.0 unx     6240 b- defN 24-Apr-18 07:48 nullspace_optimizer/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-02 14:40 nullspace_optimizer/examples/__init__.py
 -rw-rw-r--  2.0 unx      241 b- defN 24-Feb-22 16:16 nullspace_optimizer/examples/run_all.py
--rw-r--r--  2.0 unx    35149 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3746 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/RECORD
-10 files, 54138 bytes uncompressed, 19751 bytes compressed:  63.5%
+-rw-rw-r--  2.0 unx      486 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/__init__.py
+-rw-rw-r--  2.0 unx     5509 b- defN 24-Apr-18 07:30 nullspace_optimizer/optimizable/bound_constraints_optimizable.py
+-rw-rw-r--  2.0 unx     5998 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/equalized_optimizable.py
+-rw-rw-r--  2.0 unx     3335 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/euclidean_optimizable.py
+-rw-rw-r--  2.0 unx     5699 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/filtered_optimizable.py
+-rw-rw-r--  2.0 unx     5313 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/minmax_optimizable.py
+-rw-rw-r--  2.0 unx    12167 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/optimizable.py
+-rw-rw-r--  2.0 unx     3387 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/symbolic_optimizable.py
+-rw-rw-r--  2.0 unx     2431 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizable/tuple_to_array_optimizable.py
+-rw-rw-r--  2.0 unx      401 b- defN 24-Feb-27 14:49 nullspace_optimizer/optimizable/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-10 08:44 nullspace_optimizer/optimizers/__init__.py
+-rw-rw-r--  2.0 unx     4529 b- defN 24-Feb-21 14:21 nullspace_optimizer/optimizers/utils.py
+-rw-rw-r--  2.0 unx       65 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/IPOPT/__init__.py
+-rw-rw-r--  2.0 unx     4612 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/IPOPT/ipopt.py
+-rw-rw-r--  2.0 unx     5780 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/MMA/MMA.py
+-rw-rw-r--  2.0 unx       27 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/MMA/__init__.py
+-rw-rw-r--  2.0 unx    24801 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/MMA/mma_lib.py
+-rw-rw-r--  2.0 unx       25 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/OC/__init__.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Nov-07 08:38 nullspace_optimizer/optimizers/OC/oc.py
+-rw-rw-r--  2.0 unx       37 b- defN 23-May-31 08:09 nullspace_optimizer/optimizers/nullspace/__init__.py
+-rw-rw-r--  2.0 unx     4989 b- defN 24-Feb-23 09:54 nullspace_optimizer/optimizers/nullspace/cvx_interface.py
+-rw-rw-r--  2.0 unx    20477 b- defN 24-Apr-24 05:43 nullspace_optimizer/optimizers/nullspace/nullspace.py
+-rw-rw-r--  2.0 unx     1937 b- defN 24-Feb-23 09:54 nullspace_optimizer/optimizers/nullspace/osqp_interface.py
+-rw-rw-r--  2.0 unx     2095 b- defN 24-Feb-23 09:54 nullspace_optimizer/optimizers/nullspace/qpalm_interface.py
+-rw-rw-r--  2.0 unx    11648 b- defN 24-Feb-23 09:54 nullspace_optimizer/optimizers/nullspace/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-24 05:50 nullspace_optimizer-1.2.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3746 b- defN 24-Apr-24 05:50 nullspace_optimizer-1.2.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 05:50 nullspace_optimizer-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-24 05:50 nullspace_optimizer-1.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3557 b- defN 24-Apr-24 05:50 nullspace_optimizer-1.2.4.dist-info/RECORD
+35 files, 186299 bytes uncompressed, 57839 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -9,23 +9,98 @@
 
 Filename: nullspace_optimizer/examples/__init__.py
 Comment: 
 
 Filename: nullspace_optimizer/examples/run_all.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.3.dist-info/LICENSE
+Filename: nullspace_optimizer/optimizable/__init__.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.3.dist-info/METADATA
+Filename: nullspace_optimizer/optimizable/bound_constraints_optimizable.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.3.dist-info/WHEEL
+Filename: nullspace_optimizer/optimizable/equalized_optimizable.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.3.dist-info/top_level.txt
+Filename: nullspace_optimizer/optimizable/euclidean_optimizable.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.3.dist-info/RECORD
+Filename: nullspace_optimizer/optimizable/filtered_optimizable.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizable/minmax_optimizable.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizable/optimizable.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizable/symbolic_optimizable.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizable/tuple_to_array_optimizable.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizable/utils.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/__init__.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/utils.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/IPOPT/__init__.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/IPOPT/ipopt.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/MMA/MMA.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/MMA/__init__.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/MMA/mma_lib.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/OC/__init__.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/OC/oc.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/__init__.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/cvx_interface.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/nullspace.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/osqp_interface.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/qpalm_interface.py
+Comment: 
+
+Filename: nullspace_optimizer/optimizers/nullspace/utils.py
+Comment: 
+
+Filename: nullspace_optimizer-1.2.4.dist-info/LICENSE
+Comment: 
+
+Filename: nullspace_optimizer-1.2.4.dist-info/METADATA
+Comment: 
+
+Filename: nullspace_optimizer-1.2.4.dist-info/WHEEL
+Comment: 
+
+Filename: nullspace_optimizer-1.2.4.dist-info/top_level.txt
+Comment: 
+
+Filename: nullspace_optimizer-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nullspace_optimizer-1.2.3.dist-info/LICENSE` & `nullspace_optimizer-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nullspace_optimizer-1.2.3.dist-info/METADATA` & `nullspace_optimizer-1.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullspace-optimizer
-Version: 1.2.3
+Version: 1.2.4
 Summary: Null space algorithm for nonlinear constrained optimization
 Home-page: https://null-space-optimizer.readthedocs.io/en/latest/
 Author: Florian Feppon
 Author-email: florian.feppon@kuleuven.be
 License: GNU GPL version 3
 Keywords: nonlinear constrained optimization
 Classifier: Programming Language :: Python :: 3
```

