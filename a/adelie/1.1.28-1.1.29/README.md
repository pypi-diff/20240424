# Comparing `tmp/adelie-1.1.28.tar.gz` & `tmp/adelie-1.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelie-1.1.28.tar", last modified: Fri Apr  5 16:11:29 2024, max compression
+gzip compressed data, was "adelie-1.1.29.tar", last modified: Wed Apr 24 03:22:08 2024, max compression
```

## Comparing `adelie-1.1.28.tar` & `adelie-1.1.29.tar`

### file list

```diff
@@ -1,722 +1,734 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 16:11:24.000000 adelie-1.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 16:11:24.000000 adelie-1.1.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-05 16:11:29.415938 adelie-1.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-05 16:11:24.000000 adelie-1.1.28/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 16:11:24.000000 adelie-1.1.28/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.307938 adelie-1.1.28/adelie/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/bcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39441 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15484 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    37164 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/adelie_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/bcd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/configs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/glm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/bcd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/configs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/glm/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_binomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_cox.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multibase.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_poisson.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/bisect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/newton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/search_pivot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/solver/
--rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23177 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/state/
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/algorithm.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/format.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/functional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/stopwatch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/tqdm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/types.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23931 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/optimization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    69765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/state.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/third_party/eigen3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/KLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.351938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.355938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.371938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.379938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.379938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.383938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.383938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.387938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
--rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.303938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.303938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
--rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)   113575 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    41758 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:11:28.000000 adelie-1.1.28/adelie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-05 16:11:24.000000 adelie-1.1.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:11:29.415938 adelie-1.1.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-05 16:11:24.000000 adelie-1.1.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.306229 adelie-1.1.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 03:22:03.000000 adelie-1.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 03:22:03.000000 adelie-1.1.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-24 03:22:08.306229 adelie-1.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-24 03:22:03.000000 adelie-1.1.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 03:22:03.000000 adelie-1.1.29/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.186230 adelie-1.1.29/adelie/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39442 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15476 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/adelie_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/bcd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/configs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/glm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.170230 adelie-1.1.29/adelie/src/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/bcd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/bcd/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/constrained/admm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/bcd/unconstrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/bcd/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/configs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/glm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_binomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_cox.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multibase.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_poisson.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.190230 adelie-1.1.29/adelie/src/include/adelie_core/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/io/io_snp_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17372 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/io/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.194230 adelie-1.1.29/adelie/src/include/adelie_core/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10809 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/matrix/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.194230 adelie-1.1.29/adelie/src/include/adelie_core/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/optimization/bisect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/optimization/newton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/optimization/nnls.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/optimization/search_pivot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.198230 adelie-1.1.29/adelie/src/include/adelie_core/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)    17965 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22175 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/solver/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.198230 adelie-1.1.29/adelie/src/include/adelie_core/state/
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.202230 adelie-1.1.29/adelie/src/include/adelie_core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/algorithm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/counting_iterator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.202230 adelie-1.1.29/adelie/src/include/adelie_core/util/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/format.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/functional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/stopwatch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/tqdm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/include/adelie_core/util/types.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24089 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/optimization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69524 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/state.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.170230 adelie-1.1.29/adelie/src/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.202230 adelie-1.1.29/adelie/src/third_party/eigen3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.206230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.178230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.206230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.206230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.222230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.174230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.222230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.226230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.226230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.226230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.226230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.174230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.230230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.234230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.234230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.234230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.238230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.242230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.246230 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.250229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.254229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.258229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.258229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.262229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.266229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.266229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.266229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.266229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.266229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.270229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.270229 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.178230 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.274229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.274229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.178230 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.286229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.182230 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.290229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.294229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.294229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.294229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.294229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.294229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.298229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.298229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.298229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.298229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.298229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.182230 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)   112000 2024-04-24 03:22:03.000000 adelie-1.1.29/adelie/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:22:08.302229 adelie-1.1.29/adelie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-24 03:22:08.000000 adelie-1.1.29/adelie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    42289 2024-04-24 03:22:08.000000 adelie-1.1.29/adelie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:22:08.000000 adelie-1.1.29/adelie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:22:07.000000 adelie-1.1.29/adelie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 03:22:08.000000 adelie-1.1.29/adelie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 03:22:08.000000 adelie-1.1.29/adelie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-24 03:22:03.000000 adelie-1.1.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:22:08.306229 adelie-1.1.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-24 03:22:03.000000 adelie-1.1.29/setup.py
```

### Comparing `adelie-1.1.28/LICENSE` & `adelie-1.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/PKG-INFO` & `adelie-1.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.28
+Version: 1.1.29
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.28/README.md` & `adelie-1.1.29/README.md`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/bcd.py` & `adelie-1.1.29/adelie/bcd.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,46 +37,49 @@
     return core.bcd.root_lower_bound(quad, linear, l1)
 
 
 def root_upper_bound(
     *,
     quad: np.ndarray,
     linear: np.ndarray,
-    zero_tol: float=1e-10,
+    l1: float,
+    zero_tol: float=1e-14,
 ):
     """Computes an upper bound on the root of BCD root function.
 
     The upper bound :math:`h^\\star` is guaranteed to be non-negative.
     However, it *may not satisfy* :math:`\\varphi(h^\\star) \\leq 0` where :math:`\\varphi`
     is given by ``adelie.bcd.root_function`` if ``zero_tol`` is too large.
-    Even when ``zero_tol`` is small enough, 
-    we assume that :math:`v_i=0` whenever :math:`\\Sigma_{ii} = 0`.
+    We assume that :math:`\\|v_S\\|_2 < \\lambda` 
+    where :math:`S = \\{i : \\Sigma_{ii} = 0\\}`.
     It is undefined behavior if the condition is not satisfied.
 
     Parameters
     ----------
     quad : (p,) np.ndarray
         See ``adelie.bcd.root_function``.
     linear : (p,) np.ndarray
         See ``adelie.bcd.root_function``.
+    l1 : float
+        See ``adelie.bcd.root_function``.
     zero_tol : float, optional
         A value is considered zero if its absolute value is less than or equal to ``zero_tol``.
-        Default is ``1e-10``.
+        Default is ``1e-14``.
     
     See Also
     --------
     adelie.bcd.root_lower_bound
     adelie.bcd.root_function
 
     Returns
     -------
     upper : float
         Upper bound on the root.
     """
-    return core.bcd.root_upper_bound(quad, linear, zero_tol)
+    return core.bcd.root_upper_bound(quad, linear, l1, zero_tol)
 
 
 def root_function(
     h: float, 
     *,
     quad: np.ndarray,
     linear: np.ndarray,
@@ -161,22 +164,22 @@
         The BCD objective.
     """
     beta_norm = np.linalg.norm(beta)
     return 0.5 * quad @ beta ** 2 - linear @ beta + l1 * beta_norm + 0.5 * l2 * beta_norm ** 2
 
 
 _solver_dict = {
-    "brent":            core.bcd.brent_solver,
-    "newton":           core.bcd.newton_solver,
-    "newton_brent":     core.bcd.newton_brent_solver,
-    "newton_abs":       core.bcd.newton_abs_solver,
-    "newton_abs_debug": core.bcd.newton_abs_debug_solver,
-    "ista":             core.bcd.ista_solver,
-    "fista":            core.bcd.fista_solver,
-    "fista_adares":     core.bcd.fista_adares_solver,
+    "brent":            core.bcd.unconstrained_brent_solver,
+    "newton":           core.bcd.unconstrained_newton_solver,
+    "newton_brent":     core.bcd.unconstrained_newton_brent_solver,
+    "newton_abs":       core.bcd.unconstrained_newton_abs_solver,
+    "newton_abs_debug": core.bcd.unconstrained_newton_abs_debug_solver,
+    "ista":             core.bcd.unconstrained_ista_solver,
+    "fista":            core.bcd.unconstrained_fista_solver,
+    "fista_adares":     core.bcd.unconstrained_fista_adares_solver,
 }
 
 
 def solve(
     *,
     quad: np.ndarray,
     linear: np.ndarray,
```

### Comparing `adelie-1.1.28/adelie/cv.py` & `adelie-1.1.29/adelie/cv.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/data.py` & `adelie-1.1.29/adelie/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,27 +222,30 @@
 def snp_unphased(
     n: int, 
     p: int, 
     *,
     K: int =1,
     glm: str ="gaussian",
     sparsity: float =0.95,
+    missing_ratio: float =0.1,
     one_ratio: float =0.25,
     two_ratio: float =0.05,
     zero_penalty: float =0,
     snr: float =1,
     seed: int =0,
 ):
     """Creates a SNP unphased dataset.
 
     - This dataset is only used for lasso, so ``groups`` is simply each individual feature
       and ``group_sizes`` is a vector of ones.
     - The calldata matrix ``X`` has sparsity ratio ``1 - one_ratio - two_ratio``
       where ``one_ratio`` of the entries are randomly set to ``1``
       and ``two_ratio`` are randomly set to ``2``.
+      The user only sees a masked version of ``X`` where
+      ``missing_ratio`` of the entries are set to ``-9``.
     - The true coefficients :math:`\\beta` are such that ``sparsity`` proportion
       of the entries are set to :math:`0`.
     - The response ``y`` is generated from the GLM specified by ``glm``.
     - The penalty factors are by default set to ``np.sqrt(group_sizes)``,
       however if ``zero_penalty > 0``, a random set of penalties will be set to zero,
       in which case, ``penalty`` is rescaled such that the :math:`\\ell_2` norm squared is ``p``.
 
@@ -266,14 +269,17 @@
             - ``"multinomial"``
             - ``"poisson"``
 
         Default is ``"gaussian"``.
     sparsity : float, optional
         Proportion of :math:`\\beta` entries to be zeroed out.
         Default is ``0.95``.
+    missing_ratio : float, optional
+        Proportion of the entries of ``X`` that is set to ``-9`` (missing).
+        Default is ``0.1``.
     one_ratio : float, optional
         Proportion of the entries of ``X`` that is set to ``1``.
         Default is ``0.25``.
     two_ratio : float, optional
         Proportion of the entries of ``X`` that is set to ``2``.
         Default is ``0.05``.
     zero_penalty : float, optional
@@ -296,14 +302,15 @@
             - ``"groups"``: mapping of group index to the starting column index of ``X``.
             - ``"group_sizes"``: mapping of group index to the group size.
             - ``"penalty"``: penalty factor for each group index.
     """
     assert n >= 1
     assert p >= 1
     assert sparsity >= 0 and sparsity <= 1
+    assert missing_ratio >= 0 and missing_ratio <= 1
     assert one_ratio >= 0 and one_ratio <= 1
     assert two_ratio >= 0 and two_ratio <= 1
     assert zero_penalty >= 0 and zero_penalty <= 1
     assert snr > 0
     assert seed >= 0
 
     np.random.seed(seed)
@@ -336,14 +343,17 @@
     glm = _sample_y(
         glm=glm,
         eta=eta,
         beta=beta_sub,
         snr=snr,
     )
 
+    n_missing = int(missing_ratio * n * p)
+    X.ravel()[np.random.choice(n * p, n_missing, replace=False)] = -9
+
     return {
         "X": np.asfortranarray(X), 
         "glm": glm,
         "groups": groups,
         "group_sizes": group_sizes,
         "penalty": penalty,
     }
```

### Comparing `adelie-1.1.28/adelie/diagnostic.py` & `adelie-1.1.29/adelie/diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         y_shape = (n,)
 
     if offsets is None:
         offsets = np.zeros(y_shape)
 
     L = betas.shape[0]
 
-    etas = np.empty((L,) + y_shape, order="C")
+    etas = np.zeros((L,) + y_shape, order="C")
     if isinstance(betas, np.ndarray):
         for i in range(etas.shape[0]):
             X.btmul(0, X.cols(), betas[i], etas[i].ravel())
     elif isinstance(betas, csr_matrix):
         X.sp_btmul(betas, etas.reshape((L, -1))) 
     else:
         raise RuntimeError("beta is not one of np.ndarray or scipy.sparse.csr_matrix.")
@@ -669,15 +669,15 @@
     fig, ax
     """
     tls = -np.log(lmdas)
 
     fig, ax = plt.subplots(figsize=(9, 6), layout="constrained")
     ax.plot(tls, devs, linestyle='-', color='r', marker='.')
     ax.set_title(r"Deviance Profile")
-    ax.set_ylabel(r"Deviance Explained (%)")
+    ax.set_ylabel(r"Deviance Explained (\%)")
     ax.set_xlabel(r"$-\log(\lambda)$")
 
     return fig, ax
 
 
 def plot_set_sizes(
     groups: np.ndarray,
```

### Comparing `adelie-1.1.28/adelie/glm.py` & `adelie-1.1.29/adelie/glm.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/logger.py` & `adelie-1.1.29/adelie/logger.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/matrix.py` & `adelie-1.1.29/adelie/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,28 +405,28 @@
 def snp_phased_ancestry(
     filename: str,
     *,
     read_mode: str ="auto",
     n_threads: int =1,
     dtype: Union[np.float32, np.float64] =np.float64,
 ):
-    """Creates a SNP phased ancestry matrix.
+    """Creates a SNP phased, ancestry matrix.
 
-    The SNP phased ancestry matrix is represented by a file with name ``filename``.
+    The SNP phased, ancestry matrix is represented by a file with name ``filename``.
     It must be in the same format as described in ``adelie.io.snp_phased_ancestry``.
     Typically, the user first writes into the file ``filename`` 
     using ``adelie.io.snp_phased_ancestry`` and then loads the matrix using this function.
 
     .. note::
         This matrix only works for naive method!
     
     Parameters
     ----------
     filename : str
-        File name that contains phased calldata with ancestry information in ``.snpdat`` format.
+        File name that contains the SNP phased, ancestry matrix in ``.snpdat`` format.
     read_mode : str, optional
         See the corresponding parameter in ``adelie.io.snp_phased_ancestry``.
         Default is ``"auto"``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
     dtype : Union[np.float32, np.float64], optional
```

### Comparing `adelie-1.1.28/adelie/solver.py` & `adelie-1.1.29/adelie/solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -315,14 +315,17 @@
 
     if warm_start is None:
         lmda = np.inf
         lmda_max = None
         screen_set = np.arange(G)[(penalty <= 0) | (alpha <= 0)]
         screen_beta = np.zeros(np.sum(group_sizes[screen_set]), dtype=dtype)
         screen_is_active = np.ones(screen_set.shape[0], dtype=bool)
+        active_set_size = screen_set.shape[0]
+        active_set = np.empty(G, dtype=int)
+        active_set[:active_set_size] = np.arange(active_set_size)
         rsq = 0
 
         subset = np.array([
             np.arange(groups[ss], groups[ss] + group_sizes[ss]) 
             for ss in screen_set
         ])
         order = np.argsort(subset)
@@ -335,27 +338,31 @@
 
     else:
         lmda = warm_start.lmda
         lmda_max = warm_start.lmda_max
         screen_set = warm_start.screen_set
         screen_beta = warm_start.screen_beta
         screen_is_active = warm_start.screen_is_active
+        active_set_size = warm_start.active_set_size
+        active_set = warm_start.active_set
         rsq = warm_start.rsq
         grad = warm_start.grad
 
     state = state_gaussian_cov(
         A=A,
         v=v,
         groups=groups,
         group_sizes=group_sizes,
         alpha=alpha,
         penalty=penalty,
         screen_set=screen_set,
         screen_beta=screen_beta,
         screen_is_active=screen_is_active,
+        active_set_size=active_set_size,
+        active_set=active_set,
         rsq=rsq,
         lmda=lmda,
         grad=grad,
         lmda_path=lmda_path,
         lmda_max=lmda_max,
         max_iters=max_iters,
         tol=tol,
@@ -741,29 +748,36 @@
 
         if warm_start is None:
             lmda = np.inf
             lmda_max = None
             screen_set = np.arange(groups.shape[0])[(penalty <= 0) | (alpha <= 0)]
             screen_beta = np.zeros(np.sum(group_sizes[screen_set]), dtype=dtype)
             screen_is_active = np.ones(screen_set.shape[0], dtype=bool)
+            active_set_size = screen_set.shape[0]
+            active_set = np.empty(groups.shape[0], dtype=int)
+            active_set[:active_set_size] = np.arange(active_set_size)
         else:
             lmda = warm_start.lmda
             lmda_max = warm_start.lmda_max
             screen_set = warm_start.screen_set
             screen_beta = warm_start.screen_beta
             screen_is_active = warm_start.screen_is_active
+            active_set_size = warm_start.active_set_size
+            active_set = warm_start.active_set
 
         solver_args["groups"] = groups
         solver_args["group_sizes"] = group_sizes
         solver_args["penalty"] = penalty
         solver_args["lmda"] = lmda
         solver_args["lmda_max"] = lmda_max
         solver_args["screen_set"] = screen_set
         solver_args["screen_beta"] = screen_beta
         solver_args["screen_is_active"] = screen_is_active
+        solver_args["active_set_size"] = active_set_size
+        solver_args["active_set"] = active_set
 
         # represent the augmented X matrix as used in single-response reformatted problem.
         X_aug = matrix.kronecker_eye(X_raw, K, n_threads=n_threads)
         if intercept:
             X_aug = matrix.concatenate(
                 [
                     matrix.kronecker_eye(
@@ -870,29 +884,37 @@
 
         if warm_start is None:
             lmda = np.inf
             lmda_max = None
             screen_set = np.arange(G)[(penalty <= 0) | (alpha <= 0)]
             screen_beta = np.zeros(np.sum(group_sizes[screen_set]), dtype=dtype)
             screen_is_active = np.ones(screen_set.shape[0], dtype=bool)
+            active_set_size = screen_set.shape[0]
+            active_set = np.empty(groups.shape[0], dtype=int)
+            active_set[:active_set_size] = np.arange(active_set_size)
+
         else:
             lmda = warm_start.lmda
             lmda_max = warm_start.lmda_max
             screen_set = warm_start.screen_set
             screen_beta = warm_start.screen_beta
             screen_is_active = warm_start.screen_is_active
+            active_set_size = warm_start.active_set_size
+            active_set = warm_start.active_set
 
         solver_args["groups"] = groups
         solver_args["group_sizes"] = group_sizes
         solver_args["penalty"] = penalty
         solver_args["lmda"] = lmda
         solver_args["lmda_max"] = lmda_max
         solver_args["screen_set"] = screen_set
         solver_args["screen_beta"] = screen_beta
         solver_args["screen_is_active"] = screen_is_active
+        solver_args["active_set_size"] = active_set_size
+        solver_args["active_set"] = active_set
 
         # special gaussian case
         if is_gaussian_opt:
             y = glm.y
             weights = glm.weights
             if warm_start is None:
                 ones = np.ones(n, dtype=dtype)
```

### Comparing `adelie-1.1.28/adelie/src/adelie_core.cpp` & `adelie-1.1.29/adelie/src/adelie_core.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/configs.cpp` & `adelie-1.1.29/adelie/src/configs.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/decl.hpp` & `adelie-1.1.29/adelie/src/decl.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/glm.cpp` & `adelie-1.1.29/adelie/src/glm.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/bcd.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,262 +1,16 @@
 #pragma once
-#include <Eigen/Core>
+#include <adelie_core/bcd/utils.hpp>
 #include <adelie_core/optimization/bisect.hpp>
 #include <adelie_core/optimization/newton.hpp>
 #include <adelie_core/util/types.hpp>
 
 namespace adelie_core {
 namespace bcd {
-
-/*
- * ISTA solver.
- */
-template <class LType, class VType, class ValueType, class XType>
-inline
-void ista_solver(
-    const LType& L,
-    const VType& v,
-    ValueType l1,
-    ValueType l2,
-    ValueType tol,
-    size_t max_iters,
-    XType& x_sol,
-    size_t& iters
-)
-{
-    using value_t = ValueType;
-    const auto lip = L.maxCoeff();
-    const auto nu = 1. / lip;
-    const auto p = L.size();
-    util::rowvec_type<value_t> x_diff(p);
-    util::rowvec_type<value_t> x_old(p);
-    util::rowvec_type<value_t> x(p); x.setZero();
-    util::rowvec_type<value_t> v_tilde(p);
-
-    iters = 0;
-    for (; iters < max_iters; ++iters) {
-        x_old.swap(x);
-        v_tilde = x_old - nu * (L * x_old - v);
-        const auto v_tilde_l2 = v_tilde.matrix().norm();
-        if (v_tilde_l2 <= l1 * nu) {
-            x.setZero();
-        } else {
-            x = ((lip /(lip + l2)) * (1 - (l1 * nu) / v_tilde_l2)) * v_tilde;
-        }
-        x_diff = x - x_old;
-        if ((x_diff.abs() <= (tol * x.abs())).all()) break;
-    }
-    
-    x_sol = x;
-}
-    
-/*
- * FISTA solver.
- */
-template <class LType, class VType, class ValueType, class XType>
-inline
-void fista_solver(
-    const LType& L,
-    const VType& v,
-    ValueType l1,
-    ValueType l2,
-    ValueType tol,
-    size_t max_iters,
-    XType& x_sol,
-    size_t& iters
-)
-{
-    using value_t = ValueType;
-    const auto lip = L.maxCoeff();
-    const auto nu = 1. / lip;
-    const auto p = L.size();
-    util::rowvec_type<value_t> x_diff(p);
-    util::rowvec_type<value_t> x_old(p);
-    util::rowvec_type<value_t> x(p); x.setZero();
-    util::rowvec_type<value_t> y(p); y = x;
-    util::rowvec_type<value_t> v_tilde(p);
-    value_t t = 1;
-
-    iters = 0;
-    for (; iters < max_iters; ++iters) {
-        x_old.swap(x);
-        v_tilde = y - nu * (L * y - v);
-        const auto v_tilde_l2 = v_tilde.matrix().norm();
-        if (v_tilde_l2 <= l1 * nu) {
-            x.setZero();
-        } else {
-            x = (lip /(lip + l2)) * (1 - (l1 * nu) / v_tilde_l2) * v_tilde;
-        }
-        const auto t_old = t;
-        t = (1 + std::sqrt(1 + 4 * t * t)) * 0.5;
-        x_diff = x - x_old;
-        y = x + (t_old - 1) / t * x_diff;
-        
-        if ((x_diff.abs() <= (tol * x.abs())).all()) break;
-    }
-    
-    x_sol = x;
-}
-
-/*
- * FISTA with adaptive restart.
- */
-template <class LType, class VType, class ValueType, class XType>
-inline
-void fista_adares_solver(
-    const LType& L,
-    const VType& v,
-    ValueType l1,
-    ValueType l2,
-    ValueType tol,
-    size_t max_iters,
-    XType& x_sol,
-    size_t& iters
-)
-{
-    using value_t = ValueType;
-    const auto lip = L.maxCoeff();
-    const auto nu = 1. / lip;
-    const auto p = L.size();
-    util::rowvec_type<value_t> x_diff(p);
-    util::rowvec_type<value_t> x_old(p);
-    util::rowvec_type<value_t> x(p); x.setZero();
-    util::rowvec_type<value_t> y(p); y = x;
-    util::rowvec_type<value_t> v_tilde(p);
-    util::rowvec_type<value_t> df(p);
-    value_t t = 1;
-
-    iters = 0;
-    for (; iters < max_iters; ++iters) {
-        x_old.swap(x);
-        df = (L * y - v);
-        v_tilde = y - nu * df;
-        const auto v_tilde_l2 = v_tilde.matrix().norm();
-        if (v_tilde_l2 <= l1 * nu) {
-            x.setZero();
-        } else {
-            x = (lip /(lip + l2)) * (1 - (l1 * nu) / v_tilde_l2) * v_tilde;
-        }
-        x_diff = x - x_old;
-        
-        // accelerated
-        if (v_tilde.matrix().dot(x_diff.matrix()) > 0) {
-            y = x;
-            t = 1;
-        } else {
-            const auto t_old = t;
-            t = (1 + std::sqrt(1 + 4 * t * t)) * 0.5;
-            y = x + (t_old - 1) / t * x_diff;
-        }
-
-        if ((x_diff.abs() <= (tol * x.abs())).all()) break;
-    }
-    
-    x_sol = x;
-}
-
-/**
- * @brief Compute lower bound h_min >= 0 such that 
- * root_function(h_min) >= 0.
- * 
- * @tparam DiagType     vector type.
- * @tparam VType        vector type.
- * @tparam ValueType    float type.
- * @param vbuffer1      vector containing L + l2.
- * @param v             any vector of same length as vbuffer1.
- * @param l1            l1 regularization.
- * @return h_min 
- */
-template <class DiagType, class VType, class ValueType>
-inline
-auto root_lower_bound(
-    const DiagType& vbuffer1,
-    const VType& v,
-    ValueType l1
-)
-{
-    using value_t = ValueType;
-    const value_t b = l1 * vbuffer1.sum();
-    const value_t a = vbuffer1.matrix().squaredNorm();
-    const value_t v_l1 = v.matrix().template lpNorm<1>();
-    const value_t c = l1 * l1 * vbuffer1.size() - v_l1 * v_l1;
-    const value_t discr = b*b - a*c;
-    value_t h_min = (discr > -1e-12) ? 
-        (-b + std::sqrt(std::max<value_t>(discr, 0.0))) / a : 0.0;
-    
-    // Otherwise, if h <= 0, we know at least 0 is a reasonable solution.
-    // The only case h <= 0 is when 0 is already close to the solution.
-    h_min = std::max<value_t>(h_min, 0.0);
-    return h_min;
-}
-
-/**
- * @brief 
- * Compute upper bound h_max >= 0 such that root_function(h_max) <= 0.
- * NOTE: if zero_tol > 0,
- * the result may NOT be a true upper bound in the sense that group_elnet_objective(result) <= 0.
- * 
- * @tparam DiagType     vector type.
- * @tparam VType        vector type.
- * @tparam ValueType    float type.
- * @param vbuffer1      vector containing L + l2.
- * @param v             any vector of same length as vbuffer1.
- * @param zero_tol      if a float is <= zero_tol, it is considered to be 0.
- * @return (h_max, vbuffer1_min_nnz)
- *  h_max: the upper bound
- *  vbuffer1_min_nnz:   smallest value in vbuffer1 among non-zero values based on zero_tol.
- */
-template <class DiagType, class VType, class ValueType>
-inline
-auto root_upper_bound(
-    const DiagType& vbuffer1,
-    const VType& v,
-    ValueType zero_tol=1e-10
-)
-{
-    using value_t = ValueType;
-
-    const value_t vbuffer1_min = vbuffer1.minCoeff();
-
-    value_t vbuffer1_min_nnz = std::numeric_limits<value_t>::infinity();
-    value_t h_max = 0;
-
-    // If L+l2 have entries <= threshold,
-    // find h_max with more numerically-stable routine.
-    // If threshold > 0, there is NO guarantee that f(h_max) <= 0, 
-    // but we will use this to bisect and find an h where f(h) >= 0,
-    // so we don't necessarily need h_max to be f(h_max) <= 0.
-    if (vbuffer1_min <= zero_tol) {
-        for (int i = 0; i < vbuffer1.size(); ++i) {
-            const bool is_nonzero = vbuffer1[i] > zero_tol;
-            const auto vi2 = v[i] * v[i];
-            h_max += is_nonzero ? vi2 / (vbuffer1[i] * vbuffer1[i]) : 0;
-            vbuffer1_min_nnz = is_nonzero ? std::min(vbuffer1_min_nnz, vbuffer1[i]) : vbuffer1_min_nnz;
-        }
-        h_max = std::sqrt(h_max);
-    } else {
-        vbuffer1_min_nnz = vbuffer1_min;
-        h_max = (v / vbuffer1).matrix().norm();
-    }
-
-    return std::make_pair(h_max, vbuffer1_min_nnz);
-}
-
-template <class ValueType, class DiagType, class VType>
-inline
-auto root_function(
-    ValueType h,
-    const DiagType& D,
-    const VType& v,
-    ValueType l1
-)
-{
-    return (v.array() / (D.array() * h + l1)).matrix().squaredNorm() - 1;
-}
-
+namespace unconstrained {
 
 /**
  * @brief Base Newton solver for the block update norm objective.
  * IMPORTANT: This solver assumes that v is of the form sqrt(L) * u.
  * 
  * @tparam LType        vector type.
  * @tparam VType        vector type.
@@ -317,19 +71,19 @@
     // First solve for h := ||x||_2
     auto vbuffer1 = buffer1.head(L.size());
     auto vbuffer2 = buffer2.head(L.size());
 
     vbuffer1 = (L + l2);
 
     const auto step_f = [&](auto h) {
-        vbuffer2 = vbuffer1 * h + l1;
-        x = (v / vbuffer2).square();
+        vbuffer2 = 1 / (vbuffer1 * h + l1);
+        x = (v * vbuffer2).square();
         auto fh = x.sum() - 1.0;
         auto dfh = -2.0 * (
-            x * (vbuffer1 / vbuffer2)
+            x * vbuffer1 * vbuffer2
         ).sum();
         return std::make_pair(fh, dfh);
     };
 
     const auto project_f = [&](auto h) {
         return std::max<value_t>(h, 0.0);
     };
@@ -340,15 +94,15 @@
         project_f,
         tol, 
         max_iters
     );
 
     const auto h = std::get<0>(root_find_state);
 
-    x = h * v / vbuffer2;
+    x = h * v * vbuffer2;
     iters = std::get<3>(root_find_state);
 }
 
 /*
  * Vanilla Newton solver.
  */
 template <class LType, class VType, class ValueType, 
@@ -395,15 +149,15 @@
 )
 {
     using value_t = ValueType;
     auto vbuffer1 = buffer1.head(L.size());
 
     const auto initial_f = [&]() {
         const value_t h_min = root_lower_bound(vbuffer1, v, l1);
-        const auto h_max_out = root_upper_bound(vbuffer1, v, 0.0); // IMPORTANT: NEEDS GUARANTEE
+        const auto h_max_out = root_upper_bound(vbuffer1, v, l1, 0.0); // IMPORTANT: NEEDS GUARANTEE
         const value_t h_max = std::get<0>(h_max_out);
 
         value_t h = 0;
         size_t iters_brent;
         optimization::brent(
             [&](auto x) { return root_function(x, vbuffer1, v, l1); },
             tol,
@@ -644,38 +398,10 @@
     // numerical stability
     h = std::max<value_t>(h, zero);
 
     // final solution
     x = h * v / vbuffer2;
 }
 
-template <class LType, class VType, class ValueType, class XType>
-void brent_solver(
-    const LType& L,
-    const VType& v,
-    ValueType l1,
-    ValueType l2,
-    ValueType tol,
-    size_t max_iters,
-    XType& x,
-    size_t& iters
-)
-{
-    using value_t = ValueType;
-    value_t h = 0;
-    const util::rowvec_type<value_t> buffer1 = L + l2;
-    const auto a = root_lower_bound(buffer1, v, l1);
-    const auto b = std::get<0>(root_upper_bound(buffer1, v, 0.0));
-    iters = 0;
-    const auto phi = [&](auto h) {
-        return root_function(h, buffer1, v, l1);
-    };
-    optimization::brent(
-        phi, tol, tol, max_iters, a, a, b, 
-        [](auto, auto, auto, auto) { return std::make_pair(false, 0.0); },
-        h, iters
-    );
-    x = h * v / (buffer1 * h + l1);
-}
-
+} // namespace unconstrained
 } // namespace bcd
 } // namespace adelie_core
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_binomial.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_binomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_cox.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_cox.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_gaussian.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_gaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multibase.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multibase.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multinomial.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_multinomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_poisson.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/glm/glm_poisson.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/io/io_snp_base.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,32 @@
 #else
 #define MAP_FLAGS 0
 #endif
 
 namespace adelie_core {
 namespace io {
 
+template <class MmapPtrType=std::unique_ptr<char, std::function<void(char*)>>>
 class IOSNPBase
 {
 public:
     using string_t = std::string;
     using file_unique_ptr_t = std::unique_ptr<
         std::FILE, 
         std::function<void(std::FILE*)>
     >;
-    using mmap_unique_ptr_t = std::unique_ptr<
-        char,
-        std::function<void(char*)>
-    >;
+    using mmap_ptr_t = MmapPtrType;
     using bool_t = bool;
     using buffer_t = util::rowvec_type<char>;
 
 protected:
     const string_t _filename;
     const util::read_mode_type _read_mode;
     buffer_t _buffer_w;             // only used when _read_mode == _file
-    mmap_unique_ptr_t _mmap_ptr;    // only used when _read_mode == _mmap
+    mmap_ptr_t _mmap_ptr;           // only used when _read_mode == _mmap 
     Eigen::Map<buffer_t> _buffer;
     bool_t _is_read;
 
     static void throw_no_read() 
     {
         throw util::adelie_core_error(
             "File is not read yet. Call read() first."
@@ -98,15 +96,15 @@
 public:
     IOSNPBase(
         const string_t& filename,
         const string_t& read_mode
     ):
         _filename(filename),
         _read_mode(convert_read_mode(read_mode)),
-        _mmap_ptr(nullptr, [](char*) {}),
+        _mmap_ptr(nullptr),
         _buffer(nullptr, 0),
         _is_read(false)
     {}
 
     bool_t endian() const { 
         if (!_is_read) throw_no_read();
         return reinterpret_cast<const bool_t&>(_buffer[0]); 
@@ -123,29 +121,34 @@
         const size_t total_bytes = std::ftell(fp);
         std::fseek(fp, 0, SEEK_SET);
 
         // use the optimized mmap routine
         if (_read_mode == util::read_mode_type::_mmap) {
 #if defined(__linux__) || defined(__APPLE__)
             int fd = open(_filename.c_str(), O_RDONLY);
+            if (fd == -1) {
+                perror("open");
+                throw util::adelie_core_error("open failed.");
+            }
             char* addr = static_cast<char*>(
                 mmap(
                     nullptr, 
                     total_bytes, 
                     PROT_READ,
                     MAP_FLAGS,
                     fd,
                     0
                 )
             );
             close(fd);
-            _mmap_ptr = mmap_unique_ptr_t(
-                addr, 
-                [=](char* ptr) { if (ptr) munmap(ptr, total_bytes); }
-            );
+            if (addr == MAP_FAILED) {
+                perror("mmap");
+                throw util::adelie_core_error("mmap failed.");
+            }
+            _mmap_ptr = mmap_ptr_t(addr, [=](char* ptr) { munmap(ptr, total_bytes); } );
             new (&_buffer) Eigen::Map<buffer_t>(addr, total_bytes);
 #else
             throw util::adelie_core_error("Only Linux and MacOS support the mmap feature.");
 #endif
         // otherwise use the more general routine using file IO
         } else if (_read_mode == util::read_mode_type::_file) {
             _buffer_w.resize(total_bytes);
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,214 +1,221 @@
 #pragma once
-#include <adelie_core/io/io_snp_base.hpp>
+#include <adelie_core/matrix/matrix_naive_base.hpp>
+#include <adelie_core/matrix/utils.hpp>
 
 namespace adelie_core {
-namespace io {
+namespace matrix {
 
-class IOSNPPhasedAncestry : public IOSNPBase
+template <class SparseType>
+class MatrixNaiveSparse: public MatrixNaiveBase<typename SparseType::Scalar>
 {
 public:
-    using base_t = IOSNPBase;
-    using outer_t = uint64_t;
-    using inner_t = uint32_t;
-    using value_t = int8_t;
-    using vec_outer_t = util::rowvec_type<outer_t>;
-    using vec_inner_t = util::rowvec_type<inner_t>;
-    using vec_value_t = util::rowvec_type<value_t>;
-    using rowarr_value_t = util::rowarr_type<value_t>;
-    using colarr_value_t = util::colarr_type<value_t>;
-    using typename base_t::buffer_t;
-
-protected:
-    static constexpr size_t _multiplier = (
-        sizeof(inner_t) + 
-        sizeof(value_t)
-    );
-    
-    using base_t::_buffer;
-    using base_t::_filename;
-    using base_t::_is_read;
-
-public:
-    using base_t::base_t;
-    using base_t::read;
-
-    inner_t rows() const {
-        if (!_is_read) throw_no_read();
-        constexpr size_t idx = sizeof(bool_t);
-        return reinterpret_cast<const inner_t&>(_buffer[idx]);
-    }
-
-    inner_t snps() const {
-        if (!_is_read) throw_no_read();
-        constexpr size_t idx = sizeof(bool_t) + sizeof(inner_t);
-        return reinterpret_cast<const inner_t&>(_buffer[idx]);
-    }
-
-    value_t ancestries() const 
-    {
-        if (!_is_read) throw_no_read();
-        constexpr size_t idx = sizeof(bool_t) + 2 * sizeof(inner_t);
-        return reinterpret_cast<const value_t&>(_buffer[idx]);
-    }
+    using base_t = MatrixNaiveBase<typename SparseType::Scalar>;
+    using sparse_t = SparseType;
+    using typename base_t::value_t;
+    using typename base_t::vec_value_t;
+    using typename base_t::vec_index_t;
+    using typename base_t::colmat_value_t;
+    using typename base_t::rowmat_value_t;
+    using typename base_t::sp_mat_value_t;
+    using vec_sp_value_t = vec_value_t;
+    using vec_sp_index_t = util::rowvec_type<typename sparse_t::StorageIndex>;
 
-    inner_t cols() const
+    static_assert(!sparse_t::IsRowMajor, "MatrixNaiveSparse: only column-major allowed!");
+    
+private:
+    const Eigen::Map<const sparse_t> _mat;  // underlying sparse matrix
+    const size_t _n_threads;                // number of threads
+
+    ADELIE_CORE_STRONG_INLINE
+    value_t _cmul(
+        int j, 
+        const Eigen::Ref<const vec_value_t>& v,
+        const Eigen::Ref<const vec_value_t>& weights
+    ) const
     {
-        return snps() * ancestries();
+        const auto outer = _mat.outerIndexPtr()[j];
+        const auto size = _mat.outerIndexPtr()[j+1] - outer;
+        const Eigen::Map<const vec_sp_index_t> inner(
+            _mat.innerIndexPtr() + outer, size
+        );
+        const Eigen::Map<const vec_sp_value_t> value(
+            _mat.valuePtr() + outer, size
+        );
+        return spddot(inner, value, v * weights);
     }
 
-    Eigen::Ref<const vec_outer_t> outer() const
+    ADELIE_CORE_STRONG_INLINE
+    void _ctmul(
+        int j, 
+        value_t v, 
+        Eigen::Ref<vec_value_t> out
+    ) const
     {
-        if (!_is_read) throw_no_read();
-        constexpr size_t idx = sizeof(bool_t) + 2 * sizeof(inner_t) + sizeof(value_t);
-        return Eigen::Map<const vec_outer_t>(
-            reinterpret_cast<const outer_t*>(&_buffer[idx]),
-            2 * snps() + 1
+        const auto outer = _mat.outerIndexPtr()[j];
+        const auto size = _mat.outerIndexPtr()[j+1] - outer;
+        const Eigen::Map<const vec_sp_index_t> inner(
+            _mat.innerIndexPtr() + outer, size
         );
+        const Eigen::Map<const vec_sp_value_t> value(
+            _mat.valuePtr() + outer, size
+        );
+        spaxi(inner, value, v, out);
     }
-
-    inner_t nnz(int j, bool haplotype) const
+    
+public:
+    explicit MatrixNaiveSparse(
+        size_t rows,
+        size_t cols,
+        size_t nnz,
+        const Eigen::Ref<const vec_sp_index_t>& outer,
+        const Eigen::Ref<const vec_sp_index_t>& inner,
+        const Eigen::Ref<const vec_sp_value_t>& value,
+        size_t n_threads
+    ): 
+        _mat(rows, cols, nnz, outer.data(), inner.data(), value.data()),
+        _n_threads(n_threads)
     {
-        if (!_is_read) throw_no_read();
-        const auto _outer = outer();
-        j = 2 * j + haplotype;
-        return (_outer[j+1] - _outer[j]) / _multiplier;
+        if (n_threads < 1) {
+            throw util::adelie_core_error("n_threads must be >= 1.");
+        }
     }
 
-    Eigen::Ref<const vec_inner_t> inner(int j, bool haplotype) const 
-    {
-        if (!_is_read) throw_no_read();
-        const auto _outer = outer();
-        return Eigen::Map<const vec_inner_t>(
-            reinterpret_cast<const inner_t*>(&_buffer[_outer[2 * j + haplotype]]),
-            nnz(j, haplotype)
-        );
+    value_t cmul(
+        int j, 
+        const Eigen::Ref<const vec_value_t>& v,
+        const Eigen::Ref<const vec_value_t>& weights
+    ) override
+    {
+        base_t::check_cmul(j, v.size(), weights.size(), rows(), cols());
+        return _cmul(j, v, weights);
+    }
+
+    void ctmul(
+        int j, 
+        value_t v, 
+        Eigen::Ref<vec_value_t> out
+    ) override
+    {
+        base_t::check_ctmul(j, out.size(), rows(), cols());
+        _ctmul(j, v, out);
+    }
+
+    void bmul(
+        int j, int q, 
+        const Eigen::Ref<const vec_value_t>& v, 
+        const Eigen::Ref<const vec_value_t>& weights,
+        Eigen::Ref<vec_value_t> out
+    ) override
+    {
+        base_t::check_bmul(j, q, v.size(), weights.size(), out.size(), rows(), cols());
+        for (int k = 0; k < q; ++k) {
+            out[k] = _cmul(j+k, v, weights);
+        }
     }
 
-    Eigen::Ref<const vec_value_t> ancestry(int j, bool haplotype) const 
-    {
-        if (!_is_read) throw_no_read();
-        const auto _outer = outer();
-        const auto _nnz = nnz(j, haplotype);
-        return Eigen::Map<const vec_value_t>(
-            reinterpret_cast<const value_t*>(&_buffer[
-                _outer[2 * j + haplotype] + sizeof(inner_t) * _nnz
-            ]),
-            _nnz
-        );
+    void btmul(
+        int j, int q, 
+        const Eigen::Ref<const vec_value_t>& v, 
+        Eigen::Ref<vec_value_t> out
+    ) override
+    {
+        base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
+        for (int k = 0; k < q; ++k) {
+            _ctmul(j+k, v[k], out);
+        }
     }
 
-    rowarr_value_t to_dense(
-        size_t n_threads
-    ) const
+    void mul(
+        const Eigen::Ref<const vec_value_t>& v, 
+        const Eigen::Ref<const vec_value_t>& weights,
+        Eigen::Ref<vec_value_t> out
+    ) override
     {
-        if (!_is_read) throw_no_read();
-        const auto n = rows();
-        const auto s = snps();
-        const auto A = ancestries();
-        rowarr_value_t dense(n, s * A);
-
-        const auto routine = [&](inner_t j) {
-            auto dense_j = dense.middleCols(A * j, A);
-            dense_j.setZero();
-            for (char hap = 0; hap < 2; ++hap) {
-                const auto _inner = inner(j, hap);
-                const auto _ancestry = ancestry(j, hap);
-                for (inner_t i = 0; i < _inner.size(); ++i) {
-                    dense_j(_inner[i], _ancestry[i]) += 1;
-                }
-            }
+        const auto routine = [&](int k) {
+            out[k] = _cmul(k, v, weights);
         };
-        if (n_threads <= 1) {
-            for (inner_t j = 0; j < s; ++j) routine(j);
+        if (_n_threads <= 1) {
+            for (int k = 0; k < out.size(); ++k) routine(k);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
-            for (inner_t j = 0; j < s; ++j) routine(j);
+            #pragma omp parallel for schedule(static) num_threads(_n_threads)
+            for (int k = 0; k < out.size(); ++k) routine(k);
         }
-
-        return dense;
     }
-
-    size_t write(
-        const Eigen::Ref<const colarr_value_t>& calldata,
-        const Eigen::Ref<const colarr_value_t>& ancestries,
-        size_t A,
-        size_t n_threads
-    )
+    
+    int rows() const override
     {
-        const bool_t endian = is_big_endian();
-        const inner_t n = calldata.rows();
-        const inner_t s = calldata.cols() / 2;
-
-        // outer[i] = number of bytes to jump from beginning of file 
-        // to start reading column i information.
-        // outer[i+1] - outer[i] = total number of bytes for column i. 
-        vec_outer_t outer(2*s + 1); 
-        outer[0] = 0;
-        outer.tail(2*s) = (calldata != 0).colwise().count().template cast<outer_t>();
-        for (int i = 1; i < outer.size(); ++i) {
-            outer[i] += outer[i-1];
-        }
-        outer *= _multiplier;
-        outer += (
-            sizeof(bool_t) +
-            2 * sizeof(inner_t) +
-            sizeof(value_t) +
-            outer.size() * sizeof(outer_t)
-        );
-
-        buffer_t buffer(outer[2*s]);
-
-        size_t idx = 0;
-        reinterpret_cast<bool_t&>(buffer[idx]) = endian; idx += sizeof(bool_t);
-        reinterpret_cast<inner_t&>(buffer[idx]) = n; idx += sizeof(inner_t);
-        reinterpret_cast<inner_t&>(buffer[idx]) = s; idx += sizeof(inner_t);
-        reinterpret_cast<value_t&>(buffer[idx]) = A; idx += sizeof(value_t);
-        Eigen::Map<vec_outer_t>(
-            reinterpret_cast<outer_t*>(&buffer[idx]),
-            outer.size()
-        ) = outer;
-
-        const auto routine = [&](inner_t j) {
-            const auto col_j = calldata.col(j);
-            const auto ancestry_j = ancestries.col(j);
-            const auto nnz_bytes = outer[j+1] - outer[j];
-            const auto nnz = nnz_bytes / _multiplier;
-            Eigen::Map<vec_inner_t> inner(
-                reinterpret_cast<inner_t*>(&buffer[outer[j]]),
-                nnz
-            );
-            Eigen::Map<vec_value_t> ancestry(
-                reinterpret_cast<value_t*>(&buffer[outer[j] + sizeof(inner_t) * nnz]),
-                nnz
-            );
-
-            size_t count = 0;
-            for (inner_t i = 0; i < n; ++i) {
-                if (col_j[i] == 0) continue;
-                inner[count] = i;
-                ancestry[count] = ancestry_j(i);
-                ++count;
+        return _mat.rows();
+    }
+    
+    int cols() const override
+    {
+        return _mat.cols();
+    }
+
+    void cov(
+        int j, int q,
+        const Eigen::Ref<const vec_value_t>& sqrt_weights,
+        Eigen::Ref<colmat_value_t> out,
+        Eigen::Ref<colmat_value_t> buffer
+    ) override
+    {
+        base_t::check_cov(
+            j, q, sqrt_weights.size(), 
+            out.rows(), out.cols(), buffer.rows(), buffer.cols(), 
+            rows(), cols()
+        );
+        const auto routine = [&](int i1) {
+            for (int i2 = 0; i2 <= i1; ++i2) {
+                const auto index_1 = j+i1;
+                const auto index_2 = j+i2;
+                const auto outer_1 = _mat.outerIndexPtr()[index_1];
+                const auto outer_2 = _mat.outerIndexPtr()[index_2];
+                const auto size_1 = _mat.outerIndexPtr()[index_1+1] - outer_1;
+                const auto size_2 = _mat.outerIndexPtr()[index_2+1] - outer_2;
+                const Eigen::Map<const vec_sp_index_t> inner_1(
+                    _mat.innerIndexPtr() + outer_1, size_1
+                );
+                const Eigen::Map<const vec_sp_index_t> inner_2(
+                    _mat.innerIndexPtr() + outer_2, size_2
+                );
+                const Eigen::Map<const vec_sp_value_t> value_1(
+                    _mat.valuePtr() + outer_1, size_1
+                );
+                const Eigen::Map<const vec_sp_value_t> value_2(
+                    _mat.valuePtr() + outer_2, size_2
+                );
+
+                out(i1, i2) = svsvwdot(
+                    inner_1, value_1,
+                    inner_2, value_2,
+                    sqrt_weights.square()
+                );
             }
         };
-        if (n_threads <= 1) {
-            for (inner_t j = 0; j < calldata.cols(); ++j) routine(j);
+        if (_n_threads <= 1) {
+            for (int i1 = 0; i1 < q; ++i1) routine(i1);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
-            for (inner_t j = 0; j < calldata.cols(); ++j) routine(j);
+            #pragma omp parallel for schedule(static) num_threads(_n_threads)
+            for (int i1 = 0; i1 < q; ++i1) routine(i1);
         }
-
-        auto file_ptr = fopen_safe(_filename.c_str(), "wb");
-        auto fp = file_ptr.get();
-        auto total_bytes = std::fwrite(buffer.data(), sizeof(char), buffer.size(), fp);
-        if (total_bytes != static_cast<size_t>(buffer.size())) {
-            throw util::adelie_core_error(
-                "Could not write the full buffer."
-            );
+        for (int i1 = 0; i1 < q; ++i1) {
+            for (int i2 = i1+1; i2 < q; ++i2) {
+                out(i1, i2) = out(i2, i1);
+            }
         }
+    }
 
-        return total_bytes;
+    void sp_btmul(
+        const sp_mat_value_t& v, 
+        Eigen::Ref<rowmat_value_t> out
+    ) override
+    {
+        base_t::check_sp_btmul(
+            v.rows(), v.cols(), out.rows(), out.cols(), rows(), cols()
+        );
+        out = v * _mat.transpose();
     }
 };
 
-} // namespace io
+} // namespace matrix
 } // namespace adelie_core
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -159,35 +159,39 @@
     void btmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
-        dvzero(out, _n_threads);
         int n_processed = 0;
         while (n_processed < q) {
             const auto j_curr = j + n_processed;
             const auto slice = _slice_map[j_curr];
             auto& mat = *_mat_list[slice];
             const auto index = _index_map[j_curr];
             const int q_curr = std::min(mat.cols()-index, q-n_processed);
-            mat.btmul(index, q_curr, v.segment(n_processed, q_curr), _buff);
-            dvaddi(out, _buff, _n_threads);
+            mat.btmul(index, q_curr, v.segment(n_processed, q_curr), out);
             n_processed += q_curr;
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
-        bmul(0, cols(), v, weights, out);
+        int n_processed = 0;
+        for (int i = 0; i < _mat_list.size(); ++i) {
+            auto& mat = *_mat_list[i];
+            const auto p = mat.cols();
+            mat.mul(v, weights, out.segment(n_processed, p));
+            n_processed += p;
+        }
     }
 
     int rows() const override
     {
         return _rows;
     }
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     void ctmul(
         int j, 
         value_t v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
-        dax(v, _mat.transpose().row(j).array(), _n_threads, out);
+        dvaddi(out, v * _mat.col(j).transpose().array(), _n_threads);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
@@ -83,15 +83,15 @@
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
         auto outm = out.matrix();
-        dgemv(
+        dgemv<util::operator_type::_add>(
             _mat.middleCols(j, q).transpose(),
             v.matrix(),
             _n_threads,
             _buff,
             outm
         );
     }
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,18 @@
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
         int i = j / _K;
         int l = j - _K * i;
-        dvzero(out, _n_threads);
         Eigen::Map<vec_value_t> _out(_buff.data(), Out.rows());
+        dvzero(_out, _n_threads);
         _mat->ctmul(i, v, _out);
-        Out.col(l) = _out;
+        Out.col(l).array() += _out;
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
@@ -116,43 +116,39 @@
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
         for (int l = 0; l < _K; ++l) {
             const auto j_l = std::max(j-l, 0);
             const auto i_begin = j_l / static_cast<int>(_K) + ((j_l % _K) != 0);
-            if (j-l+q <= 0) {
-                Out.col(l).setZero();
-                continue;
-            }
+            if (j-l+q <= 0) continue;
             const auto i_end = (j-l+q-1) / static_cast<int>(_K) + 1;
             const auto i_q = i_end - i_begin;
-            if (i_q <= 0) {
-                Out.col(l).setZero();
-                continue;
-            }
+            if (i_q <= 0) continue;
             Eigen::Map<vec_value_t> _v(_buff.data(), i_q);
             for (int i = i_begin; i < i_end; ++i) {
                 _v[i-i_begin] = v[i*_K+l-j];
             }
             Eigen::Map<vec_value_t> _out(
                 _buff.data() + i_q,
                 Out.rows()
             );
+            _out.setZero();
             _mat->btmul(i_begin, i_q, _v, _out);
-            Out.col(l) = _out;
+            Out.col(l).array() += _out;
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
+        // TODO: this can maybe be parallelized?
         bmul(0, cols(), v, weights, out);
     }
 
     void cov(
         int j, int q,
         const Eigen::Ref<const vec_value_t>& sqrt_weights,
         Eigen::Ref<colmat_value_t> out,
@@ -323,17 +319,16 @@
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
         const int i = j / _K;
         const int l = j - _K * i;
-        dvzero(out, _n_threads);
         auto _out = Out.col(l);
-        dax(v, _mat.col(i), _n_threads, _out);
+        dvaddi(_out, v * _mat.col(i), _n_threads);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
@@ -363,15 +358,14 @@
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
-        dvzero(out, _n_threads);
         int n_processed = 0;
         while (n_processed < q) {
             const int i = (j + n_processed) / _K;
             const int l = (j + n_processed) - _K * i;
             const int size = std::min<int>(_K-l, q-n_processed);
             Eigen::Map<const vec_value_t> _v(v.data() + n_processed, size);
             for (int k = 0; k < size; ++k) {
@@ -423,20 +417,27 @@
             auto buff_array = buff.array();
             dmmeq(
                 buff_array,
                 _mat.middleCols(i_begin, i_q).array().colwise() * sqrt_W.col(l).array(),
                 _n_threads
             );
             for (int i1 = 0; i1 < i_q; ++i1) {
-                for (int i2 = 0; i2 < i_q; ++i2) {
+                for (int i2 = 0; i2 <= i1; ++i2) {
                     out((i1+i_begin)*_K+l-j, (i2+i_begin)*_K+l-j) = (
                         buff.col(i1).dot(buff.col(i2))
                     );
                 }
             }
+            for (int i1 = 0; i1 < i_q; ++i1) {
+                for (int i2 = i1 + 1; i2 < i_q; ++i2) {
+                    const auto fi1 = (i1+i_begin)*_K+l-j;
+                    const auto fi2 = (i2+i_begin)*_K+l-j;
+                    out(fi1, fi2) = out(fi2, fi1);
+                }
+            }
         }
     }
 
     int rows() const override { return _K * _mat.rows(); }
     int cols() const override { return _K * _mat.cols(); }
 
     void sp_btmul(
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -4,256 +4,183 @@
 #include <adelie_core/matrix/matrix_naive_base.hpp>
 #include <adelie_core/matrix/utils.hpp>
 #include <adelie_core/io/io_snp_phased_ancestry.hpp>
 
 namespace adelie_core {
 namespace matrix {
 
-template <class ValueType>
+template <class ValueType,
+          class MmapPtrType=std::unique_ptr<char, std::function<void(char*)>>>
 class MatrixNaiveSNPPhasedAncestry: public MatrixNaiveBase<ValueType>
 {
 public:
     using base_t = MatrixNaiveBase<ValueType>;
     using typename base_t::value_t;
     using typename base_t::vec_value_t;
     using typename base_t::vec_index_t;
     using typename base_t::colmat_value_t;
     using typename base_t::rowmat_value_t;
     using typename base_t::sp_mat_value_t;
     using string_t = std::string;
-    using io_t = io::IOSNPPhasedAncestry;
-    using dyn_vec_io_t = std::vector<io_t>;
+    using io_t = io::IOSNPPhasedAncestry<MmapPtrType>;
     
 protected:
-    const string_t _filename;   // filename because why not? :)
     const io_t _io;             // IO handler
     const size_t _n_threads;    // number of threads
-    vec_value_t _vbuff;         // vector buffer
-    util::rowarr_type<value_t> _buff;           // buffer
+    util::rowvec_type<char> _bbuff;
+    vec_index_t _ibuff;
 
     static auto init_io(
         const string_t& filename,
         const string_t& read_mode
     )
     {
         io_t io(filename, read_mode);
         io.read();
         return io;
     }
 
-    static void throw_bad_start_index(int j, int A)
+    ADELIE_CORE_STRONG_INLINE
+    value_t _cmul(
+        int j,
+        const Eigen::Ref<const vec_value_t>& v,
+        const Eigen::Ref<const vec_value_t>& weights
+    ) const
     {
-        throw util::adelie_core_error(
-            "Bad starting index " + std::to_string(j) +
-            " with ancestries " + std::to_string(A)
-        );
+        const auto A = ancestries();
+        const auto snp = j / A;
+        const auto anc = j % A;
+
+        value_t sum = 0;
+        for (int hap = 0; hap < io_t::n_haps; ++hap) {
+            auto it = _io.begin(snp, anc, hap);
+            const auto end = _io.end(snp, anc, hap);
+            for (; it != end; ++it) {
+                const auto idx = *it;
+                sum += v[idx] * weights[idx];
+            }
+        }
+
+        return sum;
     }
 
-    static void throw_bad_size(int q, int A)
+    ADELIE_CORE_STRONG_INLINE
+    void _ctmul(
+        int j,
+        value_t v,
+        Eigen::Ref<vec_value_t> out
+    )
     {
-        throw util::adelie_core_error(
-            "Bad size " + std::to_string(q) +
-            " with ancestries " + std::to_string(A)
-        );
+        const auto A = ancestries();
+        const auto snp = j / A;
+        const auto anc = j % A;
+
+        for (int hap = 0; hap < io_t::n_haps; ++hap) {
+            auto it = _io.begin(snp, anc, hap);
+            const auto end = _io.end(snp, anc, hap);
+            for (; it != end; ++it) {
+                out[*it] += v;
+            }
+        }
     }
 
+    auto ancestries() const { return _io.ancestries(); }
+
 public:
     explicit MatrixNaiveSNPPhasedAncestry(
         const string_t& filename,
         const string_t& read_mode,
         size_t n_threads
     ): 
-        _filename(filename),
         _io(init_io(filename, read_mode)),
         _n_threads(n_threads),
-        _vbuff(n_threads),
-        _buff(n_threads, _io.ancestries())
+        _bbuff(_io.rows()),
+        _ibuff(_io.rows())
     {
         if (n_threads < 1) {
             throw util::adelie_core_error("n_threads must be >= 1.");
         }
+        _bbuff.setZero();
     }
 
-    auto ancestries() const { return _io.ancestries(); }
-
     value_t cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
         const Eigen::Ref<const vec_value_t>& weights
     ) override
     {
         base_t::check_cmul(j, v.size(), weights.size(), rows(), cols());
-
-        const auto A = ancestries();
-        const auto snp = j / A;
-        const auto anc = j % A;
-
-        value_t sum = 0;
-        for (int hap = 0; hap < 2; ++hap) {
-            const auto inner = _io.inner(snp, hap);
-            const auto ancestry = _io.ancestry(snp, hap);
-
-            for (int i = 0; i < inner.size(); ++i) {
-                if (ancestry[i] != anc) continue;
-                sum += v[inner[i]] * weights[inner[i]];
-            }
-        }
-
-        return sum;
+        return _cmul(j, v, weights);
     }
 
     void ctmul(
         int j, 
         value_t v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
-
-        const auto A = ancestries();
-        const auto snp = j / A;
-        const auto anc = j % A;
-
-        dvzero(out, _n_threads);
-
-        for (int hap = 0; hap < 2; ++hap) {
-            const auto inner = _io.inner(snp, hap);
-            const auto ancestry = _io.ancestry(snp, hap);
-            for (int i = 0; i < inner.size(); ++i) {
-                if (ancestry[i] != anc) continue;
-                out[inner[i]] += v;
-            }
-        }
+        _ctmul(j, v, out);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_bmul(j, q, v.size(), weights.size(), out.size(), rows(), cols());
-
-        const int A = ancestries();
-
-        out.setZero(); // don't parallelize! q is usually small
-
-        int n_batches = (
-            (j + q - A * (j / A) + A - 1) / A
-        );
-
-        const auto routine = [&](int b) {
-            const auto n_solved =  (b > 0) * (A * ((j / A) + 1) - j + (b-1) * A);
-            const auto begin = j + n_solved;
-            const auto snp = begin / A;
-            const auto ancestry_lower = begin % A;
-            const auto ancestry_upper = std::min<int>(ancestry_lower + q - n_solved, A);
-
-            const auto _common_routine = [&](const auto func) {
-                for (int hap = 0; hap < 2; ++hap) {
-                    const auto inner = _io.inner(snp, hap);
-                    const auto ancestry = _io.ancestry(snp, hap);
-                    func(inner, ancestry);
-                }
-            };
-
-            // optimized routine when additional check is not required
-            if (ancestry_lower == 0 && ancestry_upper == A) {
-                _common_routine([&](const auto& inner, const auto& ancestry) {
-                    for (int i = 0; i < inner.size(); ++i) {
-                        out[n_solved+ancestry[i]] += v[inner[i]] * weights[inner[i]];
-                    }
-                });
-            } else {
-                _common_routine([&](const auto& inner, const auto& ancestry) {
-                    for (int i = 0; i < inner.size(); ++i) {
-                        if (ancestry[i] < ancestry_lower || ancestry[i] >= ancestry_upper) continue;
-                        out[n_solved+ancestry[i]-ancestry_lower] += v[inner[i]] * weights[inner[i]];
-                    }
-                });
-            }
-        };
-        if (_n_threads <= 1) {
-            for (int b = 0; b < n_batches; ++b) routine(b);
-        } else {
-            #pragma omp parallel for schedule(static) num_threads(_n_threads)
-            for (int b = 0; b < n_batches; ++b) routine(b);
+        for (int t = 0; t < q; ++t) {
+            out[t] = _cmul(j + t, v, weights);
         }
     }
 
     void btmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
-
-        const int A = ancestries();
-
-        dvzero(out, _n_threads);
-
-        int n_solved = 0;
-        while (n_solved < q) 
-        {
-            const auto begin = j + n_solved;
-            const auto snp = begin / A;
-            const auto ancestry_lower = begin % A;
-            const auto ancestry_upper = std::min<int>(ancestry_lower + q - n_solved, A);
-
-            const auto _common_routine = [&](const auto func) {
-                for (int hap = 0; hap < 2; ++hap) {
-                    const auto inner = _io.inner(snp, hap);
-                    const auto ancestry = _io.ancestry(snp, hap);
-                    func(inner, ancestry);
-                }
-            };
-
-            if (ancestry_lower == 0 && ancestry_upper == A) {
-                _common_routine([&](const auto& inner, const auto& ancestry) {
-                    for (int i = 0; i < inner.size(); ++i) {
-                        out[inner[i]] += v[n_solved + ancestry[i]];
-                    }
-                });
-            } else {
-                _common_routine([&](const auto& inner, const auto& ancestry) {
-                    for (int i = 0; i < inner.size(); ++i) {
-                        if (ancestry[i] < ancestry_lower || ancestry[i] >= ancestry_upper) continue;
-                        out[inner[i]] += v[n_solved + ancestry[i] - ancestry_lower];
-                    }
-                });
-            }
-
-            n_solved += ancestry_upper - ancestry_lower;
+        for (int t = 0; t < q; ++t) {
+            _ctmul(j + t, v[t], out);
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
-        bmul(0, out.size(), v, weights, out);
+        const auto routine = [&](int t) {
+            out[t] = _cmul(t, v, weights);
+        };
+        if (_n_threads <= 1) {
+            for (int t = 0; t < cols(); ++t) routine(t);
+        } else {
+            #pragma omp parallel for schedule(static) num_threads(_n_threads)
+            for (int t = 0; t < cols(); ++t) routine(t);
+        }
     }
 
     void cov(
         int j, int q,
         const Eigen::Ref<const vec_value_t>& sqrt_weights,
         Eigen::Ref<colmat_value_t> out,
         Eigen::Ref<colmat_value_t> buffer
     ) override
     {
         base_t::check_cov(
             j, q, sqrt_weights.size(), 
             out.rows(), out.cols(), buffer.rows(), buffer.cols(), 
             rows(), cols()
         );
-
+        
         const auto A = ancestries();
 
         out.setZero(); // don't parallelize! q is usually small
 
         int n_solved0 = 0;
         while (n_solved0 < q) {
             const auto begin0 = j + n_solved0;
@@ -264,68 +191,127 @@
             int n_solved1 = 0;
             while (n_solved1 <= n_solved0) {
                 const auto begin1 = j + n_solved1;
                 const auto snp1 = begin1 / A;
                 const auto ancestry_lower1 = begin1 % A;
                 const auto ancestry_upper1 = std::min<int>(ancestry_lower1 + q - n_solved1, A);
 
-                for (int hap0 = 0; hap0 < 2; ++hap0) {
-                    for (int hap1 = 0; hap1 < 2; ++hap1) {
-                        const auto inner0 = _io.inner(snp0, hap0);
-                        const auto ancestry0 = _io.ancestry(snp0, hap0);
-                        const auto inner1 = _io.inner(snp1, hap1);
-                        const auto ancestry1 = _io.ancestry(snp1, hap1);
-
-                        int i0 = 0;
-                        int i1 = 0;
-                        while (
-                            (i0 < inner0.size()) &&
-                            (i1 < inner1.size())
-                        ) {
-                            while ((i0 < inner0.size()) && (inner0[i0] < inner1[i1])) ++i0;
-                            if (i0 == inner0.size()) break;
-                            while ((i1 < inner1.size()) && (inner1[i1] < inner0[i0])) ++i1;
-                            if (i1 == inner1.size()) break;
-                            while (
-                                (i0 < inner0.size()) &&
-                                (i1 < inner1.size()) &&
-                                (inner0[i0] == inner1[i1])
-                            ) {
-                                if (
-                                    ((n_solved0 == n_solved1) && (ancestry0[i0] < ancestry1[i1])) ||
-                                    (ancestry0[i0] < ancestry_lower0) ||
-                                    (ancestry0[i0] >= ancestry_upper0) ||
-                                    (ancestry1[i1] < ancestry_lower1) ||
-                                    (ancestry1[i1] >= ancestry_upper1)
-                                ) {
-                                    ++i0;
-                                    ++i1;
-                                    continue;
-                                }
-                                const auto k0 = n_solved0 + ancestry0[i0] - ancestry_lower0;
-                                const auto k1 = n_solved1 + ancestry1[i1] - ancestry_lower1;
-                                const auto sw = sqrt_weights[inner1[i1]];
-                                out(k0, k1) += sw * sw;
-                                ++i0;
-                                ++i1;
+                if (n_solved0 == n_solved1) {
+                    const auto begin = begin0;
+                    const auto snp = snp0;
+                    const auto a_low = ancestry_lower0;
+                    const auto a_high = ancestry_upper0;
+                    const auto a_size = a_high - a_low;
+
+                    // compute quadratic diagonal part
+                    for (int k = 0; k < a_size; ++k) {
+                        value_t sum = 0;
+                        for (size_t hap = 0; hap < io_t::n_haps; ++hap) {
+                            const auto anc = a_low + k;
+                            auto it = _io.begin(snp, anc, hap);
+                            const auto end = _io.end(snp, anc, hap);
+                            for (; it != end; ++it) {
+                                const auto idx = *it;
+                                const auto sqrt_w = sqrt_weights[idx];
+                                sum += sqrt_w * sqrt_w;
+                            }
+                        }
+                        const auto kk = n_solved0 + k;
+                        out(kk, kk) = sum;
+                    }
+
+                    // compute cross-terms
+                    for (int k0 = 0; k0 < a_size; ++k0) {
+                        // cache hap0 information
+                        size_t nnz = 0;
+                        auto it0 = _io.begin(snp, a_low + k0, 0);
+                        const auto end0 = _io.end(snp, a_low + k0, 0);
+                        for (; it0 != end0; ++it0) {
+                            const auto idx = *it0;
+                            _bbuff[idx] = true;
+                            _ibuff[nnz] = idx;
+                            ++nnz;
+                        }
+
+                        // loop through hap1's ancestries
+                        for (int k1 = 0; k1 < a_size; ++k1) {
+                            auto it1 = _io.begin(snp, a_low + k1, 1);
+                            const auto end1 = _io.end(snp, a_low + k1, 1);
+                            value_t sum = 0;
+                            for (; it1 != end1; ++it1) {
+                                const auto idx = *it1;
+                                if (!_bbuff[idx]) continue;
+                                const auto sqrt_w = sqrt_weights[idx];
+                                sum += sqrt_w * sqrt_w;
                             }
+
+                            const auto kk0 = n_solved0 + k0;
+                            const auto kk1 = n_solved0 + k1;
+                            out(kk0, kk1) += sum;
+                            out(kk1, kk0) += sum;
+                        }
+
+                        // keep invariance by populating with false
+                        for (size_t i = 0; i < nnz; ++i) {
+                            _bbuff[_ibuff[i]] = false;
                         }
                     }
+
+                    n_solved1 += ancestry_upper1 - ancestry_lower1;
+                    continue;
+                }
+
+                /* general routine */
+
+                const auto ancestry_size0 = ancestry_upper0-ancestry_lower0;
+                const auto ancestry_size1 = ancestry_upper1-ancestry_lower1;
+                for (int a0 = 0; a0 < ancestry_size0; ++a0) {
+                    size_t nnz = 0;
+                    for (int hap0 = 0; hap0 < io_t::n_haps; ++hap0) {
+                        auto it = _io.begin(snp0, ancestry_lower0+a0, hap0);
+                        const auto end = _io.end(snp0, ancestry_lower0+a0, hap0);
+                        for (; it != end; ++it) {
+                            const auto idx = *it;
+                            if (!_bbuff[idx]) {
+                                _ibuff[nnz] = idx;
+                                ++nnz;
+                            }
+                            _bbuff[idx] += 1;
+                        }
+                    }
+
+                    for (int a1 = 0; a1 < ancestry_size1; ++a1) {
+                        value_t sum = 0;
+                        for (int hap1 = 0; hap1 < io_t::n_haps; ++hap1) {
+                            auto it = _io.begin(snp1, ancestry_lower1+a1, hap1);
+                            const auto end = _io.end(snp1, ancestry_lower1+a1, hap1);
+                            for (; it != end; ++it) {
+                                const auto idx = *it;
+                                const auto v0 = _bbuff[idx];
+                                if (!v0) continue;
+                                const auto sqrt_w = sqrt_weights[idx];
+                                sum += sqrt_w * sqrt_w * v0;
+                            }
+                        }
+                        const auto kk0 = n_solved0 + a0;
+                        const auto kk1 = n_solved1 + a1;
+                        out(kk0, kk1) = sum;
+                        // populate the mirror side
+                        out(kk1, kk0) = sum;
+                    }
+
+                    for (size_t i = 0; i < nnz; ++i) {
+                        _bbuff[_ibuff[i]] = 0;
+                    }
                 }
 
                 n_solved1 += ancestry_upper1 - ancestry_lower1;
             }
             n_solved0 += ancestry_upper0 - ancestry_lower0;
         }     
-
-        for (int i1 = 0; i1 < q; ++i1) {
-            for (int i2 = i1+1; i2 < q; ++i2) {
-                out(i1, i2) = out(i2, i1);
-            }
-        }
     }
 
     int rows() const override { return _io.rows(); }
     int cols() const override { return _io.snps() * ancestries(); }
 
     void sp_btmul(
         const sp_mat_value_t& v,
@@ -336,28 +322,16 @@
             v.rows(), v.cols(), out.rows(), out.cols(), rows(), cols()
         );
         const auto A = ancestries();
         const auto routine = [&](int k) {
             typename sp_mat_value_t::InnerIterator it(v, k);
             auto out_k = out.row(k);
             out_k.setZero();
-            for (; it; ++it) 
-            {
-                const auto t = it.index();
-                const auto snp = t / A;
-                const auto anc = t % A;
-
-                for (int hap = 0; hap < 2; ++hap) {
-                    const auto inner = _io.inner(snp, hap);
-                    const auto ancestry = _io.ancestry(snp, hap);
-                    for (int i = 0; i < inner.size(); ++i) {
-                        if (ancestry[i] != anc) continue;
-                        out_k[inner[i]] += it.value();
-                    }
-                }
+            for (; it; ++it) {
+                _ctmul(it.index(), it.value(), out_k);
             }
         };
         if (_n_threads <= 1) {
             for (int k = 0; k < v.outerSize(); ++k) routine(k);
         } else {
             #pragma omp parallel for schedule(static) num_threads(_n_threads)
             for (int k = 0; k < v.outerSize(); ++k) routine(k);
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/matrix/utils.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/matrix/utils.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -188,26 +188,36 @@
             + std::max<int>(t-remainder, 0) * block_size
         );
         const auto size = block_size + (t < remainder);
         out.segment(begin, size).setZero();
     }
 }
 
-template <class MType, class VType, class BuffType, class OutType>
+template <util::operator_type op=util::operator_type::_eq, 
+          class MType, class VType, class BuffType, class OutType>
 ADELIE_CORE_STRONG_INLINE
 void dgemv(
     const MType& m,
     const VType& v,
     size_t n_threads,
     BuffType& buff,
     OutType& out
 )
 {
     assert(n_threads > 0);
-    if (n_threads <= 1) { out.noalias() = v * m; return; }
+    if (n_threads <= 1) { 
+        if constexpr (op == util::operator_type::_eq) {
+            out.noalias() = v * m; 
+        } else if constexpr (op == util::operator_type::_add) {
+            out += v * m; 
+        } else {
+            static_assert("Bad operator type!");
+        }
+        return; 
+    }
     const size_t n = m.rows();
     const size_t p = m.cols();
     const size_t max_np = std::max(n, p);
     const int n_blocks = std::min(n_threads, max_np);
     const int block_size = max_np / n_blocks;
     const int remainder = max_np % n_blocks;
 
@@ -216,15 +226,21 @@
         for (int t = 0; t < n_blocks; ++t)
         {
             const auto begin = (
                 std::min<int>(t, remainder) * (block_size + 1) 
                 + std::max<int>(t-remainder, 0) * block_size
             );
             const auto size = block_size + (t < remainder);
-            out.segment(begin, size).noalias() = v * m.middleCols(begin, size);
+            if constexpr (op == util::operator_type::_eq) {
+                out.segment(begin, size).noalias() = v * m.middleCols(begin, size);
+            } else if constexpr (op == util::operator_type::_add) {
+                out.segment(begin, size).noalias() += v * m.middleCols(begin, size);
+            } else {
+                static_assert("Bad operator type!");
+            }
         }
     } else {
         assert(buff.rows() >= n_blocks);
         assert(buff.cols() >= p);
         #pragma omp parallel for schedule(static) num_threads(n_threads)
         for (int t = 0; t < n_blocks; ++t)
         {
@@ -233,15 +249,21 @@
                 + std::max<int>(t-remainder, 0) * block_size
             );
             const auto size = block_size + (t < remainder);
             buff.row(t).head(p).noalias() = (
                 v.segment(begin, size) * m.middleRows(begin, size)
             );
         }
-        out = buff.block(0, 0, n_blocks, p).colwise().sum();
+        if constexpr (op == util::operator_type::_eq) {
+            out = buff.block(0, 0, n_blocks, p).colwise().sum();
+        } else if constexpr (op == util::operator_type::_add) {
+            out += buff.block(0, 0, n_blocks, p).colwise().sum();
+        } else {
+            static_assert("Bad operator type!");
+        }
     }
 }
 
 template <class InnerType, class ValueType, class WeightsType>
 ADELIE_CORE_STRONG_INLINE
 auto svsvwdot(
     const InnerType& inner_1,
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/optimization/bisect.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/optimization/bisect.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/optimization/newton.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/optimization/newton.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/optimization/search_pivot.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/optimization/search_pivot.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_base.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -90,62 +90,67 @@
     assert(screen_set.size() <= abs_grad.size());
 
     const auto is_screen = [&](auto i) { 
         return screen_hashset.find(i) != screen_hashset.end(); 
     };
 
     const auto do_pivot = [&]() {
-        const int G = abs_grad.size();
-        vec_index_t order = vec_index_t::LinSpaced(G, 0, G-1);
-        vec_value_t weights = vec_value_t::NullaryExpr(
-            G, [&](auto i) { 
-                return (penalty[i] <= 0) ? 
-                    alpha * lmda : std::min(abs_grad[i] / penalty[i], alpha * lmda); 
+        // Only compute pivot rule if new active variables entered.
+        // The pivot rule doesn't include new screen variables otherwise,
+        // so no need to do any computations.
+        if (n_new_active) {
+            const int G = abs_grad.size();
+            vec_index_t order = vec_index_t::LinSpaced(G, 0, G-1);
+            vec_value_t weights = vec_value_t::NullaryExpr(
+                G, [&](auto i) { 
+                    return (penalty[i] <= 0) ? 
+                        alpha * lmda : std::min(abs_grad[i] / penalty[i], alpha * lmda); 
+                }
+            );
+            std::sort(
+                order.data(), 
+                order.data() + order.size(), 
+                [&](auto i, auto j) { 
+                    return weights[i] < weights[j]; 
+                }
+            );
+            const int subset_size = std::min<int>(std::max<int>(
+                old_screen_set_size * (1 + pivot_subset_ratio),
+                pivot_subset_min
+            ), G);
+            // top largest subset_size number of weights
+            vec_value_t weights_sorted_sub = vec_value_t::NullaryExpr(
+                subset_size,
+                [&](auto i) { return weights[order[G-subset_size+i]]; } 
+            );
+
+            vec_value_t mses(subset_size);
+            vec_value_t indices = vec_value_t::LinSpaced(subset_size, 0, subset_size-1);
+            const int pivot_idx = optimization::search_pivot(
+                indices, 
+                weights_sorted_sub, 
+                mses
+            );
+            const int full_pivot_idx = G - subset_size + pivot_idx;
+
+            // add everything beyond the cutoff index that isn't screen yet
+            for (int ii = G-1; ii >= full_pivot_idx; --ii) {
+                const auto i = order[ii];
+                if (is_screen(i)) continue;
+                screen_set.push_back(i); 
             }
-        );
-        std::sort(
-            order.data(), 
-            order.data() + order.size(), 
-            [&](auto i, auto j) { 
-                return weights[i] < weights[j]; 
+            // add some slack of new groups below the pivot
+            int count = 0;
+            for (int ii = full_pivot_idx - 1; ii >= 0; --ii) {
+                if (count >= pivot_slack_ratio * n_new_active) break;
+                const auto i = order[ii]; 
+                if (is_screen(i)) continue;
+                screen_set.push_back(i);
+                ++count;
             }
-        );
-        const int subset_size = std::min<int>(std::max<int>(
-            old_screen_set_size * (1 + pivot_subset_ratio),
-            pivot_subset_min
-        ), G);
-        // top largest subset_size number of weights
-        vec_value_t weights_sorted_sub = vec_value_t::NullaryExpr(
-            subset_size,
-            [&](auto i) { return weights[order[G-subset_size+i]]; } 
-        );
-
-        vec_value_t mses(subset_size);
-        vec_value_t indices = vec_value_t::LinSpaced(subset_size, 0, subset_size-1);
-        const int pivot_idx = optimization::search_pivot(
-            indices, 
-            weights_sorted_sub, 
-            mses
-        );
-        const int full_pivot_idx = G - subset_size + pivot_idx;
-
-        // add everything beyond the cutoff index that isn't screen yet
-        for (int ii = G-1; ii >= full_pivot_idx; --ii) {
-            const auto i = order[ii];
-            if (is_screen(i)) continue;
-            screen_set.push_back(i); 
-        }
-        // add some slack of new groups below the pivot
-        int count = 0;
-        for (int ii = full_pivot_idx - 1; ii >= 0; --ii) {
-            if (count >= pivot_slack_ratio * std::max<int>(n_new_active, 1)) break;
-            const auto i = order[ii]; 
-            if (is_screen(i)) continue;
-            screen_set.push_back(i);
-            ++count;
         }
 
         // this case should rarely happen, but we arrived here because
         // previous iteration added all pivot-rule predictions and KKT still failed.
         // In this case, do the most safe thing, which is to add all failed variables.
         if ((screen_set.size() == static_cast<size_t>(old_screen_set_size)) && !all_kkt_passed) {
             for (int i = 0; i < abs_grad.size(); ++i) {
@@ -247,14 +252,15 @@
     const auto& screen_set = state.screen_set;
     const auto max_screen_size = state.max_screen_size;
     const auto setup_lmda_max = state.setup_lmda_max;
     const auto setup_lmda_path = state.setup_lmda_path;
     const auto lmda_path_size = state.lmda_path_size;
     const auto min_ratio = state.min_ratio;
     const auto& screen_is_active = state.screen_is_active;
+    const auto& active_set_size = state.active_set_size;
     const auto& abs_grad = state.abs_grad;
     auto& lmda_max = state.lmda_max;
     auto& lmda_path = state.lmda_path;
     auto& benchmark_screen = state.benchmark_screen;
     auto& benchmark_fit_screen = state.benchmark_fit_screen;
     auto& benchmark_fit_active = state.benchmark_fit_active;
     auto& benchmark_kkt = state.benchmark_kkt;
@@ -271,15 +277,21 @@
     // Initial fit for lambda ~ infinity to setup lmda_max
     // ==================================================================================== 
     // Only unpenalized (l1) groups are active in this case.
     // State must include all unpenalized groups.
     // We solve for large lambda, then back-track the KKT condition to find the lambda
     // that leads to that solution where all penalized variables have 0 coefficient.
     if (setup_lmda_max) {
-        const auto large_lmda = std::numeric_limits<value_t>::max(); 
+        // Must divide by at least the max penalty amount
+        // so that we don't overflow.
+       // Just to be safe, we divide by at least a fixed constant > 1 as well.
+        const value_t large_lmda = (
+            1e-3 * std::numeric_limits<value_t>::max() /
+            std::max<value_t>(1, penalty.maxCoeff())
+        ); 
 
         auto tup = fit_f(state, large_lmda);
         auto&& state_gaussian_pin = std::get<0>(tup);
 
         update_invariance_f(state, state_gaussian_pin, large_lmda);
 
         lmda_max = compute_lmda_max(abs_grad, alpha, penalty);
@@ -303,14 +315,19 @@
     // Since state is in its invariance (solution at state.lmda) and unpenalized groups
     // are ALWAYS active, state includes all unpenalized groups.
     // If no lambda in lmda_path is > lmda_max and setup at lmda_max is not required, 
     // state is left unchanged.
     // Otherwise, it is in its invariance at lmda = lmda_max.
     // All solutions to lambda > lambda_max are saved.
 
+    // initialize progress bar
+    auto pb = util::tq::trange(lmda_path.size());
+    pb.set_display(display);
+    auto pb_it = pb.begin();
+
     // slice lambda_path up to lmda_max
     const auto large_lmda_path_size = std::find_if(
         lmda_path.data(), 
         lmda_path.data() + lmda_path.size(),
         [&](auto x) { return x <= lmda_max; }
     ) - lmda_path.data();
 
@@ -319,25 +336,40 @@
         // and additionally lambda_max at the end.
         // If large_lmda_path_size > 0, mind as well fit for lambda_max as well to go down the path.
         vec_value_t large_lmda_path(large_lmda_path_size + 1);
         large_lmda_path.head(large_lmda_path_size) = lmda_path.head(large_lmda_path_size);
         large_lmda_path[large_lmda_path_size] = lmda_max;
 
         for (int i = 0; i < large_lmda_path.size(); ++i) {
+            if (i < large_lmda_path.size()-1) {
+                // update progress bar
+                pb_it != pb.end();
+
+                // Do not check for early-stopping.
+                // This choice is deliberate for these reasons:
+                // We are in this loop only because the user has supplied their path.
+                // In this case, we should provide what they asked for.
+                // If alpha == 0, this loop is costly but this is also the only time the solutions are actually changing.
+                // If alpha > 0, the solution is the same at every iteration.
+                // Depending on alpha, we have different reasons for not early stopping.
+            }
+
             auto tup = fit_f(state, large_lmda_path[i]);
             auto&& state_gaussian_pin = std::get<0>(tup);
 
             /* Invariance */
             // save only the solutions that the user asked for (up to and not including lmda_max)
             if (i < large_lmda_path.size()-1) {
                 update_solutions_f(
                     state, 
                     state_gaussian_pin,
                     large_lmda_path[i]
                 );
+                pb_add_suffix_f(state, pb);
+                ++pb_it;
             // otherwise, put the state at the last fitted lambda (lmda_max)
             } else {
                 update_invariance_f(state, state_gaussian_pin, large_lmda_path[i]);
             }
         }
     }
 
@@ -345,28 +377,20 @@
 
     // ==================================================================================== 
     // BASIL iterations for lambda <= lambda_max
     // ==================================================================================== 
     // In this case, screen_set may not contain the true active set.
     // We must go through BASIL iterations to solve each lambda.
     sw_t sw;
-    int current_active_size = Eigen::Map<const vec_safe_bool_t>(
-        screen_is_active.data(),
-        screen_is_active.size()
-    ).sum();
+    int current_active_size = active_set_size;
     bool kkt_passed = true;
     int n_new_active = 0;
 
-    auto pb = util::tq::trange(lmda_path.size() - lmda_path_idx);
-    pb.set_display(display);
-
-    for (int _ : pb)
+    for (; pb_it != pb.end(); ++pb_it)
     {
-        static_cast<void>(_);
-
         // check early exit
         if (early_exit_f(state)) {
             pb_add_suffix_f(state, pb);
             break;
         }
 
         // batch the next set of lambdas
@@ -413,21 +437,21 @@
                 }
                 benchmark_kkt.push_back(sw.elapsed());
 
                 // ==================================================================================== 
                 // Diagnostic step
                 // ==================================================================================== 
                 if (kkt_passed) {
-                    active_sizes.push_back(state_gaussian_pin.active_set.size());
+                    active_sizes.push_back(active_set_size);
                     screen_sizes.push_back(state.screen_set.size());
                 }
                 // compute the number of new active groups 
                 n_new_active = (
                     kkt_passed ?
-                    active_sizes.back() - current_active_size : n_new_active
+                    (active_sizes.back() - current_active_size) : n_new_active
                 );
                 current_active_size = (
                     kkt_passed ?
                     active_sizes.back() : current_active_size
                 );
             } catch (...) {
                 pb_add_suffix_f(state, pb);
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,14 @@
 
     auto& A = *state.A;
     const auto& groups = state.groups;
     const auto& group_sizes = state.group_sizes;
     const auto alpha = state.alpha;
     const auto& penalty = state.penalty;
     const auto& screen_set = state.screen_set;
-    const auto& screen_g1 = state.screen_g1;
-    const auto& screen_g2 = state.screen_g2;
     const auto& screen_begins = state.screen_begins;
     const auto& screen_subset_order = state.screen_subset_order;
     const auto& screen_subset_ordered = state.screen_subset_ordered;
     const auto& screen_vars = state.screen_vars;
     const auto& screen_transforms = state.screen_transforms;
     const auto max_active_size = state.max_active_size;
     const auto max_iters = state.max_iters;
@@ -142,14 +140,16 @@
     const auto newton_tol = state.newton_tol;
     const auto newton_max_iters = state.newton_max_iters;
     const auto n_threads = state.n_threads;
     auto& rsq = state.rsq;
     auto& screen_beta = state.screen_beta;
     auto& screen_grad = state.screen_grad;
     auto& screen_is_active = state.screen_is_active;
+    auto& active_set_size = state.active_set_size;
+    auto& active_set = state.active_set;
 
     auto& screen_grad_prev = buffer_pack.screen_grad_prev;
     auto& screen_beta_prev = buffer_pack.screen_beta_prev;
     auto& screen_is_active_prev = buffer_pack.screen_is_active_prev;
 
     util::rowvec_type<value_t, 1> lmda_path;
     lmda_path = lmda;
@@ -173,44 +173,45 @@
     state_gaussian_pin_cov_t state_gaussian_pin_cov(
         A,
         groups, 
         group_sizes,
         alpha, 
         penalty,
         Eigen::Map<const vec_index_t>(screen_set.data(), screen_set.size()), 
-        Eigen::Map<const vec_index_t>(screen_g1.data(), screen_g1.size()), 
-        Eigen::Map<const vec_index_t>(screen_g2.data(), screen_g2.size()), 
         Eigen::Map<const vec_index_t>(screen_begins.data(), screen_begins.size()), 
         Eigen::Map<const vec_value_t>(screen_vars.data(), screen_vars.size()), 
         screen_transforms,
         Eigen::Map<const vec_index_t>(screen_subset_order.data(), screen_subset_order.size()),
         Eigen::Map<const vec_index_t>(screen_subset_ordered.data(), screen_subset_ordered.size()),
         lmda_path,
         max_active_size, max_iters, 
         tol, 
         rdev_tol,
         newton_tol, newton_max_iters, n_threads,
         rsq,
         Eigen::Map<vec_value_t>(screen_beta.data(), screen_beta.size()), 
         Eigen::Map<vec_value_t>(screen_grad.data(), screen_grad.size()), 
-        Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size())
+        Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size()),
+        active_set_size,
+        active_set
     );
 
     try {
         pin::cov::solve(
             state_gaussian_pin_cov, 
             update_coefficients_f, 
             check_user_interrupt
         );
     } catch(...) {
         load_prev_valid();
         throw;
     }
 
     rsq = state_gaussian_pin_cov.rsq;
+    active_set_size = state_gaussian_pin_cov.active_set_size;
 
     const auto screen_time = Eigen::Map<const util::rowvec_type<double>>(
         state_gaussian_pin_cov.benchmark_screen.data(),
         state_gaussian_pin_cov.benchmark_screen.size()
     ).sum();
     const auto active_time = Eigen::Map<const util::rowvec_type<double>>(
         state_gaussian_pin_cov.benchmark_active.data(),
@@ -263,15 +264,14 @@
         const auto& screen_is_active = state.screen_is_active;
         const auto n_threads = state.n_threads;
         auto& A = *state.A;
         auto& grad = state.grad;
         auto& buffer_p = buffer_pack.buffer_p;
 
         state.lmda = lmda;
-        grad = v;
 
         const auto& beta = state_gaussian_pin_cov.betas.back();
         const Eigen::Map<const vec_index_t> beta_indices(
             beta.innerIndexPtr(),
             beta.nonZeros()
         );
         const Eigen::Map<const vec_value_t> beta_values(
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,14 @@
     const auto y_var = state.y_var;
     const auto& groups = state.groups;
     const auto& group_sizes = state.group_sizes;
     const auto alpha = state.alpha;
     const auto& penalty = state.penalty;
     const auto& weights = state.weights;
     const auto& screen_set = state.screen_set;
-    const auto& screen_g1 = state.screen_g1;
-    const auto& screen_g2 = state.screen_g2;
     const auto& screen_begins = state.screen_begins;
     const auto& screen_vars = state.screen_vars;
     const auto& screen_X_means = state.screen_X_means;
     const auto& screen_transforms = state.screen_transforms;
     const auto intercept = state.intercept;
     const auto max_active_size = state.max_active_size;
     const auto max_iters = state.max_iters;
@@ -105,14 +103,16 @@
     const auto newton_max_iters = state.newton_max_iters;
     const auto n_threads = state.n_threads;
     auto& rsq = state.rsq;
     auto& resid_sum = state.resid_sum;
     auto& resid = state.resid;
     auto& screen_beta = state.screen_beta;
     auto& screen_is_active = state.screen_is_active;
+    auto& active_set_size = state.active_set_size;
+    auto& active_set = state.active_set;
 
     auto& resid_prev = buffer_pack.resid_prev;
     auto& screen_beta_prev = buffer_pack.screen_beta_prev;
     auto& screen_is_active_prev = buffer_pack.screen_is_active_prev;
 
     util::rowvec_type<value_t, 1> lmda_path;
     lmda_path = lmda;
@@ -139,31 +139,32 @@
         y_var,
         groups, 
         group_sizes,
         alpha, 
         penalty,
         weights,
         Eigen::Map<const vec_index_t>(screen_set.data(), screen_set.size()), 
-        Eigen::Map<const vec_index_t>(screen_g1.data(), screen_g1.size()), 
-        Eigen::Map<const vec_index_t>(screen_g2.data(), screen_g2.size()), 
         Eigen::Map<const vec_index_t>(screen_begins.data(), screen_begins.size()), 
         Eigen::Map<const vec_value_t>(screen_vars.data(), screen_vars.size()), 
         Eigen::Map<const vec_value_t>(screen_X_means.data(), screen_X_means.size()), 
         screen_transforms,
         lmda_path,
         intercept, max_active_size, max_iters, 
+        // TODO: still unclear whether we should be max'ing or not.
         // tolerance is relative to the scaling of null deviance and current total weight sum (== 1)
         tol * std::max<value_t>(y_var, 1), 
         adev_tol, ddev_tol, 
         newton_tol, newton_max_iters, n_threads,
         rsq,
         Eigen::Map<vec_value_t>(resid.data(), resid.size()),
         resid_sum,
         Eigen::Map<vec_value_t>(screen_beta.data(), screen_beta.size()), 
-        Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size())
+        Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size()),
+        active_set_size,
+        active_set
     );
 
     try {
         pin::naive::solve(
             state_gaussian_pin_naive, 
             update_coefficients_f, 
             check_user_interrupt
@@ -171,14 +172,15 @@
     } catch(...) {
         load_prev_valid();
         throw;
     }
 
     resid_sum = state_gaussian_pin_naive.resid_sum;
     rsq = state_gaussian_pin_naive.rsq;
+    active_set_size = state_gaussian_pin_naive.active_set_size;
 
     const auto screen_time = Eigen::Map<const util::rowvec_type<double>>(
         state_gaussian_pin_naive.benchmark_screen.data(),
         state_gaussian_pin_naive.benchmark_screen.size()
     ).sum();
     const auto active_time = Eigen::Map<const util::rowvec_type<double>>(
         state_gaussian_pin_naive.benchmark_active.data(),
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pragma once
 #include <adelie_core/util/types.hpp>
 #include <adelie_core/util/macros.hpp>
-#include <adelie_core/bcd.hpp>
+#include <adelie_core/bcd/unconstrained/newton.hpp>
 
 namespace adelie_core {
 namespace solver {
 namespace gaussian {
 namespace pin {
 
 /**
@@ -151,20 +151,23 @@
     size_t max_iters,
     XType& x,
     size_t& iters,
     BufferType& buffer1,
     BufferType& buffer2
 )
 {
-    bcd::newton_abs_solver(
+    bcd::unconstrained::newton_abs_solver(
         L, v, l1, l2, tol, max_iters,
         x, iters, buffer1, buffer2
     );
     if (iters >= max_iters) {
-        throw util::adelie_core_solver_error("Newton-ABS max iteration reached! Try increasing newton_max_iters.");
+        throw util::adelie_core_solver_error(
+            "Newton-ABS max iteration reached! "
+            "Try increasing newton_max_iters."
+        );
     }
 }
 
 template <class ValueType>
 ADELIE_CORE_STRONG_INLINE
 void update_coefficient(
     ValueType& coeff,
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #pragma once
 #include <adelie_core/configs.hpp>
+#include <adelie_core/util/counting_iterator.hpp>
 #include <adelie_core/util/exceptions.hpp>
 #include <adelie_core/util/functional.hpp>
 #include <adelie_core/util/stopwatch.hpp>
 #include <adelie_core/util/eigen/map_sparsevector.hpp>
 #include <adelie_core/solver/solver_gaussian_pin_base.hpp>
 
 namespace adelie_core {
@@ -170,26 +171,24 @@
         );
         vals_seg = ab_diff.segment(active_begins[active_order[i]], group_size);
         idxs_begin += group_size;
         vals_begin += group_size;
     }        
 }
 
-template <class StateType, class G1Iter, class G2Iter,
+template <class StateType, class Iter,
           class ValueType, class BufferPackType,
           class UpdateCoefficientsType,
           class UpdateScreenGradType,
           class AdditionalStepType=util::no_op>
 ADELIE_CORE_STRONG_INLINE
 void coordinate_descent(
     StateType&& state,
-    G1Iter g1_begin,
-    G1Iter g1_end,
-    G2Iter g2_begin,
-    G2Iter g2_end,
+    Iter begin,
+    Iter end,
     size_t lmda_idx,
     ValueType& convg_measure,
     BufferPackType& buffer_pack,
     UpdateCoefficientsType update_coefficients_f,
     UpdateScreenGradType update_screen_grad_f,
     AdditionalStepType additional_step=AdditionalStepType()
 )
@@ -219,107 +218,100 @@
     auto& buffer4 = buffer_pack.buffer4;
     auto& buffer_index = buffer_pack.buffer_index;
 
     const auto l1 = lmda * alpha;
     const auto l2 = lmda * (1-alpha);
 
     convg_measure = 0;
-    // iterate over the groups of size 1
-    for (auto it = g1_begin; it != g1_end; ++it) {
+    for (auto it = begin; it != end; ++it) {
         const auto ss_idx = *it;              // index to screen set
         const auto k = screen_set[ss_idx];    // actual group index
         const auto ss_value_begin = screen_begins[ss_idx]; // value begin index at ss_idx
-        auto& ak = screen_beta[ss_value_begin]; // corresponding beta
-        const auto gk = screen_grad[ss_value_begin]; // corresponding gradient
-        const auto A_kk = screen_vars[ss_value_begin];  // corresponding A diagonal 
-        const auto pk = penalty[k];
-
-        const auto ak_old = ak;
-
-        // update coefficient
-        update_coefficient(
-            ak, A_kk, l1, l2, pk, gk
-        );
+        const auto gsize = group_sizes[k]; // group size  
 
-        if (ak_old == ak) continue;
+        if (gsize == 1) {
+            auto& ak = screen_beta[ss_value_begin]; // corresponding beta
+            const auto gk = screen_grad[ss_value_begin]; // corresponding gradient
+            const auto A_kk = screen_vars[ss_value_begin];  // corresponding A diagonal 
+            const auto pk = penalty[k];
 
-        auto del = ak - ak_old;
+            const auto ak_old = ak;
 
-        // update measure of convergence
-        update_convergence_measure(convg_measure, del, A_kk);
+            update_coefficient(
+                ak, A_kk, l1, l2, pk, gk
+            );
 
-        update_rsq(rsq, del, A_kk, gk);
+            if (ak_old == ak) continue;
 
-        // update gradient 
-        util::rowvec_type<index_t, 1> indices; 
-        util::rowvec_type<value_t, 1> values;
-        indices[0] = groups[k];
-        values[0] = del;
-        update_screen_grad_f(state, buffer_pack, indices, values);
+            auto del = ak - ak_old;
 
-        additional_step(ss_idx);
-    }
-    
-    // iterate over the groups of dynamic size
-    for (auto it = g2_begin; it != g2_end; ++it) {
-        const auto ss_idx = *it;              // index to screen set
-        const auto k = screen_set[ss_idx];    // actual group index
-        const auto ss_value_begin = screen_begins[ss_idx]; // value begin index at ss_idx
-        const auto gsize = group_sizes[k]; // group size  
-        auto ak = screen_beta.segment(ss_value_begin, gsize); // corresponding beta
-        auto gk = screen_grad.segment(ss_value_begin, gsize); // corresponding gradient
-        const auto& Vk = screen_transforms[ss_idx]; // corresponding V in SVD of X_c
-        const auto A_kk = screen_vars.segment(ss_value_begin, gsize);  // corresponding A diagonal 
-        const auto pk = penalty[k];
-
-        auto gk_transformed = buffer3.head(ak.size());
-        gk_transformed.matrix().noalias() = (
-            gk.matrix() * Vk
-        );
+            update_convergence_measure(convg_measure, del, A_kk);
 
-        // save old beta in buffer with transformation
-        auto ak_old = buffer4.head(ak.size());
-        ak_old = ak;
-        auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
-        ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
-        auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
-
-        // update group coefficients
-        size_t iters;
-        gk_transformed += A_kk * ak_old_transformed; 
-        update_coefficients_f(
-            A_kk, gk_transformed, l1 * pk, l2 * pk, 
-            newton_tol, newton_max_iters,
-            ak_transformed, iters, buffer1, buffer2
-        );
-        gk_transformed -= A_kk * ak_old_transformed; 
+            update_rsq(rsq, del, A_kk, gk);
 
-        if ((ak_old_transformed - ak_transformed).matrix().norm() <=  
-            Configs::dbeta_tol * std::sqrt(gsize)) continue;
-        
-        auto del_transformed = buffer1.head(ak.size());
-        del_transformed = ak_transformed - ak_old_transformed;
-
-        update_convergence_measure(convg_measure, del_transformed, A_kk);
-
-        update_rsq(rsq, del_transformed, A_kk, gk_transformed);
-
-        // update new coefficient
-        ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
-
-        // update gradient
-        auto del = buffer2.head(ak.size());
-        del = ak - ak_old;
-        auto indices = buffer_index.head(ak.size());
-        indices = util::rowvec_type<index_t>::LinSpaced(
-            ak.size(), 
-            groups[k], 
-            groups[k] + ak.size() - 1
-        );
-        update_screen_grad_f(state, buffer_pack, indices, del);
+            // update gradient 
+            util::rowvec_type<index_t, 1> indices; 
+            util::rowvec_type<value_t, 1> values;
+            indices[0] = groups[k];
+            values[0] = del;
+            update_screen_grad_f(state, buffer_pack, indices, values);
+
+        } else {
+            auto ak = screen_beta.segment(ss_value_begin, gsize); // corresponding beta
+            auto gk = screen_grad.segment(ss_value_begin, gsize); // corresponding gradient
+            const auto& Vk = screen_transforms[ss_idx]; // corresponding V in SVD of X_c
+            const auto A_kk = screen_vars.segment(ss_value_begin, gsize);  // corresponding A diagonal 
+            const auto pk = penalty[k];
+
+            auto gk_transformed = buffer3.head(ak.size());
+            gk_transformed.matrix().noalias() = (
+                gk.matrix() * Vk
+            );
+
+            // save old beta in buffer with transformation
+            auto ak_old = buffer4.head(ak.size());
+            ak_old = ak;
+            auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
+            ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
+            auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
+
+            // update group coefficients
+            size_t iters;
+            gk_transformed += A_kk * ak_old_transformed; 
+            update_coefficients_f(
+                A_kk, gk_transformed, l1 * pk, l2 * pk, 
+                newton_tol, newton_max_iters,
+                ak_transformed, iters, buffer1, buffer2
+            );
+            gk_transformed -= A_kk * ak_old_transformed; 
+
+            if ((ak_old_transformed - ak_transformed).matrix().norm() <=  
+                Configs::dbeta_tol * std::sqrt(gsize)) continue;
+            
+            auto del_transformed = buffer1.head(ak.size());
+            del_transformed = ak_transformed - ak_old_transformed;
+
+            update_convergence_measure(convg_measure, del_transformed, A_kk);
+
+            update_rsq(rsq, del_transformed, A_kk, gk_transformed);
+
+            // update new coefficient
+            ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
+
+            // update gradient
+            auto del = buffer2.head(ak.size());
+            del = ak - ak_old;
+            auto indices = buffer_index.head(ak.size());
+            indices = util::rowvec_type<index_t>::LinSpaced(
+                ak.size(), 
+                groups[k], 
+                groups[k] + ak.size() - 1
+            );
+            update_screen_grad_f(state, buffer_pack, indices, del);
+        }
 
         additional_step(ss_idx);
     }
 }
 
 /**
  * Applies multiple blockwise coordinate descent on the active set.
@@ -341,46 +333,45 @@
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
 
     const auto& group_sizes = state.group_sizes;
     const auto& screen_set = state.screen_set;
     const auto& screen_begins = state.screen_begins;
+    const auto& active_set_size = state.active_set_size;
     const auto& active_set = state.active_set;
-    const auto& active_g1 = state.active_g1;
-    const auto& active_g2 = state.active_g2;
     const auto& active_begins = state.active_begins;
     const auto& screen_beta = state.screen_beta;
     const auto tol = state.tol;
     const auto max_iters = state.max_iters;
     auto& iters = state.iters;
 
     auto& active_beta_diff = buffer_pack.active_beta_diff;
     auto& active_beta_diff_indices = buffer_pack.active_beta_diff_indices;
     auto& active_beta_diff_ordered = buffer_pack.active_beta_diff_ordered;
 
     // update sizes
     size_t active_beta_size = 0;
-    if (active_set.size()) {
-        const auto last_idx = active_set.size()-1;
+    if (active_set_size) {
+        const auto last_idx = active_set_size-1;
         const auto last_group = screen_set[active_set[last_idx]];
         const auto group_size = group_sizes[last_group];
         active_beta_size = active_begins[last_idx] + group_size;
     }
     active_beta_diff.resize(active_beta_size);
     active_beta_diff_indices.resize(active_beta_size);
     active_beta_diff_ordered.resize(active_beta_size);
 
     Eigen::Map<vec_value_t> ab_diff_view(
         active_beta_diff.data(), 
         active_beta_diff.size()
     );
     
     // save old active beta
-    for (size_t i = 0; i < active_set.size(); ++i) {
+    for (size_t i = 0; i < active_set_size; ++i) {
         const auto ss_idx_group = active_set[i];
         const auto ss_group = screen_set[ss_idx_group];
         const auto ss_group_size = group_sizes[ss_group];
         const auto sb_begin = screen_begins[ss_idx_group];
         const auto sb = screen_beta.segment(sb_begin, ss_group_size);
         const auto ab_begin = active_begins[i];
         auto ab_diff_view_curr = ab_diff_view.segment(ab_begin, ss_group_size);
@@ -389,45 +380,44 @@
     
     while (1) {
         check_user_interrupt();
         ++iters;
         value_t convg_measure;
         coordinate_descent(
             state, 
-            active_g1.data(), active_g1.data() + active_g1.size(),
-            active_g2.data(), active_g2.data() + active_g2.size(),
+            active_set.data(), active_set.data() + active_set_size,
             lmda_idx, 
             convg_measure, 
             buffer_pack,
             update_coefficients_f,
             [](auto& state, auto& buffer_pack, const auto& indices, const auto& values) { 
                 update_screen_grad_active(state, buffer_pack, indices, values); 
             }
         );
         if (convg_measure < tol) break;
         if (iters >= max_iters) throw util::max_cds_error(lmda_idx);
     }
     
     // compute new active beta - old active beta
-    for (size_t i = 0; i < active_set.size(); ++i) {
+    for (size_t i = 0; i < active_set_size; ++i) {
         const auto ss_idx_group = active_set[i];
         const auto ss_group = screen_set[ss_idx_group];
         const auto ss_group_size = group_sizes[ss_group];
         const auto sb_begin = screen_begins[ss_idx_group];
         const auto sb = screen_beta.segment(sb_begin, ss_group_size);
         const auto ab_begin = active_begins[i];
         auto ab_diff_view_curr = ab_diff_view.segment(ab_begin, ss_group_size);
         ab_diff_view_curr = sb - ab_diff_view_curr;
     }
 
     /* update screen gradient for non-active screen variables */
 
     // optimization: if active set is empty or active set is the same as screen set.
     if ((ab_diff_view.size() == 0) ||
-        (static_cast<size_t>(active_set.size()) 
+        (static_cast<size_t>(active_set_size) 
             == static_cast<size_t>(screen_set.size()))) return;
 
     // sparsify ab_diff_view_curr
     Eigen::Map<vec_index_t> ab_diff_indices_view(
         active_beta_diff_indices.data(), 
         active_beta_diff_indices.size()
     );
@@ -465,25 +455,22 @@
     using sp_vec_value_t = typename state_t::sp_vec_value_t;
     using sw_t = util::Stopwatch;
 
     auto& A = *state.A;
     const auto& groups = state.groups;
     const auto& group_sizes = state.group_sizes;
     const auto& screen_set = state.screen_set;
-    const auto& screen_g1 = state.screen_g1;
-    const auto& screen_g2 = state.screen_g2;
     const auto& screen_beta = state.screen_beta;
     const auto& lmda_path = state.lmda_path;
     const auto max_active_size = state.max_active_size;
     const auto tol = state.tol;
     const auto rdev_tol = state.rdev_tol;
     const auto max_iters = state.max_iters;
+    auto& active_set_size = state.active_set_size;
     auto& active_set = state.active_set;
-    auto& active_g1 = state.active_g1;
-    auto& active_g2 = state.active_g2;
     auto& active_begins = state.active_begins;
     auto& active_order = state.active_order;
     auto& screen_is_active = state.screen_is_active;
     auto& betas = state.betas;
     auto& intercepts = state.intercepts;
     auto& rsqs = state.rsqs;
     auto& lmdas = state.lmdas;
@@ -508,100 +495,87 @@
     );    
     // buffer to store final result
     auto& active_beta_indices = buffer_pack.active_beta_indices; 
     auto& active_beta_ordered = buffer_pack.active_beta_ordered;
 
     // compute number of active coefficients
     size_t active_beta_size = 0;
-    if (active_set.size()) {
-        const auto last_idx = active_set.size()-1;
+    if (active_set_size) {
+        const auto last_idx = active_set_size-1;
         const auto last_group = screen_set[active_set[last_idx]];
         const auto group_size = group_sizes[last_group];
         active_beta_size = active_begins[last_idx] + group_size;
     }
     
-    bool lasso_active_called = false;
-
     const auto add_active_set = [&](auto ss_idx) {
         if (!screen_is_active[ss_idx]) {
-            if (active_set.size() >= max_active_size) {
+            if (active_set_size >= max_active_size) {
                 throw util::adelie_core_solver_error("Maximum number of active groups reached.");
             }
 
             screen_is_active[ss_idx] = true;
 
-            active_set.push_back(ss_idx);
-
-            const auto group = screen_set[ss_idx];
-            const auto group_size = group_sizes[group];
-            if (group_size == 1) {
-                active_g1.push_back(ss_idx);
-            } else {
-                active_g2.push_back(ss_idx);
-            }
+            active_set[active_set_size] = ss_idx;
+            ++active_set_size;
         }
     };
 
     const auto lasso_active_and_update = [&](size_t l) {
         solve_active(
             state, 
             l, 
             buffer_pack,
             update_coefficients_f,
             check_user_interrupt
         );
-        lasso_active_called = true;
     };
 
     for (int l = 0; l < lmda_path.size(); ++l) {
         double screen_time = 0;
         double active_time = 0;
 
-        if (lasso_active_called) {
+        while (1) {
             stopwatch.start();
             lasso_active_and_update(l);
             active_time += stopwatch.elapsed();
-        }
 
-        while (1) {
             check_user_interrupt();
             ++iters;
             value_t convg_measure;
-            const auto old_active_size = active_set.size();
+            const auto old_active_size = active_set_size;
             stopwatch.start();
             coordinate_descent(
                 state,
-                screen_g1.data(), screen_g1.data() + screen_g1.size(),
-                screen_g2.data(), screen_g2.data() + screen_g2.size(),
+                util::counting_iterator<size_t>(0),
+                util::counting_iterator<size_t>(screen_set.size()),
                 l, 
                 convg_measure,
                 buffer_pack,
                 update_coefficients_f,
                 [](auto& state, auto& buffer_pack, const auto& indices, const auto& values) { 
                     update_screen_grad_screen(state, buffer_pack, indices, values); 
                 },
                 add_active_set
             );
             screen_time += stopwatch.elapsed();
-            const bool new_active_added = (old_active_size < active_set.size());
+            const bool new_active_added = (old_active_size < active_set_size);
 
             if (new_active_added) {
-                active_begins.resize(active_set.size());
+                active_begins.resize(active_set_size);
                 for (size_t i = old_active_size; i < active_begins.size(); ++i) {
                     active_begins[i] = active_beta_size;
                     const auto curr_group = screen_set[active_set[i]];
                     const auto curr_size = group_sizes[curr_group];
                     active_beta_size += curr_size;
                 }
 
                 // update active_order
                 // NOTE: this is different from naive version.
                 // solve_active() requires active_order so it must be updated.
-                const auto old_active_size = active_order.size();
-                active_order.resize(active_set.size());
+                active_order.resize(active_set_size);
                 std::iota(
                     std::next(active_order.begin(), old_active_size), 
                     active_order.end(), 
                     old_active_size
                 );
                 std::sort(
                     active_order.begin(), active_order.end(),
@@ -611,18 +585,14 @@
                 );
 
                 state::gaussian::pin::cov::update_active_inactive_subset(state);
             }
 
             if (convg_measure < tol) break;
             if (iters >= max_iters) throw util::max_cds_error(l);
-
-            stopwatch.start();
-            lasso_active_and_update(l);
-            active_time += stopwatch.elapsed();
         }
 
         // order the active betas
         active_beta_indices.resize(active_beta_size);
         active_beta_ordered.resize(active_beta_size);
         sparsify_active_beta(
             state,
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #pragma once
 #include <numeric>
 #include <adelie_core/configs.hpp>
+#include <adelie_core/util/counting_iterator.hpp>
 #include <adelie_core/util/exceptions.hpp>
 #include <adelie_core/util/functional.hpp>
 #include <adelie_core/util/stopwatch.hpp>
 #include <adelie_core/util/eigen/map_sparsevector.hpp>
 #include <adelie_core/solver/solver_gaussian_pin_base.hpp>
 #include <adelie_core/matrix/utils.hpp>
 
 namespace adelie_core {
 namespace solver {
 namespace gaussian {
 namespace pin {
 namespace naive {
 
-template <class StateType, class G1Iter, class G2Iter,
+template <class StateType, class Iter,
           class ValueType, class BufferPackType,
           class UpdateCoefficientsType,
           class AdditionalStepType=util::no_op>
 ADELIE_CORE_STRONG_INLINE
 void coordinate_descent(
     StateType&& state,
-    G1Iter g1_begin,
-    G1Iter g1_end,
-    G2Iter g2_begin,
-    G2Iter g2_end,
+    Iter begin,
+    Iter end,
     size_t lmda_idx,
     ValueType& convg_measure,
     BufferPackType& buffer_pack,
     UpdateCoefficientsType update_coefficients_f,
     AdditionalStepType additional_step=AdditionalStepType()
 )
 {
@@ -59,112 +58,103 @@
     auto& buffer3 = buffer_pack.buffer3;
     auto& buffer4 = buffer_pack.buffer4;
 
     const auto l1 = lmda * alpha;
     const auto l2 = lmda * (1-alpha);
 
     convg_measure = 0;
-    // iterate over the groups of size 1
-    for (auto it = g1_begin; it != g1_end; ++it) {
+    for (auto it = begin; it != end; ++it) {
         const auto ss_idx = *it;              // index to screen set
         const auto k = screen_set[ss_idx];    // actual group index
         const auto ss_value_begin = screen_begins[ss_idx]; // value begin index at ss_idx
-        auto& ak = screen_beta[ss_value_begin]; // corresponding beta
-        auto& gk = screen_grad[ss_value_begin]; // corresponding gradient
-        const auto Xk_mean = screen_X_means[ss_value_begin]; // corresponding X[:,k] mean
-        const auto A_kk = screen_vars[ss_value_begin];  // corresponding A diagonal 
-        const auto pk = penalty[k]; // corresponding penalty
+        const auto gsize = group_sizes[k]; // group size  
 
-        const auto ak_old = ak;
+        if (gsize == 1) {
+            auto& ak = screen_beta[ss_value_begin]; // corresponding beta
+            auto& gk = screen_grad[ss_value_begin]; // corresponding gradient
+            const auto Xk_mean = screen_X_means[ss_value_begin]; // corresponding X[:,k] mean
+            const auto A_kk = screen_vars[ss_value_begin];  // corresponding A diagonal 
+            const auto pk = penalty[k]; // corresponding penalty
 
-        // compute gradient
-        gk = X.cmul(groups[k], resid, weights) - Xk_mean * resid_sum * intercept;
+            const auto ak_old = ak;
 
-        update_coefficient(
-            ak, A_kk, l1, l2, pk, gk
-        );
+            // compute gradient
+            gk = X.cmul(groups[k], resid, weights) - Xk_mean * resid_sum * intercept;
 
-        if (ak_old == ak) continue;
+            update_coefficient(
+                ak, A_kk, l1, l2, pk, gk
+            );
 
-        const auto del = ak - ak_old;
+            if (ak_old == ak) continue;
 
-        update_convergence_measure(convg_measure, del, A_kk);
+            const auto del = ak - ak_old;
 
-        update_rsq(rsq, del, A_kk, gk);
+            update_convergence_measure(convg_measure, del, A_kk);
 
-        // update residual 
-        auto dresid = buffer4.head(resid.size());
-        X.ctmul(groups[k], del, dresid);
-        matrix::dvsubi(resid, dresid, n_threads);
-        resid_sum -= Xk_mean * del;
+            update_rsq(rsq, del, A_kk, gk);
 
-        additional_step(ss_idx);
-    }
-    
-    // iterate over the groups of dynamic size
-    for (auto it = g2_begin; it != g2_end; ++it) {
-        const auto ss_idx = *it;              // index to screen set
-        const auto k = screen_set[ss_idx];    // actual group index
-        const auto ss_value_begin = screen_begins[ss_idx]; // value begin index at ss_idx
-        const auto gsize = group_sizes[k]; // group size  
-        auto ak = screen_beta.segment(ss_value_begin, gsize); // corresponding beta
-        auto gk = screen_grad.segment(ss_value_begin, gsize); // corresponding gradient
-        const auto Xk_mean = screen_X_means.segment(ss_value_begin, gsize); // corresponding X[:, g:g+gs] means
-        const auto& Vk = screen_transforms[ss_idx]; // corresponding V in SVD of X_c
-        const auto A_kk = screen_vars.segment(ss_value_begin, gsize);  // corresponding A diagonal 
-        const auto pk = penalty[k]; // corresponding penalty
-
-        // compute current gradient
-        X.bmul(groups[k], gsize, resid, weights, gk);
-        if (intercept) {
-            gk -= resid_sum * Xk_mean;
-        }
+            // update residual 
+            X.ctmul(groups[k], -del, resid);
+            resid_sum -= Xk_mean * del;
+
+        } else {
+            auto ak = screen_beta.segment(ss_value_begin, gsize); // corresponding beta
+            auto gk = screen_grad.segment(ss_value_begin, gsize); // corresponding gradient
+            const auto Xk_mean = screen_X_means.segment(ss_value_begin, gsize); // corresponding X[:, g:g+gs] means
+            const auto& Vk = screen_transforms[ss_idx]; // corresponding V in SVD of X_c
+            const auto A_kk = screen_vars.segment(ss_value_begin, gsize);  // corresponding A diagonal 
+            const auto pk = penalty[k]; // corresponding penalty
+
+            // compute current gradient
+            X.bmul(groups[k], gsize, resid, weights, gk);
+            if (intercept) {
+                gk -= resid_sum * Xk_mean;
+            }
 
-        auto gk_transformed = buffer3.head(ak.size());
-        gk_transformed.matrix().noalias() = (
-            gk.matrix() * Vk
-        );
+            auto gk_transformed = buffer3.head(ak.size());
+            gk_transformed.matrix().noalias() = (
+                gk.matrix() * Vk
+            );
 
-        // save old beta in buffer with transformation
-        auto ak_old = buffer4.head(ak.size());
-        ak_old = ak;
-        auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
-        ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
-        auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
-
-        // update group coefficients
-        size_t iters;
-        gk_transformed += A_kk * ak_old_transformed; 
-        update_coefficients_f(
-            A_kk, gk_transformed, l1 * pk, l2 * pk, 
-            newton_tol, newton_max_iters,
-            ak_transformed, iters, buffer1, buffer2
-        );
-        gk_transformed -= A_kk * ak_old_transformed; 
-        
-        if ((ak_old_transformed - ak_transformed).matrix().norm() <=  
-            Configs::dbeta_tol * std::sqrt(gsize)) continue;
-
-        auto del_transformed = buffer1.head(ak.size());
-        del_transformed = ak_transformed - ak_old_transformed;
-
-        update_convergence_measure(convg_measure, del_transformed, A_kk);
-
-        update_rsq(rsq, del_transformed, A_kk, gk_transformed);
-
-        // update new coefficient
-        ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
-
-        // update residual
-        auto del = buffer1.head(ak.size());
-        del = ak - ak_old;
-        auto dresid = buffer4.head(resid.size());
-        X.btmul(groups[k], gsize, del, dresid);
-        matrix::dvsubi(resid, dresid, n_threads);
-        resid_sum -= (Xk_mean * del).sum();
+            // save old beta in buffer with transformation
+            auto ak_old = buffer4.head(ak.size());
+            ak_old = ak;
+            auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
+            ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
+            auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
+
+            // update group coefficients
+            size_t iters;
+            gk_transformed += A_kk * ak_old_transformed; 
+            update_coefficients_f(
+                A_kk, gk_transformed, l1 * pk, l2 * pk, 
+                newton_tol, newton_max_iters,
+                ak_transformed, iters, buffer1, buffer2
+            );
+            gk_transformed -= A_kk * ak_old_transformed; 
+            
+            if ((ak_old_transformed - ak_transformed).matrix().norm() <=  
+                Configs::dbeta_tol * std::sqrt(gsize)) continue;
+
+            auto del_transformed = buffer1.head(ak.size());
+            del_transformed = ak_transformed - ak_old_transformed;
+
+            update_convergence_measure(convg_measure, del_transformed, A_kk);
+
+            update_rsq(rsq, del_transformed, A_kk, gk_transformed);
+
+            // update new coefficient
+            ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
+
+            // update residual
+            auto del = buffer1.head(ak.size());
+            del = ak_old - ak;
+            X.btmul(groups[k], gsize, del, resid);
+            resid_sum += (Xk_mean * del).sum();
+        }
 
         additional_step(ss_idx);
     }
 }
 
 /**
  * Applies multiple blockwise coordinate descent on the active set.
@@ -181,28 +171,27 @@
     UpdateCoefficientsType update_coefficients_f,
     CUIType check_user_interrupt
 )
 {
     using state_t = std::decay_t<StateType>;
     using value_t = typename state_t::value_t;
 
-    const auto& active_g1 = state.active_g1;
-    const auto& active_g2 = state.active_g2;
+    const auto& active_set_size = state.active_set_size;
+    const auto& active_set = state.active_set;
     const auto tol = state.tol;
     const auto max_iters = state.max_iters;
     auto& iters = state.iters;
 
     while (1) {
         check_user_interrupt();
         ++iters;
         value_t convg_measure;
         coordinate_descent(
             state, 
-            active_g1.data(), active_g1.data() + active_g1.size(),
-            active_g2.data(), active_g2.data() + active_g2.size(),
+            active_set.data(), active_set.data() + active_set_size,
             lmda_idx, 
             convg_measure, 
             buffer_pack,
             update_coefficients_f
         );
         if (convg_measure < tol) break;
         if (iters >= max_iters) throw util::max_cds_error(lmda_idx);
@@ -226,30 +215,27 @@
 
     auto& X = *state.X;
     const auto y_mean = state.y_mean;
     const auto y_var = state.y_var;
     const auto& groups = state.groups;
     const auto& group_sizes = state.group_sizes;
     const auto& screen_set = state.screen_set;
-    const auto& screen_g1 = state.screen_g1;
-    const auto& screen_g2 = state.screen_g2;
     const auto& screen_beta = state.screen_beta;
     const auto& lmda_path = state.lmda_path;
     const auto& rsq = state.rsq;
     const auto& resid_sum = state.resid_sum;
     const auto intercept = state.intercept;
     const auto tol = state.tol;
     const auto max_active_size = state.max_active_size;
     const auto max_iters = state.max_iters;
     const auto adev_tol = state.adev_tol;
     const auto ddev_tol = state.ddev_tol;
     auto& screen_is_active = state.screen_is_active;
+    auto& active_set_size = state.active_set_size;
     auto& active_set = state.active_set;
-    auto& active_g1 = state.active_g1;
-    auto& active_g2 = state.active_g2;
     auto& active_begins = state.active_begins;
     auto& active_order = state.active_order;
     auto& betas = state.betas;
     auto& intercepts = state.intercepts;
     auto& rsqs = state.rsqs;
     auto& lmdas = state.lmdas;
     auto& iters = state.iters;
@@ -271,103 +257,87 @@
     );
     // buffer to store final result
     auto& active_beta_indices = buffer_pack.active_beta_indices; 
     auto& active_beta_ordered = buffer_pack.active_beta_ordered;
 
     // compute number of active coefficients
     size_t active_beta_size = 0;
-    if (active_set.size()) {
-        const auto last_idx = active_set.size()-1;
+    if (active_set_size) {
+        const auto last_idx = active_set_size-1;
         const auto last_group = screen_set[active_set[last_idx]];
         const auto group_size = group_sizes[last_group];
         active_beta_size = active_begins[last_idx] + group_size;
     }
-    
-    bool lasso_active_called = false;
 
     const auto add_active_set = [&](auto ss_idx) {
         if (!screen_is_active[ss_idx]) {
-            if (active_set.size() >= max_active_size) {
+            if (active_set_size >= max_active_size) {
                 throw util::adelie_core_solver_error("Maximum number of active groups reached.");
             }
             screen_is_active[ss_idx] = true;
 
-            active_set.push_back(ss_idx);
-
-            const auto group = screen_set[ss_idx];
-            const auto group_size = group_sizes[group];
-            if (group_size == 1) {
-                active_g1.push_back(ss_idx);
-            } else {
-                active_g2.push_back(ss_idx);
-            }
+            active_set[active_set_size] = ss_idx;
+            ++active_set_size;
         }
     };
 
     const auto lasso_active_and_update = [&](size_t l) {
         solve_active(
             state, 
             l, 
             buffer_pack,
             update_coefficients_f,
             check_user_interrupt
         );
-        lasso_active_called = true;
     };
 
     for (int l = 0; l < lmda_path.size(); ++l) {
         double screen_time = 0;
         double active_time = 0;
 
-        if (lasso_active_called) {
+        while (1) {
             stopwatch.start();
             lasso_active_and_update(l);
             active_time += stopwatch.elapsed();
-        }
 
-        while (1) {
             check_user_interrupt();
             ++iters;
             value_t convg_measure;
-            const auto old_active_size = active_set.size();
+            const auto old_active_size = active_set_size;
             stopwatch.start();
             coordinate_descent(
                 state,
-                screen_g1.data(), screen_g1.data() + screen_g1.size(),
-                screen_g2.data(), screen_g2.data() + screen_g2.size(),
+                util::counting_iterator<size_t>(0),
+                util::counting_iterator<size_t>(screen_set.size()),
                 l, 
                 convg_measure,
                 buffer_pack,
                 update_coefficients_f,
                 add_active_set
             );
             screen_time += stopwatch.elapsed();
-            const bool new_active_added = (old_active_size < active_set.size());
+            const bool new_active_added = (old_active_size < active_set_size);
 
             if (new_active_added) {
-                active_begins.resize(active_set.size());
+                active_begins.resize(active_set_size);
                 for (size_t i = old_active_size; i < active_begins.size(); ++i) {
                     active_begins[i] = active_beta_size;
                     const auto curr_group = screen_set[active_set[i]];
                     const auto curr_size = group_sizes[curr_group];
                     active_beta_size += curr_size;
                 }
             }
 
             if (convg_measure < tol) break;
             if (iters >= max_iters) throw util::max_cds_error(l);
-
-            stopwatch.start();
-            lasso_active_and_update(l);
-            active_time += stopwatch.elapsed();
         }
 
         // update active_order
         const auto old_active_size = active_order.size();
-        active_order.resize(active_set.size());
+        active_order.resize(active_set_size);
         std::iota(
             std::next(active_order.begin(), old_active_size), 
             active_order.end(), 
             old_active_size
         );
         std::sort(
             active_order.begin(), active_order.end(),
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
 
     // make copies since we do not want to mess with the warm-start.
     // this function is only needed to fit intercept-only model and get loss_null.
     value_t beta0 = state.beta0;
     vec_value_t eta = state.eta;
     vec_value_t resid = state.resid;
 
-    auto& irls_weights = buffer_pack.irls_weights;
     auto& irls_y = buffer_pack.irls_y;
     auto& resid_prev = buffer_pack.resid_prev;
     auto& eta_prev = buffer_pack.eta_prev;
     auto& hess = buffer_pack.hess;
 
     size_t irls_it = 0;
 
@@ -133,19 +132,17 @@
 
         /* compute rest of quadratic approximation quantities */
         glm.hessian(eta, resid, hess);
         glm.inv_hessian_gradient(eta, resid, hess, irls_y);
         // hessian is raised whenever <= 0 for well-defined proximal Newton iterations
         hess = hess.max(0) + value_t(Configs::hessian_min) * (hess <= 0).template cast<value_t>();
         const auto hess_sum = hess.sum();
-        irls_weights = hess / hess_sum;
-        irls_y += eta - offsets;
 
         /* fit beta0 */
-        beta0 = (irls_weights * irls_y).sum();
+        beta0 = (hess * (irls_y + eta - offsets)).sum() / hess_sum;
 
         // update eta
         eta.swap(eta_prev);
         eta = beta0 + offsets;
 
         // update resid
         resid_prev.swap(resid);
@@ -195,30 +192,30 @@
     auto& X = *state.X;
     const auto& groups = state.groups;
     const auto& group_sizes = state.group_sizes;
     const auto alpha = state.alpha;
     const auto& penalty = state.penalty;
     const auto& offsets = state.offsets;
     const auto& screen_set = state.screen_set;
-    const auto& screen_g1 = state.screen_g1;
-    const auto& screen_g2 = state.screen_g2;
     const auto& screen_begins = state.screen_begins;
     const auto intercept = state.intercept;
     const auto max_active_size = state.max_active_size;
     const auto irls_max_iters = state.irls_max_iters;
     const auto irls_tol = state.irls_tol;
     const auto max_iters = state.max_iters;
     const auto tol = state.tol;
     const auto newton_tol = state.newton_tol;
     const auto newton_max_iters = state.newton_max_iters;
     const auto n_threads = state.n_threads;
     const auto loss_null = state.loss_null;
     const auto loss_full = state.loss_full;
     auto& screen_beta = state.screen_beta;
     auto& screen_is_active = state.screen_is_active;
+    auto& active_set_size = state.active_set_size;
+    auto& active_set = state.active_set;
     auto& beta0 = state.beta0;
     auto& eta = state.eta;
     auto& resid = state.resid;
 
     const auto& ones = buffer_pack.ones;
     auto& X_means = buffer_pack.X_means;
     auto& screen_X_means = buffer_pack.screen_X_means;
@@ -257,24 +254,24 @@
             throw util::adelie_core_solver_error("Maximum IRLS iterations reached.");
         }
 
         save_prev_valid();
 
         /* compute rest of quadratic approximation quantities */
         glm.hessian(eta, resid, hess);
-        glm.inv_hessian_gradient(eta, resid, hess, irls_y);
+        glm.inv_hessian_gradient(eta, resid, hess, irls_resid);
         // hessian is raised whenever <= 0 for well-defined proximal Newton iterations
         hess = hess.max(0) + value_t(Configs::hessian_min) * (hess <= 0).template cast<value_t>();
         const auto hess_sum = hess.sum();
         irls_weights = hess / hess_sum;
         irls_weights_sqrt = irls_weights.sqrt();
-        irls_y += eta - offsets;
+        irls_y = irls_resid + eta - offsets;
         const auto y_mean = (irls_weights * irls_y).sum();
         const auto y_var = (irls_weights * irls_y.square()).sum() - intercept * y_mean * y_mean;
-        irls_resid = irls_y + offsets - eta + intercept * (beta0 - y_mean);
+        if (intercept) irls_resid += (beta0 - y_mean);
         const auto resid_sum = (irls_weights * irls_resid).sum();
         lmda_path_adjusted = lmda / hess_sum;
         if (std::isinf(lmda_path_adjusted[0])) {
             if (lmda == std::numeric_limits<value_t>::max()) {
                 lmda_path_adjusted = lmda;
             }
             else {
@@ -316,31 +313,32 @@
             y_var,
             groups, 
             group_sizes,
             alpha, 
             penalty,
             irls_weights,
             Eigen::Map<const vec_index_t>(screen_set.data(), screen_set.size()), 
-            Eigen::Map<const vec_index_t>(screen_g1.data(), screen_g1.size()), 
-            Eigen::Map<const vec_index_t>(screen_g2.data(), screen_g2.size()), 
             Eigen::Map<const vec_index_t>(screen_begins.data(), screen_begins.size()), 
             Eigen::Map<const vec_value_t>(screen_vars.data(), screen_vars.size()), 
             Eigen::Map<const vec_value_t>(screen_X_means.data(), screen_X_means.size()), 
             screen_transforms,
             lmda_path_adjusted,
             intercept, max_active_size, max_iters, 
+            // TODO: still unclear whether we should be max'ing or not.
             // tolerance is relative to the scaling of null deviance and current total weight sum
             tol * std::max<value_t>((loss_null - loss_full) / hess_sum, 1), 
             0 /* adev_tol */, 0 /* ddev_tol */,
             newton_tol, newton_max_iters, n_threads,
             0 /* rsq (no need to track) */,
             Eigen::Map<vec_value_t>(irls_resid.data(), irls_resid.size()),
             resid_sum,
             Eigen::Map<vec_value_t>(screen_beta.data(), screen_beta.size()), 
-            Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size())
+            Eigen::Map<vec_safe_bool_t>(screen_is_active.data(), screen_is_active.size()),
+            active_set_size,
+            active_set
         );
         try { 
             gaussian::pin::naive::solve(
                 state_gaussian_pin_naive, 
                 update_coefficients_f, 
                 check_user_interrupt
             );
@@ -355,33 +353,35 @@
             state_gaussian_pin_naive.benchmark_screen.size()
         ).sum();
         active_time += Eigen::Map<const util::rowvec_type<double>>(
             state_gaussian_pin_naive.benchmark_active.data(),
             state_gaussian_pin_naive.benchmark_active.size()
         ).sum();
 
-        // update beta0
+        // update invariants
+        active_set_size = state_gaussian_pin_naive.active_set_size;
         beta0 = state_gaussian_pin_naive.intercepts[0];
 
         // update eta
         eta.swap(eta_prev);
-        eta = irls_y + offsets - irls_resid + intercept * (beta0 - y_mean);
+        eta = irls_y + offsets - irls_resid;
+        if (intercept) eta += beta0 - y_mean;
 
         // update resid
         resid_prev.swap(resid);
         glm.gradient(eta, resid); 
 
         /* check convergence */
         // check directional derivative of gradient (resid) as an approximation
         // to the quadratic loss. 
         const auto& active_set = state_gaussian_pin_naive.active_set;
         const auto& active_begins = state_gaussian_pin_naive.active_begins;
         const auto n_active = (
             (active_begins.size() == 0) ? 1 : (
-                active_begins.back() + group_sizes[screen_set[active_set.back()]]
+                active_begins.back() + group_sizes[screen_set[active_set[active_set_size-1]]]
             )
         );
         if (std::abs(((resid - resid_prev) * (eta - eta_prev)).sum()) <= irls_tol * n_active) {
             return std::make_tuple(
                 std::move(state_gaussian_pin_naive),
                 screen_time,
                 active_time
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/solver/utils.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/solver/utils.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_base.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -109,37 +109,30 @@
 void update_screen_derived_base(
     StateType& state
 )
 {
     const auto& group_sizes = state.group_sizes;
     const auto& screen_set = state.screen_set;
     auto& screen_hashset = state.screen_hashset;
-    auto& screen_g1 = state.screen_g1;
-    auto& screen_g2 = state.screen_g2;
     auto& screen_begins = state.screen_begins;
     auto& screen_beta = state.screen_beta;
     auto& screen_is_active = state.screen_is_active;
 
     /* update screen_hashset */
     const auto old_screen_size = screen_begins.size();
     const auto screen_set_new_begin = std::next(screen_set.begin(), old_screen_size);
     screen_hashset.insert(screen_set_new_begin, screen_set.end());
 
-    /* update screen_g1, screen_g2, screen_begins */
+    /* update screen_begins */
     size_t screen_value_size = (
         (old_screen_size == 0) ? 
         0 : (screen_begins.back() + group_sizes[screen_set[old_screen_size-1]])
     );
     for (size_t i = old_screen_size; i < screen_set.size(); ++i) {
         const auto curr_size = group_sizes[screen_set[i]];
-        if (curr_size == 1) {
-            screen_g1.push_back(i);
-        } else {
-            screen_g2.push_back(i);
-        }
         screen_begins.push_back(screen_value_size);
         screen_value_size += curr_size;
     }
 
     /* update screen_beta */
     screen_beta.resize(screen_value_size, 0);
 
@@ -208,19 +201,19 @@
     /* dynamic states */
     value_t lmda_max;
     vec_value_t lmda_path;
 
     // invariants
     uset_index_t screen_hashset;
     dyn_vec_index_t screen_set; 
-    dyn_vec_index_t screen_g1;
-    dyn_vec_index_t screen_g2;
     dyn_vec_index_t screen_begins;
     dyn_vec_value_t screen_beta;
     dyn_vec_bool_t screen_is_active;
+    size_t active_set_size;
+    vec_index_t active_set;
     value_t lmda;
     vec_value_t grad;
     vec_value_t abs_grad;
 
     // final results
     dyn_vec_sp_vec_t betas;
     dyn_vec_value_t intercepts;
@@ -264,14 +257,16 @@
         bool setup_lmda_max,
         bool setup_lmda_path,
         bool intercept,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         groups(groups.data(), groups.size()),
         group_sizes(group_sizes.data(), group_sizes.size()),
         alpha(alpha),
         penalty(penalty.data(), penalty.size()),
@@ -295,14 +290,16 @@
         intercept(intercept),
         n_threads(n_threads),
         lmda_max(lmda_max),
         lmda_path(lmda_path),
         screen_set(screen_set.data(), screen_set.data() + screen_set.size()),
         screen_beta(screen_beta.data(), screen_beta.data() + screen_beta.size()),
         screen_is_active(screen_is_active.data(), screen_is_active.data() + screen_is_active.size()),
+        active_set_size(active_set_size),
+        active_set(active_set),
         lmda(lmda),
         grad(grad),
         abs_grad(groups.size())
     {
         // sanity checks
         const auto G = groups.size();
         if (group_sizes.size() != G) {
@@ -346,26 +343,34 @@
         }
         if (screen_beta.size() < screen_set.size()) {
             throw util::adelie_core_error(
                 "screen_beta has smaller length than screen_set. "
                 "It is likely screen_beta has been initialized incorrectly."
             );
         }
+        if (active_set_size > G) {
+            throw util::adelie_core_error(
+                "active_set_size must be <= active_set.size()."
+            );
+        }
+        if (active_set.size() != G) {
+            throw util::adelie_core_error(
+                "active_set must have the same length as groups."
+            );
+        }
         if (grad.size() != groups[G-1] + group_sizes[G-1]) {
             throw util::adelie_core_error(
                 "grad.size() != groups[G-1] + group_sizes[G-1]. "
                 "It is likely either grad has the wrong shape, "
                 "or groups/group_sizes have been initialized incorrectly."
             );
         }
 
         /* initialize screen_set derived quantities */
         screen_begins.reserve(screen_set.size());
-        screen_g1.reserve(screen_set.size());
-        screen_g2.reserve(screen_set.size());
         update_screen_derived_base(*this);
 
         /* initialize abs_grad */
         update_abs_grad(*this, lmda);
 
         /* optimize for output storage size */
         const auto n_lmdas = std::max<size_t>(lmda_path.size(), lmda_path_size);
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -203,25 +203,27 @@
         bool early_exit,
         bool setup_lmda_max,
         bool setup_lmda_path,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t rsq,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         base_t(
             groups, group_sizes, alpha, penalty, lmda_path, lmda_max, min_ratio, lmda_path_size,
             max_screen_size, max_active_size,
             pivot_subset_ratio, pivot_subset_min, pivot_slack_ratio, screen_rule, 
             max_iters, tol, 0, 0, newton_tol, newton_max_iters, early_exit, 
             setup_lmda_max, setup_lmda_path, false, n_threads,
-            screen_set, screen_beta, screen_is_active, lmda, grad
+            screen_set, screen_beta, screen_is_active, active_set_size, active_set, lmda, grad
         ),
         v(v.data(), v.size()),
         rdev_tol(rdev_tol),
         A(&A),
         rsq(rsq)
     {
         /* initialize the rest of the screen quantities */
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -220,25 +220,27 @@
         bool setup_lmda_max,
         bool setup_lmda_path,
         bool intercept,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t rsq,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         base_t(
             groups, group_sizes, alpha, penalty, lmda_path, lmda_max, min_ratio, lmda_path_size,
             max_screen_size, max_active_size,
             pivot_subset_ratio, pivot_subset_min, pivot_slack_ratio, screen_rule, 
             max_iters, tol, adev_tol, ddev_tol, newton_tol, newton_max_iters, early_exit, 
             setup_lmda_max, setup_lmda_path, intercept, n_threads,
-            screen_set, screen_beta, screen_is_active, lmda, grad
+            screen_set, screen_beta, screen_is_active, active_set_size, active_set, lmda, grad
         ),
         weights(weights.data(), weights.size()),
         weights_sqrt(weights.sqrt()),
         X_means(X_means.data(), X_means.size()),
         y_mean(y_mean),
         y_var(y_var),
         loss_null(-0.5 * y_mean * y_mean),
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     using index_t = IndexType;
     using bool_t = BoolType;
     using vec_value_t = util::rowvec_type<value_t>;
     using vec_index_t = util::rowvec_type<index_t>;
     using vec_bool_t = util::rowvec_type<bool_t>;
     using sp_vec_value_t = util::sp_vec_type<value_t, Eigen::RowMajor, index_t>;
     using map_vec_value_t = Eigen::Map<vec_value_t>;
+    using map_vec_index_t = Eigen::Map<vec_index_t>;
     using map_vec_bool_t = Eigen::Map<vec_bool_t>;
     using map_cvec_value_t = Eigen::Map<const vec_value_t>;
     using map_cvec_index_t = Eigen::Map<const vec_index_t>;
     using dyn_vec_value_t = std::vector<value_t>;
     using dyn_vec_index_t = std::vector<index_t>;
     using dyn_vec_sp_vec_t = std::vector<sp_vec_value_t>;
     using dyn_vec_vec_value_t = std::vector<vec_value_t>;
@@ -32,16 +33,14 @@
 
     /* static states */
     const map_cvec_index_t groups;
     const map_cvec_index_t group_sizes;
     const value_t alpha;
     const map_cvec_value_t penalty;
     const map_cvec_index_t screen_set;
-    const map_cvec_index_t screen_g1;
-    const map_cvec_index_t screen_g2;
     const map_cvec_index_t screen_begins;
     const map_cvec_value_t screen_vars;
     const dyn_vec_mat_value_t* screen_transforms;
     const map_cvec_value_t lmda_path;
 
     /* configurations */
     const bool intercept;
@@ -54,17 +53,16 @@
     const size_t newton_max_iters;
     const size_t n_threads;
 
     /* dynamic states */
     value_t rsq;
     map_vec_value_t screen_beta;
     map_vec_bool_t screen_is_active;
-    dyn_vec_index_t active_set;
-    dyn_vec_index_t active_g1;
-    dyn_vec_index_t active_g2;
+    size_t active_set_size;
+    map_vec_index_t active_set;
     dyn_vec_index_t active_begins;
     dyn_vec_index_t active_order;
     dyn_vec_sp_vec_t betas;
     dyn_vec_value_t intercepts;
     dyn_vec_value_t rsqs;
     dyn_vec_value_t lmdas;
     size_t iters = 0;
@@ -77,16 +75,14 @@
     
     explicit StateGaussianPinBase(
         const Eigen::Ref<const vec_index_t>& groups, 
         const Eigen::Ref<const vec_index_t>& group_sizes,
         value_t alpha, 
         const Eigen::Ref<const vec_value_t>& penalty,
         const Eigen::Ref<const vec_index_t>& screen_set, 
-        const Eigen::Ref<const vec_index_t>& screen_g1,
-        const Eigen::Ref<const vec_index_t>& screen_g2,
         const Eigen::Ref<const vec_index_t>& screen_begins, 
         const Eigen::Ref<const vec_value_t>& screen_vars,
         const dyn_vec_mat_value_t& screen_transforms,
         const Eigen::Ref<const vec_value_t>& lmda_path, 
         bool intercept,
         size_t max_active_size,
         size_t max_iters,
@@ -94,23 +90,23 @@
         value_t adev_tol,
         value_t ddev_tol,
         value_t newton_tol,
         size_t newton_max_iters,
         size_t n_threads,
         value_t rsq,
         Eigen::Ref<vec_value_t> screen_beta, 
-        Eigen::Ref<vec_bool_t> screen_is_active
+        Eigen::Ref<vec_bool_t> screen_is_active,
+        size_t active_set_size,
+        Eigen::Ref<vec_index_t> active_set
     ): 
         groups(groups.data(), groups.size()),
         group_sizes(group_sizes.data(), group_sizes.size()),
         alpha(alpha),
         penalty(penalty.data(), penalty.size()),
         screen_set(screen_set.data(), screen_set.size()),
-        screen_g1(screen_g1.data(), screen_g1.size()),
-        screen_g2(screen_g2.data(), screen_g2.size()),
         screen_begins(screen_begins.data(), screen_begins.size()),
         screen_vars(screen_vars.data(), screen_vars.size()),
         screen_transforms(&screen_transforms),
         lmda_path(lmda_path.data(), lmda_path.size()),
         intercept(intercept),
         max_active_size(max_active_size),
         max_iters(max_iters),
@@ -118,35 +114,28 @@
         adev_tol(adev_tol),
         ddev_tol(ddev_tol),
         newton_tol(newton_tol),
         newton_max_iters(newton_max_iters),
         n_threads(n_threads),
         rsq(rsq),
         screen_beta(screen_beta.data(), screen_beta.size()),
-        screen_is_active(screen_is_active.data(), screen_is_active.size())
+        screen_is_active(screen_is_active.data(), screen_is_active.size()),
+        active_set_size(active_set_size),
+        active_set(active_set.data(), active_set.size())
     {
-        active_set.reserve(screen_set.size());
-        active_g1.reserve(screen_set.size());
-        active_g2.reserve(screen_set.size());
-        active_begins.reserve(screen_beta.size());
+        active_begins.reserve(screen_set.size());
         int active_begin = 0;
-        for (int i = 0; i < screen_is_active.size(); ++i) {
-            if (!screen_is_active[i]) continue;
-            active_set.push_back(i);
-            int curr_size = group_sizes[screen_set[i]];
-            if (curr_size == 1) {
-                active_g1.push_back(i);
-            } else {
-                active_g2.push_back(i);
-            }
+        for (int i = 0; i < active_set_size; ++i) {
+            const auto ia = active_set[i];
+            const auto curr_size = group_sizes[screen_set[ia]];
             active_begins.push_back(active_begin);
             active_begin += curr_size;
         }
 
-        active_order.resize(active_set.size());
+        active_order.resize(active_set_size);
         std::iota(active_order.begin(), active_order.end(), 0);
         std::sort(
             active_order.begin(),
             active_order.end(),
             [&](auto i, auto j) { 
                 return groups[screen_set[active_set[i]]] < groups[screen_set[active_set[j]]]; 
             }
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -112,16 +112,14 @@
     explicit StateGaussianPinCov(
         matrix_t& A,
         const Eigen::Ref<const vec_index_t>& groups, 
         const Eigen::Ref<const vec_index_t>& group_sizes,
         value_t alpha, 
         const Eigen::Ref<const vec_value_t>& penalty,
         const Eigen::Ref<const vec_index_t>& screen_set, 
-        const Eigen::Ref<const vec_index_t>& screen_g1,
-        const Eigen::Ref<const vec_index_t>& screen_g2,
         const Eigen::Ref<const vec_index_t>& screen_begins, 
         const Eigen::Ref<const vec_value_t>& screen_vars,
         const dyn_vec_mat_value_t& screen_transforms,
         const Eigen::Ref<const vec_index_t>& screen_subset_order,
         const Eigen::Ref<const vec_index_t>& screen_subset_ordered,
         const Eigen::Ref<const vec_value_t>& lmda_path, 
         size_t max_active_size,
@@ -130,21 +128,23 @@
         value_t rdev_tol,
         value_t newton_tol,
         size_t newton_max_iters,
         size_t n_threads,
         value_t rsq,
         Eigen::Ref<vec_value_t> screen_beta, 
         Eigen::Ref<vec_value_t> screen_grad,
-        Eigen::Ref<vec_bool_t> screen_is_active
+        Eigen::Ref<vec_bool_t> screen_is_active,
+        size_t active_set_size,
+        Eigen::Ref<vec_index_t> active_set
     ): 
         base_t(
             groups, group_sizes, alpha, penalty, 
-            screen_set, screen_g1, screen_g2, screen_begins, screen_vars, screen_transforms, lmda_path, 
+            screen_set, screen_begins, screen_vars, screen_transforms, lmda_path, 
             false, max_active_size, max_iters, tol, 0, 0, newton_tol, newton_max_iters, n_threads,
-            rsq, screen_beta, screen_is_active
+            rsq, screen_beta, screen_is_active, active_set_size, active_set
         ),
         screen_subset_order(screen_subset_order.data(), screen_subset_order.size()),
         screen_subset_ordered(screen_subset_ordered.data(), screen_subset_ordered.size()),
         rdev_tol(rdev_tol),
         A(&A),
         screen_grad(screen_grad.data(), screen_grad.size()),
         screen_is_active_subset(screen_grad.size())
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -58,16 +58,14 @@
         value_t y_var,
         const Eigen::Ref<const vec_index_t>& groups, 
         const Eigen::Ref<const vec_index_t>& group_sizes,
         value_t alpha, 
         const Eigen::Ref<const vec_value_t>& penalty,
         const Eigen::Ref<const vec_value_t>& weights,
         const Eigen::Ref<const vec_index_t>& screen_set, 
-        const Eigen::Ref<const vec_index_t>& screen_g1,
-        const Eigen::Ref<const vec_index_t>& screen_g2,
         const Eigen::Ref<const vec_index_t>& screen_begins, 
         const Eigen::Ref<const vec_value_t>& screen_vars,
         const Eigen::Ref<const vec_value_t>& screen_X_means,
         const dyn_vec_mat_value_t& screen_transforms,
         const Eigen::Ref<const vec_value_t>& lmda_path, 
         bool intercept,
         size_t max_active_size,
@@ -78,21 +76,23 @@
         value_t newton_tol,
         size_t newton_max_iters,
         size_t n_threads,
         value_t rsq,
         Eigen::Ref<vec_value_t> resid,
         value_t resid_sum,
         Eigen::Ref<vec_value_t> screen_beta, 
-        Eigen::Ref<vec_bool_t> screen_is_active
+        Eigen::Ref<vec_bool_t> screen_is_active,
+        size_t active_set_size,
+        Eigen::Ref<vec_index_t> active_set
     ): 
         base_t(
             groups, group_sizes, alpha, penalty,
-            screen_set, screen_g1, screen_g2, screen_begins, screen_vars, screen_transforms, lmda_path, 
+            screen_set, screen_begins, screen_vars, screen_transforms, lmda_path, 
             intercept, max_active_size, max_iters, tol, adev_tol, ddev_tol, newton_tol, newton_max_iters, n_threads,
-            rsq, screen_beta, screen_is_active
+            rsq, screen_beta, screen_is_active, active_set_size, active_set
         ),
         weights(weights.data(), weights.size()),
         y_mean(y_mean),
         y_var(y_var),
         screen_X_means(screen_X_means.data(), screen_X_means.size()),
         X(&X),
         resid(resid.data(), resid.size()),
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_glm_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_glm_naive.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -143,25 +143,27 @@
         bool setup_lmda_max,
         bool setup_lmda_path,
         bool intercept,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t beta0,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         base_t(
             groups, group_sizes, alpha, penalty, lmda_path, lmda_max, min_ratio, lmda_path_size,
             max_screen_size, max_active_size,
             pivot_subset_ratio, pivot_subset_min, pivot_slack_ratio, screen_rule, 
             max_iters, tol, adev_tol, ddev_tol, newton_tol, newton_max_iters, early_exit, 
             setup_lmda_max, setup_lmda_path, intercept, n_threads,
-            screen_set, screen_beta, screen_is_active, lmda, grad
+            screen_set, screen_beta, screen_is_active, active_set_size, active_set, lmda, grad
         ),
         loss_full(loss_full),
         offsets(offsets.data(), offsets.size()),
         irls_max_iters(irls_max_iters),
         irls_tol(irls_tol),
         setup_loss_null(setup_loss_null),
         loss_null(loss_null),
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -82,26 +82,28 @@
         bool setup_lmda_max,
         bool setup_lmda_path,
         bool intercept,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t rsq,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         base_t(
             X, X_means, y_mean, y_var, resid, resid_sum,
             groups, group_sizes, alpha, penalty, weights, lmda_path, lmda_max, min_ratio, lmda_path_size,
             max_screen_size, max_active_size,
             pivot_subset_ratio, pivot_subset_min, pivot_slack_ratio, screen_rule, 
             max_iters, tol, adev_tol, ddev_tol, 
             newton_tol, newton_max_iters, early_exit, setup_lmda_max, setup_lmda_path, intercept, n_threads,
-            screen_set, screen_beta, screen_is_active, rsq, lmda, grad
+            screen_set, screen_beta, screen_is_active, active_set_size, active_set, rsq, lmda, grad
         ),
         group_type(util::convert_multi_group(group_type)),
         n_classes(n_classes),
         multi_intercept(multi_intercept)
     {}
 };
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -84,25 +84,27 @@
         bool setup_lmda_max,
         bool setup_lmda_path,
         bool intercept,
         size_t n_threads,
         const Eigen::Ref<const vec_index_t>& screen_set,
         const Eigen::Ref<const vec_value_t>& screen_beta,
         const Eigen::Ref<const vec_bool_t>& screen_is_active,
+        size_t active_set_size,
+        const Eigen::Ref<const vec_index_t>& active_set,
         value_t beta0,
         value_t lmda,
         const Eigen::Ref<const vec_value_t>& grad
     ):
         base_t(
             X, eta, resid, groups, group_sizes, alpha, penalty, offsets, lmda_path, 
             loss_null, loss_full, lmda_max, min_ratio, lmda_path_size, max_screen_size, max_active_size,
             pivot_subset_ratio, pivot_subset_min, pivot_slack_ratio, screen_rule, 
             irls_max_iters, irls_tol, max_iters, tol, adev_tol, ddev_tol,
             newton_tol, newton_max_iters, early_exit, setup_loss_null, setup_lmda_max, setup_lmda_path, intercept, n_threads,
-            screen_set, screen_beta, screen_is_active, beta0, lmda, grad
+            screen_set, screen_beta, screen_is_active, active_set_size, active_set, beta0, lmda, grad
         ),
         group_type(util::convert_multi_group(group_type)),
         n_classes(n_classes),
         multi_intercept(multi_intercept)
     {}
 };
```

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/algorithm.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/exceptions.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/format.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/format.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/macros.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/macros.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/stopwatch.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/stopwatch.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/tqdm.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/tqdm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/include/adelie_core/util/types.hpp` & `adelie-1.1.29/adelie/src/include/adelie_core/util/types.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,26 @@
 enum class read_mode_type
 {
     _file,
     _mmap,
     _auto
 };
 
+enum class impute_method_type
+{
+    _mean,
+    _user
+};
+
+enum class operator_type
+{
+    _eq,
+    _add
+};
+
 inline screen_rule_type convert_screen_rule(
     const std::string& rule
 )
 {
     if (rule == "strong") return screen_rule_type::_strong;
     if (rule == "pivot") return screen_rule_type::_pivot;
     throw util::adelie_core_error("Invalid screen rule type: " + rule);
@@ -101,9 +113,18 @@
 {
     if (read_mode == "file") return read_mode_type::_file;
     if (read_mode == "mmap") return read_mode_type::_mmap;
     if (read_mode == "auto") return read_mode_type::_auto;
     throw util::adelie_core_error("Invalid read mode type: " + read_mode);
 }
 
+inline impute_method_type convert_impute_method(
+    const std::string& impute_method
+)
+{
+    if (impute_method == "mean") return impute_method_type::_mean;
+    if (impute_method == "user") return impute_method_type::_user;
+    throw util::adelie_core_error("Invalid read mode type: " + impute_method);
+}
+
 } // namespace util
 } // namespace adelie_core
```

### Comparing `adelie-1.1.28/adelie/src/matrix.cpp` & `adelie-1.1.29/adelie/src/matrix.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     using cref_mvec_value_t = Eigen::Ref<const Eigen::Matrix<value_t, 1, Eigen::Dynamic, Eigen::RowMajor>>;
 
     m.def("dvaddi", ad::matrix::dvaddi<ref_vec_value_t, cref_vec_value_t>);
     m.def("dmmeq", ad::matrix::dmmeq<ref_rowarr_value_t, cref_rowarr_value_t>);
     m.def("dvzero", ad::matrix::dvzero<ref_vec_value_t>);
     m.def("ddot", ad::matrix::ddot<cref_mvec_value_t, cref_mvec_value_t, ref_vec_value_t>);
     m.def("dax", ad::matrix::dax<value_t, cref_vec_value_t, ref_vec_value_t>);
-    m.def("dgemv", ad::matrix::dgemv<cref_colmat_value_t, cref_mvec_value_t, ref_rowmat_value_t, ref_mvec_value_t>);
+    m.def("dgemv", ad::matrix::dgemv<ad::util::operator_type::_eq, cref_colmat_value_t, cref_mvec_value_t, ref_rowmat_value_t, ref_mvec_value_t>);
 }
 
 template <class T>
 class PyMatrixCovBase: public ad::matrix::MatrixCovBase<T>
 {
     using base_t = ad::matrix::MatrixCovBase<T>;
 public:
@@ -256,23 +256,24 @@
         w : (n,) np.ndarray
             Vector of weights.
         )delimiter")
         .def("ctmul", &internal_t::ctmul, R"delimiter(
         Column vector-scalar multiplication.
 
         Computes the vector-scalar multiplication ``v * X[:,j]`` for a column ``j``.
+        The result is *incremented* into the output vector.
 
         Parameters
         ----------
         j : int
             Column index.
         v : float
             Scalar to multiply with the ``j`` th column.
         out : (n,) np.ndarray
-            Vector to store in-place the result.
+            Vector to increment in-place the result.
         )delimiter")
         .def("bmul", &internal_t::bmul, R"delimiter(
         Column block matrix-vector multiplication.
 
         Computes the matrix-vector multiplication ``(v * w).T @ X[:, j:j+q]``.
 
         Parameters
@@ -289,25 +290,26 @@
             Vector to store in-place the result.
         )delimiter")
         .def("btmul", &internal_t::btmul, R"delimiter(
         Column block matrix transpose-vector multiplication.
 
         Computes the matrix-vector multiplication
         ``v.T @ X[:, j:j+q].T``.
+        The result is *incremented* into the output vector.
 
         Parameters
         ----------
         j : int
             Column index.
         q : int
             Number of columns.
         v : (q,) np.ndarray
             Vector to multiply with the block matrix.
         out : (n,) np.ndarray
-            Vector to store in-place the result.
+            Vector to increment in-place the result.
         )delimiter")
         .def("mul", &internal_t::mul, R"delimiter(
         Matrix-vector multiplication.
 
         Computes the matrix-vector multiplication
         ``(v * w).T @ X``.
```

### Comparing `adelie-1.1.28/adelie/src/solver.cpp` & `adelie-1.1.29/adelie/src/solver.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/state.cpp` & `adelie-1.1.29/adelie/src/state.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,14 @@
         )delimiter")
         .def(py::init<
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&, 
-            const Eigen::Ref<const vec_index_t>&,
-            const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_value_t>&,
             const dyn_vec_mat_value_t&,
             const Eigen::Ref<const vec_value_t>&, 
             bool,
             size_t,
             size_t,
@@ -103,23 +101,23 @@
             value_t,
             value_t,
             value_t,
             size_t,
             size_t,
             value_t,
             Eigen::Ref<vec_value_t>,
-            Eigen::Ref<vec_bool_t>
+            Eigen::Ref<vec_bool_t>,
+            size_t,
+            Eigen::Ref<vec_index_t>
         >(),
             py::arg("groups").noconvert(),
             py::arg("group_sizes").noconvert(),
             py::arg("alpha"),
             py::arg("penalty").noconvert(),
             py::arg("screen_set").noconvert(),
-            py::arg("screen_g1").noconvert(),
-            py::arg("screen_g2").noconvert(),
             py::arg("screen_begins").noconvert(),
             py::arg("screen_vars").noconvert(),
             py::arg("screen_transforms").noconvert(),
             py::arg("lmda_path").noconvert(),
             py::arg("intercept"),
             py::arg("max_active_size"),
             py::arg("max_iters"),
@@ -127,15 +125,17 @@
             py::arg("adev_tol"),
             py::arg("ddev_tol"),
             py::arg("newton_tol"),
             py::arg("newton_max_iters"),
             py::arg("n_threads"),
             py::arg("rsq"),
             py::arg("screen_beta").noconvert(),
-            py::arg("screen_is_active").noconvert()
+            py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert()
         )
         .def_readonly("groups", &state_t::groups, R"delimiter(
         List of starting indices to each group where `G` is the number of groups.
         ``groups[i]`` is the starting index of the ``i`` th group. 
         )delimiter")
         .def_readonly("group_sizes", &state_t::group_sizes, R"delimiter(
         List of group sizes corresponding to each element in ``groups``.
@@ -147,24 +147,14 @@
         .def_readonly("penalty", &state_t::penalty, R"delimiter(
         Penalty factor for each group in the same order as ``groups``.
         )delimiter")
         .def_readonly("screen_set", &state_t::screen_set, R"delimiter(
         List of indices into ``groups`` that correspond to the screen groups.
         ``screen_set[i]`` is ``i`` th screen group.
         )delimiter")
-        .def_readonly("screen_g1", &state_t::screen_g1, R"delimiter(
-        List of indices into ``screen_set`` that correspond to groups of size ``1``.
-        ``screen_set[screen_g1[i]]`` is the ``i`` th screen group of size ``1``
-        such that ``group_sizes[screen_set[screen_g1[i]]]`` is ``1``.
-        )delimiter")
-        .def_readonly("screen_g2", &state_t::screen_g2, R"delimiter(
-        List of indices into ``screen_set`` that correspond to groups more than size ``1``.
-        ``screen_set[screen_g2[i]]`` is the ``i`` th screen group of size more than ``1``
-        such that ``group_sizes[screen_set[screen_g2[i]]]`` is more than ``1``.
-        )delimiter")
         .def_readonly("screen_begins", &state_t::screen_begins, R"delimiter(
         List of indices that index a corresponding list of values for each screen group.
         ``screen_begins[i]`` is the starting index corresponding to the ``i`` th screen group.
         From this index, reading ``group_sizes[screen_set[i]]`` number of elements
         will grab values corresponding to the full ``i`` th screen group block.
         )delimiter")
         .def_readonly("lmda_path", &state_t::lmda_path, R"delimiter(
@@ -205,14 +195,19 @@
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         )delimiter")
         .def_readonly("screen_is_active", &state_t::screen_is_active, R"delimiter(
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
         )delimiter")
+        .def_readonly("active_set_size", &state_t::active_set_size, R"delimiter(
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+        )delimiter")
         .def_property_readonly("active_set", [](const state_t& s) {
             return Eigen::Map<const ad::util::rowvec_type<index_t>>(
                 s.active_set.data(),
                 s.active_set.size()
             );
         }, R"delimiter(
         List of indices into ``screen_set`` that correspond to active groups.
@@ -221,30 +216,14 @@
         that is, for every ``i`` th active group, 
         ``screen_beta[b:b+p] == 0`` where 
         ``j = active_set[i]``,
         ``k = screen_set[j]``,
         ``b = screen_begins[j]``,
         and ``p = group_sizes[k]``.
         )delimiter")
-        .def_property_readonly("active_g1", [](const state_t& s) {
-            return Eigen::Map<const ad::util::rowvec_type<index_t>>(
-                s.active_g1.data(),
-                s.active_g1.size()
-            );
-        }, R"delimiter(
-        Subset of ``active_set`` that correspond to groups of size ``1``.
-        )delimiter")
-        .def_property_readonly("active_g2", [](const state_t& s) {
-            return Eigen::Map<const ad::util::rowvec_type<index_t>>(
-                s.active_g2.data(),
-                s.active_g2.size()
-            );
-        }, R"delimiter(
-        Subset of ``active_set`` that correspond to groups of size more than ``1``.
-        )delimiter")
         .def_property_readonly("active_begins", [](const state_t& s) {
             return Eigen::Map<const ad::util::rowvec_type<index_t>>(
                 s.active_begins.data(),
                 s.active_begins.size()
             );
         }, R"delimiter(
         List of indices that index a corresponding list of values for each active group.
@@ -333,16 +312,14 @@
             value_t,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&, 
-            const Eigen::Ref<const vec_index_t>&,
-            const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
             const dyn_vec_mat_value_t&,
             const Eigen::Ref<const vec_value_t>&, 
             bool,
             size_t,
@@ -353,27 +330,27 @@
             value_t,
             size_t,
             size_t,
             value_t,
             Eigen::Ref<vec_value_t>,
             value_t,
             Eigen::Ref<vec_value_t>, 
-            Eigen::Ref<vec_bool_t>
+            Eigen::Ref<vec_bool_t>,
+            size_t,
+            Eigen::Ref<vec_index_t>
         >(),
             py::arg("X"),
             py::arg("y_mean"),
             py::arg("y_var"),
             py::arg("groups").noconvert(),
             py::arg("group_sizes").noconvert(),
             py::arg("alpha"),
             py::arg("penalty").noconvert(),
             py::arg("weights").noconvert(),
             py::arg("screen_set").noconvert(),
-            py::arg("screen_g1").noconvert(),
-            py::arg("screen_g2").noconvert(),
             py::arg("screen_begins").noconvert(),
             py::arg("screen_vars").noconvert(),
             py::arg("screen_X_means").noconvert(),
             py::arg("screen_transforms").noconvert(),
             py::arg("lmda_path").noconvert(),
             py::arg("intercept"),
             py::arg("max_active_size"),
@@ -384,15 +361,17 @@
             py::arg("newton_tol"),
             py::arg("newton_max_iters"),
             py::arg("n_threads"),
             py::arg("rsq"),
             py::arg("resid").noconvert(),
             py::arg("resid_sum"),
             py::arg("screen_beta").noconvert(),
-            py::arg("screen_is_active").noconvert()
+            py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_readonly("weights", &state_t::weights, R"delimiter(
         Observation weights :math:`W`.
         )delimiter")
         .def_readonly("y_mean", &state_t::y_mean, R"delimiter(
         Mean of the response vector :math:`y` (weighted by :math:`W`),
@@ -478,16 +457,14 @@
         .def(py::init<
             matrix_t&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&, 
-            const Eigen::Ref<const vec_index_t>&,
-            const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_value_t>&,
             const dyn_vec_mat_value_t&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_value_t>&, 
             size_t,
@@ -496,24 +473,24 @@
             value_t,
             value_t,
             size_t,
             size_t,
             value_t,
             Eigen::Ref<vec_value_t>, 
             Eigen::Ref<vec_value_t>,
-            Eigen::Ref<vec_bool_t>
+            Eigen::Ref<vec_bool_t>,
+            size_t,
+            Eigen::Ref<vec_index_t>
         >(),
             py::arg("A"),
             py::arg("groups").noconvert(),
             py::arg("group_sizes").noconvert(),
             py::arg("alpha"),
             py::arg("penalty").noconvert(),
             py::arg("screen_set").noconvert(),
-            py::arg("screen_g1").noconvert(),
-            py::arg("screen_g2").noconvert(),
             py::arg("screen_begins").noconvert(),
             py::arg("screen_vars").noconvert(),
             py::arg("screen_transforms").noconvert(),
             py::arg("screen_subset_order").noconvert(),
             py::arg("screen_subset_ordered").noconvert(),
             py::arg("lmda_path").noconvert(),
             py::arg("max_active_size"),
@@ -522,15 +499,17 @@
             py::arg("rdev_tol"),
             py::arg("newton_tol"),
             py::arg("newton_max_iters"),
             py::arg("n_threads"),
             py::arg("rsq"),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_grad").noconvert(),
-            py::arg("screen_is_active").noconvert()
+            py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_readonly("screen_subset_order", &state_t::screen_subset_order, R"delimiter(
         Ordering such that ``screen_subset`` is sorted in ascending order where
         ``screen_subset`` is a list of column indices into :math:`A`
         in the implicit ordering of ``screen_grad``.
         ``screen_subset[screen_subset_order[i]]`` is the ``i`` th
@@ -592,14 +571,15 @@
 // ========================================================================
 
 template <class ValueType>
 void state_base(py::module_& m, const char* name)
 {
     using state_t = ad::state::StateBase<ValueType>;
     using value_t = typename state_t::value_t;
+    using index_t = typename state_t::index_t;
     using safe_bool_t = typename state_t::safe_bool_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t>(m, name, R"delimiter(
         Base core state class for all non-pin methods.
         )delimiter") 
@@ -628,14 +608,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("groups").noconvert(),
             py::arg("group_sizes").noconvert(),
             py::arg("alpha"),
             py::arg("penalty").noconvert(),
@@ -659,14 +641,16 @@
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("intercept"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def_readonly("groups", &state_t::groups, R"delimiter(
         List of starting indices to each group where `G` is the number of groups.
         ``groups[i]`` is the starting index of the ``i`` th group. 
         )delimiter")
@@ -763,28 +747,14 @@
         )delimiter")
         .def_property_readonly("screen_set", [](const state_t& s) {
             return Eigen::Map<const vec_index_t>(s.screen_set.data(), s.screen_set.size());
         }, R"delimiter(
         List of indices into ``groups`` that correspond to the screen groups.
         ``screen_set[i]`` is ``i`` th screen group.
         )delimiter")
-        .def_property_readonly("screen_g1", [](const state_t& s) {
-            return Eigen::Map<const vec_index_t>(s.screen_g1.data(), s.screen_g1.size());
-        }, R"delimiter(
-        List of indices into ``screen_set`` that correspond to groups of size ``1``.
-        ``screen_set[screen_g1[i]]`` is the ``i`` th screen group of size ``1``
-        such that ``group_sizes[screen_set[screen_g1[i]]]`` is ``1``.
-        )delimiter")
-        .def_property_readonly("screen_g2", [](const state_t& s) {
-            return Eigen::Map<const vec_index_t>(s.screen_g2.data(), s.screen_g2.size());
-        }, R"delimiter(
-        List of indices into ``screen_set`` that correspond to groups more than size ``1``.
-        ``screen_set[screen_g2[i]]`` is the ``i`` th screen group of size more than ``1``
-        such that ``group_sizes[screen_set[screen_g2[i]]]`` is more than ``1``.
-        )delimiter")
         .def_property_readonly("screen_begins", [](const state_t& s) {
             return Eigen::Map<const vec_index_t>(s.screen_begins.data(), s.screen_begins.size());
         }, R"delimiter(
         List of indices that index a corresponding list of values for each screen group.
         ``screen_begins[i]`` is the starting index corresponding to the ``i`` th screen group.
         From this index, reading ``group_sizes[screen_set[i]]`` number of elements
         will grab values corresponding to the full ``i`` th screen group block.
@@ -804,14 +774,35 @@
                 s.screen_is_active.data(), 
                 s.screen_is_active.size()
             );
         }, R"delimiter(
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
         )delimiter")
+        .def_readonly("active_set_size", &state_t::active_set_size, R"delimiter(
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+        )delimiter")
+        .def_property_readonly("active_set", [](const state_t& s) {
+            return Eigen::Map<const ad::util::rowvec_type<index_t>>(
+                s.active_set.data(),
+                s.active_set.size()
+            );
+        }, R"delimiter(
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
+        )delimiter")
         .def_readonly("lmda", &state_t::lmda, R"delimiter(
         The last regularization parameter that was attempted to be solved.
         )delimiter")
         .def_readonly("grad", &state_t::grad, R"delimiter(
         The full gradient :math:`-X^\top \nabla \ell(\eta)`.
         )delimiter")
         .def_readonly("abs_grad", &state_t::abs_grad, R"delimiter(
@@ -967,14 +958,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("X"),
             py::arg("X_means").noconvert(),
             py::arg("y_mean"),
@@ -1006,14 +999,16 @@
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("intercept"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("rsq"),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_readonly("weights", &state_t::weights, R"delimiter(
         Observation weights :math:`W`.
@@ -1137,14 +1132,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("group_type"),
             py::arg("n_classes"),
             py::arg("multi_intercept"),
@@ -1179,14 +1176,16 @@
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("intercept"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("rsq"),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_property_readonly("group_type", [](const state_t& s) -> std::string {
             switch (s.group_type) {
@@ -1274,14 +1273,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("A"),
             py::arg("v").noconvert(),
             py::arg("groups").noconvert(),
@@ -1306,14 +1307,16 @@
             py::arg("early_exit"),
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("rsq"),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_readonly("v", &state_t::v, R"delimiter(
         Linear term.
@@ -1428,14 +1431,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("X"),
             py::arg("eta").noconvert(),
             py::arg("resid").noconvert(),
@@ -1469,14 +1474,16 @@
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("intercept"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("beta0"),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_readonly("offsets", &state_t::offsets, R"delimiter(
         Observation offsets :math:`\eta^0`.
@@ -1585,14 +1592,16 @@
             bool,
             bool,
             bool,
             size_t,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_value_t>&, 
             const Eigen::Ref<const vec_bool_t>&,
+            size_t,
+            const Eigen::Ref<const vec_index_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>& 
         >(),
             py::arg("group_type"),
             py::arg("n_classes"),
             py::arg("multi_intercept"),
@@ -1629,14 +1638,16 @@
             py::arg("setup_lmda_max"),
             py::arg("setup_lmda_path"),
             py::arg("intercept"),
             py::arg("n_threads"),
             py::arg("screen_set").noconvert(),
             py::arg("screen_beta").noconvert(),
             py::arg("screen_is_active").noconvert(),
+            py::arg("active_set_size"),
+            py::arg("active_set").noconvert(),
             py::arg("beta0"),
             py::arg("lmda"),
             py::arg("grad").noconvert()
         )
         .def(py::init([](const state_t& s) { return new state_t(s); }))
         .def_property_readonly("group_type", [](const state_t& s) -> std::string {
             switch (s.group_type) {
@@ -1674,18 +1685,18 @@
         ;
 }
 
 void register_state(py::module_& m)
 {
     state_gaussian_pin_base<double>(m, "StateGaussianPinBase64");
     state_gaussian_pin_base<float>(m, "StateGaussianPinBase32");
-    state_gaussian_pin_naive<ad::matrix::MatrixNaiveBase<double>>(m, "StateGaussianPinNaive64");
-    state_gaussian_pin_naive<ad::matrix::MatrixNaiveBase<float>>(m, "StateGaussianPinNaive32");
     state_gaussian_pin_cov<ad::matrix::MatrixCovBase<double>>(m, "StateGaussianPinCov64");
     state_gaussian_pin_cov<ad::matrix::MatrixCovBase<float>>(m, "StateGaussianPinCov32");
+    state_gaussian_pin_naive<ad::matrix::MatrixNaiveBase<double>>(m, "StateGaussianPinNaive64");
+    state_gaussian_pin_naive<ad::matrix::MatrixNaiveBase<float>>(m, "StateGaussianPinNaive32");
 
     state_base<double>(m, "StateBase64");
     state_base<float>(m, "StateBase32");
     state_gaussian_cov<ad::matrix::MatrixCovBase<double>>(m, "StateGaussianCov64");
     state_gaussian_cov<ad::matrix::MatrixCovBase<float>>(m, "StateGaussianCov32");
     state_gaussian_naive<ad::matrix::MatrixNaiveBase<double>>(m, "StateGaussianNaive64");
     state_gaussian_naive<ad::matrix::MatrixNaiveBase<float>>(m, "StateGaussianNaive32");
```

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Cholesky` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/CholmodSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Core` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Core`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigenvalues` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Geometry` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Householder` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Jacobi` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/KLUSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/LU` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/LU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/MetisSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/OrderingMethods` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PaStiXSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PardisoSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QR` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/QR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SPQRSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SVD` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Sparse` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCholesky` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCore` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseLU` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseQR` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdDeque` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdList` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdVector` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SuperLUSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/UmfPackSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/BVH` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/FFT` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Splines` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h` & `adelie-1.1.29/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/adelie/state.py` & `adelie-1.1.29/adelie/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 
 def deduce_states(
     *,
     group_sizes: np.ndarray,
     screen_set: np.ndarray,
 ):
     S = screen_set.shape[0]
-    screen_g1 = np.arange(S)[group_sizes[screen_set] == 1]
-    screen_g2 = np.arange(S)[group_sizes[screen_set] > 1]
     screen_begins = np.cumsum(
         np.concatenate([[0], group_sizes[screen_set]]),
         dtype=int,
     )[:-1]
     return (
-        screen_g1,
-        screen_g2,
         screen_begins,
     )
 
 
 class base:
     """Base wrapper state class.
 
@@ -154,32 +150,20 @@
         )
         self._check(
             np.allclose(self.groups, np.cumsum(np.concatenate([[0], self.group_sizes]))[:-1]),
             "check groups and group_sizes consistency",
             method, logger,
         )
 
-        # ================ alpha check ====================
-        self._check(
-            (self.alpha >= 0) and (self.alpha <= 1),
-            "check alpha is in [0, 1]",
-            method, logger,
-        )
-
         # ================ penalty check ====================
         self._check(
             np.all(self.penalty >= 0),
             "check penalty is non-negative",
             method, logger,
         )
-        self._check(
-            len(self.penalty) == G,
-            "check penalty and groups have same length",
-            method, logger,
-        )
 
         # ================ screen_set check ====================
         self._check(
             np.all((0 <= self.screen_set) & (self.screen_set < G)),
             "check screen_set is a subset of [0, G)",
             method, logger,
         )
@@ -191,63 +175,14 @@
         self._check(
             self.screen_set.dtype == np.dtype("int"),
             "check screen_set dtype is int",
             method, logger,
         )
         S = len(self.screen_set)
 
-        # ================ screen_g1 check ====================
-        self._check(
-            np.all((0 <= self.screen_g1) & (self.screen_g1 < S)),
-            "check screen_g1 is in [0, S)",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g1) == len(np.unique(self.screen_g1)),
-            "check screen_g1 has unique values",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.screen_g1]] == 1),
-            "check screen_g1 has group sizes of 1",
-            method, logger,
-        )
-        self._check(
-            self.screen_g1.dtype == np.dtype("int"),
-            "check screen_g1 dtype is int",
-            method, logger,
-        )
-
-        # ================ screen_g2 check ====================
-        self._check(
-            np.all((0 <= self.screen_g2) & (self.screen_g2 < S)),
-            "check screen_g2 is in [0, S)",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g2) == len(np.unique(self.screen_g2)),
-            "check screen_g2 has unique values",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.screen_g2]] > 1),
-            "check screen_g2 has group sizes more than 1",
-            method, logger,
-        )
-        self._check(
-            self.screen_g2.dtype == np.dtype("int"),
-            "check screen_g2 dtype is int",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g1) + len(self.screen_g2) == S,
-            "check screen_g1 and screen_g2 combined have length S",
-            method, logger,
-        )
-
         # ================ screen_begins check ====================
         expected = np.cumsum(
             np.concatenate([[0], self.group_sizes[self.screen_set]], dtype=int)
         )
         WS = expected[-1]
         expected = expected[:-1]
         self._check(
@@ -286,145 +221,48 @@
             "check lmda_path is non-negative",
             method, logger,
         )
         # if not sorted in decreasing order
         if np.any(self.lmda_path != np.sort(self.lmda_path)[::-1]):
             logger.warning("lmda_path are not sorted in decreasing order")
 
-        # ================ max_iters check ====================
-        self._check(
-            self.max_iters >= 0,
-            "check max_iters >= 0",
-            method, logger,
-        )
-
-        # ================ tol check ====================
-        self._check(
-            self.tol >= 0,
-            "check tol >= 0",
-            method, logger,
-        )
-
-        # ================ newton_tol check ====================
-        self._check(
-            self.newton_tol >= 0,
-            "check newton_tol >= 0",
-            method, logger,
-        )
-
-        # ================ newton_max_iters check ====================
-        self._check(
-            self.newton_max_iters >= 0,
-            "check newton_max_iters >= 0",
-            method, logger,
-        )
-
-        # ================ newton_max_iters check ====================
-        self._check(
-            self.n_threads > 0,
-            "check n_threads > 0",
-            method, logger,
-        )
-
-        # ================ rsq check ====================
-        self._check(
-            self.rsq >= 0,
-            "check rsq >= 0",
-            method, logger,
-        )
-
-        # ================ screen_beta check ====================
-        self._check(
-            len(self.screen_beta) == WS,
-            "check screen_beta size",
-            method, logger,
-        )
-
         # ================ screen_is_active check ====================
+        active_set = self.active_set[:self.active_set_size]
         self._check(
-            np.all(np.arange(S)[self.screen_is_active] == np.sort(self.active_set)),
+            np.all(np.arange(S)[self.screen_is_active] == np.sort(active_set)),
             "check screen_is_active is consistent with active_set",
             method, logger,
         )
         self._check(
             self.screen_is_active.dtype == np.dtype("bool"),
             "check screen_is_active dtype is bool",
             method, logger,
         )
 
         # ================ active_set check ====================
         self._check(
-            np.all((0 <= self.active_set) & (self.active_set < S)),
+            np.all((0 <= active_set) & (active_set < S)),
             "check active_set is in [0, S)",
             method, logger,
         )
         self._check(
-            len(self.active_set) == len(np.unique(self.active_set)),
+            len(active_set) == len(np.unique(active_set)),
             "check active_set is unique",
             method, logger,
         )
         self._check(
-            self.active_set.dtype == np.dtype("int"),
+            active_set.dtype == np.dtype("int"),
             "check active_set dtype is int",
             method, logger,
         )
-        A = len(self.active_set)
-
-        # ================ active_g1 check ====================
-        self._check(
-            set(self.active_g1) <= set(self.active_set),
-            "check active_g1 subset of active_set",
-            method, logger,
-        )
-        self._check(
-            len(self.active_g1) == len(np.unique(self.active_g1)),
-            "check active_g1 is unique",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.active_g1]] == 1),
-            "check active_g1 has group sizes of 1",
-            method, logger,
-        )
-        self._check(
-            self.active_g1.dtype == np.dtype("int"),
-            "check active_g1 dtype is int",
-            method, logger,
-        )
-
-        # ================ active_g2 check ====================
-        self._check(
-            set(self.active_g2) <= set(self.active_set),
-            "check active_g2 subset of active_set",
-            method, logger,
-        )
-        self._check(
-            len(self.active_g2) == len(np.unique(self.active_g2)),
-            "check active_g2 is unique",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.active_g2]] > 1),
-            "check active_g2 has group sizes more than 1",
-            method, logger,
-        )
-        self._check(
-            self.active_g2.dtype == np.dtype("int"),
-            "check active_g2 dtype is int",
-            method, logger,
-        )
-        self._check(
-            len(self.active_g1) + len(self.active_g2) == A,
-            "check active_g1 and active_g2 combined have length A",
-            method, logger,
-        )
+        A = len(active_set)
 
         # ================ active_begins check ====================
         expected = np.cumsum(
-            np.concatenate([[0], self.group_sizes[self.screen_set[self.active_set]]], dtype=int)
+            np.concatenate([[0], self.group_sizes[self.screen_set[active_set]]], dtype=int)
         )
         WA = expected[-1]
         expected = expected[:-1]
         self._check(
             np.all(self.active_begins == expected),
             "check active_begins is [0, g1, g2, ...] where gi is the group size of (i-1)th active group.",
             method, logger,
@@ -432,15 +270,15 @@
         self._check(
             self.active_begins.dtype == np.dtype("int"),
             "check active_begins dtype is int",
             method, logger,
         )
 
         # ================ active_order check ====================
-        actual = self.groups[self.screen_set[self.active_set[self.active_order]]]
+        actual = self.groups[self.screen_set[active_set[self.active_order]]]
         self._check(
             np.all(actual == np.sort(actual)),
             "check active_order orders active_set such that groups is ordered",
             method, logger,
         )
         self._check(
             self.active_order.dtype == np.dtype("int"),
@@ -516,14 +354,16 @@
     weights: np.ndarray,
     screen_set: np.ndarray,
     lmda_path: np.ndarray,
     rsq: float,
     resid: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     intercept: bool =True,
     max_active_size: int =None,
     max_iters: int =int(1e5),
     tol: float =1e-7,
     adev_tol: float =0.9,
     ddev_tol: float =1e-4,
     newton_tol: float =1e-12,
@@ -584,17 +424,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     intercept : bool, optional
         ``True`` to fit with intercept.
         Default is ``True``.
     max_active_size : int, optional
         Maximum number of active groups allowed.
         The function will return a valid state and guarantees to have active set size
         less than or equal to ``max_active_size``.
@@ -673,18 +527,17 @@
             self._weights = np.array(weights, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             # dynamic inputs require a copy to not modify user's inputs
             self._resid = np.copy(resid).astype(dtype)
             self._screen_beta = np.copy(screen_beta).astype(dtype)
             self._screen_is_active = np.copy(screen_is_active).astype(bool)
+            self._active_set = np.copy(active_set).astype(int)
 
             (
-                self._screen_g1,
-                self._screen_g2,
                 self._screen_begins,
             ) = deduce_states(
                 group_sizes=group_sizes,
                 screen_set=screen_set,
             )
 
             self._max_active_size = (
@@ -706,16 +559,16 @@
                 g, gs = groups[i], group_sizes[i]
                 XiTXi = np.empty((gs, gs), dtype=dtype, order="F")
                 buffer = np.empty((n, gs), dtype=dtype, order="F")
                 X.cov(g, gs, sqrt_weights, XiTXi, buffer)
                 Xi_means = X_means[g:g+gs]
                 if intercept:
                     XiTXi -= Xi_means[:, None] @ Xi_means[None]
-                vars, v = np.linalg.eigh(XiTXi)
-                self._screen_vars.append(np.maximum(vars, 0))
+                evars, v = np.linalg.eigh(XiTXi)
+                self._screen_vars.append(np.maximum(evars, 0))
                 self._screen_X_means.append(Xi_means)
                 self._screen_transforms.append(np.array(v, copy=False, dtype=dtype, order="F"))
             self._screen_vars = np.concatenate(self._screen_vars, dtype=dtype)
             self._screen_X_means = np.concatenate(self._screen_X_means, dtype=dtype)
             vecmat_type = (
                 core.VectorMatrix64
                 if dtype == np.float64 else
@@ -734,16 +587,14 @@
                 y_var=y_var,
                 groups=self._groups,
                 group_sizes=self._group_sizes,
                 alpha=alpha,
                 penalty=self._penalty,
                 weights=self._weights,
                 screen_set=self._screen_set,
-                screen_g1=self._screen_g1,
-                screen_g2=self._screen_g2,
                 screen_begins=self._screen_begins,
                 screen_vars=self._screen_vars,
                 screen_X_means=self._screen_X_means,
                 screen_transforms=self._screen_transforms,
                 lmda_path=self._lmda_path,
                 intercept=intercept,
                 max_active_size=self._max_active_size,
@@ -755,14 +606,16 @@
                 newton_max_iters=newton_max_iters,
                 n_threads=n_threads,
                 rsq=rsq,
                 resid=self._resid,
                 resid_sum=resid_sum,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
             obj = base.create_from_core(
                 cls, state, core_state, _gaussian_pin_naive, core_base,
             )
@@ -796,14 +649,16 @@
     penalty: np.ndarray,
     screen_set: np.ndarray,
     lmda_path: np.ndarray,
     rsq: float,
     screen_beta: np.ndarray,
     screen_grad: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     max_active_size: int =None,
     max_iters: int =int(1e5),
     tol: float =1e-7,
     rdev_tol: float =1e-4,
     newton_tol: float =1e-12,
     newton_max_iters: int =1000,
     n_threads: int =1,
@@ -855,17 +710,31 @@
     screen_grad : (ws,) np.ndarray
         Gradient :math:`X_{c,k}^\\top W (y_c-X_c\\beta)` on the screen groups :math:`k` where :math:`\\beta` is given by ``screen_beta``.
         ``screen_grad[b:b+p]`` is the gradient for the ``i`` th screen group
         where 
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     max_active_size : int, optional
         Maximum number of active groups allowed.
         The function will return a valid state and guarantees to have active set size
         less than or equal to ``max_active_size``.
         If ``None``, it will be set to the total number of groups.
         Default is ``None``.
     max_iters : int, optional
@@ -936,18 +805,17 @@
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             # dynamic inputs require a copy to not modify user's inputs
             self._screen_beta = np.copy(screen_beta).astype(dtype)
             self._screen_grad = np.copy(screen_grad).astype(dtype)
             self._screen_is_active = np.copy(screen_is_active).astype(bool)
+            self._active_set = np.copy(active_set).astype(int)
 
             (
-                self._screen_g1,
-                self._screen_g2,
                 self._screen_begins,
             ) = deduce_states(
                 group_sizes=group_sizes,
                 screen_set=screen_set,
             )
 
             self._max_active_size = (
@@ -984,16 +852,14 @@
                 self,
                 A=A,
                 groups=self._groups,
                 group_sizes=self._group_sizes,
                 alpha=alpha,
                 penalty=self._penalty,
                 screen_set=self._screen_set,
-                screen_g1=self._screen_g1,
-                screen_g2=self._screen_g2,
                 screen_begins=self._screen_begins,
                 screen_vars=self._screen_vars,
                 screen_transforms=self._screen_transforms,
                 screen_subset_order=self._screen_subset_order,
                 screen_subset_ordered=self._screen_subset_ordered,
                 lmda_path=self._lmda_path,
                 max_active_size=self._max_active_size,
@@ -1003,14 +869,16 @@
                 newton_tol=newton_tol,
                 newton_max_iters=newton_max_iters,
                 n_threads=n_threads,
                 rsq=rsq,
                 screen_beta=self._screen_beta,
                 screen_grad=self._screen_grad,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
             obj = base.create_from_core(
                 cls, state, core_state, _gaussian_pin_cov, core_base,
             )
@@ -1152,14 +1020,16 @@
     groups: np.ndarray,
     group_sizes: np.ndarray,
     alpha: float,
     penalty: np.ndarray,
     screen_set: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     rsq: float,
     lmda: float,
     grad: np.ndarray,
     lmda_path: np.ndarray =None,
     lmda_max: float =None,
     max_iters: int =int(1e5),
     tol: float =1e-7,
@@ -1175,16 +1045,14 @@
     max_active_size: int =None,
     pivot_subset_ratio: float =0.1,
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
 ):
     """Creates a gaussian, covariance method state object.
 
-    Define the following quantities:
-
     Parameters
     ----------
     A : (p, p) Union[adelie.matrix.MatrixCovBase64, adelie.matrix.MatrixCovBase32]
         Positive semi-definite matrix.
         It is typically one of the matrices defined in ``adelie.matrix`` submodule.
     v : (p,) np.ndarray
         Linear term.
@@ -1209,17 +1077,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     rsq : float
         The change in unnormalized :math:`R^2` given by 
         :math:`2(\\ell(\\beta_{\\mathrm{old}}) - \\ell(\\beta_{\\mathrm{curr}}))`.
         Usually, :math:`\\beta_{\\mathrm{old}} = 0` 
         and :math:`\\beta_{\\mathrm{curr}}` is given by ``screen_beta``.
     lmda : float
         The last regularization parameter that was attempted to be solved.
@@ -1355,14 +1237,15 @@
             self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._grad = np.array(grad, copy=False, dtype=dtype)
+            self._active_set = np.array(active_set, copy=False, dtype=int)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 A=self._A,
                 v=self._v,
@@ -1388,14 +1271,16 @@
                 early_exit=early_exit,
                 setup_lmda_max=setup_lmda_max,
                 setup_lmda_path=setup_lmda_path,
                 n_threads=n_threads,
                 screen_set=self._screen_set,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
                 rsq=rsq,
                 lmda=lmda,
                 grad=self._grad,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
@@ -1460,21 +1345,14 @@
         )
         self._check(
             np.allclose(self.groups, np.cumsum(np.concatenate([[0], self.group_sizes]))[:-1]),
             "check groups and group_sizes consistency",
             method, logger,
         )
 
-        # ================ alpha check ====================
-        self._check(
-            (self.alpha >= 0) and (self.alpha <= 1),
-            "check alpha is in [0, 1]",
-            method, logger,
-        )
-
         # ================ penalty check ====================
         self._check(
             np.all(self.penalty >= 0),
             "check penalty is non-negative",
             method, logger,
         )
         self._check(
@@ -1509,63 +1387,14 @@
         self._check(
             self.screen_set.dtype == np.dtype("int"),
             "check screen_set dtype is int",
             method, logger,
         )
         S = len(self.screen_set)
 
-        # ================ screen_g1 check ====================
-        self._check(
-            np.all((0 <= self.screen_g1) & (self.screen_g1 < S)),
-            "check screen_g1 is in [0, S)",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g1) == len(np.unique(self.screen_g1)),
-            "check screen_g1 has unique values",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.screen_g1]] == 1),
-            "check screen_g1 has group sizes of 1",
-            method, logger,
-        )
-        self._check(
-            self.screen_g1.dtype == np.dtype("int"),
-            "check screen_g1 dtype is int",
-            method, logger,
-        )
-
-        # ================ screen_g2 check ====================
-        self._check(
-            np.all((0 <= self.screen_g2) & (self.screen_g2 < S)),
-            "check screen_g2 is in [0, S)",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g2) == len(np.unique(self.screen_g2)),
-            "check screen_g2 has unique values",
-            method, logger,
-        )
-        self._check(
-            np.all(self.group_sizes[self.screen_set[self.screen_g2]] > 1),
-            "check screen_g2 has group sizes more than 1",
-            method, logger,
-        )
-        self._check(
-            self.screen_g2.dtype == np.dtype("int"),
-            "check screen_g2 dtype is int",
-            method, logger,
-        )
-        self._check(
-            len(self.screen_g1) + len(self.screen_g2) == S,
-            "check screen_g1 and screen_g2 combined have length S",
-            method, logger,
-        )
-
         # ================ screen_begins check ====================
         expected = np.cumsum(
             np.concatenate([[0], self.group_sizes[self.screen_set]], dtype=int)
         )
         WS = expected[-1]
         expected = expected[:-1]
         self._check(
@@ -1603,24 +1432,22 @@
             np.all(self.screen_is_active[nnz_idxs]),
             "check screen_is_active is only active on non-zeros of screen_beta",
             method, logger,
         )
 
         # ================ rsq check ====================
         screen_indices = []
-        tmp = np.empty(n)
         Xbeta = np.zeros(n)
         for g, gs, b in zip(
             self.groups[self.screen_set], 
             self.group_sizes[self.screen_set],
             self.screen_begins,
         ):
             screen_indices.append(np.arange(g, g + gs))
-            self.X.btmul(g, gs, self.screen_beta[b:b+gs], tmp)
-            Xbeta += tmp
+            self.X.btmul(g, gs, self.screen_beta[b:b+gs], Xbeta)
 
         if len(screen_indices) == 0:
             screen_indices = np.array(screen_indices, dtype=int)
         else:
             screen_indices = np.concatenate(screen_indices, dtype=int)
 
         resid = yc - Xbeta
@@ -1725,14 +1552,16 @@
     alpha: float,
     penalty: np.ndarray,
     weights: np.ndarray,
     offsets: np.ndarray,
     screen_set: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     rsq: float,
     lmda: float,
     grad: np.ndarray,
     lmda_path: np.ndarray =None,
     lmda_max: float =None,
     max_iters: int =int(1e5),
     tol: float =1e-7,
@@ -1812,17 +1641,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     rsq : float
         The change in unnormalized :math:`R^2` given by 
         :math:`\\|y_c-X_c\\beta_{\\mathrm{old}}\\|_{W}^2 - \\|y_c-X_c\\beta_{\\mathrm{curr}}\\|_{W}^2`.
         Usually, :math:`\\beta_{\\mathrm{old}} = 0` 
         and :math:`\\beta_{\\mathrm{curr}}` is given by ``screen_beta``.
     lmda : float
         The last regularization parameter that was attempted to be solved.
@@ -1966,14 +1809,15 @@
             self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._offsets = np.array(offsets, copy=False, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
+            self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 X=self._X,
@@ -2007,14 +1851,16 @@
                 setup_lmda_max=setup_lmda_max,
                 setup_lmda_path=setup_lmda_path,
                 intercept=intercept,
                 n_threads=n_threads,
                 screen_set=self._screen_set,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
                 rsq=rsq,
                 lmda=lmda,
                 grad=self._grad,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
@@ -2040,14 +1886,16 @@
     alpha: float,
     penalty: np.ndarray,
     weights: np.ndarray,
     offsets: np.ndarray,
     screen_set: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     rsq: float,
     lmda: float,
     grad: np.ndarray,
     lmda_path: np.ndarray =None,
     lmda_max: float =None,
     max_iters: int =int(1e5),
     tol: float =1e-7,
@@ -2126,17 +1974,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     rsq : float
         The change in unnormalized :math:`R^2` given by 
         :math:`\\|\\tilde{y}-\\tilde{X}\\beta_{\\mathrm{old}}\\|_{\\tilde{W}}^2 - \\|\\tilde{y}-\\tilde{X}\\beta_{\\mathrm{curr}}\\|_{\\tilde{W}}^2`.
         Usually, :math:`\\beta_{\\mathrm{old}} = 0` 
         and :math:`\\beta_{\\mathrm{curr}}` is given by ``screen_beta``.
     lmda : float
         The last regularization parameter that was attempted to be solved.
@@ -2294,14 +2156,15 @@
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._weights_expanded = np.repeat(self._glm.weights, repeats=n_classes) / n_classes
             self._offsets = np.array(offsets, copy=False, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
+            self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 group_type=group_type,
@@ -2342,14 +2205,16 @@
                 setup_lmda_max=setup_lmda_max,
                 setup_lmda_path=setup_lmda_path,
                 intercept=False,
                 n_threads=n_threads,
                 screen_set=self._screen_set,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
                 rsq=rsq,
                 lmda=lmda,
                 grad=self._grad,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
@@ -2383,14 +2248,16 @@
     group_sizes: np.ndarray,
     alpha: float,
     penalty: np.ndarray,
     offsets: np.ndarray,
     screen_set: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     beta0: float,
     lmda: float,
     grad: np.ndarray,
     eta: np.ndarray,
     resid: np.ndarray,
     loss_full: float,
     loss_null: float =None,
@@ -2449,17 +2316,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     beta0 : float
         The current intercept value.
         The value can be arbitrary but it is recommended to be close to the solution at ``lmda``.
     lmda : float
         The last regularization parameter that was attempted to be solved.
     grad : (p,) np.ndarray
         The full gradient :math:`-X^\\top \\nabla \\ell(\\eta)` where
@@ -2627,14 +2508,15 @@
             self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._offsets = np.array(offsets, copy=False, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
+            self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 X=self._X,
@@ -2668,14 +2550,16 @@
                 setup_lmda_max=setup_lmda_max,
                 setup_lmda_path=setup_lmda_path,
                 intercept=intercept,
                 n_threads=n_threads,
                 screen_set=self._screen_set,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
                 beta0=beta0,
                 lmda=lmda,
                 grad=self._grad,
                 eta=eta,
                 resid=resid,
             )
 
@@ -2697,14 +2581,16 @@
     group_sizes: np.ndarray,
     alpha: float,
     penalty: np.ndarray,
     offsets: np.ndarray,
     screen_set: np.ndarray,
     screen_beta: np.ndarray,
     screen_is_active: np.ndarray,
+    active_set_size: int,
+    active_set: np.ndarray,
     lmda: float,
     grad: np.ndarray,
     eta: np.ndarray,
     resid: np.ndarray,
     loss_full: float,
     loss_null: float =None,
     lmda_path: np.ndarray =None,
@@ -2771,17 +2657,31 @@
         Coefficient vector on the screen set.
         ``screen_beta[b:b+p]`` is the coefficient for the ``i`` th screen group 
         where
         ``k = screen_set[i]``,
         ``b = screen_begins[i]``,
         and ``p = group_sizes[k]``.
         The values can be arbitrary but it is recommended to be close to the solution at ``lmda``.
-    screen_is_active : (a,) np.ndarray
+    screen_is_active : (s,) np.ndarray
         Boolean vector that indicates whether each screen group in ``groups`` is active or not.
         ``screen_is_active[i]`` is ``True`` if and only if ``screen_set[i]`` is active.
+    active_set_size : int
+        Number of active groups.
+        ``active_set[i]`` is only well-defined
+        for ``i`` in the range ``[0, active_set_size)``.
+    active_set : (G,) np.ndarray
+        List of indices into ``screen_set`` that correspond to active groups.
+        ``screen_set[active_set[i]]`` is the ``i`` th active group.
+        An active group is one with non-zero coefficient block,
+        that is, for every ``i`` th active group, 
+        ``screen_beta[b:b+p] == 0`` where 
+        ``j = active_set[i]``,
+        ``k = screen_set[j]``,
+        ``b = screen_begins[j]``,
+        and ``p = group_sizes[k]``.
     lmda : float
         The last regularization parameter that was attempted to be solved.
     grad : ((p+intercept)*K,) np.ndarray
         The full gradient :math:`-\\tilde{X}^\\top \\nabla \\ell(\\tilde{\\eta})` where
         :math:`\\tilde{\\eta}` is given by ``eta``.
     eta : (n*K,) np.ndarray
         The natural parameter :math:`\\tilde{\\eta} = \\tilde{X}\\beta + \\tilde{\\eta}^0`
@@ -2959,14 +2859,15 @@
             self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
             self._penalty = np.array(penalty, copy=False, dtype=dtype)
             self._offsets = np.array(offsets, copy=False, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
+            self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 group_type=group_type,
@@ -3003,14 +2904,16 @@
                 setup_lmda_max=setup_lmda_max,
                 setup_lmda_path=setup_lmda_path,
                 intercept=False,
                 n_threads=n_threads,
                 screen_set=self._screen_set,
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
+                active_set_size=active_set_size,
+                active_set=self._active_set,
                 beta0=0,
                 lmda=lmda,
                 grad=self._grad,
                 eta=eta,
                 resid=resid,
             )
```

### Comparing `adelie-1.1.28/adelie.egg-info/PKG-INFO` & `adelie-1.1.29/adelie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.28
+Version: 1.1.29
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.28/adelie.egg-info/SOURCES.txt` & `adelie-1.1.29/adelie.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,34 @@
 adelie/src/decl.hpp
 adelie/src/glm.cpp
 adelie/src/io.cpp
 adelie/src/matrix.cpp
 adelie/src/optimization.cpp
 adelie/src/solver.cpp
 adelie/src/state.cpp
-adelie/src/include/adelie_core/bcd.hpp
 adelie/src/include/adelie_core/configs.hpp
+adelie/src/include/adelie_core/bcd/utils.hpp
+adelie/src/include/adelie_core/bcd/constrained/admm.hpp
+adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp
+adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp
+adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp
+adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp
+adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp
 adelie/src/include/adelie_core/glm/glm_base.hpp
 adelie/src/include/adelie_core/glm/glm_binomial.hpp
 adelie/src/include/adelie_core/glm/glm_cox.hpp
 adelie/src/include/adelie_core/glm/glm_gaussian.hpp
 adelie/src/include/adelie_core/glm/glm_multibase.hpp
 adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
 adelie/src/include/adelie_core/glm/glm_multinomial.hpp
 adelie/src/include/adelie_core/glm/glm_poisson.hpp
 adelie/src/include/adelie_core/io/io_snp_base.hpp
 adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
 adelie/src/include/adelie_core/io/io_snp_unphased.hpp
+adelie/src/include/adelie_core/io/utils.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
@@ -57,14 +64,15 @@
 adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
 adelie/src/include/adelie_core/matrix/utils.hpp
 adelie/src/include/adelie_core/optimization/bisect.hpp
 adelie/src/include/adelie_core/optimization/newton.hpp
+adelie/src/include/adelie_core/optimization/nnls.hpp
 adelie/src/include/adelie_core/optimization/search_pivot.hpp
 adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
 adelie/src/include/adelie_core/solver/solver_base.hpp
 adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
 adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
 adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
 adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
@@ -79,14 +87,15 @@
 adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
 adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
 adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
 adelie/src/include/adelie_core/state/state_glm_naive.hpp
 adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
 adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
 adelie/src/include/adelie_core/util/algorithm.hpp
+adelie/src/include/adelie_core/util/counting_iterator.hpp
 adelie/src/include/adelie_core/util/exceptions.hpp
 adelie/src/include/adelie_core/util/format.hpp
 adelie/src/include/adelie_core/util/functional.hpp
 adelie/src/include/adelie_core/util/macros.hpp
 adelie/src/include/adelie_core/util/queue.hpp
 adelie/src/include/adelie_core/util/stopwatch.hpp
 adelie/src/include/adelie_core/util/tqdm.hpp
```

### Comparing `adelie-1.1.28/pyproject.toml` & `adelie-1.1.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adelie-1.1.28/setup.py` & `adelie-1.1.29/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             "adelie/src/include",
             "adelie/src/third_party/eigen3",
         ],
         extra_compile_args=extra_compile_args,
         extra_link_args=extra_link_args,
         runtime_library_dirs=runtime_library_dirs,
         libraries=libraries,
-        cxx_std=17, # TODO: changed from 14 to 17 just because of tqdm
+        cxx_std=17,
     ),
 ]
 
 setup(
     name='adelie', 
     version=__version__,
     description='A fast, flexible package for group elastic net.',
```

