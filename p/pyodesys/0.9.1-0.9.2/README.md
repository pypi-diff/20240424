# Comparing `tmp/pyodesys-0.9.1.tar.gz` & `tmp/pyodesys-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyodesys-0.9.1.tar", last modified: Mon Sep  4 22:08:06 2017, max compression
+gzip compressed data, was "dist/pyodesys-0.9.2.tar", last modified: Fri Sep  8 14:52:50 2017, max compression
```

## Comparing `pyodesys-0.9.1.tar` & `pyodesys-0.9.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3274 2017-09-04 21:48:42.000000 pyodesys-0.9.1/CHANGES.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2017-08-13 10:49:40.000000 pyodesys-0.9.1/LICENSE
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2017-08-13 10:49:40.000000 pyodesys-0.9.1/AUTHORS
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      101 2017-08-13 10:49:40.000000 pyodesys-0.9.1/MANIFEST.in
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7890 2017-08-13 10:49:40.000000 pyodesys-0.9.1/README.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9914 2017-09-04 22:08:06.000000 pyodesys-0.9.1/PKG-INFO
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      528 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10485 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/results.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3346 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/convergence.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2017-09-04 22:08:05.000000 pyodesys-0.9.1/pyodesys/_release.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5485 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/integrators.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8731 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/plotting.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/native/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      750 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11624 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/_base.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/native/sources/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    12270 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_numpy.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      738 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_parallel.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5266 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_decomposition.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4117 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_blas_lapack.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4057 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_iterative.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7497 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_matrix.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      820 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_buffer.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5791 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      797 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_iterative.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10547 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/_cvode_wrapper.pyx
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2056 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6897 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/_gsl_wrapper.pyx
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2101 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_iterative.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      531 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_util.hpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      644 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8761 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/standalone_template.cpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6183 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/native/sources/_odeint_wrapper.pyx
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      440 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_util.pxd
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8946 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_template.cpp
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1877 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/cvode.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/native/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6149 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/test_cvode.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    13698 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/_tests.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3134 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/test_gsl.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2679 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/_test_robertson_native.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2597 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/tests/test_odeint.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      959 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/gsl.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      713 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/odeint.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      978 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/native/util.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/analysis.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    50797 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/symbolic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    33542 2017-09-04 22:04:53.000000 pyodesys-0.9.1/pyodesys/core.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6777 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/_robertson.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    51277 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/test_symbolic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8841 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/test_robertson.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3969 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/_cetsa.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1494 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/test_results.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      643 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/test_plotting.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    17183 2017-09-04 21:48:42.000000 pyodesys-0.9.1/pyodesys/tests/test_core.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1171 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/bateman.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      918 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/tests/test_util.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8527 2017-08-13 10:49:40.000000 pyodesys-0.9.1/pyodesys/util.py
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4093 2017-09-04 21:48:42.000000 pyodesys-0.9.1/setup.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      385 2017-09-04 22:08:06.000000 pyodesys-0.9.1/setup.cfg
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      485 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/requires.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1994 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/SOURCES.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9914 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        9 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/top_level.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2017-09-04 22:08:06.000000 pyodesys-0.9.1/pyodesys.egg-info/dependency_links.txt
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       38 2017-02-07 10:55:32.000000 pyodesys-0.9.2/AUTHORS
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      101 2017-02-07 11:51:49.000000 pyodesys-0.9.2/MANIFEST.in
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3332 2017-09-08 14:48:25.000000 pyodesys-0.9.2/CHANGES.rst
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        1 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1994 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        9 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/top_level.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      485 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/requires.txt
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     9914 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys.egg-info/PKG-INFO
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      528 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/__init__.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/tests/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1494 2017-03-10 07:55:45.000000 pyodesys-0.9.2/pyodesys/tests/test_results.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        0 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/tests/__init__.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1171 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/tests/bateman.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      918 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/tests/test_util.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      643 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/tests/test_plotting.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3969 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/tests/_cetsa.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6777 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/tests/_robertson.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    51277 2017-03-26 13:05:41.000000 pyodesys-0.9.2/pyodesys/tests/test_symbolic.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     8841 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/tests/test_robertson.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    17183 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/tests/test_core.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     8731 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/plotting.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    10485 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/results.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     8527 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/util.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        0 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/analysis.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)       22 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/_release.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/native/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      750 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/native/__init__.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    11884 2017-09-08 14:47:57.000000 pyodesys-0.9.2/pyodesys/native/_base.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/native/tests/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)        0 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/native/tests/__init__.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3134 2017-03-03 13:22:34.000000 pyodesys-0.9.2/pyodesys/native/tests/test_gsl.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6149 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/native/tests/test_cvode.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    13698 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/native/tests/_tests.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     2597 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/tests/test_odeint.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     2679 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/tests/_test_robertson_native.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      978 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/util.py
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/native/sources/
+drwxrwxr-x   0 bjorn      (528) bjorn      (528)        0 2017-09-08 14:52:50.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      820 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_buffer.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     5266 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_decomposition.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    12270 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_numpy.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     5791 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     4057 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_iterative.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     4117 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_blas_lapack.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     7497 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_matrix.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      738 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_parallel.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6183 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/_odeint_wrapper.pyx
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    10547 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/_cvode_wrapper.pyx
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     8946 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_template.cpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     6897 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/_gsl_wrapper.pyx
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     2056 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     8761 2017-03-25 18:53:25.000000 pyodesys-0.9.2/pyodesys/native/sources/standalone_template.cpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     2101 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_iterative.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      531 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_util.hpp
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      797 2017-03-21 12:14:50.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_iterative.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      644 2017-03-21 12:14:50.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      440 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/native/sources/odesys_util.pxd
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1877 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/cvode.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      713 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/odeint.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      959 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/native/gsl.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     3346 2017-03-16 13:23:51.000000 pyodesys-0.9.2/pyodesys/convergence.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    50797 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/symbolic.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)    33542 2017-09-08 07:31:33.000000 pyodesys-0.9.2/pyodesys/core.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     5485 2017-02-07 10:55:32.000000 pyodesys-0.9.2/pyodesys/integrators.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)      364 2017-09-08 14:52:50.000000 pyodesys-0.9.2/setup.cfg
+-rwxrwxr-x   0 bjorn      (528) bjorn      (528)     4093 2017-09-08 07:31:33.000000 pyodesys-0.9.2/setup.py
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     9914 2017-09-08 14:52:50.000000 pyodesys-0.9.2/PKG-INFO
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     7890 2017-03-26 13:19:23.000000 pyodesys-0.9.2/README.rst
+-rw-rw-r--   0 bjorn      (528) bjorn      (528)     1303 2017-03-16 13:23:51.000000 pyodesys-0.9.2/LICENSE
```

### Comparing `pyodesys-0.9.1/CHANGES.rst` & `pyodesys-0.9.2/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v0.9.2
+======
+- Copy pyx to cache dir prior to cythonize
+
 v0.9.1
 ======
 - Address ``indep`` by name
 - Bumpy AnyODE
 
 v0.9.0
 ======
```

### Comparing `pyodesys-0.9.1/LICENSE` & `pyodesys-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/README.rst` & `pyodesys-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/PKG-INFO` & `pyodesys-0.9.2/pyodesys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyodesys
-Version: 0.9.1
+Version: 0.9.2
 Summary: Straightforward numerical integration of ODE systems from SymPy.
 Home-page: https://github.com/bjodah/pyodesys
 Author: Bjoern I. Dahlgren 
 Author-email: bjodah@gmail.com
 License: BSD
 Description: pyodesys
         ========
```

### Comparing `pyodesys-0.9.1/pyodesys/__init__.py` & `pyodesys-0.9.2/pyodesys/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/results.py` & `pyodesys-0.9.2/pyodesys/results.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/convergence.py` & `pyodesys-0.9.2/pyodesys/convergence.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/integrators.py` & `pyodesys-0.9.2/pyodesys/integrators.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/plotting.py` & `pyodesys-0.9.2/pyodesys/plotting.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/__init__.py` & `pyodesys-0.9.2/pyodesys/native/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/_base.py` & `pyodesys-0.9.2/pyodesys/native/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,21 @@
         self.namespace_extend = kwargs.pop('namespace_extend', {})
         self.tempdir_basename = '_pycodeexport_pyodesys_%s' % self.__class__.__name__
         self.obj_files = self.obj_files + ('%s%s' % (self.wrapper_name, _obj_suffix),)
         self.so_file = '%s%s' % (self.wrapper_name, '.so')
         _wrapper_src = pkg_resources.resource_filename(
             __name__, 'sources/%s.pyx' % self.wrapper_name)
         if cachedir is None:
-            raise ImportError("No module named appdirs (needed for caching)")
-        _wrapper_obj = os.path.join(cachedir, '%s%s' % (self.wrapper_name, _obj_suffix))
+            raise ImportError("No module named appdirs (needed for caching). Install 'appdirs' using e.g. pip/conda.")
         if not os.path.exists(cachedir):
             os.makedirs(cachedir)
+        _wrapper_src = os.path.join(cachedir, '%s%s' % (self.wrapper_name, '.pyx'))
+        shutil.copy(pkg_resources.resource_filename(__name__, 'sources/%s.pyx' % self.wrapper_name),
+                    _wrapper_src)
+        _wrapper_obj = os.path.join(cachedir, '%s%s' % (self.wrapper_name, _obj_suffix))
         prebuild = {_wrapper_src: _wrapper_obj}
 
         self.build_files = self.build_files + tuple(prebuild.values())
 
         self.odesys = odesys
         for _src, _dest in prebuild.items():
             if not os.path.exists(_dest):
```

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_numpy.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_parallel.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_parallel.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_decomposition.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_blas_lapack.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_blas_lapack.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_iterative.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_iterative.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_matrix.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode_buffer.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode_buffer.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/anyode/anyode.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/anyode/anyode.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_iterative.pxd` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_iterative.pxd`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/_cvode_wrapper.pyx` & `pyodesys-0.9.2/pyodesys/native/sources/_cvode_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/_gsl_wrapper.pyx` & `pyodesys-0.9.2/pyodesys/native/sources/_gsl_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_iterative.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_iterative.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_util.hpp` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_util.hpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode.pxd` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode.pxd`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/standalone_template.cpp` & `pyodesys-0.9.2/pyodesys/native/sources/standalone_template.cpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/_odeint_wrapper.pyx` & `pyodesys-0.9.2/pyodesys/native/sources/_odeint_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/sources/odesys_anyode_template.cpp` & `pyodesys-0.9.2/pyodesys/native/sources/odesys_anyode_template.cpp`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/cvode.py` & `pyodesys-0.9.2/pyodesys/native/cvode.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/tests/test_cvode.py` & `pyodesys-0.9.2/pyodesys/native/tests/test_cvode.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/tests/_tests.py` & `pyodesys-0.9.2/pyodesys/native/tests/_tests.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/tests/test_gsl.py` & `pyodesys-0.9.2/pyodesys/native/tests/test_gsl.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/tests/_test_robertson_native.py` & `pyodesys-0.9.2/pyodesys/native/tests/_test_robertson_native.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/tests/test_odeint.py` & `pyodesys-0.9.2/pyodesys/native/tests/test_odeint.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/gsl.py` & `pyodesys-0.9.2/pyodesys/native/gsl.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/odeint.py` & `pyodesys-0.9.2/pyodesys/native/odeint.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/native/util.py` & `pyodesys-0.9.2/pyodesys/native/util.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/symbolic.py` & `pyodesys-0.9.2/pyodesys/symbolic.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/core.py` & `pyodesys-0.9.2/pyodesys/core.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/_robertson.py` & `pyodesys-0.9.2/pyodesys/tests/_robertson.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_symbolic.py` & `pyodesys-0.9.2/pyodesys/tests/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_robertson.py` & `pyodesys-0.9.2/pyodesys/tests/test_robertson.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/_cetsa.py` & `pyodesys-0.9.2/pyodesys/tests/_cetsa.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_results.py` & `pyodesys-0.9.2/pyodesys/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_plotting.py` & `pyodesys-0.9.2/pyodesys/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_core.py` & `pyodesys-0.9.2/pyodesys/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/bateman.py` & `pyodesys-0.9.2/pyodesys/tests/bateman.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/tests/test_util.py` & `pyodesys-0.9.2/pyodesys/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys/util.py` & `pyodesys-0.9.2/pyodesys/util.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/setup.py` & `pyodesys-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys.egg-info/SOURCES.txt` & `pyodesys-0.9.2/pyodesys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodesys-0.9.1/pyodesys.egg-info/PKG-INFO` & `pyodesys-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyodesys
-Version: 0.9.1
+Version: 0.9.2
 Summary: Straightforward numerical integration of ODE systems from SymPy.
 Home-page: https://github.com/bjodah/pyodesys
 Author: Bjoern I. Dahlgren 
 Author-email: bjodah@gmail.com
 License: BSD
 Description: pyodesys
         ========
```

