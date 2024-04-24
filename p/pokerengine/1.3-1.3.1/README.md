# Comparing `tmp/pokerengine-1.3.tar.gz` & `tmp/pokerengine-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.3.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.3.tar` & `pokerengine-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.3/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.3/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.3/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.3/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2040 2022-11-09 12:37:21.000000 pokerengine-1.3/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.3/README.md
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.3/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3364 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31680 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    12020 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.3/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.3/licenses/MIT
--rw-r--r--   0        0        0     1188 2022-11-09 12:37:21.000000 pokerengine-1.3/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/card.py
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/constants.py
--rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7925 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.3/src/pokerengine.cpp
--rw-r--r--   0        0        0      701 2022-11-09 12:37:21.000000 pokerengine-1.3/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.3.1/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.3.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.3.1/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.3.1/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.3.1/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.3.1/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.3.1/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3364 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31680 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    12020 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.3.1/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.3.1/licenses/MIT
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/card.py
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7925 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.3.1/src/pokerengine.cpp
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.3.1/PKG-INFO
```

### Comparing `pokerengine-1.3/.clang-format` & `pokerengine-1.3.1/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.3.1/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/.gitignore` & `pokerengine-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/.pre-commit-config.yaml` & `pokerengine-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/CMakeLists.txt` & `pokerengine-1.3.1/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.3)
+project(pokerengine VERSION 1.3.1)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 
 set(LIBRARY_NAME pokerengine_core)
```

### Comparing `pokerengine-1.3/examples/hand_straight.py` & `pokerengine-1.3.1/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/bits.hpp` & `pokerengine-1.3.1/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/card/card.hpp` & `pokerengine-1.3.1/include/pokerengine/card/card.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/card/cards.hpp` & `pokerengine-1.3.1/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/card/hand.hpp` & `pokerengine-1.3.1/include/pokerengine/card/hand.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/constants.hpp` & `pokerengine-1.3.1/include/pokerengine/constants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/engine.hpp` & `pokerengine-1.3.1/include/pokerengine/engine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/enums.hpp` & `pokerengine-1.3.1/include/pokerengine/enums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.3.1/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.3.1/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.3.1/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.3.1/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/python/pycard.hpp` & `pokerengine-1.3.1/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.3.1/include/pokerengine/python/pyconstants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.3.1/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.3.1/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.3.1/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/string.hpp` & `pokerengine-1.3.1/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/include/pokerengine/vector.hpp` & `pokerengine-1.3.1/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/licenses/MIT` & `pokerengine-1.3.1/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/pyproject.toml` & `pokerengine-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.3"
+version = "1.3.1"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.3/src/pokerengine/constants.py` & `pokerengine-1.3.1/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine/enums.py` & `pokerengine-1.3.1/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.3.1/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.3.1/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.3.1/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.3.1/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/src/pokerengine.cpp` & `pokerengine-1.3.1/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.3/PKG-INFO` & `pokerengine-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.3
+Version: 1.3.1
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

