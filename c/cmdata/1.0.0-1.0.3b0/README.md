# Comparing `tmp/cmdata-1.0.0.tar.gz` & `tmp/cmdata-1.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdata-1.0.0.tar", last modified: Wed Dec 20 14:52:12 2023, max compression
+gzip compressed data, was "/Users/rh/dev/cmdata/dist/.tmp-ym2fbi_t/cmdata-1.0.3b0.tar", last modified: Wed Apr 24 12:25:52 2024, max compression
```

## Comparing `cmdata-1.0.0.tar` & `cmdata-1.0.3b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lfo        (502) staff       (20)        0 2023-12-20 14:52:12.862275 cmdata-1.0.0/
--rw-r--r--   0 lfo        (502) staff       (20)     1087 2023-12-01 14:48:50.000000 cmdata-1.0.0/LICENSE
--rw-r--r--   0 lfo        (502) staff       (20)     3438 2023-12-20 14:52:12.862082 cmdata-1.0.0/PKG-INFO
--rw-r--r--   0 lfo        (502) staff       (20)     1054 2023-12-20 14:48:49.000000 cmdata-1.0.0/README.md
--rw-r--r--   0 lfo        (502) staff       (20)     1421 2023-12-20 14:52:06.000000 cmdata-1.0.0/pyproject.toml
--rw-r--r--   0 lfo        (502) staff       (20)       38 2023-12-20 14:52:12.862322 cmdata-1.0.0/setup.cfg
-drwxr-xr-x   0 lfo        (502) staff       (20)        0 2023-12-20 14:52:12.859990 cmdata-1.0.0/src/
-drwxr-xr-x   0 lfo        (502) staff       (20)        0 2023-12-20 14:52:12.860609 cmdata-1.0.0/src/cmdata/
--rw-r--r--   0 lfo        (502) staff       (20)     1168 2023-12-20 14:48:49.000000 cmdata-1.0.0/src/cmdata/__init__.py
-drwxr-xr-x   0 lfo        (502) staff       (20)        0 2023-12-20 14:52:12.861345 cmdata-1.0.0/src/cmdata/commodities/
--rw-r--r--   0 lfo        (502) staff       (20)        0 2023-12-20 14:48:49.000000 cmdata-1.0.0/src/cmdata/commodities/__init__.py
--rw-r--r--   0 lfo        (502) staff       (20)     9989 2023-12-20 14:48:49.000000 cmdata-1.0.0/src/cmdata/commodities/point_in_time.py
--rw-r--r--   0 lfo        (502) staff       (20)      432 2023-12-20 14:48:49.000000 cmdata-1.0.0/src/cmdata/common.py
-drwxr-xr-x   0 lfo        (502) staff       (20)        0 2023-12-20 14:52:12.861535 cmdata-1.0.0/src/cmdata.egg-info/
--rw-r--r--   0 lfo        (502) staff       (20)     3438 2023-12-20 14:52:12.000000 cmdata-1.0.0/src/cmdata.egg-info/PKG-INFO
--rw-r--r--   0 lfo        (502) staff       (20)      320 2023-12-20 14:52:12.000000 cmdata-1.0.0/src/cmdata.egg-info/SOURCES.txt
--rw-r--r--   0 lfo        (502) staff       (20)        1 2023-12-20 14:52:12.000000 cmdata-1.0.0/src/cmdata.egg-info/dependency_links.txt
--rw-r--r--   0 lfo        (502) staff       (20)       95 2023-12-20 14:52:12.000000 cmdata-1.0.0/src/cmdata.egg-info/requires.txt
--rw-r--r--   0 lfo        (502) staff       (20)        7 2023-12-20 14:52:12.000000 cmdata-1.0.0/src/cmdata.egg-info/top_level.txt
+drwxr-xr-x   0 rh         (501) staff       (20)        0 2024-04-24 12:25:52.801329 cmdata-1.0.3b0/
+-rw-r--r--   0 rh         (501) staff       (20)     1087 2024-03-01 13:06:36.000000 cmdata-1.0.3b0/LICENSE
+-rw-r--r--   0 rh         (501) staff       (20)    11075 2024-04-24 12:25:52.800865 cmdata-1.0.3b0/PKG-INFO
+-rw-r--r--   0 rh         (501) staff       (20)     8688 2024-03-15 16:49:57.000000 cmdata-1.0.3b0/README.md
+-rw-r--r--   0 rh         (501) staff       (20)     1422 2024-04-24 12:25:23.000000 cmdata-1.0.3b0/pyproject.toml
+-rw-r--r--   0 rh         (501) staff       (20)       38 2024-04-24 12:25:52.801419 cmdata-1.0.3b0/setup.cfg
+drwxr-xr-x   0 rh         (501) staff       (20)        0 2024-04-24 12:25:52.795244 cmdata-1.0.3b0/src/
+drwxr-xr-x   0 rh         (501) staff       (20)        0 2024-04-24 12:25:52.796674 cmdata-1.0.3b0/src/cmdata/
+-rw-r--r--   0 rh         (501) staff       (20)     1168 2024-03-01 13:06:36.000000 cmdata-1.0.3b0/src/cmdata/__init__.py
+drwxr-xr-x   0 rh         (501) staff       (20)        0 2024-04-24 12:25:52.798578 cmdata-1.0.3b0/src/cmdata/commodities/
+-rw-r--r--   0 rh         (501) staff       (20)        0 2024-03-01 13:06:36.000000 cmdata-1.0.3b0/src/cmdata/commodities/__init__.py
+-rw-r--r--   0 rh         (501) staff       (20)     9976 2024-04-23 15:47:03.000000 cmdata-1.0.3b0/src/cmdata/commodities/point_in_time.py
+-rw-r--r--   0 rh         (501) staff       (20)      432 2024-03-01 13:06:36.000000 cmdata-1.0.3b0/src/cmdata/common.py
+drwxr-xr-x   0 rh         (501) staff       (20)        0 2024-04-24 12:25:52.799038 cmdata-1.0.3b0/src/cmdata.egg-info/
+-rw-r--r--   0 rh         (501) staff       (20)    11075 2024-04-24 12:25:52.000000 cmdata-1.0.3b0/src/cmdata.egg-info/PKG-INFO
+-rw-r--r--   0 rh         (501) staff       (20)      320 2024-04-24 12:25:52.000000 cmdata-1.0.3b0/src/cmdata.egg-info/SOURCES.txt
+-rw-r--r--   0 rh         (501) staff       (20)        1 2024-04-24 12:25:52.000000 cmdata-1.0.3b0/src/cmdata.egg-info/dependency_links.txt
+-rw-r--r--   0 rh         (501) staff       (20)       95 2024-04-24 12:25:52.000000 cmdata-1.0.3b0/src/cmdata.egg-info/requires.txt
+-rw-r--r--   0 rh         (501) staff       (20)        7 2024-04-24 12:25:52.000000 cmdata-1.0.3b0/src/cmdata.egg-info/top_level.txt
```

### Comparing `cmdata-1.0.0/LICENSE` & `cmdata-1.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdata-1.0.0/pyproject.toml` & `cmdata-1.0.3b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0", "wheel>=0.41"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmdata"
-version = "1.0.0"
+version = "1.0.3b"
 authors = [
   { name="CargoMetrics Technologies Inc.", email="support@cargometrics.com" },
 ]
 description = "A package to process datasets provided by CargoMetrics Technologies Inc."
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["cmdata", "cargometrics", "point in time"]
```

### Comparing `cmdata-1.0.0/src/cmdata/__init__.py` & `cmdata-1.0.3b0/src/cmdata/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdata-1.0.0/src/cmdata/commodities/point_in_time.py` & `cmdata-1.0.3b0/src/cmdata/commodities/point_in_time.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import typing
 
 import numpy
 import pandas
 
 from cmdata import common
 
+# lags expressed in days
 MIN_LAG = 3
 MAX_LAG = 90
 
 
 def read(path: str) -> pandas.DataFrame:
     """
     Reads a commodity pack point-in-time dataset
@@ -19,30 +20,30 @@
     :return: a pandas DataFrame
     """
     df = pandas.read_csv(path, parse_dates=['activity_date', 'publication_timestamp'])
 
     return df
 
 
-def select_publications(df: pandas.DataFrame,
-                        asof=typing.Optional[pandas.Timestamp]) -> pandas.DataFrame:
+def select_increments(df: pandas.DataFrame,
+                      asof=typing.Optional[pandas.Timestamp]) -> pandas.DataFrame:
     """
-    Select only the publications in `df` that are
+    Select only the increments in `df` that are
     at or before `asof`.
 
     This step removes the possibility of look-ahead-bias
     by explicitly removing any data that depends on
     information observed after `asof`.
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
-    :param asof: date; any publications later than this date will
+    :param asof: date; any increments later than this date will
                  be removed from `df`
 
     :return: pandas.DataFrame containing a CM point-in-time dataset
-             excluding any publications after `asof`
+             excluding any increments after `asof`
     """
     if asof is not None:
         # use .copy() to avoid a SettingWithCopyWarning
         df = df[df.publication_timestamp <= asof].copy()
 
     return df
 
@@ -91,21 +92,21 @@
     that were available at or before `asof` in order to generate samples
     without look-ahead bias. If asof is None, all estimaes will
     be considered.
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
     :param selector: callable that returns the set of `(activity_date, lag)`
                      to be included in the view
-    :param asof: optional date; any publications later than this date will
+    :param asof: optional date; any increments later than this date will
                  be excluded from the view
 
     :return: point-in-time view pandas.DataFrame
     """
-    # select only the publications we're interested in
-    df = select_publications(df, asof)
+    # select only the increments we're interested in
+    df = select_increments(df, asof)
     # add a (convenience) lag column
     df = add_lag_column(df)
 
     # select exactly one estimate for each activity_date per (country, direction)
     #
     #  1: get the set of (activity_date, lag)s from the selector
     activity_date_and_lags = selector(df)
@@ -126,63 +127,63 @@
 
     return df
 
 #
 # view_selectors need to define which `(activity_date, lag)` combinations are
 #   included in the view. `lag` is a proxy for the publication timestamp.
 #
-# The point-in-time dataset has several publications of the same `activity_date`
-#   and the role of the view_selector is to pick which publication it wants to
+# The point-in-time dataset has several increments of the same `activity_date`
+#   and the role of the view_selector is to pick which increment it wants to
 #   include in the view for each `activity_date`. I.e., within a view,
-#   each `activity_date` can only be associated with a single publication,
+#   each `activity_date` can only be associated with a single increment,
 #   i.e., a single lag.
 #
 def fixed_lag_view_selector(df: pandas.DataFrame, lag: int) -> pandas.DataFrame:
     """
     Returns a data-frame of {`activity_date`, `lag`} containing
     the (activity_date, lag) combinations that we want to keep
     in the dataset view.
 
     Here we are selecting a view that has a FIXED lag, i.e., we
     only select activity_dates that have the same lag of `lag`.
 
-    This means we select one activity_date per publication.
+    This means we select one activity_date per increment.
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
     :param lag: lag to be included in the view
 
     :return: pandas.DataFrame[activity_date, lag]
     """
-    # find the earliest and latest publication in `df`
+    # find the earliest and latest increment in `df`
     min_publication = common.to_date(df.publication_timestamp.min())
     max_publication = common.to_date(df.publication_timestamp.max())
 
-    # based on the earliest and latest publications find the
+    # based on the earliest and latest increments find the
     #   range of activity_dates we expect to see, which is the
-    #   publication date minus the requested lag for both of them
+    #   increment date minus the requested lag for both of them
     min_activity_date = min_publication - pandas.Timedelta(f'{lag}D')
     max_activity_date = max_publication - pandas.Timedelta(f'{lag}D')
 
     # generate dataframe of activity_dates and lags
     return pandas.DataFrame({'activity_date': pandas.date_range(min_activity_date, max_activity_date),
                              'lag': lag})
 
 
 def standard_view_selector(df: pandas.DataFrame, min_lag: int = MIN_LAG, max_lag: int = MAX_LAG) -> pandas.DataFrame:
     """
     Returns a data-frame of {`activity_date`, `lag`} containing
     the (activity_date, lag) combinations that we want to keep
     in the dataset view.
 
-    Here we are selecting the publication for each activity_date
+    Here we are selecting the increment for each activity_date
     that incorporates the most information, i.e., activity_dates
     with a lag of 90 (which is the maximum lag possible in the
     CargoMetrics point-in-time datasets).
 
-    If a max_lag activity_date does not exist for a given publication
+    If a max_lag activity_date does not exist for a given increment
     (which will be the case for the estimates at the leading edge
     of time) pick the activity_date with the maximum available lag.
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
     :param min_lag: minimum lag to be included in the view (default 3)
     :param max_lag: maximum lag to be included in the view (default 90)
 
@@ -208,15 +209,15 @@
                    asof: typing.Optional[typing.Union[str, pandas.Timestamp]] = None) -> pandas.DataFrame:
     """
     Generates  a fixed lag view at lag `lag` from a point-in-time
     dataset.
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
     :param lag: lag to be included in the view
-    :param asof: optional date; any publications later than this date will
+    :param asof: optional date; any increments later than this date will
                  be excluded from the view
 
     :return: pandas.DataFrame containing the fixed-lag view
     """
     selector = functools.partial(fixed_lag_view_selector, lag=lag)
 
     return select_view(df, selector, asof=asof)
@@ -237,15 +238,15 @@
     and greatest information, i.e., input data, available at `asof`,
     which in turn allows the model to make the best possible assessment
     of maritime trade for each activity date
 
     :param df: pandas.DataFrame containing a CM point-in-time dataset
     :param min_lag: minimum lag to be included in the view (default 3)
     :param max_lag: maximum lag to be included in the view (default 90)
-    :param asof: optional date; any publications later than this date will
+    :param asof: optional date; any increments later than this date will
                  be excluded from the view
 
     :return: pandas.DataFrame containing the fixed-lag view
     """
     selector = functools.partial(standard_view_selector, min_lag=min_lag, max_lag=min(MAX_LAG, max_lag))
 
     return select_view(df, selector, asof=asof)
```

