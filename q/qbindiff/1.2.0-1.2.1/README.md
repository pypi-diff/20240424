# Comparing `tmp/qbindiff-1.2.0.tar.gz` & `tmp/qbindiff-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbindiff-1.2.0.tar", last modified: Wed Apr 10 13:49:15 2024, max compression
+gzip compressed data, was "qbindiff-1.2.1.tar", last modified: Wed Apr 24 12:27:37 2024, max compression
```

## Comparing `qbindiff-1.2.0.tar` & `qbindiff-1.2.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      138 2024-04-10 13:47:47.000000 qbindiff-1.2.0/.git-blame-ignore-revs
--rwxr-xr-x   0        0        0     2211 2024-04-10 13:47:47.000000 qbindiff-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1284 2024-04-10 13:47:47.000000 qbindiff-1.2.0/.gitignore
--rw-r--r--   0        0        0    10173 2024-04-10 13:47:47.000000 qbindiff-1.2.0/LICENSE
--rw-r--r--   0        0        0     8373 2024-04-10 13:47:47.000000 qbindiff-1.2.0/README.md
--rw-r--r--   0        0        0      638 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/Makefile
--rw-r--r--   0        0        0    50152 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/feature_obfu.png
--rw-r--r--   0        0        0   365659 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/graph_alignment.png
--rw-r--r--   0        0        0   364674 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/node_similarity.png
--rw-r--r--   0        0        0      154 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/style.css
--rw-r--r--   0        0        0  2139380 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/thesis.pdf
--rw-r--r--   0        0        0   125461 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/_static/thesis.png
--rw-r--r--   0        0        0      129 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/backend.rst
--rw-r--r--   0        0        0     1127 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/backends/abstract.rst
--rw-r--r--   0        0        0     1174 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/backends/binexport.rst
--rw-r--r--   0        0        0     1108 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/backends/quokka.rst
--rw-r--r--   0        0        0      793 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/differ.rst
--rw-r--r--   0        0        0       67 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/distances.rst
--rw-r--r--   0        0        0     1434 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/extractor.rst
--rw-r--r--   0        0        0     6115 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/features.rst
--rw-r--r--   0        0        0     1976 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/loader.rst
--rw-r--r--   0        0        0      181 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/mapping.rst
--rw-r--r--   0        0        0      571 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/matcher.rst
--rw-r--r--   0        0        0      292 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/metrics.rst
--rw-r--r--   0        0        0      349 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/passes.rst
--rw-r--r--   0        0        0      202 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/qbindiff.rst
--rw-r--r--   0        0        0      142 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/types.rst
--rw-r--r--   0        0        0      558 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/api/visitor.rst
--rw-r--r--   0        0        0     9882 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/basicex.rst
--rw-r--r--   0        0        0      328 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/belief_propagation.rst
--rw-r--r--   0        0        0     3546 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/binary_diffing.rst
--rw-r--r--   0        0        0     2918 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/conf.py
--rw-r--r--   0        0        0     1410 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/export.rst
--rw-r--r--   0        0        0    10579 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/features.rst
--rw-r--r--   0        0        0      167 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/how.rst
--rw-r--r--   0        0        0    87225 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/images/diff_CG.png
--rw-r--r--   0        0        0     1007 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/index.rst
--rw-r--r--   0        0        0     1082 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/install.rst
--rw-r--r--   0        0        0     5666 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/intro.rst
--rw-r--r--   0        0        0     5059 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/params.rst
--rw-r--r--   0        0        0      120 2024-04-10 13:47:47.000000 qbindiff-1.2.0/doc/source/tutorial.rst
--rw-r--r--   0        0        0     1925 2024-04-10 13:47:47.000000 qbindiff-1.2.0/meson.build
--rw-r--r--   0        0        0     1525 2024-04-10 13:47:47.000000 qbindiff-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2632 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/__init__.py
--rw-r--r--   0        0        0    16399 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/__main__.py
--rw-r--r--   0        0        0     3013 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/abstract.py
--rw-r--r--   0        0        0    24439 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/differ.py
--rw-r--r--   0        0        0     2758 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/__init__.py
--rw-r--r--   0        0        0     5853 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/artefact.py
--rw-r--r--   0        0        0     9333 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/extractor.py
--rw-r--r--   0        0        0    13450 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/graph.py
--rw-r--r--   0        0        0     2265 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/manager.py
--rw-r--r--   0        0        0      248 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/meson.build
--rw-r--r--   0        0        0     3002 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/mnemonic.py
--rw-r--r--   0        0        0     3558 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/topology.py
--rw-r--r--   0        0        0     5933 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/features/wlgk.py
--rw-r--r--   0        0        0     1293 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/__init__.py
--rw-r--r--   0        0        0     1044 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/__init__.py
--rw-r--r--   0        0        0     7708 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/abstract.py
--rw-r--r--   0        0        0    16795 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/binexport.py
--rw-r--r--   0        0        0    15160 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/ida.py
--rw-r--r--   0        0        0      214 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/meson.build
--rw-r--r--   0        0        0    18517 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/quokka.py
--rw-r--r--   0        0        0     9409 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/backend/utils.py
--rw-r--r--   0        0        0     2119 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/basic_block.py
--rw-r--r--   0        0        0      911 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/data.py
--rw-r--r--   0        0        0     7325 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/function.py
--rw-r--r--   0        0        0     3397 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/instruction.py
--rw-r--r--   0        0        0      289 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/meson.build
--rw-r--r--   0        0        0     2041 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/operand.py
--rw-r--r--   0        0        0    10129 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/program.py
--rw-r--r--   0        0        0     2425 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/structure.py
--rw-r--r--   0        0        0     3393 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/loader/types.py
--rw-r--r--   0        0        0      671 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/mapping/__init__.py
--rw-r--r--   0        0        0     6776 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/mapping/bindiff.py
--rw-r--r--   0        0        0     8534 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/mapping/mapping.py
--rw-r--r--   0        0        0      157 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/mapping/meson.build
--rw-r--r--   0        0        0       25 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/.gitignore
--rw-r--r--   0        0        0      695 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/belief_propagation.py
--rw-r--r--   0        0        0    10659 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/matcher.py
--rw-r--r--   0        0        0      411 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/meson.build
--rw-r--r--   0        0        0     6908 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/matcher/squares.pyx
--rw-r--r--   0        0        0      325 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/meson.build
--rw-r--r--   0        0        0       33 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/.gitignore
--rw-r--r--   0        0        0     1064 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/__init__.py
--rw-r--r--   0        0        0    13643 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/base.py
--rw-r--r--   0        0        0     7259 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/fast_metrics.pyx
--rw-r--r--   0        0        0      438 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/meson.build
--rw-r--r--   0        0        0    10113 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/metrics.py
--rw-r--r--   0        0        0     5949 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/passes.py
--rw-r--r--   0        0        0     1250 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/passes/utils.py
--rw-r--r--   0        0        0     6618 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/types.py
--rw-r--r--   0        0        0       37 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/.gitignore
--rw-r--r--   0        0        0      717 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/__init__.py
--rw-r--r--   0        0        0      380 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/meson.build
--rw-r--r--   0        0        0     1022 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/openmp_helpers.pxd
--rw-r--r--   0        0        0     3908 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/openmp_helpers.pyx
--rw-r--r--   0        0        0     2579 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/utils/utils.py
--rw-r--r--   0        0        0      644 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/version.py
--rw-r--r--   0        0        0    10004 2024-04-10 13:47:47.000000 qbindiff-1.2.0/src/qbindiff/visitor.py
--rwxr-xr-x   0        0        0   146056 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin
--rw-r--r--   0        0        0     6097 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin-binexport.results
--rw-r--r--   0        0        0     6061 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin-quokka.results
--rw-r--r--   0        0        0   543235 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin.BinExport
--rw-r--r--   0        0        0   490110 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin.quokka
--rwxr-xr-x   0        0        0   146056 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin2
--rw-r--r--   0        0        0   543309 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin2.BinExport
--rw-r--r--   0        0        0   490371 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/binaries/test-bin2.quokka
--rw-r--r--   0        0        0      626 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_no_sim/simple-graph.1
--rw-r--r--   0        0        0      852 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_no_sim/simple-graph.2
--rw-r--r--   0        0        0       86 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_no_sim/simple-graph.output
--rw-r--r--   0        0        0      362 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/partial-match.1
--rw-r--r--   0        0        0      323 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/partial-match.2
--rw-r--r--   0        0        0       49 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/partial-match.output
--rw-r--r--   0        0        0      132 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/partial-match.similarity
--rw-r--r--   0        0        0      362 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/simple-graph.1
--rw-r--r--   0        0        0      442 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/simple-graph.2
--rw-r--r--   0        0        0       53 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/simple-graph.output
--rw-r--r--   0        0        0      210 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/data/graphs_sim/simple-graph.similarity
--rw-r--r--   0        0        0     3303 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/test_binary.py
--rw-r--r--   0        0        0     2991 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/test_graph.py
--rw-r--r--   0        0        0     1783 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/test_sparse_matrix.py
--rw-r--r--   0        0        0     5617 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tests/test_squares.py
--rw-r--r--   0        0        0      993 2024-04-10 13:47:47.000000 qbindiff-1.2.0/tox.ini
--rw-r--r--   0        0        0     9566 2024-04-10 13:49:16.129643 qbindiff-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2024-04-24 12:25:12.000000 qbindiff-1.2.1/.git-blame-ignore-revs
+-rwxr-xr-x   0        0        0     2211 2024-04-24 12:25:12.000000 qbindiff-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1284 2024-04-24 12:25:12.000000 qbindiff-1.2.1/.gitignore
+-rw-r--r--   0        0        0    10173 2024-04-24 12:25:12.000000 qbindiff-1.2.1/LICENSE
+-rw-r--r--   0        0        0     8373 2024-04-24 12:25:12.000000 qbindiff-1.2.1/README.md
+-rw-r--r--   0        0        0      638 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/Makefile
+-rw-r--r--   0        0        0    50152 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/feature_obfu.png
+-rw-r--r--   0        0        0   365659 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/graph_alignment.png
+-rw-r--r--   0        0        0   364674 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/node_similarity.png
+-rw-r--r--   0        0        0      154 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/style.css
+-rw-r--r--   0        0        0  2139380 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/thesis.pdf
+-rw-r--r--   0        0        0   125461 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/_static/thesis.png
+-rw-r--r--   0        0        0      129 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/backend.rst
+-rw-r--r--   0        0        0     1127 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/backends/abstract.rst
+-rw-r--r--   0        0        0     1174 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/backends/binexport.rst
+-rw-r--r--   0        0        0     1108 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/backends/quokka.rst
+-rw-r--r--   0        0        0      793 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/differ.rst
+-rw-r--r--   0        0        0       67 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/distances.rst
+-rw-r--r--   0        0        0     1434 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/extractor.rst
+-rw-r--r--   0        0        0     6115 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/features.rst
+-rw-r--r--   0        0        0     1976 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/loader.rst
+-rw-r--r--   0        0        0      181 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/mapping.rst
+-rw-r--r--   0        0        0      571 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/matcher.rst
+-rw-r--r--   0        0        0      292 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/metrics.rst
+-rw-r--r--   0        0        0      349 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/passes.rst
+-rw-r--r--   0        0        0      202 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/qbindiff.rst
+-rw-r--r--   0        0        0      142 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/types.rst
+-rw-r--r--   0        0        0      558 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/api/visitor.rst
+-rw-r--r--   0        0        0     9882 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/basicex.rst
+-rw-r--r--   0        0        0      328 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/belief_propagation.rst
+-rw-r--r--   0        0        0     3546 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/binary_diffing.rst
+-rw-r--r--   0        0        0     2918 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/conf.py
+-rw-r--r--   0        0        0     1410 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/export.rst
+-rw-r--r--   0        0        0    10579 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/features.rst
+-rw-r--r--   0        0        0      167 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/how.rst
+-rw-r--r--   0        0        0    87225 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/images/diff_CG.png
+-rw-r--r--   0        0        0     1007 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/index.rst
+-rw-r--r--   0        0        0     1082 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/install.rst
+-rw-r--r--   0        0        0     5666 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/intro.rst
+-rw-r--r--   0        0        0     5059 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/params.rst
+-rw-r--r--   0        0        0      120 2024-04-24 12:25:12.000000 qbindiff-1.2.1/doc/source/tutorial.rst
+-rw-r--r--   0        0        0     1925 2024-04-24 12:25:12.000000 qbindiff-1.2.1/meson.build
+-rw-r--r--   0        0        0     1525 2024-04-24 12:25:12.000000 qbindiff-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2632 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/__init__.py
+-rw-r--r--   0        0        0    16399 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/__main__.py
+-rw-r--r--   0        0        0     3013 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/abstract.py
+-rw-r--r--   0        0        0    24439 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/differ.py
+-rw-r--r--   0        0        0     2758 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/__init__.py
+-rw-r--r--   0        0        0     5853 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/artefact.py
+-rw-r--r--   0        0        0     9333 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/extractor.py
+-rw-r--r--   0        0        0    13450 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/graph.py
+-rw-r--r--   0        0        0     2265 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/manager.py
+-rw-r--r--   0        0        0      248 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/meson.build
+-rw-r--r--   0        0        0     3002 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/mnemonic.py
+-rw-r--r--   0        0        0     3558 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/topology.py
+-rw-r--r--   0        0        0     5933 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/features/wlgk.py
+-rw-r--r--   0        0        0     1293 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/__init__.py
+-rw-r--r--   0        0        0     1044 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/__init__.py
+-rw-r--r--   0        0        0     7708 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/abstract.py
+-rw-r--r--   0        0        0    16795 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/binexport.py
+-rw-r--r--   0        0        0    15160 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/ida.py
+-rw-r--r--   0        0        0      214 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/meson.build
+-rw-r--r--   0        0        0    18517 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/quokka.py
+-rw-r--r--   0        0        0     9409 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/backend/utils.py
+-rw-r--r--   0        0        0     2119 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/basic_block.py
+-rw-r--r--   0        0        0      911 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/data.py
+-rw-r--r--   0        0        0     7325 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/function.py
+-rw-r--r--   0        0        0     3397 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/instruction.py
+-rw-r--r--   0        0        0      289 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/meson.build
+-rw-r--r--   0        0        0     2041 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/operand.py
+-rw-r--r--   0        0        0    10129 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/program.py
+-rw-r--r--   0        0        0     2425 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/structure.py
+-rw-r--r--   0        0        0     3393 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/loader/types.py
+-rw-r--r--   0        0        0      671 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/mapping/__init__.py
+-rw-r--r--   0        0        0     6776 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/mapping/bindiff.py
+-rw-r--r--   0        0        0     8534 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/mapping/mapping.py
+-rw-r--r--   0        0        0      157 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/mapping/meson.build
+-rw-r--r--   0        0        0       25 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/.gitignore
+-rw-r--r--   0        0        0      695 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/belief_propagation.py
+-rw-r--r--   0        0        0    10659 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/matcher.py
+-rw-r--r--   0        0        0      411 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/meson.build
+-rw-r--r--   0        0        0     6908 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/matcher/squares.pyx
+-rw-r--r--   0        0        0      325 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/meson.build
+-rw-r--r--   0        0        0       33 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/.gitignore
+-rw-r--r--   0        0        0     1064 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/__init__.py
+-rw-r--r--   0        0        0    13643 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/base.py
+-rw-r--r--   0        0        0     7259 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/fast_metrics.pyx
+-rw-r--r--   0        0        0      438 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/meson.build
+-rw-r--r--   0        0        0    10113 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/metrics.py
+-rw-r--r--   0        0        0     5949 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/passes.py
+-rw-r--r--   0        0        0     1250 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/passes/utils.py
+-rw-r--r--   0        0        0     6618 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/types.py
+-rw-r--r--   0        0        0       37 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/.gitignore
+-rw-r--r--   0        0        0      717 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/meson.build
+-rw-r--r--   0        0        0     1022 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/openmp_helpers.pxd
+-rw-r--r--   0        0        0     3908 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/openmp_helpers.pyx
+-rw-r--r--   0        0        0     2579 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/utils/utils.py
+-rw-r--r--   0        0        0      644 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/version.py
+-rw-r--r--   0        0        0    10004 2024-04-24 12:25:12.000000 qbindiff-1.2.1/src/qbindiff/visitor.py
+-rwxr-xr-x   0        0        0   146056 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin
+-rw-r--r--   0        0        0     6097 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin-binexport.results
+-rw-r--r--   0        0        0     6061 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin-quokka.results
+-rw-r--r--   0        0        0   543235 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin.BinExport
+-rw-r--r--   0        0        0   490110 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin.quokka
+-rwxr-xr-x   0        0        0   146056 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin2
+-rw-r--r--   0        0        0   543309 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin2.BinExport
+-rw-r--r--   0        0        0   490371 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/binaries/test-bin2.quokka
+-rw-r--r--   0        0        0      626 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_no_sim/simple-graph.1
+-rw-r--r--   0        0        0      852 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_no_sim/simple-graph.2
+-rw-r--r--   0        0        0       86 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_no_sim/simple-graph.output
+-rw-r--r--   0        0        0      362 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/partial-match.1
+-rw-r--r--   0        0        0      323 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/partial-match.2
+-rw-r--r--   0        0        0       49 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/partial-match.output
+-rw-r--r--   0        0        0      132 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/partial-match.similarity
+-rw-r--r--   0        0        0      362 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/simple-graph.1
+-rw-r--r--   0        0        0      442 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/simple-graph.2
+-rw-r--r--   0        0        0       53 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/simple-graph.output
+-rw-r--r--   0        0        0      210 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/data/graphs_sim/simple-graph.similarity
+-rw-r--r--   0        0        0     3303 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/test_binary.py
+-rw-r--r--   0        0        0     2991 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/test_graph.py
+-rw-r--r--   0        0        0     1783 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/test_sparse_matrix.py
+-rw-r--r--   0        0        0     5617 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tests/test_squares.py
+-rw-r--r--   0        0        0      993 2024-04-24 12:25:12.000000 qbindiff-1.2.1/tox.ini
+-rw-r--r--   0        0        0     9566 2024-04-24 12:27:37.949453 qbindiff-1.2.1/PKG-INFO
```

### Comparing `qbindiff-1.2.0/.github/workflows/release.yml` & `qbindiff-1.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/.gitignore` & `qbindiff-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/LICENSE` & `qbindiff-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/README.md` & `qbindiff-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/Makefile` & `qbindiff-1.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/_static/feature_obfu.png` & `qbindiff-1.2.1/doc/source/_static/feature_obfu.png`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/_static/graph_alignment.png` & `qbindiff-1.2.1/doc/source/_static/graph_alignment.png`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/_static/node_similarity.png` & `qbindiff-1.2.1/doc/source/_static/node_similarity.png`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/_static/thesis.pdf` & `qbindiff-1.2.1/doc/source/_static/thesis.pdf`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/_static/thesis.png` & `qbindiff-1.2.1/doc/source/_static/thesis.png`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/backends/abstract.rst` & `qbindiff-1.2.1/doc/source/api/backends/abstract.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/backends/binexport.rst` & `qbindiff-1.2.1/doc/source/api/backends/binexport.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/backends/quokka.rst` & `qbindiff-1.2.1/doc/source/api/backends/quokka.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/differ.rst` & `qbindiff-1.2.1/doc/source/api/differ.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/extractor.rst` & `qbindiff-1.2.1/doc/source/api/extractor.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/features.rst` & `qbindiff-1.2.1/doc/source/api/features.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/loader.rst` & `qbindiff-1.2.1/doc/source/api/loader.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/matcher.rst` & `qbindiff-1.2.1/doc/source/api/matcher.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/api/visitor.rst` & `qbindiff-1.2.1/doc/source/api/visitor.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/basicex.rst` & `qbindiff-1.2.1/doc/source/basicex.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/binary_diffing.rst` & `qbindiff-1.2.1/doc/source/binary_diffing.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/conf.py` & `qbindiff-1.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/export.rst` & `qbindiff-1.2.1/doc/source/export.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/features.rst` & `qbindiff-1.2.1/doc/source/features.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/images/diff_CG.png` & `qbindiff-1.2.1/doc/source/images/diff_CG.png`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/index.rst` & `qbindiff-1.2.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/install.rst` & `qbindiff-1.2.1/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/intro.rst` & `qbindiff-1.2.1/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/doc/source/params.rst` & `qbindiff-1.2.1/doc/source/params.rst`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/meson.build` & `qbindiff-1.2.1/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 project(
     'qbindiff',
     'cython', 'c', 'cpp',
-    version: '1.2.0',
+    version: '1.2.1',
     license: 'Apache-2.0',
     license_files: 'LICENSE',
     meson_version: '>= 1.1.0',
 )
 
 py = import('python').find_installation(pure: false)
 py_deps = py.dependency()
```

### Comparing `qbindiff-1.2.0/pyproject.toml` & `qbindiff-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "networkx",
     "capstone>=5.0.1",
     "datasketch",
     "scikit-learn",
     "python-louvain",
     "enum_tools",
     "python-bindiff",
-    "python-binexport>=0.2.0",
+    "python-binexport>=0.3.2",
     "quokka-project",
     "idascript",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 qbindiff = 'qbindiff.__main__:main'
```

### Comparing `qbindiff-1.2.0/src/qbindiff/__init__.py` & `qbindiff-1.2.1/src/qbindiff/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/__main__.py` & `qbindiff-1.2.1/src/qbindiff/__main__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/abstract.py` & `qbindiff-1.2.1/src/qbindiff/abstract.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/differ.py` & `qbindiff-1.2.1/src/qbindiff/differ.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/__init__.py` & `qbindiff-1.2.1/src/qbindiff/features/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/artefact.py` & `qbindiff-1.2.1/src/qbindiff/features/artefact.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/extractor.py` & `qbindiff-1.2.1/src/qbindiff/features/extractor.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/graph.py` & `qbindiff-1.2.1/src/qbindiff/features/graph.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/manager.py` & `qbindiff-1.2.1/src/qbindiff/features/manager.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/mnemonic.py` & `qbindiff-1.2.1/src/qbindiff/features/mnemonic.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/topology.py` & `qbindiff-1.2.1/src/qbindiff/features/topology.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/features/wlgk.py` & `qbindiff-1.2.1/src/qbindiff/features/wlgk.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/__init__.py` & `qbindiff-1.2.1/src/qbindiff/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/__init__.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/abstract.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/abstract.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/binexport.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/binexport.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/ida.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/ida.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/quokka.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/quokka.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/backend/utils.py` & `qbindiff-1.2.1/src/qbindiff/loader/backend/utils.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/basic_block.py` & `qbindiff-1.2.1/src/qbindiff/loader/basic_block.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/data.py` & `qbindiff-1.2.1/src/qbindiff/loader/data.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/function.py` & `qbindiff-1.2.1/src/qbindiff/loader/function.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/instruction.py` & `qbindiff-1.2.1/src/qbindiff/loader/instruction.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/operand.py` & `qbindiff-1.2.1/src/qbindiff/loader/operand.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/program.py` & `qbindiff-1.2.1/src/qbindiff/loader/program.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/structure.py` & `qbindiff-1.2.1/src/qbindiff/loader/structure.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/loader/types.py` & `qbindiff-1.2.1/src/qbindiff/loader/types.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/mapping/__init__.py` & `qbindiff-1.2.1/src/qbindiff/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/mapping/bindiff.py` & `qbindiff-1.2.1/src/qbindiff/mapping/bindiff.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/mapping/mapping.py` & `qbindiff-1.2.1/src/qbindiff/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/matcher/__init__.py` & `qbindiff-1.2.1/src/qbindiff/matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/matcher/belief_propagation.py` & `qbindiff-1.2.1/src/qbindiff/matcher/belief_propagation.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/matcher/matcher.py` & `qbindiff-1.2.1/src/qbindiff/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/matcher/squares.pyx` & `qbindiff-1.2.1/src/qbindiff/matcher/squares.pyx`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/__init__.py` & `qbindiff-1.2.1/src/qbindiff/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/base.py` & `qbindiff-1.2.1/src/qbindiff/passes/base.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/fast_metrics.pyx` & `qbindiff-1.2.1/src/qbindiff/passes/fast_metrics.pyx`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/metrics.py` & `qbindiff-1.2.1/src/qbindiff/passes/metrics.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/passes.py` & `qbindiff-1.2.1/src/qbindiff/passes/passes.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/passes/utils.py` & `qbindiff-1.2.1/src/qbindiff/passes/utils.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/types.py` & `qbindiff-1.2.1/src/qbindiff/types.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/utils/__init__.py` & `qbindiff-1.2.1/src/qbindiff/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/utils/openmp_helpers.pxd` & `qbindiff-1.2.1/src/qbindiff/utils/openmp_helpers.pxd`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/utils/openmp_helpers.pyx` & `qbindiff-1.2.1/src/qbindiff/utils/openmp_helpers.pyx`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/utils/utils.py` & `qbindiff-1.2.1/src/qbindiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/src/qbindiff/version.py` & `qbindiff-1.2.1/src/qbindiff/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  limitations under the License.
 
 """Version
 
 Version of qbindiff
 """
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
```

### Comparing `qbindiff-1.2.0/src/qbindiff/visitor.py` & `qbindiff-1.2.1/src/qbindiff/visitor.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin` & `qbindiff-1.2.1/tests/data/binaries/test-bin`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin-binexport.results` & `qbindiff-1.2.1/tests/data/binaries/test-bin-binexport.results`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin-quokka.results` & `qbindiff-1.2.1/tests/data/binaries/test-bin-quokka.results`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin.BinExport` & `qbindiff-1.2.1/tests/data/binaries/test-bin.BinExport`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin.quokka` & `qbindiff-1.2.1/tests/data/binaries/test-bin.quokka`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin2` & `qbindiff-1.2.1/tests/data/binaries/test-bin2`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin2.BinExport` & `qbindiff-1.2.1/tests/data/binaries/test-bin2.BinExport`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/binaries/test-bin2.quokka` & `qbindiff-1.2.1/tests/data/binaries/test-bin2.quokka`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/graphs_no_sim/simple-graph.1` & `qbindiff-1.2.1/tests/data/graphs_no_sim/simple-graph.1`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/data/graphs_no_sim/simple-graph.2` & `qbindiff-1.2.1/tests/data/graphs_no_sim/simple-graph.2`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/test_binary.py` & `qbindiff-1.2.1/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/test_graph.py` & `qbindiff-1.2.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/test_sparse_matrix.py` & `qbindiff-1.2.1/tests/test_sparse_matrix.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tests/test_squares.py` & `qbindiff-1.2.1/tests/test_squares.py`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/tox.ini` & `qbindiff-1.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `qbindiff-1.2.0/PKG-INFO` & `qbindiff-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbindiff
-Version: 1.2.0
+Version: 1.2.1
 Summary: QBindiff binary diffing tool based on a Network Alignment problem
 Author-Email: Quarkslab <diffing@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/qbindiff
 Project-URL: Repository, https://github.com/quarkslab/qbindiff
 Project-URL: Documentation, https://github.com/quarkslab/qbindiff
 Requires-Python: >=3.10
@@ -15,15 +15,15 @@
 Requires-Dist: networkx
 Requires-Dist: capstone>=5.0.1
 Requires-Dist: datasketch
 Requires-Dist: scikit-learn
 Requires-Dist: python-louvain
 Requires-Dist: enum_tools
 Requires-Dist: python-bindiff
-Requires-Dist: python-binexport>=0.2.0
+Requires-Dist: python-binexport>=0.3.2
 Requires-Dist: quokka-project
 Requires-Dist: idascript
 Requires-Dist: sphinx>=7.2.0; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-rtd-theme>=1.3; extra == "doc"
 Requires-Dist: enum-tools[sphinx]; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints; extra == "doc"
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: qbindiff Version: 1.2.0 Summary: QBindiff binary
+Metadata-Version: 2.1 Name: qbindiff Version: 1.2.1 Summary: QBindiff binary
 diffing tool based on a Network Alignment problem Author-Email: Quarkslab
 quarkslab.com> License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/qbindiff Project-URL:
 Repository, https://github.com/quarkslab/qbindiff Project-URL: Documentation,
 https://github.com/quarkslab/qbindiff Requires-Python: >=3.10 Requires-Dist:
 rich-click Requires-Dist: numpy Requires-Dist: scipy Requires-Dist: lapjv
 Requires-Dist: networkx Requires-Dist: capstone>=5.0.1 Requires-Dist:
 datasketch Requires-Dist: scikit-learn Requires-Dist: python-louvain Requires-
 Dist: enum_tools Requires-Dist: python-bindiff Requires-Dist: python-
-binexport>=0.2.0 Requires-Dist: quokka-project Requires-Dist: idascript
+binexport>=0.3.2 Requires-Dist: quokka-project Requires-Dist: idascript
 Requires-Dist: sphinx>=7.2.0; extra == "doc" Requires-Dist: sphinx-design;
 extra == "doc" Requires-Dist: sphinx-rtd-theme>=1.3; extra == "doc" Requires-
 Dist: enum-tools[sphinx]; extra == "doc" Requires-Dist:
 sphinx_autodoc_typehints; extra == "doc" Requires-Dist: tox; extra == "dev"
 Provides-Extra: doc Provides-Extra: dev Description-Content-Type: text/markdown
 # QBinDiff
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_q_u_a_r_k_s_l_a_b_/_q_b_i_n_d_i_f_f_?_l_o_g_o_=_g_i_t_h_u_b_][https:
```

