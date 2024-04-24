# Comparing `tmp/thetagang-1.9.1.tar.gz` & `tmp/thetagang-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.9.1.tar", max compression
+gzip compressed data, was "thetagang-1.9.2.tar", max compression
```

## Comparing `thetagang-1.9.1.tar` & `thetagang-1.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    34523 2024-01-10 20:31:22.290995 thetagang-1.9.1/LICENSE
--rw-r--r--   0        0        0    14488 2024-01-10 20:31:22.290995 thetagang-1.9.1/README.md
--rw-r--r--   0        0        0     1758 2024-01-10 20:31:22.290995 thetagang-1.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/__init__.py
--rw-r--r--   0        0        0    10529 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/config.py
--rw-r--r--   0        0        0     1659 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/entry.py
--rw-r--r--   0        0        0     1091 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/fmt.py
--rw-r--r--   0        0        0     1022 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/main.py
--rw-r--r--   0        0        0      377 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/options.py
--rw-r--r--   0        0        0    85491 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/test_util.py
--rwxr-xr-x   0        0        0    12513 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/thetagang.py
--rw-r--r--   0        0        0     8399 2024-01-10 20:31:22.294995 thetagang-1.9.1/thetagang/util.py
--rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 thetagang-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-01-12 17:34:47.777806 thetagang-1.9.2/LICENSE
+-rw-r--r--   0        0        0    14488 2024-01-12 17:34:47.777806 thetagang-1.9.2/README.md
+-rw-r--r--   0        0        0     1758 2024-01-12 17:34:47.777806 thetagang-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/__init__.py
+-rw-r--r--   0        0        0    10701 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/config.py
+-rw-r--r--   0        0        0     1659 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/main.py
+-rw-r--r--   0        0        0      377 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/options.py
+-rw-r--r--   0        0        0    85499 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/test_util.py
+-rwxr-xr-x   0        0        0    12513 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/thetagang.py
+-rw-r--r--   0        0        0     9192 2024-01-12 17:34:47.781806 thetagang-1.9.2/thetagang/util.py
+-rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 thetagang-1.9.2/PKG-INFO
```

### Comparing `thetagang-1.9.1/LICENSE` & `thetagang-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/README.md` & `thetagang-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/pyproject.toml` & `thetagang-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.9.1"
+version = "1.9.2"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
 ib_insync = "^0.9.86"
 python = ">=3.9,<3.13"
 python-dateutil = "^2.8.1"
```

### Comparing `thetagang-1.9.1/thetagang/config.py` & `thetagang-1.9.2/thetagang/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
                     Optional("write_threshold_sigma"): And(float, lambda n: n > 0),
                     Optional("calls"): {
                         Optional("delta"): And(float, lambda n: 0 <= n <= 1),
                         Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                         Optional("write_threshold_sigma"): And(float, lambda n: n > 0),
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                         Optional("maintain_high_water_mark"): bool,
+                        Optional("cap_factor"): And(float, lambda n: 0 <= n <= 1),
+                        Optional("cap_target_floor"): And(float, lambda n: 0 <= n <= 1),
                     },
                     Optional("puts"): {
                         Optional("delta"): And(float, lambda n: 0 <= n <= 1),
                         Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                         Optional("write_threshold_sigma"): And(float, lambda n: n > 0),
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                     },
```

### Comparing `thetagang-1.9.1/thetagang/config_defaults.py` & `thetagang-1.9.2/thetagang/config_defaults.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/dict_merge.py` & `thetagang-1.9.2/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/fmt.py` & `thetagang-1.9.2/thetagang/fmt.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/main.py` & `thetagang-1.9.2/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/portfolio_manager.py` & `thetagang-1.9.2/thetagang/portfolio_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,15 @@
                         for p in portfolio_positions[symbol]
                         if isinstance(p.contract, Stock)
                     ]
                 )
             )
 
             target_short_calls = get_target_calls(
-                self.config, stock_count, self.target_quantities[symbol]
+                self.config, symbol, stock_count, self.target_quantities[symbol]
             )
             new_contracts_needed = target_short_calls - short_call_count
             excess_calls = short_call_count - target_short_calls
 
             if excess_calls > 0:
                 self.has_excess_calls.add(symbol)
                 call_actions_table.add_row(
```

### Comparing `thetagang-1.9.1/thetagang/test_util.py` & `thetagang-1.9.2/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/thetagang.py` & `thetagang-1.9.2/thetagang/thetagang.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.9.1/thetagang/util.py` & `thetagang-1.9.2/thetagang/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from datetime import datetime
 from typing import Optional
 
-from ib_insync import PortfolioItem, TagValue, util
+from ib_insync import PortfolioItem, TagValue, Ticker, util
 from ib_insync.contract import Option
 
 from thetagang.options import option_dte
 
 
 def account_summary_to_dict(account_summary):
     d = dict()
@@ -97,74 +97,98 @@
             "Exhausted retries waiting on predicate. This shouldn't happen."
         )
     if pred():
         body(remaining)
         wait_n_seconds(pred, body, seconds_to_wait, started_at)
 
 
-def get_higher_price(ticker) -> float:
+def get_higher_price(ticker: Ticker) -> float:
     # Returns the highest of either the option model price, the midpoint, or the
     # market price. The midpoint is usually a bit higher than the IB model's
     # pricing, but we want to avoid leaving money on the table in cases where
     # the spread might be messed up. This may in some cases make it harder for
     # orders to fill in a given day, but I think that's a reasonable tradeoff to
     # avoid leaving money on the table.
-    if ticker.modelGreeks:
+    if ticker.modelGreeks and ticker.modelGreeks.optPrice:
         return max([midpoint_or_market_price(ticker), ticker.modelGreeks.optPrice])
     return midpoint_or_market_price(ticker)
 
 
-def get_lower_price(ticker) -> float:
+def get_lower_price(ticker: Ticker) -> float:
     # Same as get_highest_price(), except get the lower price instead.
-    if ticker.modelGreeks:
+    if ticker.modelGreeks and ticker.modelGreeks.optPrice:
         return min([midpoint_or_market_price(ticker), ticker.modelGreeks.optPrice])
     return midpoint_or_market_price(ticker)
 
 
-def midpoint_or_market_price(ticker) -> float:
+def midpoint_or_market_price(ticker: Ticker) -> float:
     # As per the ib_insync docs, marketPrice returns the last price first, but
     # we often prefer the midpoint over the last price. This function pulls the
     # midpoint first, then falls back to marketPrice() if midpoint is nan.
     if util.isNan(ticker.midpoint()):
-        if util.isNan(ticker.marketPrice()) and ticker.modelGreeks:
+        if (
+            util.isNan(ticker.marketPrice())
+            and ticker.modelGreeks
+            and ticker.modelGreeks.optPrice
+        ):
             # Fallback to the model price if the greeks are available
             return ticker.modelGreeks.optPrice
         else:
             return ticker.marketPrice()
 
     return ticker.midpoint()
 
 
-def get_target_delta(config, symbol, right):
+def get_target_delta(config: dict, symbol: str, right: str):
     p_or_c = "calls" if right.upper().startswith("C") else "puts"
     if (
         p_or_c in config["symbols"][symbol]
         and "delta" in config["symbols"][symbol][p_or_c]
     ):
         return config["symbols"][symbol][p_or_c]["delta"]
     if "delta" in config["symbols"][symbol]:
         return config["symbols"][symbol]["delta"]
     if p_or_c in config["target"]:
         return config["target"][p_or_c]["delta"]
     return config["target"]["delta"]
 
 
+def get_cap_factor(config: dict, symbol: str):
+    if (
+        "calls" in config["symbols"][symbol]
+        and "cap_factor" in config["symbols"][symbol]["calls"]
+    ):
+        return config["symbols"][symbol]["calls"]["cap_factor"]
+    return config["write_when"]["calls"]["cap_factor"]
+
+
+def get_cap_target_floor(config: dict, symbol: str):
+    if (
+        "calls" in config["symbols"][symbol]
+        and "cap_target_floor" in config["symbols"][symbol]["calls"]
+    ):
+        return config["symbols"][symbol]["calls"]["cap_target_floor"]
+    return config["write_when"]["calls"]["cap_target_floor"]
+
+
 def get_strike_limit(config: dict, symbol: str, right: str) -> Optional[float]:
     p_or_c = "calls" if right.upper().startswith("C") else "puts"
     if (
         p_or_c in config["symbols"][symbol]
         and "strike_limit" in config["symbols"][symbol][p_or_c]
     ):
         return config["symbols"][symbol][p_or_c]["strike_limit"]
     return None
 
 
-def get_target_calls(config: dict, current_shares: int, target_shares: int) -> int:
-    cap_factor = config["write_when"]["calls"]["cap_factor"]
-    cap_target_floor = config["write_when"]["calls"]["cap_target_floor"]
+def get_target_calls(
+    config: dict, symbol: str, current_shares: int, target_shares: int
+) -> int:
+    cap_factor = get_cap_factor(config, symbol)
+    cap_target_floor = get_cap_target_floor(config, symbol)
     min_uncovered = (target_shares * cap_target_floor) // 100
     max_covered = (current_shares * cap_factor) // 100
     total_coverable = current_shares // 100
 
     return max([0, math.floor(min([max_covered, total_coverable - min_uncovered]))])
```

### Comparing `thetagang-1.9.1/PKG-INFO` & `thetagang-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.9.1
+Version: 1.9.2
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

