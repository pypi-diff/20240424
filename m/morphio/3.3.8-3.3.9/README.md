# Comparing `tmp/morphio-3.3.8.tar.gz` & `tmp/morphio-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphio-3.3.8.tar", last modified: Wed Apr 24 13:23:21 2024, max compression
+gzip compressed data, was "morphio-3.3.9.tar", last modified: Wed Apr 24 15:47:27 2024, max compression
```

## Comparing `morphio-3.3.8.tar` & `morphio-3.3.9.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.801626 morphio-3.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-24 13:23:09.000000 morphio-3.3.8/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.745626 morphio-3.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.753626 morphio-3.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/check-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/clang_format_check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/coverage_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/docstring_check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/publish-sdist-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 13:23:09.000000 morphio-3.3.8/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 13:23:09.000000 morphio-3.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 13:23:09.000000 morphio-3.3.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 13:23:09.000000 morphio-3.3.8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.753626 morphio-3.3.8/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 13:23:09.000000 morphio-3.3.8/3rdparty/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/GSL_LITE/
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/GSL_LITE/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/gsl-lite.natvis
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/GSL_LITE/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
--rw-r--r--   0 runner    (1001) docker     (127)   188581 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl-lite/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 13:23:14.000000 morphio-3.3.8/3rdparty/GSL_LITE/include/gsl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/HighFive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/HighFive/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/HighFive/CMake/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMake/config/TestHelpers.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/HighFive/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   114912 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/DoxygenLayout.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.757626 morphio-3.3.8/3rdparty/HighFive/doc/doxygen-awesome-css/
--rw-r--r--   0 runner    (1001) docker     (127)    63015 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.761626 morphio-3.3.8/3rdparty/HighFive/doc/poster/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example1_highfive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example6.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_boost.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_easy_h5py.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/example_props.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/examples.js
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/godbolt.org.ico
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/doc/poster/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/3rdparty/HighFive/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.765626 morphio-3.3.8/3rdparty/HighFive/include/highfive/
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Attribute.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataSet.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataType.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Easy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Exception.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5File.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Group.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Object.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16748 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Reference.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Selection.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Utility.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17579 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/ghc_filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/ghc_filesystem/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/cmake/config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/3rdparty/ghc_filesystem/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/
--rw-r--r--   0 runner    (1001) docker     (127)   192164 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 13:23:15.000000 morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.769626 morphio-3.3.8/3rdparty/lexertl14/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/3rdparty/lexertl14/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.773626 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/char_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/dot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/enums.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34590 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30752 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/generator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/internals.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/lookup.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/match_results.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/memory_file.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/narrow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.773626 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    37446 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.777626 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
--rw-r--r--   0 runner    (1001) docker     (127)    32275 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    39423 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29156 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    51193 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28271 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23049 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
--rw-r--r--   0 runner    (1001) docker     (127)    46160 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.777626 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.777626 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/partition/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34712 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/rules.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/serialise.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/state_machine.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/string_token.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-24 13:23:16.000000 morphio-3.3.8/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 13:23:09.000000 morphio-3.3.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-24 13:23:09.000000 morphio-3.3.8/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.777626 morphio-3.3.8/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)    31017 2024-04-24 13:23:09.000000 morphio-3.3.8/CMake/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-24 13:23:09.000000 morphio-3.3.8/CMake/CompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 13:23:09.000000 morphio-3.3.8/CMake/MorphIOConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-24 13:23:09.000000 morphio-3.3.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-24 13:23:09.000000 morphio-3.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-24 13:23:09.000000 morphio-3.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 13:23:09.000000 morphio-3.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-24 13:23:21.801626 morphio-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-24 13:23:09.000000 morphio-3.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/binds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.781626 morphio-3.3.8/binds/python/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_enums.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_enums.h
--rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_immutable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_immutable.h
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_misc.h
--rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_mutable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_mutable.h
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_vasculature.h
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_warnings_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bind_warnings_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bindings_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/bindings_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.781626 morphio-3.3.8/binds/python/generated/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/generated/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)    87786 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/generated/docstrings.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 13:23:09.000000 morphio-3.3.8/binds/python/morphio.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.781626 morphio-3.3.8/binds/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/binds/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.785626 morphio-3.3.8/binds/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    71139 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.785626 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53771 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    29033 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    49892 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.785626 morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/gil_safe_call_once.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    84243 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   129569 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98953 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.785626 morphio-3.3.8/binds/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/include/pybind11/typing.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.789626 morphio-3.3.8/binds/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-24 13:23:17.000000 morphio-3.3.8/binds/python/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.749626 morphio-3.3.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.789626 morphio-3.3.8/include/morphio/
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/collection.h
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/enums.h
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/errorMessages.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/morphology.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/include/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/dendritic_spine.h
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/endoplasmic_reticulum.h
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/glial_cell.h
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/mito_section.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/mitochondria.h
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/modifiers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/morphology.h
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/section.h
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/soma.h
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/mut/writers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/properties.h
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/section.h
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/section_base.h
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/section_iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/soma.h
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/types.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/include/morphio/vasc/
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/vasc/iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/vasc/properties.h
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/vasc/section.h
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/vasc/vasculature.h
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/vector_types.h
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/version.h
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-24 13:23:09.000000 morphio-3.3.8/include/morphio/warning_handling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/morphio/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-24 13:23:09.000000 morphio-3.3.8/morphio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/morphio/mut/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 13:23:09.000000 morphio-3.3.8/morphio/mut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/morphio/vasculature/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 13:23:09.000000 morphio-3.3.8/morphio/vasculature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.793626 morphio-3.3.8/morphio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 13:23:21.000000 morphio-3.3.8/morphio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 13:23:09.000000 morphio-3.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:23:21.801626 morphio-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-24 13:23:09.000000 morphio-3.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.797626 morphio-3.3.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-24 13:23:09.000000 morphio-3.3.8/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-24 13:23:09.000000 morphio-3.3.8/src/collection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 13:23:09.000000 morphio-3.3.8/src/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 13:23:09.000000 morphio-3.3.8/src/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 13:23:09.000000 morphio-3.3.8/src/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 13:23:09.000000 morphio-3.3.8/src/errorMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-24 13:23:09.000000 morphio-3.3.8/src/error_message_generation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-24 13:23:09.000000 morphio-3.3.8/src/error_message_generation.h
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-24 13:23:09.000000 morphio-3.3.8/src/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-24 13:23:09.000000 morphio-3.3.8/src/morphology.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.797626 morphio-3.3.8/src/mut/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/dendritic_spine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/endoplasmic_reticulum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/glial_cell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/mito_section.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/mitochondria.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/modifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/morphology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/section.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/soma.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/writer_asc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/writer_hdf5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/writer_swc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/writer_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 13:23:09.000000 morphio-3.3.8/src/mut/writer_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-24 13:23:09.000000 morphio-3.3.8/src/point_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 13:23:09.000000 morphio-3.3.8/src/point_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-24 13:23:09.000000 morphio-3.3.8/src/properties.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.801626 morphio-3.3.8/src/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/NeurolucidaLexer.inc
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologyASC.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologyASC.h
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologyHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologyHDF5.h
--rw-r--r--   0 runner    (1001) docker     (127)    16032 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologySWC.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/morphologySWC.h
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/vasculatureHDF5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 13:23:09.000000 morphio-3.3.8/src/readers/vasculatureHDF5.h
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 13:23:09.000000 morphio-3.3.8/src/section.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-24 13:23:09.000000 morphio-3.3.8/src/shared_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 13:23:09.000000 morphio-3.3.8/src/shared_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 13:23:09.000000 morphio-3.3.8/src/soma.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:23:21.801626 morphio-3.3.8/src/vasc/
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-24 13:23:09.000000 morphio-3.3.8/src/vasc/properties.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-24 13:23:09.000000 morphio-3.3.8/src/vasc/section.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-24 13:23:09.000000 morphio-3.3.8/src/vasc/vasculature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-24 13:23:09.000000 morphio-3.3.8/src/version.cpp.in
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-24 13:23:09.000000 morphio-3.3.8/src/warning_handling.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.977918 morphio-3.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-24 15:47:12.000000 morphio-3.3.9/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.929918 morphio-3.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/check-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/clang_format_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/coverage_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/docstring_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/publish-sdist-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 15:47:12.000000 morphio-3.3.9/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 15:47:12.000000 morphio-3.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 15:47:12.000000 morphio-3.3.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 15:47:12.000000 morphio-3.3.9/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 15:47:12.000000 morphio-3.3.9/3rdparty/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/GSL_LITE/
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/GSL_LITE/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/cmake/gsl-lite-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/gsl-lite.natvis
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/GSL_LITE/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)   188581 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl-lite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/GSL_LITE/include/gsl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.937918 morphio-3.3.9/3rdparty/HighFive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.941918 morphio-3.3.9/3rdparty/HighFive/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.941918 morphio-3.3.9/3rdparty/HighFive/CMake/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMake/config/TestHelpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.941918 morphio-3.3.9/3rdparty/HighFive/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   114912 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/DoxygenLayout.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.941918 morphio-3.3.9/3rdparty/HighFive/doc/doxygen-awesome-css/
+-rw-r--r--   0 runner    (1001) docker     (127)    63015 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.941918 morphio-3.3.9/3rdparty/HighFive/doc/poster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example1_hdf5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example1_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example6.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_boost.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_easy_h5py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/example_props.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/examples.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/godbolt.org.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/doc/poster/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/3rdparty/HighFive/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.945918 morphio-3.3.9/3rdparty/HighFive/include/highfive/
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Attribute.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataSpace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataType.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Easy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5File.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5FileDriver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Group.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Object.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16748 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5PropertyList.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Selection.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Utility.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Version.hpp.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30878 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Friends.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17579 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 15:47:16.000000 morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/ghc_filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/ghc_filesystem/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/cmake/config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/3rdparty/ghc_filesystem/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/
+-rw-r--r--   0 runner    (1001) docker     (127)   192164 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.949918 morphio-3.3.9/3rdparty/lexertl14/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/3rdparty/lexertl14/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.953918 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/char_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/dot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/enums.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34590 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30752 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/generator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/internals.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/licence_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/lookup.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/match_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/memory_file.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/narrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/observer_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.953918 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    37446 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/parser.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.957918 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/
+-rw-r--r--   0 runner    (1001) docker     (127)    32275 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39423 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29156 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    51193 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28271 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23049 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    46160 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.957918 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.957918 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/partition/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/partition/charset.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34712 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/rules.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/runtime_error.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/serialise.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/sm_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/state_machine.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/string_token.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-24 15:47:19.000000 morphio-3.3.9/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 15:47:12.000000 morphio-3.3.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-24 15:47:12.000000 morphio-3.3.9/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.957918 morphio-3.3.9/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)    31017 2024-04-24 15:47:12.000000 morphio-3.3.9/CMake/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-24 15:47:12.000000 morphio-3.3.9/CMake/CompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 15:47:12.000000 morphio-3.3.9/CMake/MorphIOConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-24 15:47:12.000000 morphio-3.3.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-24 15:47:12.000000 morphio-3.3.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-24 15:47:12.000000 morphio-3.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 15:47:12.000000 morphio-3.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-24 15:47:27.977918 morphio-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-24 15:47:12.000000 morphio-3.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/binds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.961918 morphio-3.3.9/binds/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_immutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_immutable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_mutable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_mutable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_warnings_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bind_warnings_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bindings_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/bindings_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.961918 morphio-3.3.9/binds/python/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/generated/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)    87786 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/generated/docstrings.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 15:47:12.000000 morphio-3.3.9/binds/python/morphio.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.961918 morphio-3.3.9/binds/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/binds/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.965918 morphio-3.3.9/binds/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71139 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.965918 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53771 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29033 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49892 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.965918 morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84243 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   129569 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98953 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.965918 morphio-3.3.9/binds/python/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/include/pybind11/typing.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.969918 morphio-3.3.9/binds/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-24 15:47:20.000000 morphio-3.3.9/binds/python/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.933918 morphio-3.3.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.969918 morphio-3.3.9/include/morphio/
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/collection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/errorMessages.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/morphology.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.969918 morphio-3.3.9/include/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/dendritic_spine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/endoplasmic_reticulum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/glial_cell.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/mito_section.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/mitochondria.h
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/modifiers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/morphology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/section.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/soma.h
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/mut/writers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/properties.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/section.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/section_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/section_iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/soma.h
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/types.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.973918 morphio-3.3.9/include/morphio/vasc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/vasc/iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/vasc/properties.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/vasc/section.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/vasc/vasculature.h
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/vector_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-24 15:47:12.000000 morphio-3.3.9/include/morphio/warning_handling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.973918 morphio-3.3.9/morphio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-24 15:47:12.000000 morphio-3.3.9/morphio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.973918 morphio-3.3.9/morphio/mut/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 15:47:12.000000 morphio-3.3.9/morphio/mut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.973918 morphio-3.3.9/morphio/vasculature/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 15:47:12.000000 morphio-3.3.9/morphio/vasculature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.973918 morphio-3.3.9/morphio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 15:47:27.000000 morphio-3.3.9/morphio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 15:47:12.000000 morphio-3.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:47:27.977918 morphio-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-24 15:47:12.000000 morphio-3.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.977918 morphio-3.3.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-24 15:47:12.000000 morphio-3.3.9/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-24 15:47:12.000000 morphio-3.3.9/src/collection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 15:47:12.000000 morphio-3.3.9/src/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 15:47:12.000000 morphio-3.3.9/src/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 15:47:12.000000 morphio-3.3.9/src/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 15:47:12.000000 morphio-3.3.9/src/errorMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-24 15:47:12.000000 morphio-3.3.9/src/error_message_generation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-24 15:47:12.000000 morphio-3.3.9/src/error_message_generation.h
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-24 15:47:12.000000 morphio-3.3.9/src/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-24 15:47:12.000000 morphio-3.3.9/src/morphology.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.977918 morphio-3.3.9/src/mut/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/dendritic_spine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/endoplasmic_reticulum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/glial_cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/mito_section.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/mitochondria.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/modifiers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/morphology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/soma.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/writer_asc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/writer_hdf5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/writer_swc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/writer_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 15:47:12.000000 morphio-3.3.9/src/mut/writer_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-24 15:47:12.000000 morphio-3.3.9/src/point_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 15:47:12.000000 morphio-3.3.9/src/point_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-24 15:47:12.000000 morphio-3.3.9/src/properties.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.977918 morphio-3.3.9/src/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/NeurolucidaLexer.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologyASC.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologyASC.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologyHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologyHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16032 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologySWC.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/morphologySWC.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/vasculatureHDF5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 15:47:12.000000 morphio-3.3.9/src/readers/vasculatureHDF5.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 15:47:12.000000 morphio-3.3.9/src/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-24 15:47:12.000000 morphio-3.3.9/src/shared_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 15:47:12.000000 morphio-3.3.9/src/shared_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 15:47:12.000000 morphio-3.3.9/src/soma.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:47:27.977918 morphio-3.3.9/src/vasc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-24 15:47:12.000000 morphio-3.3.9/src/vasc/properties.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-24 15:47:12.000000 morphio-3.3.9/src/vasc/section.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-24 15:47:12.000000 morphio-3.3.9/src/vasc/vasculature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-24 15:47:12.000000 morphio-3.3.9/src/version.cpp.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-24 15:47:12.000000 morphio-3.3.9/src/warning_handling.cpp
```

### Comparing `morphio-3.3.8/.clang-format` & `morphio-3.3.9/.clang-format`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/check-sdist.yml` & `morphio-3.3.9/.github/workflows/check-sdist.yml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/clang_format_check.yaml` & `morphio-3.3.9/.github/workflows/clang_format_check.yaml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/coverage_test.yaml` & `morphio-3.3.9/.github/workflows/coverage_test.yaml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/docstring_check.yaml` & `morphio-3.3.9/.github/workflows/docstring_check.yaml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/publish-sdist-wheels.yml` & `morphio-3.3.9/.github/workflows/publish-sdist-wheels.yml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.github/workflows/run-tests.yml` & `morphio-3.3.9/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.gitmodules` & `morphio-3.3.9/.gitmodules`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/.readthedocs.yaml` & `morphio-3.3.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/CMakeLists.txt` & `morphio-3.3.9/3rdparty/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/CMakeLists.txt` & `morphio-3.3.9/3rdparty/GSL_LITE/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in` & `morphio-3.3.9/3rdparty/GSL_LITE/cmake/gsl-lite-config-version.cmake.in`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/gsl-lite.natvis` & `morphio-3.3.9/3rdparty/GSL_LITE/gsl-lite.natvis`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite-vc6.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite.h` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl-lite/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl.h` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/GSL_LITE/include/gsl.hpp` & `morphio-3.3.9/3rdparty/GSL_LITE/include/gsl.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in` & `morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake` & `morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveTargetDeps.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake` & `morphio-3.3.9/3rdparty/HighFive/CMake/HighFiveTargetExport.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake` & `morphio-3.3.9/3rdparty/HighFive/CMake/config/CompilerFlagsHelpers.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake` & `morphio-3.3.9/3rdparty/HighFive/CMake/config/ReleaseDebugAutoFlags.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMake/config/TestHelpers.cmake` & `morphio-3.3.9/3rdparty/HighFive/CMake/config/TestHelpers.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/CMakeLists.txt` & `morphio-3.3.9/3rdparty/HighFive/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/Doxyfile` & `morphio-3.3.9/3rdparty/HighFive/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/DoxygenLayout.xml` & `morphio-3.3.9/3rdparty/HighFive/doc/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css` & `morphio-3.3.9/3rdparty/HighFive/doc/doxygen-awesome-css/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh` & `morphio-3.3.9/3rdparty/HighFive/doc/doxygen-awesome-css/update_doxygen_awesome.sh`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example1_hdf5.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example1_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example3.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example3.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example6.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example6.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_boost.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_boost.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_boost_ublas.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_easy_h5py.py` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_easy_h5py.py`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_easy_highfive.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_eigen.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_eigen.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/example_props.cpp` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/example_props.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/examples.js` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/examples.js`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/godbolt.org.ico` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/godbolt.org.ico`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/doc/poster/index.html` & `morphio-3.3.9/3rdparty/HighFive/doc/poster/index.html`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Attribute.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Attribute.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataSet.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataSet.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataSpace.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataSpace.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5DataType.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5DataType.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Easy.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Easy.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Exception.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Exception.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5File.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5File.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5FileDriver.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5FileDriver.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Group.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Group.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Object.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Object.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5PropertyList.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5PropertyList.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Reference.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Reference.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Selection.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Selection.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Utility.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Utility.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/H5Version.hpp.in` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/H5Version.hpp.in`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Annotate_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Attribute_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Converter_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5DataSet_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5DataType_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Dataspace_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Exception_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5FileDriver_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5File_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Iterables_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Node_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Node_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Object_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Path_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Path_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5PropertyList_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5ReadWrite_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Reference_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Selection_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Slice_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Slice_traits_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5Utils.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/bits/H5_definitions.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_Eigen.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_misc.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_opencv.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_public.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_scalar.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_vector.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp` & `morphio-3.3.9/3rdparty/HighFive/include/highfive/h5easy_bits/H5Easy_xtensor.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/CMakeLists.txt` & `morphio-3.3.9/3rdparty/ghc_filesystem/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/LICENSE` & `morphio-3.3.9/3rdparty/ghc_filesystem/LICENSE`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake` & `morphio-3.3.9/3rdparty/ghc_filesystem/cmake/GhcHelper.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/filesystem.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_fwd.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_impl.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std_fwd.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp` & `morphio-3.3.9/3rdparty/ghc_filesystem/include/ghc/fs_std_impl.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/CMakeLists.txt` & `morphio-3.3.9/3rdparty/lexertl14/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/char_traits.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/char_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/debug.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/debug.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/dot.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/dot.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/enums.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/enums.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/generate_cpp.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/generator.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/generator.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/internals.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/internals.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/iterator.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/iterator.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/licence_1_0.txt` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/licence_1_0.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/lookup.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/lookup.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/match_results.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/match_results.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/memory_file.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/memory_file.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/narrow.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/narrow.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/parser.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/parser.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/blocks.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold2.inc`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/fold4.inc`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_token.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_helper.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/re_tokeniser_state.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/scripts.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/table.inc`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tokeniser/unicode.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/end_node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/iteration_node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/leaf_node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/selection_node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/parser/tree/sequence_node.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/partition/charset.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/partition/charset.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/partition/equivset.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/rules.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/rules.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/runtime_error.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/runtime_error.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/serialise.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/serialise.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/sm_to_csm.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/sm_traits.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/sm_traits.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/state_machine.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/state_machine.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/stream_shared_iterator.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/string_token.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/string_token.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp` & `morphio-3.3.9/3rdparty/lexertl14/include/lexertl/utf_iterators.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/CHANGELOG.md` & `morphio-3.3.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/CMake/CodeCoverage.cmake` & `morphio-3.3.9/CMake/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/CMake/CompilerFlags.cmake` & `morphio-3.3.9/CMake/CompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/CMakeLists.txt` & `morphio-3.3.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/CONTRIBUTING.md` & `morphio-3.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/LICENSE.txt` & `morphio-3.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/MANIFEST.in` & `morphio-3.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/PKG-INFO` & `morphio-3.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphio
-Version: 3.3.8
+Version: 3.3.9
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Keywords: computational neuroscience,morphology,neuron,neurolucida,neuromorphology
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `morphio-3.3.8/README.rst` & `morphio-3.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_enums.cpp` & `morphio-3.3.9/binds/python/bind_enums.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_immutable.cpp` & `morphio-3.3.9/binds/python/bind_immutable.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_misc.cpp` & `morphio-3.3.9/binds/python/bind_misc.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_mutable.cpp` & `morphio-3.3.9/binds/python/bind_mutable.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_mutable.h` & `morphio-3.3.9/binds/python/bind_mutable.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_vasculature.cpp` & `morphio-3.3.9/binds/python/bind_vasculature.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bind_warnings_exceptions.cpp` & `morphio-3.3.9/binds/python/bind_warnings_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bindings_utils.cpp` & `morphio-3.3.9/binds/python/bindings_utils.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/bindings_utils.h` & `morphio-3.3.9/binds/python/bindings_utils.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/generated/docstrings.h` & `morphio-3.3.9/binds/python/generated/docstrings.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/morphio.cpp` & `morphio-3.3.9/binds/python/morphio.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/CMakeLists.txt` & `morphio-3.3.9/binds/python/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/LICENSE` & `morphio-3.3.9/binds/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/attr.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/buffer_info.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/cast.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/chrono.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/complex.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/class.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/common.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/descr.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/init.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/internals.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/type_caster_base.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/detail/typeid.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/matrix.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/eigen/tensor.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/embed.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/eval.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/functional.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/gil.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/gil_safe_call_once.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/gil_safe_call_once.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/iostream.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/numpy.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/operators.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/options.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/pybind11.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/pytypes.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/stl/filesystem.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/stl.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/stl_bind.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/include/pybind11/typing.h` & `morphio-3.3.9/binds/python/pybind11/include/pybind11/typing.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/FindCatch.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/FindEigen3.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/FindPythonLibsNew.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/JoinPaths.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/pybind11Common.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/pybind11NewTools.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/binds/python/pybind11/tools/pybind11Tools.cmake` & `morphio-3.3.9/binds/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/collection.h` & `morphio-3.3.9/include/morphio/collection.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/dendritic_spine.h` & `morphio-3.3.9/include/morphio/dendritic_spine.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/endoplasmic_reticulum.h` & `morphio-3.3.9/include/morphio/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/enums.h` & `morphio-3.3.9/include/morphio/enums.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/errorMessages.h` & `morphio-3.3.9/include/morphio/errorMessages.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/exceptions.h` & `morphio-3.3.9/include/morphio/exceptions.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mito_section.h` & `morphio-3.3.9/include/morphio/mito_section.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mitochondria.h` & `morphio-3.3.9/include/morphio/mitochondria.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/morphology.h` & `morphio-3.3.9/include/morphio/morphology.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/dendritic_spine.h` & `morphio-3.3.9/include/morphio/mut/dendritic_spine.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/endoplasmic_reticulum.h` & `morphio-3.3.9/include/morphio/mut/endoplasmic_reticulum.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/mito_section.h` & `morphio-3.3.9/include/morphio/mut/mito_section.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/mitochondria.h` & `morphio-3.3.9/include/morphio/mut/mitochondria.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/modifiers.h` & `morphio-3.3.9/include/morphio/mut/modifiers.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/morphology.h` & `morphio-3.3.9/include/morphio/mut/morphology.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/section.h` & `morphio-3.3.9/include/morphio/mut/section.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/soma.h` & `morphio-3.3.9/include/morphio/mut/soma.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/mut/writers.h` & `morphio-3.3.9/include/morphio/mut/writers.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/properties.h` & `morphio-3.3.9/include/morphio/properties.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/section.h` & `morphio-3.3.9/include/morphio/section.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/section_base.h` & `morphio-3.3.9/include/morphio/section_base.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/section_iterators.hpp` & `morphio-3.3.9/include/morphio/section_iterators.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/soma.h` & `morphio-3.3.9/include/morphio/soma.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/tools.h` & `morphio-3.3.9/include/morphio/tools.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/types.h` & `morphio-3.3.9/include/morphio/types.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/vasc/iterators.hpp` & `morphio-3.3.9/include/morphio/vasc/iterators.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/vasc/properties.h` & `morphio-3.3.9/include/morphio/vasc/properties.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/vasc/section.h` & `morphio-3.3.9/include/morphio/vasc/section.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/vasc/vasculature.h` & `morphio-3.3.9/include/morphio/vasc/vasculature.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/vector_types.h` & `morphio-3.3.9/include/morphio/vector_types.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/include/morphio/warning_handling.h` & `morphio-3.3.9/include/morphio/warning_handling.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/morphio/__init__.py` & `morphio-3.3.9/morphio/__init__.py`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/morphio.egg-info/PKG-INFO` & `morphio-3.3.9/morphio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphio
-Version: 3.3.8
+Version: 3.3.9
 Summary: A neuron morphology IO library
 Home-page: https://github.com/BlueBrain/MorphIO/
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Keywords: computational neuroscience,morphology,neuron,neurolucida,neuromorphology
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `morphio-3.3.8/morphio.egg-info/SOURCES.txt` & `morphio-3.3.9/morphio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/setup.py` & `morphio-3.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/CMakeLists.txt` & `morphio-3.3.9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/collection.cpp` & `morphio-3.3.9/src/collection.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/dendritic_spine.cpp` & `morphio-3.3.9/src/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/endoplasmic_reticulum.cpp` & `morphio-3.3.9/src/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/enums.cpp` & `morphio-3.3.9/src/enums.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/errorMessages.cpp` & `morphio-3.3.9/src/errorMessages.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/error_message_generation.cpp` & `morphio-3.3.9/src/error_message_generation.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/error_message_generation.h` & `morphio-3.3.9/src/error_message_generation.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/glial_cell.cpp` & `morphio-3.3.9/src/glial_cell.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mito_section.cpp` & `morphio-3.3.9/src/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mitochondria.cpp` & `morphio-3.3.9/src/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/morphology.cpp` & `morphio-3.3.9/src/morphology.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/dendritic_spine.cpp` & `morphio-3.3.9/src/mut/dendritic_spine.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/endoplasmic_reticulum.cpp` & `morphio-3.3.9/src/mut/endoplasmic_reticulum.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/glial_cell.cpp` & `morphio-3.3.9/src/mut/glial_cell.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/mito_section.cpp` & `morphio-3.3.9/src/mut/mito_section.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/mitochondria.cpp` & `morphio-3.3.9/src/mut/mitochondria.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/modifiers.cpp` & `morphio-3.3.9/src/mut/modifiers.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/morphology.cpp` & `morphio-3.3.9/src/mut/morphology.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/section.cpp` & `morphio-3.3.9/src/mut/section.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/soma.cpp` & `morphio-3.3.9/src/mut/soma.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/writer_asc.cpp` & `morphio-3.3.9/src/mut/writer_asc.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/writer_hdf5.cpp` & `morphio-3.3.9/src/mut/writer_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/writer_swc.cpp` & `morphio-3.3.9/src/mut/writer_swc.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/writer_utils.cpp` & `morphio-3.3.9/src/mut/writer_utils.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/mut/writer_utils.h` & `morphio-3.3.9/src/mut/writer_utils.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/point_utils.cpp` & `morphio-3.3.9/src/point_utils.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/point_utils.h` & `morphio-3.3.9/src/point_utils.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/properties.cpp` & `morphio-3.3.9/src/properties.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/NeurolucidaLexer.inc` & `morphio-3.3.9/src/readers/NeurolucidaLexer.inc`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/morphologyASC.cpp` & `morphio-3.3.9/src/readers/morphologyASC.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/morphologyHDF5.cpp` & `morphio-3.3.9/src/readers/morphologyHDF5.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/morphologyHDF5.h` & `morphio-3.3.9/src/readers/morphologyHDF5.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/morphologySWC.cpp` & `morphio-3.3.9/src/readers/morphologySWC.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/morphologySWC.h` & `morphio-3.3.9/src/readers/morphologySWC.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/vasculatureHDF5.cpp` & `morphio-3.3.9/src/readers/vasculatureHDF5.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/readers/vasculatureHDF5.h` & `morphio-3.3.9/src/readers/vasculatureHDF5.h`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/section.cpp` & `morphio-3.3.9/src/section.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/shared_utils.cpp` & `morphio-3.3.9/src/shared_utils.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,14 @@
     } else if (column_mask.count() == 1) {
         return OneColumnIsTheSame;
     } else if (column_mask.all()) {
         return ThreeColumnsAreTheSame;
     }
 
     const size_t col = !column_mask[0] ? 0 : !column_mask[1] ? 1 : 2;
-    std::cout << "asdf\n";
 
     if (!(withinTolerance(points[0][col], points[1][col] - radius) &&
           withinTolerance(points[0][col], points[2][col] + radius)) &&
         !(withinTolerance(points[0][col], points[1][col] + radius) &&
           withinTolerance(points[0][col], points[2][col] - radius))) {
         return NotRadiusOffset;
     }
```

### Comparing `morphio-3.3.8/src/shared_utils.hpp` & `morphio-3.3.9/src/shared_utils.hpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/soma.cpp` & `morphio-3.3.9/src/soma.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/vasc/properties.cpp` & `morphio-3.3.9/src/vasc/properties.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/vasc/section.cpp` & `morphio-3.3.9/src/vasc/section.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/vasc/vasculature.cpp` & `morphio-3.3.9/src/vasc/vasculature.cpp`

 * *Files identical despite different names*

### Comparing `morphio-3.3.8/src/warning_handling.cpp` & `morphio-3.3.9/src/warning_handling.cpp`

 * *Files identical despite different names*

