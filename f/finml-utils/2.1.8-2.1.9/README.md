# Comparing `tmp/finml_utils-2.1.8.tar.gz` & `tmp/finml_utils-2.1.9.tar.gz`

## Comparing `finml_utils-2.1.8.tar` & `finml_utils-2.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.1.8/codecov.yml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/__init__.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/dataframes.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/enums.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/files.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/introspection.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/list.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/parallel.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/returns.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/s3_store.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/shuffle.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 finml_utils-2.1.8/src/finml_utils/stats.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.1.8/.gitignore
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.1.8/README.md
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finml_utils-2.1.9/codecov.yml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/__init__.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/dataframes.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/enums.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/files.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/introspection.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/list.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/parallel.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/returns.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/s3_store.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/shuffle.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 finml_utils-2.1.9/src/finml_utils/stats.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 finml_utils-2.1.9/.gitignore
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 finml_utils-2.1.9/README.md
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 finml_utils-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 finml_utils-2.1.9/PKG-INFO
```

### Comparing `finml_utils-2.1.8/src/finml_utils/dataframes.py` & `finml_utils-2.1.9/src/finml_utils/dataframes.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,26 @@
 def remove_duplicate_columns(df: pd.DataFrame) -> pd.DataFrame:
     """
     Remove duplicate columns from a DataFrame, keep the last occurences.
     """
     return df.loc[:, ~df.columns[::-1].duplicated()[::-1]]  # type: ignore
 
 
+def remove_columns_with_missing_values(
+    df: pd.DataFrame, threshold: float | int
+) -> pd.DataFrame:
+    def calculate_window_size(window_size: int | float, length: int) -> int:
+        return window_size if window_size > 1 else int(length * window_size)  # type: ignore
+
+    notna = df.notna().sum()
+    threshold = calculate_window_size(threshold, df.shape[0])
+    return df[notna[notna > threshold].index]
+
+
+
 
 def rebase(prices: pd.Series, base: float = 1.0) -> pd.Series:
     """
     Rebase all series to a given intial base.
     This makes comparing/plotting different series together easier.
     Args:
         * prices: Expects a price series/dataframe
```

### Comparing `finml_utils-2.1.8/src/finml_utils/list.py` & `finml_utils-2.1.9/src/finml_utils/list.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/src/finml_utils/parallel.py` & `finml_utils-2.1.9/src/finml_utils/parallel.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/src/finml_utils/returns.py` & `finml_utils-2.1.9/src/finml_utils/returns.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/src/finml_utils/s3_store.py` & `finml_utils-2.1.9/src/finml_utils/s3_store.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/src/finml_utils/shuffle.py` & `finml_utils-2.1.9/src/finml_utils/shuffle.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/src/finml_utils/stats.py` & `finml_utils-2.1.9/src/finml_utils/stats.py`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/.gitignore` & `finml_utils-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `finml_utils-2.1.8/pyproject.toml` & `finml_utils-2.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "finml-utils"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -50,15 +50,15 @@
   "pytest~=7.1.2",
   "pytest-cov>=4.0",
 ]
 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "2.1.8"
+current_version = "2.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `finml_utils-2.1.8/PKG-INFO` & `finml_utils-2.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: finml-utils
-Version: 2.1.8
+Version: 2.1.9
 Project-URL: Issues, https://github.com/dream-faster/finml-utils/issues
 Project-URL: Source, https://github.com/dream-faster/finml-utils
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License-Expression: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

