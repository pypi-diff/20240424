# Comparing `tmp/quool-5.0.7.tar.gz` & `tmp/quool-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quool-5.0.7.tar", last modified: Fri Mar 22 08:16:29 2024, max compression
+gzip compressed data, was "quool-5.0.8.tar", last modified: Tue Apr  9 05:38:09 2024, max compression
```

## Comparing `quool-5.0.7.tar` & `quool-5.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:16:29.975154 quool-5.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-22 08:16:02.000000 quool-5.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-03-22 08:16:29.975154 quool-5.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-03-22 08:16:02.000000 quool-5.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:16:29.975154 quool-5.0.7/quool/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-22 08:16:02.000000 quool-5.0.7/quool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-03-22 08:16:02.000000 quool-5.0.7/quool/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-03-22 08:16:02.000000 quool-5.0.7/quool/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19288 2024-03-22 08:16:02.000000 quool-5.0.7/quool/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-22 08:16:02.000000 quool-5.0.7/quool/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-22 08:16:02.000000 quool-5.0.7/quool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:16:29.975154 quool-5.0.7/quool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-03-22 08:16:29.000000 quool-5.0.7/quool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-22 08:16:29.000000 quool-5.0.7/quool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 08:16:29.000000 quool-5.0.7/quool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-22 08:16:29.000000 quool-5.0.7/quool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 08:16:29.000000 quool-5.0.7/quool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 08:16:29.975154 quool-5.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-22 08:16:02.000000 quool-5.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 05:37:43.000000 quool-5.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-09 05:38:09.513256 quool-5.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-09 05:37:43.000000 quool-5.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/quool/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 05:37:43.000000 quool-5.0.8/quool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-09 05:37:43.000000 quool-5.0.8/quool/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-09 05:37:43.000000 quool-5.0.8/quool/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-09 05:37:43.000000 quool-5.0.8/quool/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-09 05:37:43.000000 quool-5.0.8/quool/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-09 05:37:43.000000 quool-5.0.8/quool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/quool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:38:09.513256 quool-5.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 05:37:43.000000 quool-5.0.8/setup.py
```

### Comparing `quool-5.0.7/LICENSE` & `quool-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/PKG-INFO` & `quool-5.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quool
-Version: 5.0.7
+Version: 5.0.8
 Summary: Quantitative Toolkit - a helper in quant developping
 Home-page: https://github.com/ppoak/quool
 Author: ppoak
 Author-email: ppoak@foxmail.com
 Keywords: quant,framework,finance
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quool-5.0.7/README.md` & `quool-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/quool/core.py` & `quool-5.0.8/quool/core.py`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/quool/factor.py` & `quool-5.0.8/quool/factor.py`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/quool/record.py` & `quool-5.0.8/quool/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,20 +103,21 @@
             trade = pd.concat([trade, cash], axis=0)
         
         self.update(trade)
 
     def peek(self, date: str | pd.Timestamp = None, price: pd.Series = None) -> pd.Series:
         df = self.read(filters=[("datetime", "<=", pd.to_datetime(date or 'now'))])
         df = df.groupby("code")[["size", "amount", "commission"]].sum()
-        df["cost"] = df["amount"] / df["size"]
+        df["cost"] = (df["amount"] / df["size"]).replace([-np.inf, np.inf], 0)
         if price is None:
             return df
         price = price.copy()
         price.loc["cash"] = 1
-        df["price"] = price.loc[df.index]
+        indexer = price.index.get_indexer_for(df.index)
+        df["price"] = price.iloc[indexer[indexer != -1]]
         df["value"] = df["price"] * df["size"]
         df["pnl"] = df["price"] / df["cost"] - 1
         return df
         
     def report(
         self, 
         price: pd.Series, 
@@ -138,16 +139,15 @@
             dates.union(x.index.get_level_values('datetime').unique().sort_values())
         ))
         cash = data.loc["cash", "amount"]
         cash = cash.fillna(0).cumsum()
 
         noncash = data.drop(labels="cash", axis=0)
         noncash.index.names = price.index.names
-        # if it raise, there are some price not available
-        price = price.loc[noncash.index]
+        price = price.loc[noncash.index.intersection(price.index)]
         delta = (price * noncash["size"]).groupby(level=date_level).sum()
         noncash = noncash.groupby(level=code_level, group_keys=False).apply(lambda x: x.fillna(0).cumsum())
         market = (price * noncash["size"]).groupby(level=date_level).sum()
         market = market.reindex(cash.index).fillna(0)
         value = market + cash
         turnover = (delta / value.shift(1)).fillna(0)
 
@@ -245,15 +245,15 @@
             if not (benchmark==0).all():
                 year = (data[['net_value', 'exvalue', 'benchmark']].resample('Y').last() - data[['net_value', 'exvalue', 'benchmark']].resample('Y').first())
             else:
                 year = (data['net_value'].resample('Y').last() - data['net_value'].resample('Y').first())
             month = (data['net_value'].resample('M').last() - data['net_value'].resample('M').first())
             year.index = year.index.year
             year.plot(ax=ax[0,1], kind='bar', title="Yearly Return", rot=45, colormap='Paired')
-            ax[0, 2].bar(month.index, month.values, width=20)
+            ax[0, 2].bar(month.index, month.values, width=20, title='Monthly Return')
 
 
             ax10 = data['exvalue'].plot(ax=ax[1,0], title='Extra Return', legend=True)
             ax10.legend(loc='lower left')
             ax10.set_ylabel("Cumulative Return")
             ax10_twi = ax[1,0].twinx()
             ax10_twi.fill_between(data.index, 0, data['exdrawdown'], color='#009100', alpha=0.3)
```

### Comparing `quool-5.0.7/quool/table.py` & `quool-5.0.8/quool/table.py`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/quool/util.py` & `quool-5.0.8/quool/util.py`

 * *Files identical despite different names*

### Comparing `quool-5.0.7/quool.egg-info/PKG-INFO` & `quool-5.0.8/quool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quool
-Version: 5.0.7
+Version: 5.0.8
 Summary: Quantitative Toolkit - a helper in quant developping
 Home-page: https://github.com/ppoak/quool
 Author: ppoak
 Author-email: ppoak@foxmail.com
 Keywords: quant,framework,finance
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quool-5.0.7/setup.py` & `quool-5.0.8/setup.py`

 * *Files identical despite different names*

