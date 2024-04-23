# Comparing `tmp/stardist-0.8.5.tar.gz` & `tmp/stardist-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stardist-0.8.5.tar", last modified: Fri Jul 21 14:51:55 2023, max compression
+gzip compressed data, was "stardist-0.9.0.tar", last modified: Tue Apr 23 22:13:57 2024, max compression
```

## Comparing `stardist-0.8.5.tar` & `stardist-0.9.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-21 14:51:44.000000 stardist-0.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 14:51:44.000000 stardist-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-21 14:51:55.934452 stardist-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-07-21 14:51:44.000000 stardist-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 14:51:44.000000 stardist-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 14:51:55.934452 stardist-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-21 14:51:44.000000 stardist-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/big.py
--rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/bioimageio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)    35505 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/histo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/img2d.tif
--rw-r--r--   0 runner    (1001) docker     (123)   138925 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/img3d.tif
--rw-r--r--   0 runner    (1001) docker     (123)   524544 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/mask2d.tif
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/data/images/mask3d.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/geom2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/geometry/geom3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/kernels/stardist2d.cl
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/kernels/stardist3d.cl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.914451 stardist-0.8.5/stardist/lib/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/clipper/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   142184 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/clipper/clipper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/nanoflann/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/nanoflann/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    73558 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/nanoflann/nanoflann.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.922452 stardist-0.8.5/stardist/lib/external/qhull_src/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/Announce.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist/lib/external/qhull_src/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.926452 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (123)    73854 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    45785 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    75784 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   140430 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    66346 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    56702 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   208318 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   145471 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    47472 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (123)    34690 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    47157 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_lib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/stardist3d_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/test_lib3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55742 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27280 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/model2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    32215 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/models/model3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/rays3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/sample_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.934452 stardist-0.8.5/stardist/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/predict2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/scripts/predict3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:51:44.000000 stardist-0.8.5/stardist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:51:55.918451 stardist-0.8.5/stardist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 14:51:55.000000 stardist-0.8.5/stardist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.337786 stardist-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-23 22:13:49.000000 stardist-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:13:49.000000 stardist-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21476 2024-04-23 22:13:57.337786 stardist-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-23 22:13:49.000000 stardist-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 22:13:49.000000 stardist-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 22:13:57.337786 stardist-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-23 22:13:49.000000 stardist-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25283 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/big.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20014 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/bioimageio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/data/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    35505 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/histo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/img2d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   138925 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/img3d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/mask2d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/mask3d.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/geom2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/geom3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/kernels/stardist2d.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/kernels/stardist3d.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.309785 stardist-0.9.0/stardist/lib/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/clipper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   142184 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/clipper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/nanoflann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/nanoflann/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    73558 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/nanoflann/nanoflann.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/qhull_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/Announce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21849 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/lib/external/qhull_src/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.325785 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (127)    73854 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45785 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    75784 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)   140430 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    66346 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    56702 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)   208318 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)   145471 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    47472 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34690 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25609 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30324 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33496 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18839 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19140 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47204 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/test_lib3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19434 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28670 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/rays3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/sample_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/predict2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/predict3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21476 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/top_level.txt
```

### Comparing `stardist-0.8.5/LICENSE.txt` & `stardist-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/PKG-INFO` & `stardist-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: stardist
-Version: 0.8.5
-Summary: StarDist - Object Detection with Star-convex Shapes
-Home-page: https://github.com/stardist/stardist
-Author: Uwe Schmidt, Martin Weigert
-Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
-License: BSD-3-Clause
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: tf1
-Provides-Extra: test
-Provides-Extra: bioimageio
-License-File: LICENSE.txt
-
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
 
@@ -66,15 +40,15 @@
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
 
 ## Installation
 
-This package is compatible with Python 3.6 - 3.10.
+This package is compatible with Python 3.6 - 3.12.
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
@@ -263,20 +237,34 @@
 Installation without using wheels requires Python 3.6 (or newer) and a working C++ compiler. We have only tested [GCC](http://gcc.gnu.org) (macOS, Linux), [Clang](https://clang.llvm.org) (macOS), and [Visual Studio](https://visualstudio.microsoft.com) (Windows 10). Please [open an issue](https://github.com/stardist/stardist/issues) if you have problems that are not resolved by the information below.
 
 If available, the C++ code will make use of [OpenMP](https://en.wikipedia.org/wiki/OpenMP) to exploit multiple CPU cores for substantially reduced runtime on modern CPUs. This can be important to prevent slow model training.
 
 #### macOS
 The default C/C++ compiler Clang that comes with the macOS command line tools (installed via `xcode-select --install`) does not support OpenMP out of the box, but it can be added. Alternatively, a suitable compiler can be installed from [conda-forge](https://conda-forge.org). Please see this [detailed guide](https://scikit-learn.org/stable/developers/advanced_installation.html#macos)  for more information on both strategies (although written for [scikit-image](https://scikit-learn.org), it also applies here).
 
-A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-10`/`g++-10` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
+A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-12`/`g++-12` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
 
-    CC=gcc-10 CXX=g++-10 pip install stardist
+    CC=gcc-12 CXX=g++-12 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
+If you encounter an `ImportError: dlopen(...): symbol not found in flat namespace ...` error on `import stardist`, you may try to install it like so:
+
+```
+brew install libomp
+
+export HOMEBREW_PREFIX=/opt/homebrew #set to your homebrew prefix
+export CPPFLAGS="$CPPFLAGS -Xpreprocessor -fopenmp"
+export CFLAGS="$CFLAGS -I/usr/local/opt/libomp/include"
+export CXXFLAGS="$CXXFLAGS -I/usr/local/opt/libomp/include"
+export LDFLAGS="$LDFLAGS -Wl,-rpath,/usr/local/opt/libomp/lib -L/usr/local/opt/libomp/lib -lomp"
+
+pip install stardist --no-binary :all:
+```
+
 ##### Apple Silicon
 
 As of StarDist 0.8.2, we provide `arm64` wheels that should work with [macOS on Apple Silicon](https://support.apple.com/en-us/HT211814) (M1 chip or newer). 
 We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) (ensure you are using macOS 12 Monterey or newer) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
 ```
 conda create -y -n stardist-env python=3.9   
 conda activate stardist-env
```

### Comparing `stardist-0.8.5/README.md` & `stardist-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: stardist
+Version: 0.9.0
+Summary: StarDist - Object Detection with Star-convex Shapes
+Home-page: https://github.com/stardist/stardist
+Author: Uwe Schmidt, Martin Weigert
+Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
+License: BSD-3-Clause
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: csbdeep>=0.8.0
+Requires-Dist: scikit-image
+Requires-Dist: numba
+Requires-Dist: imageio
+Provides-Extra: tf1
+Requires-Dist: csbdeep[tf1]>=0.8.0; extra == "tf1"
+Provides-Extra: test
+Requires-Dist: pytest; python_version < "3.7" and extra == "test"
+Requires-Dist: pytest>=7.2.0; python_version >= "3.7" and extra == "test"
+Provides-Extra: bioimageio
+Requires-Dist: bioimageio.core>=0.5.0; extra == "bioimageio"
+Requires-Dist: importlib-metadata; extra == "bioimageio"
+
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
 
@@ -40,15 +76,15 @@
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
 
 ## Installation
 
-This package is compatible with Python 3.6 - 3.10.
+This package is compatible with Python 3.6 - 3.12.
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
@@ -237,20 +273,34 @@
 Installation without using wheels requires Python 3.6 (or newer) and a working C++ compiler. We have only tested [GCC](http://gcc.gnu.org) (macOS, Linux), [Clang](https://clang.llvm.org) (macOS), and [Visual Studio](https://visualstudio.microsoft.com) (Windows 10). Please [open an issue](https://github.com/stardist/stardist/issues) if you have problems that are not resolved by the information below.
 
 If available, the C++ code will make use of [OpenMP](https://en.wikipedia.org/wiki/OpenMP) to exploit multiple CPU cores for substantially reduced runtime on modern CPUs. This can be important to prevent slow model training.
 
 #### macOS
 The default C/C++ compiler Clang that comes with the macOS command line tools (installed via `xcode-select --install`) does not support OpenMP out of the box, but it can be added. Alternatively, a suitable compiler can be installed from [conda-forge](https://conda-forge.org). Please see this [detailed guide](https://scikit-learn.org/stable/developers/advanced_installation.html#macos)  for more information on both strategies (although written for [scikit-image](https://scikit-learn.org), it also applies here).
 
-A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-10`/`g++-10` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
+A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-12`/`g++-12` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
 
-    CC=gcc-10 CXX=g++-10 pip install stardist
+    CC=gcc-12 CXX=g++-12 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
+If you encounter an `ImportError: dlopen(...): symbol not found in flat namespace ...` error on `import stardist`, you may try to install it like so:
+
+```
+brew install libomp
+
+export HOMEBREW_PREFIX=/opt/homebrew #set to your homebrew prefix
+export CPPFLAGS="$CPPFLAGS -Xpreprocessor -fopenmp"
+export CFLAGS="$CFLAGS -I/usr/local/opt/libomp/include"
+export CXXFLAGS="$CXXFLAGS -I/usr/local/opt/libomp/include"
+export LDFLAGS="$LDFLAGS -Wl,-rpath,/usr/local/opt/libomp/lib -L/usr/local/opt/libomp/lib -lomp"
+
+pip install stardist --no-binary :all:
+```
+
 ##### Apple Silicon
 
 As of StarDist 0.8.2, we provide `arm64` wheels that should work with [macOS on Apple Silicon](https://support.apple.com/en-us/HT211814) (M1 chip or newer). 
 We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) (ensure you are using macOS 12 Monterey or newer) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
 ```
 conda create -y -n stardist-env python=3.9   
 conda activate stardist-env
```

### Comparing `stardist-0.8.5/setup.py` & `stardist-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from __future__ import absolute_import, print_function
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
-from numpy.distutils.misc_util import get_numpy_include_dirs
+from numpy import get_include
 from os import path
 from glob import glob
 
+
+def get_numpy_include_dirs():
+    return [get_include()]
+
+
 class build_ext_openmp(build_ext):
     # https://www.openmp.org/resources/openmp-compilers-tools/
     # python setup.py build_ext --help-compiler
     openmp_compile_args = {
         'msvc':  [['/openmp']],
         'intel': [['-qopenmp']],
         '*':     [['-fopenmp'], ['-Xpreprocessor','-fopenmp']],
@@ -124,25 +129,26 @@
 
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 
     install_requires=[
-        'csbdeep>=0.7.4',
+        'csbdeep>=0.8.0',
         'scikit-image',
         'numba',
         'imageio',
     ],
 
     extras_require={
-        "tf1":  ["csbdeep[tf1]>=0.7.4"],
+        "tf1":  ["csbdeep[tf1]>=0.8.0"],
         "test": [
             "pytest;        python_version< '3.7'",
             "pytest>=7.2.0; python_version>='3.7'",
          ],
         "bioimageio": ["bioimageio.core>=0.5.0","importlib-metadata"],
     },
```

### Comparing `stardist-0.8.5/stardist/__init__.py` & `stardist-0.9.0/stardist/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .geometry import star_dist3D, polyhedron_to_label, relabel_image_stardist3D
 from .plot.plot import random_label_cmap, draw_polygons, _draw_polygons
 from .plot.render import render_label, render_label_pred
 from .rays3d import rays_from_json, Rays_Cartesian, Rays_SubDivide, Rays_Tetra, Rays_Octo, Rays_GoldenSpiral, Rays_Explicit
 from .sample_patches import sample_patches
 from .bioimageio_utils import export_bioimageio, import_bioimageio
 
-def _py_deprecation(ver_python=(3,6), ver_stardist='0.9.0'):
-     import sys
-     from distutils.version import LooseVersion
-     if sys.version_info[:2] == ver_python and LooseVersion(__version__) < LooseVersion(ver_stardist):
-         print(f"You are using Python {ver_python[0]}.{ver_python[1]}, which will no longer be supported in StarDist {ver_stardist}.\n"
-               f"→ Please upgrade to Python {ver_python[0]}.{ver_python[1]+1} or later.", file=sys.stderr, flush=True)
+def _py_deprecation(ver_python=(3,6), ver_stardist=None):
+    import sys
+    from packaging.version import Version
+    if sys.version_info[:2] == ver_python and (ver_stardist is None or Version(__version__) < Version(ver_stardist)):
+        print(f"You are using Python {ver_python[0]}.{ver_python[1]}, which is deprecated and will no longer be supported in {'future versions of StarDist' if ver_stardist is None else f'StarDist {ver_stardist}'}.\n"
+              f"→ Please upgrade to Python {ver_python[0]}.{ver_python[1]+1} or later.", file=sys.stderr, flush=True)
 _py_deprecation()
 del _py_deprecation
```

### Comparing `stardist-0.8.5/stardist/big.py` & `stardist-0.9.0/stardist/big.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         self.context = int(context)
         self.pred = pred
         self.succ = None
         assert 0 <= self.min_overlap + 2*self.context < self.size
         self.stride = self.size - (self.min_overlap + 2*self.context)
         self._start = 0
         self._frozen = False
+        self._extra_context_start = 0
+        self._extra_context_end = 0
 
     @property
     def start(self):
         return self._start if (self.frozen or self.at_begin) else self.pred.succ_start
 
     @property
     def end(self):
@@ -135,27 +137,27 @@
 
     @property
     def overlap(self):
         return self.size - self.stride
 
     @property
     def context_start(self):
-        return 0 if self.at_begin else self.context
+        return 0 if self.at_begin else self.context + self._extra_context_start
 
     @property
     def context_end(self):
-        return 0 if self.at_end else self.context
+        return 0 if self.at_end else self.context + self._extra_context_end
 
     def __repr__(self):
-        shared  = f'{self.start:03}:{self.end:03}'
-        shared += f', size={self.context_start}-{self.size-self.context_start-self.context_end}-{self.context_end}'
-        if self.at_end:
-            return f'{self.__class__.__name__}({shared})'
-        else:
-            return f'{self.__class__.__name__}({shared}, overlap={self.overlap}/{self.overlap-self.context_start-self.context_end})'
+        text  = f'{self.start:03}:{self.end:03}'
+        text += f', write={self.slice_write.start:03}:{self.slice_write.stop:03}'
+        text += f', size={self.context_start}+{self.size-self.context_start-self.context_end}+{self.context_end}'
+        if not self.at_end:
+            text += f', overlap={self.overlap}R/{self.overlap-self.context_end-self.succ.context_start}W'
+        return f'{self.__class__.__name__}({text})'
 
     @property
     def chain(self):
         blocks = [self]
         while not blocks[-1].at_end:
             blocks.append(blocks[-1].succ)
         return blocks
@@ -200,56 +202,76 @@
 
         # compute cover in grid-multiples
         t = first = Block(block_size, min_overlap, context, None)
         while t.end < size:
             t = t.add_succ()
         last = t
 
-        # [print(t) for t in first]
+        # print(); [print(t) for t in first]
 
         # move blocks around to make it fit
         excess = last.end - size
         t = first
         while excess > 0:
             t.decrease_stride(1)
             excess -= 1
             t = t.succ
             if (t == last): t = first
+        # print(); [print(t) for t in first]
+
+        # add extra context to avoid overlapping write regions of non-neighboring blocks
+        t = first
+        while not t.at_end:
+            if (t.succ is not None and t.succ.succ is not None):
+                overlap_write = t.slice_write.stop - t.succ.succ.slice_write.start
+                if overlap_write > 0:
+                    overlap_split1, overlap_split2 = overlap_write // 2, overlap_write - overlap_write // 2
+                    t._extra_context_end             += overlap_split1
+                    t.succ.succ._extra_context_start += overlap_split2
+            t = t.succ
+        # print(); [print(t) for t in first]
+
 
         # make a copy of the cover and multiply sizes by grid
         if grid > 1:
             size *= grid
             block_size *= grid
             min_overlap *= grid
             context *= grid
             #
             _t = _first = first
             t = first = Block(block_size, min_overlap, context, None)
             t.stride = _t.stride*grid
+            t._extra_context_start = _t._extra_context_start*grid
+            t._extra_context_end   = _t._extra_context_end*grid
             while not _t.at_end:
                 _t = _t.succ
                 t = t.add_succ()
                 t.stride = _t.stride*grid
+                t._extra_context_start = _t._extra_context_start*grid
+                t._extra_context_end   = _t._extra_context_end*grid
             last = t
 
             # change size of last block
             # will be padded internally to the same size
             # as the others by model.predict_instances
             size_delta = size - size_orig
             last.size -= size_delta
             assert 0 <= size_delta < grid
 
         # for efficiency (to not determine starts recursively from now on)
         first.freeze()
 
         blocks = first.chain
+        # print(); [print(t) for t in first]
 
         # sanity checks
         assert first.start == 0 and last.end == size_orig
         assert all(t.overlap-2*context >= min_overlap for t in blocks if t != last)
+        assert all(t.slice_write.stop-t.succ.slice_write.start >= min_overlap for t in blocks if t != last)
         assert all(t.start % grid == 0 and t.end % grid == 0 for t in blocks if t != last)
         # print(); [print(t) for t in first]
 
         # only neighboring blocks should be overlapping
         if len(blocks) >= 3:
             for t in blocks[:-2]:
                 assert t.slice_write.stop <= t.succ.succ.slice_write.start
```

### Comparing `stardist-0.8.5/stardist/bioimageio_utils.py` & `stardist-0.9.0/stardist/bioimageio_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from pkg_resources import get_distribution
 from zipfile import ZipFile
 import numpy as np
 import tempfile
-from distutils.version import LooseVersion
+from packaging.version import Version
 from csbdeep.utils import axes_check_and_normalize, normalize, _raise
 
 
 DEEPIMAGEJ_MACRO = \
 """
 //*******************************************************************
 // Date: July-2021
@@ -72,24 +72,24 @@
 
 def _create_stardist_dependencies(outdir):
     from ruamel.yaml import YAML
     from tensorflow import __version__ as tf_version
     from . import __version__ as stardist_version
     pkg_info = get_distribution("stardist")
     # dependencies that start with the name "bioimageio" will be added as conda dependencies
-    reqs_conda = [str(req) for req in pkg_info.requires(extras=['bioimageio']) if str(req).startswith('bioimageio')]
+    reqs_conda = [f"{req.project_name}{req.specifier}" for req in pkg_info.requires(extras=['bioimageio']) if req.key.startswith('bioimageio')]
     # only stardist and tensorflow as pip dependencies
-    tf_major, tf_minor = LooseVersion(tf_version).version[:2]
-    reqs_pip = (f"stardist>={stardist_version}", f"tensorflow>={tf_major}.{tf_minor},<{tf_major+1}")
+    v_tf = Version(tf_version)
+    reqs_pip = (f"stardist>={stardist_version}", f"tensorflow>={v_tf.major}.{v_tf.minor},<{v_tf.major+1}")
     # conda environment
     env = dict(
         name = 'stardist',
         channels = ['defaults', 'conda-forge'],
         dependencies = [
-            ('python>=3.7,<3.8' if tf_major == 1 else 'python>=3.7'),
+            ('python>=3.7,<3.8' if v_tf.major == 1 else 'python>=3.7'),
             *reqs_conda,
             'pip', {'pip': reqs_pip},
         ],
     )
     yaml = YAML(typ='safe')
     path = outdir / "environment.yaml"
     with open(path, "w") as f:
@@ -105,29 +105,28 @@
         "Please see the [StarDist repository](https://github.com/stardist/stardist) for details."
     )
     with open(doc_path, "w") as f:
         f.write(text)
     return doc_path
 
 
-def _get_stardist_metadata(outdir, model):
+def _get_stardist_metadata(outdir, model, generate_default_deps):
     metadata, *_ = _import()
     package_data = metadata("stardist")
     doi_2d = "https://doi.org/10.1007/978-3-030-00934-2_30"
     doi_3d = "https://doi.org/10.1109/WACV45572.2020.9093435"
     authors = {
         'Martin Weigert': dict(name='Martin Weigert', github_user='maweigert'),
         'Uwe Schmidt': dict(name='Uwe Schmidt', github_user='uschmidt83'),
     }
     data = dict(
         description=package_data["Summary"],
         authors=list(authors.get(name.strip(),dict(name=name.strip())) for name in package_data["Author"].split(",")),
         git_repo=package_data["Home-Page"],
         license=package_data["License"],
-        dependencies=_create_stardist_dependencies(outdir),
         cite=[{"text": "Cell Detection with Star-Convex Polygons", "doi": doi_2d},
               {"text": "Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy", "doi": doi_3d}],
         tags=[
             'fluorescence-light-microscopy', 'whole-slide-imaging', 'other', # modality
             f'{model.config.n_dim}d', # dims
             'cells', 'nuclei', # content
             'tensorflow', # framework
@@ -135,14 +134,17 @@
             'unet', # network
             'instance-segmentation', 'object-detection', # task
             'stardist',
         ],
         covers=["https://raw.githubusercontent.com/stardist/stardist/master/images/stardist_logo.jpg"],
         documentation=_create_stardist_doc(outdir),
     )
+    if generate_default_deps:  # only if requested, as not required for bioimage.io
+        data['dependencies'] = _create_stardist_dependencies(outdir)
+
     return data
 
 
 def _predict_tf(model_path, test_input):
     import tensorflow as tf
     from csbdeep.utils.tf import IS_TF_1
     # need to unzip the model assets
@@ -340,14 +342,15 @@
     test_input_axes=None,
     test_input_norm_axes='ZYX',
     name=None,
     mode="tensorflow_saved_model_bundle",
     min_percentile=1.0,
     max_percentile=99.8,
     overwrite_spec_kwargs=None,
+    generate_default_deps=False,
 ):
     """Export stardist model into bioimage.io format, https://github.com/bioimage-io/spec-bioimage-io.
 
     Parameters
     ----------
     model: StarDist2D, StarDist3D
         the model to convert
@@ -368,14 +371,18 @@
         the export type for this model (default: "tensorflow_saved_model_bundle")
     min_percentile: float
         min percentile to be used for image normalization (default: 1.0)
     max_percentile: float
         max percentile to be used for image normalization (default: 99.8)
     overwrite_spec_kwargs: dict or None
         spec keywords that should be overloaded (default: None)
+    generate_default_deps: bool
+        not required for bioimage.io, i.e. StarDist models don't need a dependencies field in rdf.yaml (default: False)
+        if True, generate an environment.yaml file recording the python, bioimageio.core, stardist and tensorflow requirements
+        from which a conda environment can be recreated to run this export
     """
     _, build_model, *_ = _import()
     from .models import StarDist2D, StarDist3D
     isinstance(model, (StarDist2D, StarDist3D)) or _raise(ValueError("not a valid model"))
     0 <= min_percentile < max_percentile <= 100 or _raise(ValueError("invalid percentile values"))
 
     if name is None:
@@ -391,15 +398,15 @@
         zip_path = outpath
     else:
         raise ValueError(f"outpath has to be a folder or zip file, got {outpath}")
     outdir.mkdir(exist_ok=True, parents=True)
 
     with tempfile.TemporaryDirectory() as _tmp_dir:
         tmp_dir = Path(_tmp_dir)
-        kwargs = _get_stardist_metadata(tmp_dir, model)
+        kwargs = _get_stardist_metadata(tmp_dir, model, generate_default_deps)
         model_kwargs = _get_weights_and_model_metadata(tmp_dir, model, test_input, test_input_axes, test_input_norm_axes, mode,
                                                        min_percentile=min_percentile, max_percentile=max_percentile)
         kwargs.update(model_kwargs)
         if overwrite_spec_kwargs is not None:
             kwargs.update(overwrite_spec_kwargs)
 
         build_model(name=name, output_path=zip_path, add_deepimagej_config=(model.config.n_dim==2), root=tmp_dir, **kwargs)
```

### Comparing `stardist-0.8.5/stardist/data/__init__.py` & `stardist-0.9.0/stardist/data/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/data/images/histo.jpg` & `stardist-0.9.0/stardist/data/images/histo.jpg`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/data/images/img2d.tif` & `stardist-0.9.0/stardist/data/images/img2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/data/images/img3d.tif` & `stardist-0.9.0/stardist/data/images/img3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/data/images/mask2d.tif` & `stardist-0.9.0/stardist/data/images/mask2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/data/images/mask3d.tif` & `stardist-0.9.0/stardist/data/images/mask3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/geometry/geom2d.py` & `stardist-0.9.0/stardist/geometry/geom2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,13 +200,16 @@
 def relabel_image_stardist(lbl, n_rays, **kwargs):
     """relabel each label region in `lbl` with its star representation"""
     _check_label_array(lbl, "lbl")
     if not lbl.ndim==2:
         raise ValueError("lbl image should be 2 dimensional")
     dist = star_dist(lbl, n_rays, **kwargs)
     points = np.array(tuple(np.array(r.centroid).astype(int) for r in regionprops(lbl)))
-    dist = dist[tuple(points.T)]
+    if len(points) == 0:
+        dist, points = np.zeros((0,n_rays),np.float32), np.zeros((0,2),int)
+    else:
+        dist = dist[tuple(points.T)]
     return polygons_to_label(dist, points, shape=lbl.shape)
 
 
 def ray_angles(n_rays=32):
     return np.linspace(0,2*np.pi,n_rays,endpoint=False)
```

### Comparing `stardist-0.8.5/stardist/geometry/geom3d.py` & `stardist-0.9.0/stardist/geometry/geom3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/kernels/stardist2d.cl` & `stardist-0.9.0/stardist/kernels/stardist2d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/kernels/stardist3d.cl` & `stardist-0.9.0/stardist/kernels/stardist3d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/clipper/LICENSE.txt` & `stardist-0.9.0/stardist/lib/external/clipper/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/clipper/clipper.cpp` & `stardist-0.9.0/stardist/lib/external/clipper/clipper.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/clipper/clipper.hpp` & `stardist-0.9.0/stardist/lib/external/clipper/clipper.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/nanoflann/LICENSE.txt` & `stardist-0.9.0/stardist/lib/external/nanoflann/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/nanoflann/nanoflann.hpp` & `stardist-0.9.0/stardist/lib/external/nanoflann/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/Announce.txt` & `stardist-0.9.0/stardist/lib/external/qhull_src/Announce.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/COPYING.txt` & `stardist-0.9.0/stardist/lib/external/qhull_src/COPYING.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/README.txt` & `stardist-0.9.0/stardist/lib/external/qhull_src/README.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp` & `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/stardist2d.cpp` & `stardist-0.9.0/stardist/lib/stardist2d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -546,28 +546,28 @@
     if (use_kdtree)
       // compute neighbors
       size_t n_matches = index.radiusSearch(&points[2*i],
                          (max_dist+radius_outer[i])*(max_dist+radius_outer[i]),
                                           results, params);
     else{
       results.resize(n_polys-i);
-      for (int n = 0; n < results.size(); ++n)
+      for (size_t n = 0; n < results.size(); ++n)
         results[n].first = i+n;
     }
     
 
     // inner loop 
     // remove  schedule(dynamic) on OSX as it leads to segfaults sometimes (TODO)
 #ifdef __APPLE__    
 #pragma omp parallel for reduction(+:count_suppressed)   shared(suppressed) 
 #else
 #pragma omp parallel for schedule(dynamic) reduction(+:count_suppressed)   shared(suppressed)
 #endif
     
-    for (int neigh=0; neigh<results.size(); neigh++) {
+    for (size_t neigh=0; neigh<results.size(); neigh++) {
     // for (int j=i+1; j<n_polys; j++) {
 
       long j = results[neigh].first;
       // printf("%d %d",i,j);
       
       if ((suppressed[j]) || (j<=i))
         continue;
```

### Comparing `stardist-0.8.5/stardist/lib/stardist3d.cpp` & `stardist-0.9.0/stardist/lib/stardist3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/stardist3d_impl.cpp` & `stardist-0.9.0/stardist/lib/stardist3d_impl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
     if (use_kdtree)
       // compute neighbors
       size_t n_matches = index.radiusSearch(&points[3*i],
                          (max_dist+radius_outer[i])*(max_dist+radius_outer[i]),
                                           results, params);
     else{
       results.resize(n_polys-i);
-      for (int n = 0; n < results.size(); ++n)
+      for (size_t n = 0; n < results.size(); ++n)
         results[n].first = i+n;
     }
     //  inner loop
     //  can be parallelized....
 #pragma omp parallel for schedule(dynamic) \
   reduction(+:count_suppressed_pretest) reduction(+:count_suppressed_kernel) \
   reduction(+:count_suppressed_rendered)                                \
@@ -1188,15 +1188,15 @@
   shared(curr_rendered)\
   shared(suppressed) 
 
     // for (int j=i+1; j<n_polys; j++) {
     //   if (suppressed[j])
     //     continue;
     
-    for (int neigh=0; neigh<results.size(); neigh++) {
+    for (size_t neigh=0; neigh<results.size(); neigh++) {
 
       long j = results[neigh].first;
 
       if ((suppressed[j]) || (j<=i))
         continue;
 
 
@@ -1454,21 +1454,20 @@
 
     hs_convex = halfspaces_convex(polyverts, n_rays);
     hs_kernel = halfspaces_kernel(polyverts, faces, n_faces);
 
 
     // loop over bounding box and label pixel if inside of the polyhedron
 #pragma omp parallel for schedule(dynamic)
-    for (int z = std::max(0,bbox[0]); z <= std::min(nz-1,bbox[1]); ++z) {
-      for (int y = std::max(0,bbox[2]); y <= std::min(ny-1,bbox[3]); ++y) {
-        for (int x = std::max(0,bbox[4]); x <= std::min(nx-1,bbox[5]); ++x) {
+    for (uint64_t z = std::max(0,bbox[0]); z <= (uint64_t) std::min(nz-1,bbox[1]); ++z) {
+      for (uint64_t y = std::max(0,bbox[2]); y <= (uint64_t) std::min(ny-1,bbox[3]); ++y) {
+        for (uint64_t x = std::max(0,bbox[4]); x <= (uint64_t) std::min(nx-1,bbox[5]); ++x) {
 
-          
           bool inside = false;
-          long offset = x+y*nx+z*(nx*ny);
+          uint64_t offset = x+y*nx+z*(nx*ny);
 
           switch(render_mode){
           case 0:
             // render_mode "full"
             // kernel and convex hull is fast, so we can formulate the condition
             // such that it can benefit from short-circuiting
             // inside  = in kernel OR (in convex hull AND in rendered)
```

### Comparing `stardist-0.8.5/stardist/lib/stardist3d_impl.h` & `stardist-0.9.0/stardist/lib/stardist3d_impl.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/stardist3d_lib.c` & `stardist-0.9.0/stardist/lib/stardist3d_lib.c`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/stardist3d_lib.h` & `stardist-0.9.0/stardist/lib/stardist3d_lib.h`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/test_lib3d.cpp` & `stardist-0.9.0/stardist/lib/test_lib3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/lib/utils.cpp` & `stardist-0.9.0/stardist/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/matching.py` & `stardist-0.9.0/stardist/matching.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/models/__init__.py` & `stardist-0.9.0/stardist/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import, print_function
 
 from .model2d import Config2D, StarDist2D, StarDistData2D
 from .model3d import Config3D, StarDist3D, StarDistData3D
 
 from csbdeep.utils import backend_channels_last
-from csbdeep.utils.tf import keras_import
-K = keras_import('backend')
+from csbdeep.utils.tf import BACKEND as K
 if not backend_channels_last():
     raise NotImplementedError(
         "Keras is configured to use the '%s' image data format, which is currently not supported. "
         "Please change it to use 'channels_last' instead: "
         "https://keras.io/getting-started/faq/#where-is-the-keras-configuration-file-stored" % K.image_data_format()
     )
 del backend_channels_last, K
```

### Comparing `stardist-0.8.5/stardist/models/base.py` & `stardist-0.9.0/stardist/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 from pathlib import Path
 import threading
 import functools
 import scipy.ndimage as ndi
 import numbers
 
 from csbdeep.models.base_model import BaseModel
-from csbdeep.utils.tf import export_SavedModel, keras_import, IS_TF_1, CARETensorBoard
+from csbdeep.utils.tf import export_SavedModel, keras_import, IS_TF_1, CARETensorBoard, BACKEND as K
 
 import tensorflow as tf
-K = keras_import('backend')
 Sequence = keras_import('utils', 'Sequence')
 Adam = keras_import('optimizers', 'Adam')
 ReduceLROnPlateau, TensorBoard = keras_import('callbacks', 'ReduceLROnPlateau', 'TensorBoard')
 
 from csbdeep.utils import _raise, backend_channels_last, axes_check_and_normalize, axes_dict, load_json, save_json
 from csbdeep.internals.predict import tile_iterator, total_n_tiles
 from csbdeep.internals.train import RollingSequence
 from csbdeep.data import Resizer
 
 from ..sample_patches import get_valid_inds
 from ..nms import _ind_prob_thresh
-from ..utils import _is_power_of_2,  _is_floatarray, optimize_threshold
+from ..utils import _is_power_of_2,  _is_floatarray, optimize_threshold, grid_divisible_patch_size
 
 # TODO: helper function to check if receptive field of cnn is sufficient for object sizes in GT
 
 def generic_masked_loss(mask, loss, weights=1, norm_by_mask=True, reg_weight=0, reg_penalty=K.abs):
+    mask = K.cast(mask, K.floatx())
+    weights = K.cast(weights, K.floatx())
+    _reg_weight = K.cast(reg_weight, K.floatx())
     def _loss(y_true, y_pred):
         actual_loss = K.mean(mask * weights * loss(y_true, y_pred), axis=-1)
         norm_mask = (K.mean(mask) + K.epsilon()) if norm_by_mask else 1
         if reg_weight > 0:
             reg_loss = K.mean((1-mask) * reg_penalty(y_pred), axis=-1)
-            return actual_loss / norm_mask + reg_weight * reg_loss
+            return actual_loss / norm_mask + _reg_weight * reg_loss
         else:
             return actual_loss / norm_mask
     return _loss
 
 def masked_loss(mask, penalty, reg_weight, norm_by_mask):
-    loss = lambda y_true, y_pred: penalty(y_true - y_pred)
+    loss = lambda y_true, y_pred: penalty(K.cast(y_true, K.floatx()) - y_pred)
     return generic_masked_loss(mask, loss, reg_weight=reg_weight, norm_by_mask=norm_by_mask)
 
 # TODO: should we use norm_by_mask=True in the loss or only in a metric?
 #       previous 2D behavior was norm_by_mask=False
 #       same question for reg_weight? use 1e-4 (as in 3D) or 0 (as in 2D)?
 
 def masked_loss_mae(mask, reg_weight=0, norm_by_mask=True):
@@ -64,35 +66,39 @@
 
 def masked_metric_mse(mask):
     def relevant_mse(y_true, y_pred):
         return masked_loss(mask, K.square, reg_weight=0, norm_by_mask=True)(y_true, y_pred)
     return relevant_mse
 
 def kld(y_true, y_pred):
-    y_true = K.clip(y_true, K.epsilon(), 1)
-    y_pred = K.clip(y_pred, K.epsilon(), 1)
+    y_true = K.cast(y_true, K.floatx())
+    mask = y_true >= 0 # pixels to ignore have y_true == -1
+    y_true = K.clip(y_true[mask], K.epsilon(), 1)
+    y_pred = K.clip(y_pred[mask], K.epsilon(), 1)
     return K.mean(K.binary_crossentropy(y_true, y_pred) - K.binary_crossentropy(y_true, y_true), axis=-1)
 
 
 def masked_loss_iou(mask, reg_weight=0, norm_by_mask=True):
     def iou_loss(y_true, y_pred):
+        y_true = K.cast(y_true, K.floatx())
         axis = -1 if backend_channels_last() else 1
         # y_pred can be negative (since not constrained) -> 'inter' can be very large for y_pred << 0
         # - clipping y_pred values at 0 can lead to vanishing gradients
         # - 'K.sign(y_pred)' term fixes issue by enforcing that y_pred values >= 0 always lead to larger 'inter' (lower loss)
         inter = K.mean(K.sign(y_pred)*K.square(K.minimum(y_true,y_pred)), axis=axis)
         union = K.mean(K.square(K.maximum(y_true,y_pred)), axis=axis)
         iou = inter/(union+K.epsilon())
         iou = K.expand_dims(iou,axis)
         loss = 1. - iou # + 0.005*K.abs(y_true-y_pred)
         return loss
     return generic_masked_loss(mask, iou_loss, reg_weight=reg_weight, norm_by_mask=norm_by_mask)
 
 def masked_metric_iou(mask, reg_weight=0, norm_by_mask=True):
     def iou_metric(y_true, y_pred):
+        y_true = K.cast(y_true, K.floatx())
         axis = -1 if backend_channels_last() else 1
         y_pred = K.maximum(0., y_pred)
         inter = K.mean(K.square(K.minimum(y_true,y_pred)), axis=axis)
         union = K.mean(K.square(K.maximum(y_true,y_pred)), axis=axis)
         iou = inter/(union+K.epsilon())
         loss = K.expand_dims(iou,axis)
         return loss
@@ -102,34 +108,35 @@
 def weighted_categorical_crossentropy(weights, ndim):
     """ ndim = (2,3) """
 
     axis = -1 if backend_channels_last() else 1
     shape = [1]*(ndim+2)
     shape[axis] = len(weights)
     weights = np.broadcast_to(weights, shape)
-    weights = K.constant(weights)
+    weights = K.cast(weights, K.floatx())
 
     def weighted_cce(y_true, y_pred):
         # ignore pixels that have y_true (prob_class) < 0
+        y_true = K.cast(y_true, K.floatx())
         mask = K.cast(y_true>=0, K.floatx())
         y_pred /= K.sum(y_pred+K.epsilon(), axis=axis, keepdims=True)
         y_pred = K.clip(y_pred, K.epsilon(), 1. - K.epsilon())
         loss = - K.sum(weights*mask*y_true*K.log(y_pred), axis = axis)
         return loss
 
     return weighted_cce
 
 
 class StarDistDataBase(RollingSequence):
 
     def __init__(self, X, Y, n_rays, grid, batch_size, patch_size, length,
                  n_classes=None, classes=None,
-                 use_gpu=False, sample_ind_cache=True, maxfilter_patch_size=None, augmenter=None, foreground_prob=0):
+                 use_gpu=False, sample_ind_cache=True, maxfilter_patch_size=None, augmenter=None, foreground_prob=0, keras_kwargs=None):
 
-        super().__init__(data_size=len(X), batch_size=batch_size, length=length, shuffle=True)
+        super().__init__(data_size=len(X), batch_size=batch_size, length=length, shuffle=True, keras_kwargs=keras_kwargs)
 
         if isinstance(X, (np.ndarray, tuple, list)):
             X = [x.astype(np.float32, copy=False) for x in X]
 
         # sanity checks
         len(X)==len(Y) and len(X)>0 or _raise(ValueError("X and Y can't be empty and must have same length"))
 
@@ -138,14 +145,15 @@
             classes = (None,)*len(X)
         else:
             n_classes is not None or warnings.warn("Ignoring classes since n_classes is None")
 
         len(classes)==len(X) or _raise(ValueError("X and classes must have same length"))
 
         self.n_classes, self.classes = n_classes, classes
+        patch_size = grid_divisible_patch_size(patch_size, grid)
 
         nD = len(patch_size)
         assert nD in (2,3)
         x_ndim = X[0].ndim
         assert x_ndim in (nD,nD+1)
 
         if isinstance(X, (np.ndarray, tuple, list)) and \
@@ -299,16 +307,19 @@
         if optimizer is None:
             optimizer = Adam(self.config.train_learning_rate)
 
         masked_dist_loss = {'mse': masked_loss_mse,
                             'mae': masked_loss_mae,
                             'iou': masked_loss_iou,
                             }[self.config.train_dist_loss]
-        prob_loss = 'binary_crossentropy'
 
+        def prob_loss(y_true, y_pred):
+            y_true = K.cast(y_true, K.floatx())
+            mask = y_true >= 0
+            return K.mean(K.binary_crossentropy(y_true[mask], y_pred[mask]), axis=-1)
 
         def split_dist_true_mask(dist_true_mask):
             return tf.split(dist_true_mask, num_or_size_splits=[self.config.n_rays,-1], axis=-1)
 
         def dist_loss(dist_true_mask, dist_pred):
             dist_true, dist_mask = split_dist_true_mask(dist_true_mask)
             return masked_dist_loss(dist_mask, reg_weight=self.config.train_background_reg)(dist_true, dist_pred)
@@ -1050,36 +1061,44 @@
             assert 'C' in axes
             if img.ndim == len(axes)-1 and self.config.n_channel_in == 1:
                 # img has no dedicated channel axis, but 'C' always part of config axes
                 axes = axes.replace('C','')
         return axes_check_and_normalize(axes, img.ndim)
 
 
-    def _compute_receptive_field(self, img_size=None):
+    def _compute_receptive_field(self, img_size=None, keras_model=None):
         # TODO: good enough?
         from scipy.ndimage import zoom
         if img_size is None:
             img_size = tuple(g*(128 if self.config.n_dim==2 else 64) for g in self.config.grid)
+        if keras_model is None:
+            keras_model = self.keras_model
         if np.isscalar(img_size):
             img_size = (img_size,) * self.config.n_dim
         img_size = tuple(img_size)
         # print(img_size)
         assert all(_is_power_of_2(s) for s in img_size)
         mid = tuple(s//2 for s in img_size)
         x = np.zeros((1,)+img_size+(self.config.n_channel_in,), dtype=np.float32)
         z = np.zeros_like(x)
         x[(0,)+mid+(slice(None),)] = 1
-        y  = self.keras_model.predict(x, verbose=0)[0][0,...,0]
-        y0 = self.keras_model.predict(z, verbose=0)[0][0,...,0]
+        y  = keras_model.predict(x, verbose=0)[0][0,...,0]
+        y0 = keras_model.predict(z, verbose=0)[0][0,...,0]
         grid = tuple((np.array(x.shape[1:-1])/np.array(y.shape)).astype(int))
         assert grid == self.config.grid
         y  = zoom(y, grid,order=0)
         y0 = zoom(y0,grid,order=0)
         ind = np.where(np.abs(y-y0)>0)
-        return [(m-np.min(i), np.max(i)-m) for (m,i) in zip(mid,ind)]
+        if any(len(i)==0 for i in ind):
+            import contextlib, io
+            with contextlib.redirect_stdout(io.StringIO()) as _:
+                keras_model_untrained = type(self)(self.config,basedir=None).keras_model
+            return self._compute_receptive_field(img_size=img_size, keras_model=keras_model_untrained)
+        else:
+            return [(m-np.min(i), np.max(i)-m) for (m,i) in zip(mid,ind)]
 
 
     def _axes_tile_overlap(self, query_axes):
         query_axes = axes_check_and_normalize(query_axes)
         try:
             self._tile_overlap
         except AttributeError:
```

### Comparing `stardist-0.8.5/stardist/models/model2d.py` & `stardist-0.9.0/stardist/models/model2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,47 @@
 import warnings
 import math
 from tqdm import tqdm
 
 from csbdeep.models import BaseConfig
 from csbdeep.internals.blocks import unet_block
 from csbdeep.utils import _raise, backend_channels_last, axes_check_and_normalize, axes_dict
-from csbdeep.utils.tf import keras_import, IS_TF_1, CARETensorBoard, CARETensorBoardImage
+from csbdeep.utils.tf import keras_import, IS_TF_1, CARETensorBoard, CARETensorBoardImage, IS_KERAS_3_PLUS, BACKEND as K
 from skimage.segmentation import clear_border
 from skimage.measure import regionprops
 from scipy.ndimage import zoom
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 keras = keras_import()
-K = keras_import('backend')
 Input, Conv2D, MaxPooling2D = keras_import('layers', 'Input', 'Conv2D', 'MaxPooling2D')
 Model = keras_import('models', 'Model')
 
 from .base import StarDistBase, StarDistDataBase, _tf_version_at_least
 from ..sample_patches import sample_patches
 from ..utils import edt_prob, _normalize_grid, mask_to_categorical
 from ..geometry import star_dist, dist_to_coord, polygons_to_label
 from ..nms import non_maximum_suppression, non_maximum_suppression_sparse
 
+_gen_rtype = list if IS_TF_1 else tuple
 
 class StarDistData2D(StarDistDataBase):
 
     def __init__(self, X, Y, batch_size, n_rays, length,
                  n_classes=None, classes=None,
                  patch_size=(256,256), b=32, grid=(1,1), shape_completion=False, augmenter=None, foreground_prob=0, **kwargs):
 
         super().__init__(X=X, Y=Y, n_rays=n_rays, grid=grid,
                          n_classes=n_classes, classes=classes,
                          batch_size=batch_size, patch_size=patch_size, length=length,
                          augmenter=augmenter, foreground_prob=foreground_prob, **kwargs)
 
         self.shape_completion = bool(shape_completion)
         if self.shape_completion and b > 0:
+            if not all(b % g == 0 for g in self.grid):
+                raise ValueError(f"'shape_completion' requires that crop size {b} ('train_completion_crop' in config) is evenly divisible by all grid values {self.grid}")
             self.b = slice(b,-b),slice(b,-b)
         else:
             self.b = slice(None),slice(None)
 
         self.sd_mode = 'opencl' if self.use_gpu else 'cpp'
 
 
@@ -55,14 +57,20 @@
         if self.n_channel is None:
             X, Y = list(zip(*[(x[0][self.b],y[0]) for y,x in arrays]))
         else:
             X, Y = list(zip(*[(np.stack([_x[0] for _x in x],axis=-1)[self.b], y[0]) for y,*x in arrays]))
 
         X, Y = tuple(zip(*tuple(self.augmenter(_x, _y) for _x, _y in zip(X,Y))))
 
+        mask_neg_labels = tuple(y[self.b][self.ss_grid[1:3]] < 0 for y in Y)
+        has_neg_labels = any(m.any() for m in mask_neg_labels)
+        if has_neg_labels:
+            mask_neg_labels = np.stack(mask_neg_labels)
+            # set negative label pixels to 0 (background)
+            Y = tuple(np.maximum(y, 0) for y in Y)
 
         prob = np.stack([edt_prob(lbl[self.b][self.ss_grid[1:3]]) for lbl in Y])
         # prob = np.stack([edt_prob(lbl[self.b]) for lbl in Y])
         # prob = prob[self.ss_grid]
 
         if self.shape_completion:
             Y_cleared = [clear_border(lbl) for lbl in Y]
@@ -87,26 +95,32 @@
         # append dist_mask to dist as additional channel
         # dist_and_mask = np.concatenate([dist,dist_mask],axis=-1)
         # faster than concatenate
         dist_and_mask = np.empty(dist.shape[:-1]+(self.n_rays+1,), np.float32)
         dist_and_mask[...,:-1] = dist
         dist_and_mask[...,-1:] = dist_mask
 
+        if has_neg_labels:
+            prob[mask_neg_labels] = -1  # set to -1 to disable loss
 
+        # note: must return tuples in keras 3 (cf. https://stackoverflow.com/a/78158487)
         if self.n_classes is None:
-            return [X], [prob,dist_and_mask]
+            return _gen_rtype((X,)), _gen_rtype((prob,dist_and_mask))
         else:
-            prob_class = np.stack(tuple((mask_to_categorical(y, self.n_classes, self.classes[k]) for y,k in zip(Y, idx))))
+            prob_class = np.stack(tuple((mask_to_categorical(y[self.b], self.n_classes, self.classes[k]) for y,k in zip(Y, idx))))
 
             # TODO: investigate downsampling via simple indexing vs. using 'zoom'
             # prob_class = prob_class[self.ss_grid]
             # 'zoom' might lead to better registered maps (especially if upscaled later)
             prob_class = zoom(prob_class, (1,)+tuple(1/g for g in self.grid)+(1,), order=0)
 
-            return [X], [prob,dist_and_mask, prob_class]
+            if has_neg_labels:
+                prob_class[mask_neg_labels] = -1  # set to -1 to disable loss
+
+            return _gen_rtype((X,)), _gen_rtype((prob,dist_and_mask, prob_class))
 
 
 
 class Config2D(BaseConfig):
     """Configuration for a :class:`StarDist2D` model.
 
     Parameters
@@ -118,15 +132,15 @@
         Recommended to use a power of 2 (default: 32).
     n_channel_in : int
         Number of channels of given input image (default: 1).
     grid : (int,int)
         Subsampling factors (must be powers of 2) for each of the axes.
         Model will predict on a subsampled grid for increased efficiency and larger field of view.
     n_classes : None or int
-        Number of object classes to use for multi-class predection (use None to disable)
+        Number of object classes to use for multi-class prediction (use None to disable)
     backbone : str
         Name of the neural network architecture to be used as backbone.
     kwargs : dict
         Overwrite (or add) configuration attributes (see below).
 
 
     Attributes
@@ -231,15 +245,15 @@
         self.train_steps_per_epoch     = 100
         self.train_learning_rate       = 0.0003
         self.train_batch_size          = 4
         self.train_n_val_patches       = None
         self.train_tensorboard         = True
         # the parameter 'min_delta' was called 'epsilon' for keras<=2.1.5
         # keras.__version__ was removed in tensorflow 2.13.0
-        min_delta_key = 'epsilon' if LooseVersion(getattr(keras, '__version__', '9.9.9'))<=LooseVersion('2.1.5') else 'min_delta'
+        min_delta_key = 'epsilon' if Version(getattr(keras, '__version__', '9.9.9'))<=Version('2.1.5') else 'min_delta'
         self.train_reduce_lr           = {'factor': 0.5, 'patience': 40, min_delta_key: 0}
 
         self.use_gpu                   = False
 
         # remove derived attributes that shouldn't be overwritten
         for k in ('n_dim', 'n_channel_out'):
             try: del kwargs[k]
@@ -340,14 +354,16 @@
 
         Parameters
         ----------
         X : tuple, list, `numpy.ndarray`, `keras.utils.Sequence`
             Input images
         Y : tuple, list, `numpy.ndarray`, `keras.utils.Sequence`
             Label masks
+            Positive pixel values denote object instance ids (0 for background).
+            Negative values can be used to turn off all losses for the corresponding pixels (e.g. for regions that haven't been labeled).
         classes (optional): 'auto' or iterable of same length as X
              label id -> class id mapping for each label mask of Y if multiclass prediction is activated (n_classes > 0)
              list of dicts with label id -> class id (1,...,n_classes)
              'auto' -> all objects will be assigned to the first non-background class,
                        or will be ignored if config.n_classes is None
         validation_data : tuple(:class:`numpy.ndarray`, :class:`numpy.ndarray`) or triple (if multiclass)
             Tuple (triple if multiclass) of X,Y,[classes] validation data.
@@ -411,14 +427,20 @@
             shape_completion = self.config.train_shape_completion,
             b                = self.config.train_completion_crop,
             use_gpu          = self.config.use_gpu,
             foreground_prob  = self.config.train_foreground_only,
             n_classes        = self.config.n_classes,
             sample_ind_cache = self.config.train_sample_cache,
         )
+        worker_kwargs = dict(workers=workers, use_multiprocessing=workers>1)
+        if IS_KERAS_3_PLUS:
+            data_kwargs['keras_kwargs'] = worker_kwargs
+            fit_kwargs = {}
+        else:
+            fit_kwargs = worker_kwargs
 
         # generate validation data and store in numpy arrays
         n_data_val = len(validation_data[0])
         classes_val = self._parse_classes_arg(validation_data[2], n_data_val) if self._is_multiclass() else None
         n_take = self.config.train_n_val_patches if self.config.train_n_val_patches is not None else n_data_val
         _data_val = StarDistData2D(validation_data[0],validation_data[1], classes=classes_val, batch_size=n_take, length=1, **data_kwargs)
         data_val = _data_val[0]
@@ -445,18 +467,18 @@
                         # target image for dist includes dist_mask and thus has more channels than dist output
                         cb.output_target_shapes = [None,[None]*4,None]
                         cb.output_target_shapes[1][1+channel] = data_val[1][1].shape[1+channel]
             elif self.basedir is not None and not any(isinstance(cb,CARETensorBoardImage) for cb in self.callbacks):
                 self.callbacks.append(CARETensorBoardImage(model=self.keras_model, data=data_val, log_dir=str(self.logdir/'logs'/'images'),
                                                            n_images=3, prob_out=False, output_slices=output_slices))
 
-        fit = self.keras_model.fit_generator if IS_TF_1 else self.keras_model.fit
+        fit = self.keras_model.fit_generator if (IS_TF_1 and not IS_KERAS_3_PLUS) else self.keras_model.fit
         history = fit(iter(self.data_train), validation_data=data_val,
                       epochs=epochs, steps_per_epoch=steps_per_epoch,
-                      workers=workers, use_multiprocessing=workers>1,
+                      **fit_kwargs,
                       callbacks=self.callbacks, verbose=1,
                       # set validation batchsize to training batchsize (only works for tf >= 2.2)
                       **(dict(validation_batch_size = self.config.train_batch_size) if _tf_version_at_least("2.2.0") else {}))
         self._training_finished()
 
         return history
 
@@ -512,15 +534,15 @@
             if prob_class is not None:
                 inds = tuple(p//g for p,g in zip(points.T, self.config.grid))
                 prob_class = prob_class[inds]
 
         if scale is not None:
             # need to undo the scaling given by the scale dict, e.g. scale = dict(X=0.5,Y=0.5):
             #   1. re-scale points (origins of polygons)
-            #   2. re-scale coordinates (computed from distances) of (zero-origin) polygons 
+            #   2. re-scale coordinates (computed from distances) of (zero-origin) polygons
             if not (isinstance(scale,dict) and 'X' in scale and 'Y' in scale):
                 raise ValueError("scale must be a dictionary with entries for 'X' and 'Y'")
             rescale = (1/scale['Y'],1/scale['X'])
             points = points * np.array(rescale).reshape(1,2)
         else:
             rescale = (1,1)
```

### Comparing `stardist-0.8.5/stardist/models/model3d.py` & `stardist-0.9.0/stardist/models/model3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 import math
 from tqdm import tqdm
 
 
 from csbdeep.models import BaseConfig
 from csbdeep.internals.blocks import conv_block3, unet_block, resnet_block
 from csbdeep.utils import _raise, backend_channels_last, axes_check_and_normalize, axes_dict
-from csbdeep.utils.tf import keras_import, IS_TF_1, CARETensorBoard, CARETensorBoardImage
-from distutils.version import LooseVersion
+from csbdeep.utils.tf import keras_import, IS_TF_1, CARETensorBoard, CARETensorBoardImage, IS_KERAS_3_PLUS, BACKEND as K
+from packaging.version import Version
 from scipy.ndimage import zoom
 from skimage.measure  import regionprops
 keras = keras_import()
-K = keras_import('backend')
 Input, Conv3D, MaxPooling3D, UpSampling3D, Add, Concatenate = keras_import('layers', 'Input', 'Conv3D', 'MaxPooling3D', 'UpSampling3D', 'Add', 'Concatenate')
 Model = keras_import('models', 'Model')
 
 from .base import StarDistBase, StarDistDataBase, _tf_version_at_least
 from ..sample_patches import sample_patches
 from ..utils import edt_prob, _normalize_grid, mask_to_categorical
 from ..matching import relabel_sequential
 from ..geometry import star_dist3D, polyhedron_to_label
 from ..rays3d import Rays_GoldenSpiral, rays_from_json
 from ..nms import non_maximum_suppression_3d, non_maximum_suppression_3d_sparse
 
+_gen_rtype = list if IS_TF_1 else tuple
 
 class StarDistData3D(StarDistDataBase):
 
     def __init__(self, X, Y, batch_size, rays, length,
                  n_classes=None, classes=None,
                  patch_size=(128,128,128), grid=(1,1,1), anisotropy=None, augmenter=None, foreground_prob=0, **kwargs):
         # TODO: support shape completion as in 2D?
@@ -42,14 +42,15 @@
         self.rays = rays
         self.anisotropy = anisotropy
         self.sd_mode = 'opencl' if self.use_gpu else 'cpp'
         # re-use arrays
         if self.batch_size > 1:
             self.out_X = np.empty((self.batch_size,)+tuple(self.patch_size)+(() if self.n_channel is None else (self.n_channel,)), dtype=np.float32)
             patch_size_grid = tuple((p-1)//g+1 for p,g in zip(self.patch_size,self.grid))
+            self.out_mask_neg_labels = np.empty((self.batch_size,)+patch_size_grid, dtype=bool)
             self.out_edt_prob = np.empty((self.batch_size,)+patch_size_grid, dtype=np.float32)
             self.out_star_dist3D = np.empty((self.batch_size,)+patch_size_grid+(len(self.rays),), dtype=np.float32)
             if self.n_classes is not None:
                 self.out_prob_class = np.empty((self.batch_size,)+tuple(self.patch_size)+(self.n_classes+1,), dtype=np.float32)
 
 
     def __getitem__(self, i):
@@ -61,14 +62,24 @@
         if self.n_channel is None:
             X, Y = list(zip(*[(x[0],y[0]) for y,x in arrays]))
         else:
             X, Y = list(zip(*[(np.stack([_x[0] for _x in x],axis=-1), y[0]) for y,*x in arrays]))
 
         X, Y = tuple(zip(*tuple(self.augmenter(_x, _y) for _x, _y in zip(X,Y))))
 
+        tmp = [y[self.ss_grid[1:]] < 0 for y in Y]
+        has_neg_labels = any(m.any() for m in tmp)
+        if has_neg_labels:
+            if len(Y) == 1:
+                mask_neg_labels = tmp[0][np.newaxis]
+            else:
+                mask_neg_labels = np.stack(tmp, out=self.out_mask_neg_labels[:len(Y)])
+            # set negative label pixels to 0 (background)
+            Y = tuple(np.maximum(y, 0) for y in Y)
+
         if len(Y) == 1:
             X = X[0][np.newaxis]
         else:
             X = np.stack(X, out=self.out_X[:len(Y)])
         if X.ndim == 4: # input image has no channel axis
             X = np.expand_dims(X,-1)
 
@@ -85,30 +96,37 @@
             dist = np.stack(tmp, out=self.out_star_dist3D[:len(Y)])
 
         prob = dist_mask = np.expand_dims(prob, -1)
 
         # append dist_mask to dist as additional channel
         dist = np.concatenate([dist,dist_mask],axis=-1)
 
+        if has_neg_labels:
+            prob[mask_neg_labels] = -1  # set to -1 to disable loss
+
+        # note: must return tuples in keras 3 (cf. https://stackoverflow.com/a/78158487)
         if self.n_classes is None:
-            return [X], [prob,dist]
+            return _gen_rtype((X,)), _gen_rtype((prob,dist))
         else:
             tmp = [mask_to_categorical(y, self.n_classes, self.classes[k]) for y,k in zip(Y, idx)]
             # TODO: downsample here before stacking?
             if len(Y) == 1:
                 prob_class = tmp[0][np.newaxis]
             else:
                 prob_class = np.stack(tmp, out=self.out_prob_class[:len(Y)])
 
             # TODO: investigate downsampling via simple indexing vs. using 'zoom'
             # prob_class = prob_class[self.ss_grid]
             # 'zoom' might lead to better registered maps (especially if upscaled later)
             prob_class = zoom(prob_class, (1,)+tuple(1/g for g in self.grid)+(1,), order=0)
 
-            return [X], [prob,dist, prob_class]
+            if has_neg_labels:
+                prob_class[mask_neg_labels] = -1  # set to -1 to disable loss
+
+            return _gen_rtype((X,)), _gen_rtype((prob,dist, prob_class))
 
 
 
 class Config3D(BaseConfig):
     """Configuration for a :class:`StarDist3D` model.
 
     Parameters
@@ -120,15 +138,15 @@
         If an integer then Ray_GoldenSpiral(rays) will be used
     n_channel_in : int
         Number of channels of given input image (default: 1).
     grid : (int,int,int)
         Subsampling factors (must be powers of 2) for each of the axes.
         Model will predict on a subsampled grid for increased efficiency and larger field of view.
     n_classes : None or int
-        Number of object classes to use for multi-class predection (use None to disable)
+        Number of object classes to use for multi-class prediction (use None to disable)
     anisotropy : (float,float,float)
         Anisotropy of objects along each of the axes.
         Use ``None`` to disable only for (nearly) isotropic objects shapes.
         Also see ``utils.calculate_extents``.
     backbone : str
         Name of the neural network architecture to be used as backbone.
     kwargs : dict
@@ -269,15 +287,15 @@
         self.train_steps_per_epoch     = 100
         self.train_learning_rate       = 0.0003
         self.train_batch_size          = 1
         self.train_n_val_patches       = None
         self.train_tensorboard         = True
         # the parameter 'min_delta' was called 'epsilon' for keras<=2.1.5
         # keras.__version__ was removed in tensorflow 2.13.0
-        min_delta_key = 'epsilon' if LooseVersion(getattr(keras, '__version__', '9.9.9'))<=LooseVersion('2.1.5') else 'min_delta'
+        min_delta_key = 'epsilon' if Version(getattr(keras, '__version__', '9.9.9'))<=Version('2.1.5') else 'min_delta'
         self.train_reduce_lr           = {'factor': 0.5, 'patience': 40, min_delta_key: 0}
 
         self.use_gpu                   = False
 
         # remove derived attributes that shouldn't be overwritten
         for k in ('n_dim', 'n_channel_out', 'n_rays', 'rays_json'):
             try: del kwargs[k]
@@ -434,14 +452,16 @@
 
         Parameters
         ----------
         X : tuple, list, `numpy.ndarray`, `keras.utils.Sequence`
             Input images
         Y : tuple, list, `numpy.ndarray`, `keras.utils.Sequence`
             Label masks
+            Positive pixel values denote object instance ids (0 for background).
+            Negative values can be used to turn off all losses for the corresponding pixels (e.g. for regions that haven't been labeled).
         classes (optional): 'auto' or iterable of same length as X
              label id -> class id mapping for each label mask of Y if multiclass prediction is activated (n_classes > 0)
              list of dicts with label id -> class id (1,...,n_classes)
              'auto' -> all objects will be assigned to the first non-background class,
                        or will be ignored if config.n_classes is None
         validation_data : tuple(:class:`numpy.ndarray`, :class:`numpy.ndarray`) or triple (if multiclass)
             Tuple (triple if multiclass) of X,Y,[classes] validation data.
@@ -502,14 +522,20 @@
             patch_size       = self.config.train_patch_size,
             anisotropy       = self.config.anisotropy,
             use_gpu          = self.config.use_gpu,
             foreground_prob  = self.config.train_foreground_only,
             n_classes        = self.config.n_classes,
             sample_ind_cache = self.config.train_sample_cache,
         )
+        worker_kwargs = dict(workers=workers, use_multiprocessing=workers>1)
+        if IS_KERAS_3_PLUS:
+            data_kwargs['keras_kwargs'] = worker_kwargs
+            fit_kwargs = {}
+        else:
+            fit_kwargs = worker_kwargs
 
         # generate validation data and store in numpy arrays
         n_data_val = len(validation_data[0])
         classes_val = self._parse_classes_arg(validation_data[2], n_data_val) if self._is_multiclass() else None
         n_take = self.config.train_n_val_patches if self.config.train_n_val_patches is not None else n_data_val
         _data_val = StarDistData3D(validation_data[0],validation_data[1], classes=classes_val, batch_size=n_take, length=1, **data_kwargs)
         data_val = _data_val[0]
@@ -544,18 +570,18 @@
                         # target image for dist includes dist_mask and thus has more channels than dist output
                         cb.output_target_shapes = [None,[None]*5,None]
                         cb.output_target_shapes[1][1+channel] = data_val[1][1].shape[1+channel]
             elif self.basedir is not None and not any(isinstance(cb,CARETensorBoardImage) for cb in self.callbacks):
                 self.callbacks.append(CARETensorBoardImage(model=self.keras_model, data=data_val, log_dir=str(self.logdir/'logs'/'images'),
                                                            n_images=3, prob_out=False, input_slices=input_slices, output_slices=output_slices))
 
-        fit = self.keras_model.fit_generator if IS_TF_1 else self.keras_model.fit
+        fit = self.keras_model.fit_generator if (IS_TF_1 and not IS_KERAS_3_PLUS) else self.keras_model.fit
         history = fit(iter(self.data_train), validation_data=data_val,
                       epochs=epochs, steps_per_epoch=steps_per_epoch,
-                      workers=workers, use_multiprocessing=workers>1,
+                      **fit_kwargs,
                       callbacks=self.callbacks, verbose=1,
                       # set validation batchsize to training batchsize (only works in tf 2.x)
                       **(dict(validation_batch_size = self.config.train_batch_size) if _tf_version_at_least("2.2.0") else {}))
         self._training_finished()
 
         return history
```

### Comparing `stardist-0.8.5/stardist/nms.py` & `stardist-0.9.0/stardist/nms.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/plot/plot.py` & `stardist-0.9.0/stardist/plot/plot.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/plot/render.py` & `stardist-0.9.0/stardist/plot/render.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/rays3d.py` & `stardist-0.9.0/stardist/rays3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/sample_patches.py` & `stardist-0.9.0/stardist/sample_patches.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/scripts/predict2d.py` & `stardist-0.9.0/stardist/scripts/predict2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/scripts/predict3d.py` & `stardist-0.9.0/stardist/scripts/predict3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.8.5/stardist/utils.py` & `stardist-0.9.0/stardist/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,7 +388,16 @@
     from pathlib import Path
     root = Path(root)
     if root.is_dir():
         path = root/relpath
     else:
         path = root.parent/relpath
     return str(path.absolute())
+
+
+def grid_divisible_patch_size(patch_size, grid, warn=True):
+    patch_size, grid = tuple(patch_size), tuple(grid)
+    assert len(patch_size) == len(grid)
+    patch_size_divisible = tuple(int(np.ceil(sh/g)*g) for sh,g in zip(patch_size,grid))
+    if patch_size != patch_size_divisible and warn:
+        warnings.warn(f"increasing patch_size from {patch_size} to {patch_size_divisible}, since it was not evenly divisible by grid {grid}")
+    return patch_size_divisible
```

### Comparing `stardist-0.8.5/stardist.egg-info/PKG-INFO` & `stardist-0.9.0/stardist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.8.5
+Version: 0.9.0
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -13,20 +13,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: csbdeep>=0.8.0
+Requires-Dist: scikit-image
+Requires-Dist: numba
+Requires-Dist: imageio
 Provides-Extra: tf1
+Requires-Dist: csbdeep[tf1]>=0.8.0; extra == "tf1"
 Provides-Extra: test
+Requires-Dist: pytest; python_version < "3.7" and extra == "test"
+Requires-Dist: pytest>=7.2.0; python_version >= "3.7" and extra == "test"
 Provides-Extra: bioimageio
-License-File: LICENSE.txt
+Requires-Dist: bioimageio.core>=0.5.0; extra == "bioimageio"
+Requires-Dist: importlib-metadata; extra == "bioimageio"
 
 [![PyPI version](https://badge.fury.io/py/stardist.svg)](https://pypi.org/project/stardist)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/stardist/badges/version.svg)](https://anaconda.org/conda-forge/stardist)
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
@@ -66,15 +76,15 @@
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
 
 ## Installation
 
-This package is compatible with Python 3.6 - 3.10.
+This package is compatible with Python 3.6 - 3.12.
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
@@ -263,20 +273,34 @@
 Installation without using wheels requires Python 3.6 (or newer) and a working C++ compiler. We have only tested [GCC](http://gcc.gnu.org) (macOS, Linux), [Clang](https://clang.llvm.org) (macOS), and [Visual Studio](https://visualstudio.microsoft.com) (Windows 10). Please [open an issue](https://github.com/stardist/stardist/issues) if you have problems that are not resolved by the information below.
 
 If available, the C++ code will make use of [OpenMP](https://en.wikipedia.org/wiki/OpenMP) to exploit multiple CPU cores for substantially reduced runtime on modern CPUs. This can be important to prevent slow model training.
 
 #### macOS
 The default C/C++ compiler Clang that comes with the macOS command line tools (installed via `xcode-select --install`) does not support OpenMP out of the box, but it can be added. Alternatively, a suitable compiler can be installed from [conda-forge](https://conda-forge.org). Please see this [detailed guide](https://scikit-learn.org/stable/developers/advanced_installation.html#macos)  for more information on both strategies (although written for [scikit-image](https://scikit-learn.org), it also applies here).
 
-A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-10`/`g++-10` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
+A third alternative (and what we did until StarDist 0.8.1) is to install the OpenMP-enabled GCC compiler via [Homebrew](https://brew.sh) with `brew install gcc` (e.g. installing `gcc-12`/`g++-12` or newer). After that, you can build the package like this (adjust compiler names/paths as necessary):
 
-    CC=gcc-10 CXX=g++-10 pip install stardist
+    CC=gcc-12 CXX=g++-12 pip install stardist
 
 If you use `conda` on macOS and after `import stardist` see errors similar to `Symbol not found: _GOMP_loop_nonmonotonic_dynamic_next`, please see [this issue](https://github.com/stardist/stardist/issues/19#issuecomment-535610758) for a temporary workaround.
 
+If you encounter an `ImportError: dlopen(...): symbol not found in flat namespace ...` error on `import stardist`, you may try to install it like so:
+
+```
+brew install libomp
+
+export HOMEBREW_PREFIX=/opt/homebrew #set to your homebrew prefix
+export CPPFLAGS="$CPPFLAGS -Xpreprocessor -fopenmp"
+export CFLAGS="$CFLAGS -I/usr/local/opt/libomp/include"
+export CXXFLAGS="$CXXFLAGS -I/usr/local/opt/libomp/include"
+export LDFLAGS="$LDFLAGS -Wl,-rpath,/usr/local/opt/libomp/lib -L/usr/local/opt/libomp/lib -lomp"
+
+pip install stardist --no-binary :all:
+```
+
 ##### Apple Silicon
 
 As of StarDist 0.8.2, we provide `arm64` wheels that should work with [macOS on Apple Silicon](https://support.apple.com/en-us/HT211814) (M1 chip or newer). 
 We recommend setting up an `arm64` `conda` environment with GPU-accelerated TensorFlow following [Apple's instructions](https://developer.apple.com/metal/tensorflow-plugin/) (ensure you are using macOS 12 Monterey or newer) using [conda-forge miniforge3 or mambaforge](https://github.com/conda-forge/miniforge). Then install `stardist` using `pip`.
 ```
 conda create -y -n stardist-env python=3.9   
 conda activate stardist-env
```

### Comparing `stardist-0.8.5/stardist.egg-info/SOURCES.txt` & `stardist-0.9.0/stardist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

