# Comparing `tmp/amplify-model-0.1.1.tar.gz` & `tmp/amplify_model-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplify-model-0.1.1.tar", max compression
+gzip compressed data, was "amplify_model-0.1.2.tar", max compression
```

## Comparing `amplify-model-0.1.1.tar` & `amplify_model-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0    11348 2022-06-29 09:12:44.566643 amplify-model-0.1.1/LICENSE
--rw-r--r--   0        0        0     1478 2022-06-29 10:20:42.169998 amplify-model-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/__init__.py
--rw-r--r--   0        0        0        0 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/src/__init__.py
--rw-r--r--   0        0        0     1172 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/src/data_classes.py
--rw-r--r--   0        0        0    56397 2022-08-02 11:05:26.396533 amplify-model-0.1.1/amplify/src/flex_calculation.py
--rw-r--r--   0        0        0        0 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0     3496 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/full_result_test_accept_long_trades_scenarios.txt
--rw-r--r--   0        0        0    12905 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/test_accept_long_trades_scenarios.py
--rw-r--r--   0        0        0     3420 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/test_accept_short_trades_scenarios.py
--rw-r--r--   0        0        0     6141 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/test_ppr_detection.py
--rw-r--r--   0        0        0     6987 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/test_total_flex_calculation.py
--rw-r--r--   0        0        0     3512 2022-06-29 09:12:44.566643 amplify-model-0.1.1/amplify/tests/unit_tests/util/aggregate_flexibility.py
--rw-r--r--   0        0        0     1274 2022-06-29 09:12:44.570643 amplify-model-0.1.1/amplify/tests/unit_tests/util/analyze_single_scenario.py
--rw-r--r--   0        0        0    26385 2022-06-29 09:12:44.570643 amplify-model-0.1.1/amplify/tests/unit_tests/util/generate_trades.py
--rw-r--r--   0        0        0     2298 2022-06-29 09:12:44.570643 amplify-model-0.1.1/amplify/tests/unit_tests/util/place_mpos.py
--rw-r--r--   0        0        0      596 2022-08-02 06:36:16.702417 amplify-model-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2391 2022-08-02 11:11:37.295272 amplify-model-0.1.1/setup.py
--rw-r--r--   0        0        0     2243 2022-08-02 11:11:37.295777 amplify-model-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-01-02 08:59:08.656707 amplify_model-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1478 2024-01-02 08:59:57.165532 amplify_model-0.1.2/README.md
+-rw-r--r--   0        0        0       81 2024-01-02 08:59:57.165532 amplify_model-0.1.2/amplify/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:59:57.165532 amplify_model-0.1.2/amplify/src/__init__.py
+-rw-r--r--   0        0        0     6737 2024-04-24 19:49:44.900533 amplify_model-0.1.2/amplify/src/amplify.py
+-rw-r--r--   0        0        0     1749 2024-04-24 19:49:44.900533 amplify_model-0.1.2/amplify/src/data_classes.py
+-rw-r--r--   0        0        0    85755 2024-04-24 19:49:44.904529 amplify_model-0.1.2/amplify/src/flex_calculation.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:59:57.169532 amplify_model-0.1.2/amplify/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:59:57.169532 amplify_model-0.1.2/amplify/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0      967 2024-01-02 08:59:57.169532 amplify_model-0.1.2/amplify/tests/unit_tests/general/evaluate_execution_time.py
+-rw-r--r--   0        0        0  9231527 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/general/execution_time.csv
+-rw-r--r--   0        0        0        0 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/general/results_execution_time.txt
+-rw-r--r--   0        0        0     6141 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/general/test_ppr_detection.py
+-rw-r--r--   0        0        0     7148 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/general/test_total_flex_calculation.py
+-rw-r--r--   0        0        0     3496 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/mpos/full_result_test_accept_long_trades_scenarios.txt
+-rw-r--r--   0        0        0    12905 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/mpos/test_accept_long_trades_scenarios.py
+-rw-r--r--   0        0        0     7471 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/mpos/test_accept_short_cap-mpos_scenarios.py
+-rw-r--r--   0        0        0     4163 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/mpos/test_accept_short_trades_scenarios.py
+-rw-r--r--   0        0        0     3512 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/util/aggregate_flexibility.py
+-rw-r--r--   0        0        0     1274 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/util/analyze_single_scenario.py
+-rw-r--r--   0        0        0     3183 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/util/generate_capacity_trades.py
+-rw-r--r--   0        0        0    26841 2024-04-24 19:49:44.904529 amplify_model-0.1.2/amplify/tests/unit_tests/util/generate_trades.py
+-rw-r--r--   0        0        0     2298 2024-01-02 08:59:57.213533 amplify_model-0.1.2/amplify/tests/unit_tests/util/place_mpos.py
+-rw-r--r--   0        0        0      671 2024-04-24 19:49:44.904529 amplify_model-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 amplify_model-0.1.2/PKG-INFO
```

### Comparing `amplify-model-0.1.1/LICENSE` & `amplify_model-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/README.md` & `amplify_model-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/amplify/src/data_classes.py` & `amplify_model-0.1.2/amplify/src/data_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,7 +35,28 @@
     """
     flex_without_mpo: Flexibility
     flex_with_mpo: Flexibility
     t_create: int
     t_start: int
     res: int
     problems: List[Problem]
+
+class MarketFlexibility (NamedTuple):
+    """
+    This class holds maximum and minimum power and energy of market 
+    flexibility
+    """
+    allowed_max_energy_delta: List[float]
+    allowed_min_energy_delta: List[float]
+    allowed_max_power: List[int]
+    allowed_min_power: List[int]
+
+class MarketFlexibilityCalculation(NamedTuple):
+    """
+    This class holds all the information of a market flex calculation
+    """
+    flex_with_mpo: MarketFlexibility
+    flex_without_mpo: MarketFlexibility
+    t_create: int
+    t_start: int
+    res: int
+    problems: List[Problem]
```

### Comparing `amplify-model-0.1.1/amplify/src/flex_calculation.py` & `amplify_model-0.1.2/amplify/src/flex_calculation.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 plex module of a storage agent and handles all the internal logic for
 calculating flexibility.
 """
 
 import time
 from math import ceil as ceil
 from math import floor as floor
+from math import isnan as isnan
 from typing import List, Tuple, Optional
 import logging
+import copy
 from .data_classes import FlexibilityCalculation, Flexibility, Problem
 
 
 module = "amplify"
 name = "flex_calculation"
 logger = logging.getLogger(f'{module}.{name}')
 
@@ -44,15 +46,15 @@
         self.capacity_energy = capacity_energy * soh  # [Wh]
         self.efficiency_charge = efficiency_charge  # [0,1]
         self.efficiency_discharge = efficiency_discharge  # [0,1]
         self.soh = soh
         self.problem_detection_horizon = problem_detection_horizon  # [s]
 
         # # DEBUG:
-        self.PPR_print = False
+        self.PPR_print = False # True # 
 
     def update(self, *, max_p_bat: int, min_p_bat: int,
                soh: float):
         """
         Updates the flex calculator
         :param max_p_bat: Maximum power of the battery (>0) [W]
         :param min_p_bat: Minimum power of the battery (<0) [W]
@@ -100,15 +102,16 @@
         if energy_diff > 0:
             total_energy = energy_diff / self.efficiency_charge  # [Wh]
         else:
             total_energy = energy_diff * self.efficiency_discharge  # [Wh]
 
         # consider the time period
         external_power = total_energy * 60 * 60 / duration  # [W]
-
+        if isnan(external_power):
+            external_power = 0
         return int(round(external_power))
 
     def calculate_start_soc_of_current_interval(
             self, *, curr_soc: float, avg_p_bat_of_curr_interval: int,
             passed_time_of_curr_interval: int) -> float:
         """
         Step 0
@@ -127,22 +130,25 @@
         start_soc = curr_soc - soc_change_from_interval_start
         # TODO start_soc has to be in [0,1]. Errors could be possible due to the parametrized constant efficiencies.
         start_soc = min(1., start_soc)
         start_soc = max(0., start_soc)
 
         return start_soc
 
-    def calculate_available_power_range(self, *, forecast: List[Optional[int]],
-                                        p_max_ps: List[int],
-                                        mpos: List[int],
-                                        avg_p_bat_of_curr_interval: int,
-                                        passed_time_of_curr_interval: int,
-                                        res: int,
-                                        critical_interval: int = 0) \
-            -> Tuple[List[int], List[int], List[Problem]]:
+    def calculate_available_power_range(
+        self, *, 
+        forecast: List[Optional[int]],
+        p_max_ps: List[int],
+        mpos: List[int],
+        cap_mpos: List[int]=None,
+        avg_p_bat_of_curr_interval: int,
+        passed_time_of_curr_interval: int,
+        res: int,
+        critical_interval: int = 0
+    ) -> Tuple[List[int], List[int], List[Problem]]:
         """
         Step 1
         Calculates the available power range (min of power diff and p_max).
         The power in the current interval respects the already realized storage
         power.
         :param forecast: the load forecast [W]
         :param p_max_ps: the p_max for peak shaving per interval [W]
@@ -156,14 +162,16 @@
         """
 
         # synchronize lengths of vectors from forecast, peak shaving power
         # and mpos
         logger.debug(f'{len(forecast)}, {len(p_max_ps)}, {len(mpos)}')
         assert len(forecast) == len(p_max_ps) == len(mpos), \
             (len(forecast), len(p_max_ps), len(mpos))
+        if cap_mpos is not None:
+            assert len(mpos) == len(cap_mpos)
         problems: List[Problem] = []
         power_diff = [x - y if y is not None else None
                       for x, y in zip(p_max_ps, forecast)]
         # get power diff
         # power range for p_max is min of power diff and physical constraint
         available_max_power = [min(x, self.max_p_bat) if x is not None
                                else self.max_p_bat for x in power_diff]
@@ -195,15 +203,15 @@
                         print('Step 1: Problem P1.1 registered.')
                     problems.append(Problem(
                         problem_type='P1.1', interval_no=interval_no,
                         negotiation_required=False, required=max_value,
                         realizable=current_p_min))
 
 
-        # respect trades
+        # respect normal mpos/trades
         for interval_no, mpo_value in enumerate(mpos):
             # print(str((interval_no,mpo_value)))
             if mpo_value > 0:
                 # charge trade
                 if mpo_value > available_max_power[interval_no]:
                     # print(f'MPO>0: {mpo_value}')
                     # we cannot fulfill trade, do as much as you can
@@ -240,23 +248,56 @@
                             realizable=available_min_power[interval_no]))
                 else:
                     # we can fulfill trade, so we should at least provide the
                     # power
                     # print(str((interval_no,mpo_value)))
                     available_max_power[interval_no] = \
                         min(mpos[interval_no], available_max_power[interval_no])
-        # print('Max: '+str(available_max_power))
-        # print('Min: '+str(available_min_power))
+
+        # TODO: Move to own method
+        if cap_mpos is not None:
+        # detect problems with capacity mpos/trades
+            for interval_no, mpo_value in enumerate(cap_mpos):
+                if interval_no < critical_interval:
+                    # print(str((interval_no,mpo_value)))
+
+                    if mpo_value > 0:
+                        # charge capacity trade
+                        available_power = available_max_power[interval_no] - \
+                            max(0, available_min_power[interval_no])
+                        if mpo_value > available_power:
+                            # cannot fulfill capMPO
+                            if self.PPR_print:
+                                print('Step 1: Problem P11.2 registered (capacity charge).')
+                            problems.append(Problem(
+                                problem_type='P11.2', interval_no=interval_no,
+                                negotiation_required=True, required=mpo_value,
+                                realizable=available_power))
+
+                    elif mpo_value < 0:
+                        # print(str((interval_no,mpo_value, available_min_power[interval_no])))
+                        # discharge trade
+                        available_power = available_min_power[interval_no] - \
+                            min(0, available_max_power[interval_no])
+                        if mpo_value < available_power:
+                            # we cannot fulfill trade, remove it
+                            if self.PPR_print:
+                                print('Step 1: Problem P11.2 registered (capacity discharge).')
+                            problems.append(Problem(
+                                problem_type='P11.2', interval_no=interval_no,
+                                negotiation_required=True, required=mpo_value,
+                                realizable=available_power))
 
         return available_max_power, available_min_power, problems
 
     def calculate_soc_flexibility_backward(
             self, *, available_max_power: List[int],
             available_min_power: List[int],
-            final_min_soc: float = 0., final_max_soc: float = 1.,
+            final_min_soc: float = 0., 
+            final_max_soc: float = 1.,
             res: int = 15 * 60) -> Tuple[List[float], List[float]]:
         """
         Step 2b: Calculate the required SoC range for the end of each
         interval
         ATTENTION: This has changed to the end of the interval
         :param available_max_power: the maximum available power
         calculated in step 1 [W]
@@ -273,20 +314,53 @@
 
         assert len(available_max_power) == len(available_min_power)
 
         # initialize return lists (-1. is just a placeholder)
         period = len(available_max_power)
         required_max_soc = [-1.] * period
         required_min_soc = [-1.] * period
+        # add the final socs to the end of the list
+        required_max_soc[-1] = final_max_soc
+        required_min_soc[-1] = final_min_soc
 
-        max_soc_at_interval_start = final_max_soc
-        min_soc_at_interval_start = final_min_soc
+        required_max_soc, required_min_soc = \
+            self.backward_integration(
+                available_max_power=available_max_power,
+                available_min_power=available_min_power,
+                required_max_soc=required_max_soc,
+                required_min_soc=required_min_soc,
+                start_index=period - 1,
+                res=res
+        )
+        return required_max_soc, required_min_soc
+
+    def backward_integration(self,
+        available_max_power: List[float],
+        available_min_power: List[float],
+        required_max_soc: List[float],
+        required_min_soc: List[float],
+        start_index: int = None,
+        ppr_detection = False,
+        res: int = 15 * 60
+    ):
+        required_max_soc = copy.deepcopy(required_max_soc)
+        required_min_soc = copy.deepcopy(required_min_soc)
+        if start_index is None:
+            start_index = len(available_max_power)-1
+        
+        if start_index >= len(available_max_power):
+            raise ValueError("Cannot start behind last value.")
+        else:
+            max_soc_at_interval_start = required_max_soc[start_index]
+            min_soc_at_interval_start = required_min_soc[start_index]
+        assert 0 <= max_soc_at_interval_start <= 1
+        assert 0 <= min_soc_at_interval_start <= 1
 
-        # starts at the last interval, until interval 1
-        for interval_no in range(period - 1, 0, -1):
+        # default: starts at the last interval, until interval 1
+        for interval_no in range(start_index, 0, -1):
             # required start soc values of next interval are required end
             # soc values for this interval
             max_soc_at_interval_end = max_soc_at_interval_start
             min_soc_at_interval_end = min_soc_at_interval_start
 
             # get maximum soc change on the basis of the available max power
             # (can be < 0 if discharging is required)
@@ -315,18 +389,14 @@
                 # no problem detection here so max is 1
                 min_soc_at_interval_start = 1
 
             # the required at the end of last interval must be this start
             required_max_soc[interval_no - 1] = max_soc_at_interval_start
             required_min_soc[interval_no - 1] = min_soc_at_interval_start
 
-        # add the final socs to the end of the list
-        required_max_soc[-1] = final_max_soc
-        required_min_soc[-1] = final_min_soc
-
         return required_max_soc, required_min_soc
 
     def calculate_soc_flexibility_forward(
             self, *, available_max_power: List[int],
             available_min_power: List[int],
             start_soc: float, res: int = 15 * 60, critical_interval_max: int = 0,
             critical_interval_min: int = 0, ) \
@@ -430,14 +500,80 @@
         if min_max_soc[-1][1] >= 0:
             min_max_soc.pop()
         if max_min_soc[-1][1] <= 1:
             max_min_soc.pop()
 
         return reachable_max_soc, reachable_min_soc, (min_max_soc, max_min_soc)
 
+    def forward_integration(self,
+        available_max_power: List[float],
+        available_min_power: List[float],
+        reachable_max_soc: List[float],
+        reachable_min_soc: List[float], 
+        start_index: int = None,
+        start_soc: float = None,
+        res: int = 15 * 60
+    ):
+        reachable_max_soc = copy.deepcopy(reachable_max_soc)
+        reachable_min_soc = copy.deepcopy(reachable_min_soc)
+        assert (start_index is not None) or \
+            (start_soc is not None)
+        if start_index is None:
+            # Maximum and minimum are defined by soc_start
+            max_soc_at_interval_end = start_soc
+            min_soc_at_interval_end = start_soc
+            start_index = 0
+        if start_soc is None:
+            max_soc_at_interval_end = reachable_max_soc[start_index - 1]
+            min_soc_at_interval_end = reachable_min_soc[start_index - 1]
+        if (start_index is not None) and \
+            (start_soc is not None):
+            max_soc_at_interval_end = start_soc
+            min_soc_at_interval_end = start_soc
+        logger.debug(f'Forward integration: Start index: {start_index}')
+        # print(f'Max available before forward: {available_max_power}')
+        # print(f'Min available before forward: {available_min_power}')
+        # print(f'Max reachable before forward: {reachable_max_soc}')
+        # print(f'Min reachable before forward: {reachable_min_soc}')
+        period = len(available_max_power)
+        for current_interval in range(start_index, period):
+            # start values are the end values of last interval
+            max_soc_at_interval_start = max_soc_at_interval_end
+            min_soc_at_interval_start = min_soc_at_interval_end
+            # print(f'Max start: {max_soc_at_interval_start}, min start: {min_soc_at_interval_start}')
+
+            # get maximum soc change on the basis of the available max power
+            # (can be < 0 if discharging is required)
+            max_soc_change = self.power_to_soc_diff(
+                power=available_max_power[current_interval], duration=res
+            )
+            # print('max_soc_change: '+str(max_soc_change))
+            # get minimum soc change on the basis of the available min power
+            # (can be > 0 if charging is required)
+            min_soc_change = self.power_to_soc_diff(
+                power=available_min_power[current_interval], duration=res
+            )
+            # print(f'Max: {max_soc_change}, min: {min_soc_change}')
+            # what soc can be reached at the end of the interval
+            max_soc_at_interval_end = min(1.0, max_soc_at_interval_start +
+                                          max_soc_change)
+            min_soc_at_interval_end = max(0.0, min_soc_at_interval_start +
+                                          min_soc_change)
+            # print(f'Max end: {max_soc_at_interval_end}, min end: {min_soc_at_interval_end}')
+            # swap if min>max
+            if min_soc_at_interval_end > max_soc_at_interval_end:
+                min_soc_at_interval_end, max_soc_at_interval_end = \
+                    max_soc_at_interval_end, min_soc_at_interval_end
+
+            # place updated values in vector
+            reachable_max_soc[current_interval] = max_soc_at_interval_end
+            reachable_min_soc[current_interval] = min_soc_at_interval_end
+
+        return reachable_max_soc, reachable_min_soc
+
     @classmethod
     def calculate_allowed_soc_range(
             cls, *, required_max_soc: List[float],
             required_min_soc: List[float], reachable_max_soc: List[float],
             reachable_min_soc: List[float], critical_interval: int = 0, ) \
             -> Tuple[List[float], List[float]]:
         """
@@ -484,14 +620,284 @@
             allowed_max_soc.append(
                 min(required_max_soc[current_interval],
                     reachable_max_soc[current_interval])
             )
 
         return allowed_max_soc, allowed_min_soc
 
+    @classmethod
+    def calculate_allowed_soc_range_with_uncertainty(
+            cls, *, max_soc_1: List[float],
+            min_soc_1: List[float], max_soc_2: List[float],
+            min_soc_2: List[float], critical_interval: int = 0, ) \
+            -> Tuple[List[float], List[float]]:
+        """
+        Step 2d: Calculate the allowed soc range at the end of each interval
+        :param max_soc_1: Required max socs
+        :param min_soc_1: Required min socs
+        :param max_soc_2: Reachable max socs
+        :param min_soc_2: Reachable min socs
+        :param critical_interval: first interval without problem detection
+        :return: allowed_max_soc, allowed_min_soc
+        """
+
+        # all lists have to have the same length
+        assert len(max_soc_1) == len(min_soc_1) == \
+               len(max_soc_2) == len(min_soc_2), \
+            f'Length of lists are not equal, ' \
+            f'len of no_1 is {len(max_soc_1)} ' \
+            f'and len of no_2 is {len(max_soc_2)}'
+
+        period = len(min_soc_1)
+
+        allowed_min_soc = []
+        allowed_max_soc = []
+        logger.debug(f'Integrate reachable: Max 1: {max_soc_1}')
+        logger.debug(f'Integrate reachable: Min 1: {min_soc_1}')
+        logger.debug(f'Integrate reachable: Max 2: {max_soc_2}')
+        logger.debug(f'Integrate reachable: Min 2: {min_soc_2}')
+                
+
+        for current_interval in range(period):
+            # remove problems, in which case these intervals do not
+            # overlap! Possible in case of very large, unshavable peaks
+            if max_soc_1[current_interval] < \
+                min_soc_2[current_interval] or \
+                min_soc_1[current_interval] > \
+                max_soc_2[current_interval]:
+
+                allowed_max_soc.append(float('NaN'))
+                allowed_min_soc.append(float('NaN'))
+            else:
+                # max SoC is min of max_required and max_reachable
+                allowed_max_soc.append(
+                    min(max_soc_1[current_interval],
+                        max_soc_2[current_interval])
+                )
+                
+                # min SoC is max of min_required and min_reachable
+                allowed_min_soc.append(
+                    max(min_soc_1[current_interval],
+                        min_soc_2[current_interval])
+                )
+                
+        return allowed_max_soc, allowed_min_soc
+
+    def integrate_cap_mpos_into_allowed_soc(
+        self, 
+        start_soc: float,
+        available_max_power: List[float], 
+        available_min_power: List[float], 
+        required_max_soc: List[float], 
+        required_min_soc: List[float], 
+        reachable_max_soc: List[float], 
+        reachable_min_soc: List[float], 
+        allowed_max_soc: List[float], 
+        allowed_min_soc: List[float],
+        mpos: List[float],
+        cap_mpos: List[float], 
+        res: int = 15 * 60,
+        critical_interval: int = 0
+    ) -> Tuple[List[float], List[float], List[float], List[Problem]]:
+        """Step 2d: Consider capacity mpos in allowed soc range.
+        :param available_max_power: the maximum available power
+        calculated in step 1 [W]
+        :param available_min_power: the minimum available power
+        calculated in step 1 [W]
+        :param required_max_soc: Required max socs (calculated in step 2b)
+        :param required_min_soc: Required min socs (calculated in step 2b)
+        :param reachable_max_soc: Reachable max socs (calculated in step 2a)
+        :param reachable_min_soc: Reachable min socs (calculated in step 2a)
+        :param allowed_max_soc: Allowed max socs (calculated in step 2c)
+        :param allowed_min_soc: Allowed min socs (calculated in step 2c)
+        :param cap_mpos: Capacity mpos
+        :param critical_interval: first interval without problem detection
+        :return: allowed_max_soc, allowed_min_soc
+        """
+        possible_max_power = copy.deepcopy(available_max_power)
+        possible_min_power = copy.deepcopy(available_min_power)
+        problems: List[Problem] = []
+
+        # adjust available to possible power including cap mpos
+        for interval_no in range(len(cap_mpos)):
+            mpo_value = mpos[interval_no]
+            cap_mpo_value = cap_mpos[interval_no]
+            mpo_sum = mpo_value + cap_mpo_value
+            if (cap_mpo_value > 0 or cap_mpo_value < 0):
+                # a cap mpo is placed at the interval
+                # check for power ppr
+                if interval_no < critical_interval and \
+                    (available_max_power[interval_no] < mpo_sum or \
+                    available_min_power[interval_no] > mpo_sum):
+                    # create problem
+                    if self.PPR_print:
+                        print('Step 1: Problem P11.3 registered (overlapping mpos).')
+                    problems.append(Problem(
+                        problem_type='P11.3', interval_no=interval_no,
+                        negotiation_required=True, required=cap_mpo_value,
+                        realizable=0))
+                    cap_mpos[interval_no] = 0
+                    continue # skip this cap_mpo
+                else: # no problem -> set default values
+                    # possible_max_power[interval_no] = mpo_value
+                    # possible_min_power[interval_no] = mpo_value
+                    # in case of discharge obligation
+                    if possible_max_power[interval_no] < 0:
+                        possible_min_power[interval_no] = \
+                            possible_max_power[interval_no]
+                    # in case of charge obligation
+                    elif possible_min_power[interval_no] > 0:
+                        possible_max_power[interval_no] = \
+                            possible_min_power[interval_no]
+                    else: # in case of no obligation
+                        possible_max_power[interval_no] = 0
+                        possible_min_power[interval_no] = 0
+                # add cap_mpo_value to max/min possible power
+                if cap_mpo_value < 0:
+                    possible_max_power[interval_no] = \
+                        possible_max_power[interval_no] + cap_mpo_value
+                if cap_mpo_value > 0:
+                    possible_min_power[interval_no] = \
+                        possible_min_power[interval_no] + cap_mpo_value
+                
+                logger.debug(f'Prepare cap-MPO integration: Max available: {available_max_power}')
+                logger.debug(f'Prepare cap-MPO integration: Min available: {available_min_power}')
+                logger.debug(f'Prepare cap-MPO integration: Max possible: {possible_max_power}')
+                logger.debug(f'Prepare cap-MPO integration: Min possible: {possible_min_power}')
+
+                # limit required soc range by capacity mpo and backward integ.
+                required_max_soc, required_min_soc = \
+                    self.backward_integration(
+                        available_max_power=possible_max_power,
+                        available_min_power=possible_min_power,
+                        required_max_soc=required_max_soc,
+                        required_min_soc=required_min_soc,
+                        start_index=interval_no,
+                        res=res
+                    )
+                logger.debug(f'Cap-MPO integration: Max required after backward: {required_max_soc}')
+                logger.debug(f'Cap-MPO integration: Min required after backward: {required_min_soc}')
+
+                # integrate limitation into reachable soc range for limited
+                # initial values
+                reachable_max_soc, reachable_min_soc = \
+                    self.calculate_allowed_soc_range(
+                        required_max_soc=required_max_soc,
+                        required_min_soc=required_min_soc,
+                        reachable_max_soc=allowed_max_soc,
+                        reachable_min_soc=allowed_min_soc,
+                    )
+                
+                logger.debug(f'Cap-MPO integration: Max reachable after backward: {reachable_max_soc}')
+                logger.debug(f'Cap-MPO integration: Min reachable after backward: {reachable_min_soc}')
+
+                # check for energy ppr
+                if interval_no == 0:
+                    start_soc_max = start_soc
+                    start_soc_min = start_soc
+                else:
+                    start_soc_max = reachable_max_soc[interval_no - 1]
+                    start_soc_min = reachable_min_soc[interval_no - 1]
+
+                max_power = max(cap_mpo_value, mpo_sum) # TODO: Hier den mpo_value ergänzen?
+                min_power = min(cap_mpo_value, mpo_sum)
+
+                max_max_soc = start_soc_max + self.power_to_soc_diff(
+                    power=max_power, duration=res
+                )
+                min_max_soc = start_soc_max + self.power_to_soc_diff(
+                    power=min_power, duration=res
+                )
+                max_min_soc = start_soc_min + self.power_to_soc_diff(
+                    power=max_power, duration=res
+                )
+                min_min_soc = start_soc_min + self.power_to_soc_diff(
+                    power=min_power, duration=res
+                )
+                logger.debug(f'Cap-MPO integration: Max soc: {(max_max_soc, min_max_soc)}')
+                logger.debug(f'Cap-MPO integration: Min soc: {(max_min_soc, min_min_soc)}')
+                # TODO: Evtl. reicht es zu überprüfen, ob der rückgerechnete max. Anfangswert unter dem min. Anfangswert liegt:
+                # F^max_start < F^min_start => PPR
+                if min(max_max_soc, max_min_soc) > allowed_max_soc[interval_no] or \
+                    max(min_max_soc, min_min_soc) < allowed_min_soc[interval_no]:
+
+                    # print(f'Max allowed: {allowed_max_soc}')
+                    # print(f'Min allowed: {allowed_min_soc}')
+                    # create problem
+                    if self.PPR_print:
+                        print('Step 2d: Problem P12.3 registered (overlapping mpos).')
+                        logger.debug(f'Step 2d: Problem P12.3 registered (overlapping mpos) in interval {interval_no}.')
+                    problems.append(Problem(
+                        problem_type='P12.3', interval_no=interval_no,
+                        negotiation_required=True, required=mpo_sum,
+                        realizable=mpo_value))
+                    cap_mpos[interval_no] = 0
+                    continue # skip this cap_mpo
+
+                possible_max_power[interval_no] = mpo_value
+                possible_min_power[interval_no] = mpo_value
+                logger.debug(f'Cap-MPO integration: Max possible: {possible_max_power}')
+                logger.debug(f'Cap-MPO integration: Min possible: {possible_min_power}')
+                
+                # limit reachable soc range by capacity mpo and forward integ.
+                reachable_max_soc_p0, reachable_min_soc_p0 = \
+                    self.forward_integration(
+                        available_max_power=possible_max_power,
+                        available_min_power=possible_min_power,
+                        reachable_max_soc=reachable_max_soc,
+                        reachable_min_soc=reachable_min_soc,
+                        start_index=interval_no,
+                        res=res
+                    )
+                
+                logger.debug(f'Cap-MPO integration: Max reachable_0 after forward: {reachable_max_soc_p0}')
+                logger.debug(f'Cap-MPO integration: Min reachable_0 after forward: {reachable_min_soc_p0}')
+
+                possible_max_power[interval_no] = mpo_sum
+                possible_min_power[interval_no] = mpo_sum
+                logger.debug(f'Cap-MPO integration: Max possible: {possible_max_power}')
+                logger.debug(f'Cap-MPO integration: Min possible: {possible_min_power}')
+
+                # limit reachable soc range by capacity mpo and forward integ.
+                reachable_max_soc_pcapmpo, reachable_min_soc_pcapmpo = \
+                    self.forward_integration(
+                        available_max_power=possible_max_power,
+                        available_min_power=possible_min_power,
+                        reachable_max_soc=reachable_max_soc,
+                        reachable_min_soc=reachable_min_soc,
+                        start_index=interval_no,
+                        res=res
+                    )
+                
+                logger.debug(f'Cap-MPO integration: Max reachable_pcapmpo after forward: {reachable_max_soc_pcapmpo}')
+                logger.debug(f'Cap-MPO integration: Min reachable_pcapmpo after forward: {reachable_min_soc_pcapmpo}')
+                logger.debug(f'Cap-MPO integration: Max reachable_p0 after forward: {reachable_max_soc_p0}')
+                logger.debug(f'Cap-MPO integration: Min reachable_p0 after forward: {reachable_min_soc_p0}')
+                # integrate all limitation into allowed soc range
+                # TODO: nur, wenn vorher kein PPR in diesem Intervall mit Cap-MPO aufgetreten ist
+                reachable_max_soc, reachable_min_soc = \
+                    self.calculate_allowed_soc_range_with_uncertainty(
+                        max_soc_1=reachable_max_soc_p0,
+                        min_soc_1=reachable_min_soc_p0,
+                        max_soc_2=reachable_max_soc_pcapmpo,
+                        min_soc_2=reachable_min_soc_pcapmpo,
+                    )
+                allowed_max_soc, allowed_min_soc = \
+                    self.calculate_allowed_soc_range_with_uncertainty(
+                        max_soc_1=reachable_max_soc,
+                        min_soc_1=reachable_min_soc,
+                        max_soc_2=allowed_max_soc,
+                        min_soc_2=allowed_min_soc,
+                    )
+
+                logger.debug(f'Cap-MPO integration: Max allowed: {allowed_max_soc}')
+                logger.debug(f'Cap-MPO integration: Min allowed: {allowed_min_soc}')
+
+        return allowed_max_soc, allowed_min_soc, cap_mpos, problems
+
     def convert_soc_range_to_energy_flex(
             self, *, max_soc: List[float], min_soc: List[float],
             start_soc: float, max_power: List[int], min_power: List[int]) \
             -> Tuple[List[int], List[int]]:
         """
         Step 3: Converts the allowed soc range to energy flexibility
         at the end of each interval, which
@@ -508,96 +914,118 @@
         assert len(max_soc) == len(min_soc) == len(max_power) == len(min_power)
         max_energy_delta = []
         min_energy_delta = []
 
         for interval_no in range(len(max_soc)):
             current_max_soc = max_soc[interval_no]
             current_min_soc = min_soc[interval_no]
-            if min_power[interval_no] > 0: # obligatory charge:
-                current_max_energy_delta = \
-                    int(floor((current_max_soc - start_soc) * \
-                    self.capacity_energy))
-                current_min_energy_delta = \
-                    min(current_max_energy_delta,
-                        int(ceil((current_min_soc - start_soc) * \
-                        self.capacity_energy))
-                    )
-            else: # obligatory discharge or standard case
-                current_min_energy_delta = \
-                    int(ceil((current_min_soc - start_soc) * \
-                    self.capacity_energy))
-                current_max_energy_delta = \
-                    max(current_min_energy_delta,
+            if isnan(current_max_soc) or isnan(current_min_soc):
+                current_max_energy_delta = None
+                current_min_energy_delta = None
+            else:
+                if min_power[interval_no] > 0: # obligatory charge:
+                    current_max_energy_delta = \
                         int(floor((current_max_soc - start_soc) * \
                         self.capacity_energy))
-                    )
+                    current_min_energy_delta = \
+                        min(current_max_energy_delta,
+                            int(ceil((current_min_soc - start_soc) * \
+                            self.capacity_energy))
+                        )
+                else: # obligatory discharge or standard case
+                    current_min_energy_delta = \
+                        int(ceil((current_min_soc - start_soc) * \
+                        self.capacity_energy))
+                    current_max_energy_delta = \
+                        max(current_min_energy_delta,
+                            int(floor((current_max_soc - start_soc) * \
+                            self.capacity_energy))
+                        )
             max_energy_delta.append(current_max_energy_delta)
             min_energy_delta.append(current_min_energy_delta)
 
         return max_energy_delta, min_energy_delta
 
     def increase_min_soc_by_discharge_efficiency_losses(
             self, *, max_soc: List[float], min_soc: List[float],
             allowed_max_power: List[float], allowed_min_power: List[float],
+            cap_mpos: List[float] = None,
             res: int = 15 * 60, start_soc: float, critical_interval: int = 0,
             debug_print: bool) \
             -> Tuple[List[int], List[int]]:
         """
         Step 3: increases the min_soc to respect the discharge efficiency
         :param max_soc: list of max soc values [0,1]
         :param min_soc: list of min soc values [0,1]
         :param allowed_max_power: allowed max power calculated in step 4
         :param allowed_min_power: allowed min power calculated in step 4
         :param res: Resolution [s], defaults to 15 * 60
         :param start_soc: the starting soc [0,1]
         :param critical_interval: first interval without problem detection
         :return: max_soc, increased_min_soc
         """
-
+        # TODO: Cap-MPOs berücksichtigen
         assert len(min_soc) == len(max_soc) == \
                len(allowed_min_power) == len(allowed_max_power)
 
         period = len(allowed_max_power)
 
         increased_max_soc = [0.0] * len(min_soc)
         increased_min_soc = [0.0] * len(min_soc)
 
         for current_interval in range(period):
             if current_interval == 0:
                 increased_min_soc[current_interval] = min_soc[current_interval]
 
             else:
                 # go back in time
+                max_soc_before_current_min_buffer = 0
                 for earlier_interval in range(current_interval, -1, -1):
                     if earlier_interval == current_interval:
                         # initialize max_soc_before_current_min
                         # which contains the max_soc from which min_soc
                         # of the current_interval can be reached
                         max_soc_before_current_min = \
                             min_soc[current_interval]
                         max_soc_before_current_min_power = \
                             min_soc[current_interval]
                     else:
                         # increase max_soc_before_current_min_power
                         # due to discharge power
+                        min_power = allowed_min_power[earlier_interval]
+                        if cap_mpos is not None and cap_mpos[earlier_interval] < 0:
+                            min_power = cap_mpos[earlier_interval]
                         max_soc_before_current_min_power = \
                             max_soc_before_current_min_power - \
-                            min(0, allowed_min_power[earlier_interval]) / \
+                            min(0, min_power) / \
                             self.efficiency_discharge * res / self.capacity_energy
                         # set max_soc_before_current_min
                         max_soc_before_current_min = min(
                             max_soc[earlier_interval],
                             max_soc_before_current_min_power
                         )
-                        # stop in case of mandatory charging or
-                        # in case of a lower earlier max soc
-                        if allowed_min_power[earlier_interval] > 0 or \
-                            (max_soc_before_current_min > max_soc[earlier_interval-1]
+                        if (max_soc_before_current_min > max_soc[earlier_interval-1]
                             and earlier_interval >= 0):
+                            # store max_soc_before_current_min if higher value was found
+                            max_soc_before_current_min_buffer = \
+                                max(max_soc_before_current_min, 
+                                max_soc_before_current_min_buffer)
+                    # stop in case of mandatory charging or charge mpo or
+                    # in case of a lower earlier max soc
+                    if cap_mpos is None:
+                        if allowed_min_power[earlier_interval] > 0:
+                            break
+                    else:
+                        if allowed_min_power[earlier_interval] > 0 or \
+                            (cap_mpos[earlier_interval] is not None and cap_mpos[earlier_interval] > 0):
                             break
+                max_soc_before_current_min = max(
+                    max_soc_before_current_min,
+                    max_soc_before_current_min_buffer
+                )
                 if debug_print:
                     print(f'Max SoC before current min in {current_interval}: {max_soc_before_current_min}')
                 delta_soc_till_current_interval = \
                     max_soc_before_current_min - min_soc[current_interval]
                 delta_soc_till_current_interval = \
                     max(0, delta_soc_till_current_interval)
                 # # Case 1: Increase by (1/eta-1)
@@ -623,15 +1051,15 @@
             print(f'Increased max soc: {increased_max_soc}')
             print(f'Increased min soc: {increased_min_soc}')
         return increased_max_soc, increased_min_soc
 
     def calculate_allowed_power_flexibility(
             self, *, allowed_max_soc: List[float],
             allowed_min_soc: List[float], available_max_power: List[int],
-            available_min_power: List[int], res: int = 15 * 60,
+            available_min_power: List[int], mpos = None, res: int = 15 * 60,
             start_soc: float, critical_interval: int = 0) \
             -> Tuple[List[int], List[int]]:
         """
         Step 4: calculates the allowed power range
         :param allowed_max_soc: Allowed max SoC calculated in step 3
         :param allowed_min_soc: Allowed min SoC calculated in step 3
         :param available_max_power: available max power calculated in step 1
@@ -640,14 +1068,17 @@
         :param start_soc: the start soc at the beginning of interval 0
         :param critical_interval: first interval without problem detection
         :return: allowed_max_power, allowed_min_power
         """
 
         assert len(allowed_min_soc) == len(allowed_max_soc) == \
                len(available_min_power) == len(available_max_power)
+            
+        if mpos is None:
+            mpos = [0.0] * len(allowed_min_soc)
 
         period = len(available_max_power)
 
         allowed_max_power = []
         allowed_min_power = []
 
         for current_interval in range(period):
@@ -664,14 +1095,19 @@
 
             # convert SoC diff to power per interval
             max_power_from_soc = self.soc_diff_to_power(soc_diff=max_soc_diff,
                                                         duration=res)
             min_power_from_soc = self.soc_diff_to_power(soc_diff=min_soc_diff,
                                                         duration=res)
 
+            if max_power_from_soc == 0 and min_power_from_soc == 0 and \
+                mpos[current_interval] != 0:
+                max_power_from_soc = mpos[current_interval]
+                min_power_from_soc = mpos[current_interval]
+
             # maximum allowed power is min of max_power_from_soc
             # and power_range_max
             allowed_max_power.append(
                 min(max_power_from_soc, available_max_power[current_interval])
             )
 
             # minimum allowed power is max of min_power_from_soc
@@ -689,17 +1125,86 @@
                 else:
                     allowed_max_power[-1] = 0
                     allowed_min_power[-1] = 0
 
         return allowed_max_power, allowed_min_power
 
 
+    def integrate_cap_mpos_into_allowed_power(
+        self,
+        available_max_power: List[float], 
+        available_min_power: List[float],
+        allowed_max_power: List[float], 
+        allowed_min_power: List[float],
+        mpos: List[float], 
+        cap_mpos: List[float], 
+        res: int = 15 * 60,
+        critical_interval: int = 0
+    ) -> Tuple[List[float], List[float]]:
+
+        for interval_no in range(len(cap_mpos)):
+            mpo_value = mpos[interval_no]
+            cap_mpo_value = cap_mpos[interval_no]
+
+            if cap_mpo_value > 0:
+                reduced_avail_power = available_max_power[interval_no] - \
+                    cap_mpo_value
+                if interval_no < critical_interval:
+                    assert reduced_avail_power >= 0
+                logger.debug(f'Cap-MPO into p_allowed: {reduced_avail_power}')
+                logger.debug(f'Cap-MPO into p_allowed: {allowed_max_power[interval_no]}')
+                allowed_max_power[interval_no] = min(
+                    allowed_max_power[interval_no],
+                    reduced_avail_power
+                )
+                logger.debug(f'Cap-MPO into p_allowed: {allowed_max_power[interval_no]}')
+                # set max power to discharge mpo or zero
+                if mpo_value > 0: # opposing mpos have to be excluded before
+                    assert allowed_min_power[interval_no] >= 0
+                allowed_min_power[interval_no] = max(
+                    allowed_min_power[interval_no],
+                    mpo_value # normally 0
+                )
+                # limit min power to max power
+                allowed_min_power[interval_no] = min(
+                    allowed_max_power[interval_no],
+                    allowed_min_power[interval_no],
+                    
+                )
+
+            if cap_mpo_value < 0:
+                reduced_avail_power = available_min_power[interval_no] - \
+                    cap_mpo_value
+                if interval_no < critical_interval:
+                    assert reduced_avail_power <= 0
+                allowed_min_power[interval_no] = max(
+                    allowed_min_power[interval_no],
+                    reduced_avail_power
+                )
+                # set max power to discharge mpo or zero
+                if mpo_value < 0: # opposing mpos have to be excluded before
+                    assert allowed_max_power[interval_no] <= 0
+                allowed_max_power[interval_no] = min(
+                    allowed_max_power[interval_no],
+                    mpo_value # normally 0
+                )
+                # limit max power to min power
+                allowed_max_power[interval_no] = max(
+                    allowed_max_power[interval_no],
+                    allowed_min_power[interval_no],
+                )
+        logger.debug(f'Cap-MPO into p_allowed: {allowed_max_power}')
+        logger.debug(f'Cap-MPO into p_allowed: {allowed_min_power}')
+
+        return allowed_max_power, allowed_min_power
+
     def calculate_total_flex(self, *, forecast: List[int],
                              p_max_ps: List[int],
                              mpos: List[int],
+                             cap_mpos: List[int] = None,
                              curr_soc: float,
                              final_min_soc: float = 0.0,
                              final_max_soc: float = 1.0,
                              avg_p_bat_of_curr_interval: int,
                              passed_time_of_curr_interval: int,
                              res: int = 15 * 60, t_start: int) \
             -> FlexibilityCalculation:
@@ -717,18 +1222,20 @@
         :param res: the resolution to use [s]
         :param t_start: start of the flexibility [Unix Timestamp]
         :return: namedtuple FlexibilityCalculation
         """
         # for debugging only:
         logger.debug(f'Forecast: {forecast[0:int(self.problem_detection_horizon/res)]}')
         logger.debug(f'Multi Purpose Orders: {mpos[0:int(self.problem_detection_horizon/res)]}')
+        if cap_mpos is not None: logger.debug(f'Capacity Multi Purpose Orders: {cap_mpos[0:int(self.problem_detection_horizon/res)]}')
         logger.debug(f'Inputs: p_grid: {p_max_ps}, curr_soc: {curr_soc}, res: {res}')
         #
 
         if self.PPR_print: print('MPOS: ' + str(mpos))
+        if self.PPR_print: print('Cap-MPOS: ' + str(cap_mpos))
 
         # Step 0
         if self.PPR_print:
             print('Step 0')
         start_soc = self.calculate_start_soc_of_current_interval(
             curr_soc=curr_soc,
             avg_p_bat_of_curr_interval=avg_p_bat_of_curr_interval,
@@ -739,14 +1246,20 @@
         critical_interval_number = self.problem_detection_horizon // res
         logger.debug(f'Critical_interval_number: {critical_interval_number}')
         # print(f'Critical Inverval: {self.problem_detection_horizon}')
         # print(f'Critical Inverval Number: {critical_interval_number}')
 
         problems: List[Problem] = []
         unproblematic_mpos: List[int] = mpos.copy()
+        
+        if cap_mpos is not None:
+            unproblematic_cap_mpos: List[int] = cap_mpos.copy()
+        else:
+            # unproblematic_cap_mpos = [0]*len(mpos)
+            unproblematic_cap_mpos = None
 
         # Only Peak Shaving:
         # Step 1 (a) without MPOs
         if self.PPR_print:
             print('Step 1 (a)')
         # Problems are not given to unit module for now
         available_max_power_no_mpo, available_min_power_no_mpo, _ = \
@@ -845,34 +1358,38 @@
         if self.PPR_print:
             print('Step 1 (b)')
 
         ## for debugging only:
         # print(f'Forecast: {forecast[0:int(self.problem_detection_horizon/res)]}')
         # print(f'Multi Purpose Orders: {unproblematic_mpos[0:int(self.problem_detection_horizon/res)]}')
         ##
-
+        
         available_max_power_with_mpo, available_min_power_with_mpo, \
         p1_problems = self.calculate_available_power_range(
             forecast=forecast, p_max_ps=p_max_ps,
             mpos=unproblematic_mpos,
+            cap_mpos=unproblematic_cap_mpos,
             avg_p_bat_of_curr_interval=avg_p_bat_of_curr_interval,
             res=res,
             passed_time_of_curr_interval=passed_time_of_curr_interval,
             critical_interval=critical_interval_number
         )
         logger.debug('1(b): Max available power: '+str(available_max_power_with_mpo))
         logger.debug('1(b): Min available power: '+str(available_min_power_with_mpo))
         logger.debug('1(b): Problems: '+str(p1_problems))
 
-        # store the open neg requests
+        # store the open negotiation requests
         for problem in p1_problems:
             problems.append(problem)
             if problem.problem_type.lower() in ('p1.3', 'p1.2'):
                 unproblematic_mpos[problem.interval_no] -= \
                     problem.required - problem.realizable
+            elif problem.problem_type.lower() in ('p11.2'):
+                unproblematic_cap_mpos[problem.interval_no] -= \
+                    problem.required - problem.realizable
 
         # Step 2a (b) with MPOs
         if self.PPR_print:
             print('Step 2a (b)')
         reachable_max_soc_with_mpo, reachable_min_soc_with_mpo, \
         extreme_values_with_mpo = \
             self.calculate_soc_flexibility_forward(
@@ -993,15 +1510,15 @@
                     available_min_power=available_min_power_with_mpo,
                     start_soc=start_soc, res=res,
                     critical_interval_max=0,
                     critical_interval_min=0,
                 )
 
         # Step 2b calculate required SoC range
-        # at this point all problems are detected and stored in problems
+        # at this point all mpo problems are detected and stored in problems
         # Step 2b (a) without MPOs
         required_max_soc_no_mpo, required_min_soc_no_mpo = \
             self.calculate_soc_flexibility_backward(
                 available_max_power=available_max_power_no_mpo,
                 available_min_power=available_min_power_no_mpo,
                 final_min_soc=final_min_soc, final_max_soc=final_max_soc,
                 res=res
@@ -1030,15 +1547,44 @@
             self.calculate_allowed_soc_range(
                 required_max_soc=required_max_soc_with_mpo,
                 required_min_soc=required_min_soc_with_mpo,
                 reachable_max_soc=reachable_max_soc_with_mpo,
                 reachable_min_soc=reachable_min_soc_with_mpo,
                 critical_interval=critical_interval_number
             )
-
+        
+        # Step 2d integrate capacity MPOs
+        logger.debug(f'Before cap-MPOs integration: Max allowed soc: {allowed_max_soc_with_mpo}')
+        logger.debug(f'Before cap-MPOs integration: Min allowed soc: {allowed_min_soc_with_mpo}')
+        if cap_mpos is not None:
+            allowed_max_soc_with_mpo, \
+            allowed_min_soc_with_mpo, \
+            unproblematic_cap_mpos, \
+            p10_problems = \
+                self.integrate_cap_mpos_into_allowed_soc(
+                    start_soc=start_soc,
+                    available_max_power=available_max_power_with_mpo,
+                    available_min_power=available_min_power_with_mpo,
+                    required_max_soc=required_max_soc_with_mpo,
+                    required_min_soc=required_min_soc_with_mpo,
+                    reachable_max_soc=reachable_max_soc_with_mpo,
+                    reachable_min_soc=reachable_min_soc_with_mpo,
+                    allowed_max_soc=allowed_max_soc_with_mpo,
+                    allowed_min_soc=allowed_min_soc_with_mpo,
+                    mpos=unproblematic_mpos,
+                    cap_mpos=unproblematic_cap_mpos,
+                    critical_interval=critical_interval_number
+                )
+                
+            logger.debug(f'Cap-MPOs integrated: Max allowed soc: {allowed_max_soc_with_mpo}')
+            logger.debug(f'Cap-MPOs integrated: Min allowed soc: {allowed_min_soc_with_mpo}')
+            # store the open negotiation requests
+            for problem in p10_problems:
+                problems.append(problem)
+                
         # Step 3 calculate allowed power flexibility
         # Step 3 (a) without mpo
 
         # print('# 977 Allowed max power')
         # print('wo MPO')
         allowed_max_power_no_mpo, allowed_min_power_no_mpo = \
             self.calculate_allowed_power_flexibility(
@@ -1053,39 +1599,61 @@
         # print('w MPO')
         allowed_max_power_with_mpo, allowed_min_power_with_mpo = \
             self.calculate_allowed_power_flexibility(
                 allowed_max_soc=allowed_max_soc_with_mpo,
                 allowed_min_soc=allowed_min_soc_with_mpo,
                 available_max_power=available_max_power_with_mpo,
                 available_min_power=available_min_power_with_mpo,
+                mpos=unproblematic_mpos,
                 res=res, start_soc=start_soc,
                 critical_interval=critical_interval_number
             )
+        logger.debug(f'Before cap-MPOs integration: Max allowed power: {allowed_max_power_with_mpo}')
+        logger.debug(f'Before cap-MPOs integration: Min allowed power: {allowed_min_power_with_mpo}')
+
+        # Step 3b integrate capacity MPOs
+        if cap_mpos is not None:
+            allowed_max_power_with_mpo, allowed_min_power_with_mpo = \
+                self.integrate_cap_mpos_into_allowed_power(
+                available_max_power=available_max_power_with_mpo,
+                available_min_power=available_min_power_with_mpo,
+                allowed_max_power=allowed_max_power_with_mpo,
+                allowed_min_power=allowed_min_power_with_mpo,
+                mpos=unproblematic_mpos,
+                cap_mpos=unproblematic_cap_mpos,
+                res=res,
+                critical_interval=critical_interval_number
+            )
+            logger.debug(f'Cap-MPOs integrated: Max allowed power: {allowed_max_power_with_mpo}')
+            logger.debug(f'Cap-MPOs integrated: Min allowed power: {allowed_min_power_with_mpo}')
 
         # Step 4 calculate energy flexibility/delta energy
         # increase min_soc to respect discharge efficiency
         # Step 4a (a) without mpo
         # print('# 962 Allowed max power')
         # print('wo MPO')
         allowed_max_incr_soc_no_mpo, allowed_min_incr_soc_no_mpo = \
             self.increase_min_soc_by_discharge_efficiency_losses(
                 max_soc=allowed_max_soc_no_mpo,
                 min_soc=allowed_min_soc_no_mpo,
                 allowed_max_power=allowed_max_power_no_mpo,
                 allowed_min_power=allowed_min_power_no_mpo,
                 res=res, start_soc=start_soc,
-                critical_interval=critical_interval_number, debug_print=False)
+                critical_interval=critical_interval_number, 
+                debug_print=False
+            )
         # Step 4a (b) with mpo
         # print('w MPO')
         allowed_max_incr_soc_with_mpo, allowed_min_incr_soc_with_mpo = \
             self.increase_min_soc_by_discharge_efficiency_losses(
                 max_soc=allowed_max_soc_with_mpo,
                 min_soc=allowed_min_soc_with_mpo,
                 allowed_max_power=allowed_max_power_with_mpo,
                 allowed_min_power=allowed_min_power_with_mpo,
+                cap_mpos=unproblematic_cap_mpos,
                 res=res, start_soc=start_soc,
                 critical_interval=critical_interval_number, debug_print=False)
 
         # convert to energy flexibility
         # Step 4b (a) without mpo
         allowed_max_energy_delta_no_mpo, allowed_min_energy_delta_no_mpo = \
             self.convert_soc_range_to_energy_flex(
@@ -1141,9 +1709,11 @@
             res=res,
             flex_with_mpo=result_with_mpo,
             flex_without_mpo=result_no_mpo,
             problems=problems,
         )
         if self.PPR_print:
             print(f'Probleme: {problems}')
+        
+        logger.debug(f'Result of flex calculation: {result}')
 
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/full_result_test_accept_long_trades_scenarios.txt` & `amplify_model-0.1.2/amplify/tests/unit_tests/mpos/full_result_test_accept_long_trades_scenarios.txt`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/test_accept_long_trades_scenarios.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/mpos/test_accept_long_trades_scenarios.py`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/test_accept_short_trades_scenarios.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/mpos/test_accept_short_trades_scenarios.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 import pytest
 from copy import deepcopy
 from amplify.src.flex_calculation import *
 from amplify.tests.unit_tests.util.generate_trades import *
 from amplify.tests.unit_tests.util.place_mpos import *
 
+import logging
+import time
+import os
+if not os.path.exists("logs"):
+    os.makedirs("logs")
+    
+level=logging.DEBUG
+timestr = time.strftime("%Y%m%d-%H%M%S")
+log_file="logs/test_"+timestr+".log"
+logging.basicConfig(filename=log_file, level=level)
+handler = logging.FileHandler(log_file)
+handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(name)s %(message)s'))
+logger = logging.getLogger("amplify.flex_calculation")
+logger.setLevel(level)
+logger.addHandler(handler)
+
 FLEX_CALC_PARAMS = ['max_p_bat', 'min_p_bat', 'capacity_energy', 'efficiency_charge', 'efficiency_discharge',
                  'soh', 'problem_detection_horizon']
 
 DEFAULT_PARAMETERS = {
     'max_p_bat': 100,
     'min_p_bat': -100,
     'capacity_energy': 100,
@@ -15,42 +31,47 @@
     'efficiency_discharge': 0.9,
     'soh': 1,
     'problem_detection_horizon': 16 * 15 * 60,
     'curr_soc': 0.55,
     'passed_time_of_curr_interval': 180,
     'avg_p_bat_of_curr_interval': 0,
     'mpos': [0] * 8,
+    'cap_mpos': [0] * 8,
     'final_min_soc': 0,
     'final_max_soc': 1,
     'forecast': [900, 1050, 1100, 1000, 1050, 850, 1000, 1100],
     'p_max_ps': [1000] * 8,
     't_start': 100,
     'res': 15 * 60
 }
 
 
 testdata = {
     'default': ({}),
     'capacity200': ({'capacity_energy': 200,}),
+    'mpo-cap1': ({
+        'forecast': [900, 1050, 1000, 1000, 1050, 850, 1000, 1100],
+        'cap_mpos': [0.0, 0.0, -50.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+    }),
 }
 
 
 @pytest.mark.parametrize(
     "adopted_params", testdata.values(), ids=testdata.keys()
 )
 def test_accept_short_trades(adopted_params):
     parameter_set = deepcopy(DEFAULT_PARAMETERS)
 
     for k, v in adopted_params.items():
         if k == 'forecast':
-            for interval, new_p in v:
+            for interval, new_p in enumerate(v):
                 # forecast adoptions are displayed differently
                 parameter_set['forecast'][interval] = new_p
         elif k == 'mpos':
-            for interval, new_p in v:
+            for interval, new_p in enumerate(v):
                 # forecast adoptions are displayed differently
                 parameter_set['mpos'][interval] = new_p
         else:
             parameter_set[k] = v
 
     # get params for flex calculator and create it
     flex_calculator_params = {}
@@ -60,14 +81,15 @@
             parameter_set.pop(k)
 
     flex_calculator = FlexCalculator(**flex_calculator_params)
     mpos_before_trades = parameter_set['mpos']
 
     flex_before_trades: FlexibilityCalculation = \
         flex_calculator.calculate_total_flex(**parameter_set)
+    print(f'Flex before trade: {flex_before_trades}')
 
     for startinterval_no in range(len(flex_before_trades.flex_with_mpo.allowed_min_power)):
     # place short power trades
         # charge trades
         if flex_before_trades.flex_with_mpo.allowed_max_power[startinterval_no] > 0:
             mpos_with_trades = generate_short_charge_trade(flex=flex_before_trades, mpos=mpos_before_trades, \
                 startinterval_no=startinterval_no)
```

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/test_ppr_detection.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/general/test_ppr_detection.py`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/test_total_flex_calculation.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/general/test_total_flex_calculation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from amplify.src.flex_calculation import *
 
-NUMBER_OF_TESTS_TO_RUN = 1000000
+NUMBER_OF_TESTS_TO_RUN = 10000000
 START_TEST_NO = 1
 
 # parameters for testing:
 MAX_P_BAT = [100, 75, 50]
 MIN_P_BAT = [-100, -75, -50]
 CAPACITY = [200, 100, 50]
 START_SOC = [0, 0.25, 0.5, 0.75, 1]
@@ -59,24 +59,30 @@
 @pytest.mark.parametrize(
     "sim_no", range(START_TEST_NO, min(START_TEST_NO + NUMBER_OF_TESTS_TO_RUN, MAX_TEST_NO))
 )
 def test_flex_calc(sim_no):
     max_p_bat, min_p_bat, capacity, start_soc, eff_charge, eff_discharge, (passed_time, avg_p_bat), mpos, \
         (final_min_soc, final_max_soc), forecast, p_max = get_parameters(sim_no)
 
+    t_start = time.time()
+
     flex_calculator: FlexCalculator = FlexCalculator(max_p_bat=max_p_bat, min_p_bat=min_p_bat, capacity_energy=capacity,
                                                      efficiency_charge=eff_charge, efficiency_discharge=eff_discharge)
 
     flex: FlexibilityCalculation = \
         flex_calculator.calculate_total_flex(curr_soc=start_soc, passed_time_of_curr_interval=passed_time,
                                              avg_p_bat_of_curr_interval=avg_p_bat,
                                              mpos=mpos, final_min_soc=final_min_soc,
                                              final_max_soc=final_max_soc, forecast=forecast, p_max_ps=p_max,
                                              t_start=0)
 
+    duration = round(time.time() - t_start, 6)
+    with open('execution_time.csv', mode='a') as f:
+        f.write(f'{duration}, ')
+
     failing_str = f'{get_parameters(sim_no, True)}\n' \
                   f'Allowed p: ' \
                   f'{list(zip(flex.flex_with_mpo.allowed_min_power, flex.flex_with_mpo.allowed_max_power))}\n' \
                   f'Allowed soc: ' \
                   f'{list(zip(flex.flex_with_mpo.allowed_min_soc, flex.flex_with_mpo.allowed_max_soc))}\n' \
                   f'Problems: {flex.problems}'
```

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/util/aggregate_flexibility.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/util/aggregate_flexibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     result = FlexibilityCalculation(
         t_create=flex1.t_create,
         t_start=flex1.t_start,
         res=flex1.res,
         flex_with_mpo=result_with_mpo,
         flex_without_mpo=result_no_mpo,
-        problems=flex1.problems.append(flex2.problems)
+        problems=flex1.problems.extend(flex2.problems)
     )
 
     if result.problems is not None:
         print(f'Probleme: {result.problems}')
 
     return result
```

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/util/analyze_single_scenario.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/util/analyze_single_scenario.py`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/util/generate_trades.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/util/generate_trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,291 +17,295 @@
     return mpos_with_trades
 
 def generate_long_fast_charge_trade(flex: FlexibilityCalculation, mpos, startinterval_no):
     """
     Generates a multi-time-step trade, which starts at startinterval_no and
     takes as much charge power as possible until the max energy level is reached
     """
-    print(f'Start interval: {startinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
+    # print(f'Start interval: {startinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
     charge_possible_until = len(flex.flex_with_mpo.allowed_min_power)
     duration = len(flex.flex_with_mpo.allowed_min_power) - startinterval_no
     for interval_no in range(startinterval_no, len(flex.flex_with_mpo.allowed_min_power)):
-        print(f'{interval_no} ',end='')
+        # print(f'{interval_no} ',end='')
         # verify charge is possible
-        if flex.flex_with_mpo.allowed_max_power[interval_no] < 0:
+        if flex.flex_with_mpo.allowed_max_power[interval_no] < 0 \
+            or flex.flex_with_mpo.allowed_max_energy_delta[interval_no] is None \
+            or flex.flex_with_mpo.allowed_min_energy_delta[interval_no] is None:
             charge_possible_until = interval_no
             duration = charge_possible_until - startinterval_no
             break
-    print(f'\nCharge possible until: {charge_possible_until}')
+    # print(f'\nCharge possible until: {charge_possible_until}')
     # generate multi-time-step trade
     trade_power = [0.0]*len(flex.flex_with_mpo.allowed_max_power)
     trade_energy_delta = [0.0]*(len(trade_power))
     if startinterval_no > 0:
         trade_energy_delta[startinterval_no-1] = flex.flex_with_mpo.allowed_min_energy_delta[startinterval_no-1]
 
     for interval_no in range(startinterval_no, charge_possible_until):
-        print(f'Initial energy level in {interval_no}: {trade_energy_delta[interval_no-1]}')
+        # print(f'Initial energy level in {interval_no}: {trade_energy_delta[interval_no-1]}')
         power_this_interval = flex.flex_with_mpo.allowed_max_power[interval_no]
-        print(f'One-step charge power in {interval_no}: {power_this_interval}')
+        # print(f'One-step charge power in {interval_no}: {power_this_interval}')
 
         # increase min energy level by max power
         increased_min_energy_delta = power_this_interval * 900/3600 + trade_energy_delta[interval_no-1]
-        print(f'Increased min energy level: {increased_min_energy_delta}, Max allowed energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no]}')
+        # print(f'Increased min energy level: {increased_min_energy_delta}, Max allowed energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no]}')
         if increased_min_energy_delta > flex.flex_with_mpo.allowed_max_energy_delta[interval_no]:
             # limit trade power in case of energy limit
             power_this_interval = (flex.flex_with_mpo.allowed_max_energy_delta[interval_no] - trade_energy_delta[interval_no-1]) / 900*3600
             if power_this_interval < max(0,flex.flex_with_mpo.allowed_min_power[interval_no]):
                 # interrupt if limited trade power not allowed
                 duration = interval_no-1
-                print(f'Break due to invalid power. Duration: {duration}')
+                # print(f'Break due to invalid power. Duration: {duration}')
                 break
 
         # update trade_energy_delta
         trade_energy_delta[interval_no] = trade_energy_delta[interval_no-1] + power_this_interval*900/3600
 
         if trade_energy_delta[interval_no] < flex.flex_with_mpo.allowed_min_energy_delta[interval_no] or \
             trade_energy_delta[interval_no] > flex.flex_with_mpo.allowed_max_energy_delta[interval_no]:
             # end trade if energy level not valid
             duration = interval_no-1
-            print(f'Break due to invalid energy. Duration: {duration}')
+            # print(f'Break due to invalid energy. Duration: {duration}')
             break
 
-        print(f'Current trade power in {interval_no}: {power_this_interval}')
+        # print(f'Current trade power in {interval_no}: {power_this_interval}')
         trade_power[interval_no] = power_this_interval
         assert trade_power[interval_no] >= 0, f'Trade power: {trade_power}'
 
-    print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
+    # print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
     mpos_with_trades = mpos.copy()
     for interval_no in range(startinterval_no, charge_possible_until):
         mpos_with_trades[interval_no] = mpos_with_trades[interval_no] + trade_power[interval_no]
         # mpos_with_trades[interval_no] = trade_power[interval_no]
 
     # validate_charge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
-    print(f'MPOs: {mpos_with_trades}')
+    # print(f'MPOs: {mpos_with_trades}')
     return mpos_with_trades
 
 def generate_long_fast_discharge_trade(flex: FlexibilityCalculation, mpos, startinterval_no):
     """
     Generates a multi-time-step trade, which starts at startinterval_no and
     takes as much discharge power as possible until the min energy level is reached
     """
-    print(f'Start interval: {startinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
+    # print(f'Start interval: {startinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
     discharge_possible_until = len(flex.flex_with_mpo.allowed_min_power)
     duration = len(flex.flex_with_mpo.allowed_min_power) - startinterval_no
     for interval_no in range(startinterval_no, len(flex.flex_with_mpo.allowed_min_power)):
-        print(f'{interval_no} ',end='')
+        # print(f'{interval_no} ',end='')
         # verify discharge is possible
-        if flex.flex_with_mpo.allowed_min_power[interval_no] > 0:
+        if flex.flex_with_mpo.allowed_min_power[interval_no] > 0 \
+            or flex.flex_with_mpo.allowed_max_energy_delta[interval_no] is None \
+            or flex.flex_with_mpo.allowed_min_energy_delta[interval_no] is None:
             discharge_possible_until = interval_no
             duration = discharge_possible_until - startinterval_no
             break
-    print(f'\nDischarge possible until: {discharge_possible_until}')
+    # print(f'\nDischarge possible until: {discharge_possible_until}')
     # generate multi-time-step trade
     trade_power = [0.0]*len(flex.flex_with_mpo.allowed_max_power)
     trade_energy_delta = [0.0]*(len(trade_power))
     if startinterval_no > 0:
         trade_energy_delta[startinterval_no-1] = flex.flex_with_mpo.allowed_max_energy_delta[startinterval_no-1]
 
     for interval_no in range(startinterval_no, discharge_possible_until):
-        print(f'Initial energy level in {interval_no}: {trade_energy_delta[interval_no-1]}')
+        # print(f'Initial energy level in {interval_no}: {trade_energy_delta[interval_no-1]}')
         power_this_interval = flex.flex_with_mpo.allowed_min_power[interval_no]
-        print(f'One-step discharge power in {interval_no}: {power_this_interval}')
+        # print(f'One-step discharge power in {interval_no}: {power_this_interval}')
 
         # decrease max energy level by min power
         decreased_max_energy_delta = power_this_interval * 900/3600 + trade_energy_delta[interval_no-1]
-        print(f'Decreased max energy level: {decreased_max_energy_delta}, Min allowed energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no]}')
+        # print(f'Decreased max energy level: {decreased_max_energy_delta}, Min allowed energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no]}')
         if decreased_max_energy_delta < flex.flex_with_mpo.allowed_min_energy_delta[interval_no]:
             # limit trade power in case of energy limit
             power_this_interval = (flex.flex_with_mpo.allowed_min_energy_delta[interval_no] - trade_energy_delta[interval_no-1]) / 900*3600
-            print(f'Limited trade power in {interval_no}: {power_this_interval}')
+            # print(f'Limited trade power in {interval_no}: {power_this_interval}')
             if power_this_interval > min(0,flex.flex_with_mpo.allowed_max_power[interval_no]):
                 # interrupt if limited trade power not allowed
                 duration = interval_no-1
-                print(f'Break due to invalid power. Duration: {duration}')
+                # print(f'Break due to invalid power. Duration: {duration}')
                 break
 
         # update trade_energy_delta
         trade_energy_delta[interval_no] = trade_energy_delta[interval_no-1] + power_this_interval*900/3600
 
         if trade_energy_delta[interval_no] < flex.flex_with_mpo.allowed_min_energy_delta[interval_no] or \
             trade_energy_delta[interval_no] > flex.flex_with_mpo.allowed_max_energy_delta[interval_no]:
             # end trade if energy level not valid
             duration = interval_no-1
-            print(f'Break due to invalid energy. Duration: {duration}')
+            # print(f'Break due to invalid energy. Duration: {duration}')
             break
 
-        print(f'Current trade power in {interval_no}: {power_this_interval}')
+        # print(f'Current trade power in {interval_no}: {power_this_interval}')
         trade_power[interval_no] = power_this_interval
         assert trade_power[interval_no] <= 0, f'Trade power: {trade_power}'
 
-    print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
+    # print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
     mpos_with_trades = mpos.copy()
     for interval_no in range(startinterval_no, discharge_possible_until):
         mpos_with_trades[interval_no] = mpos_with_trades[interval_no] + trade_power[interval_no]
         # mpos_with_trades[interval_no] = trade_power[interval_no]
 
     # validate_discharge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
-    print(f'MPOs: {mpos_with_trades}')
+    # print(f'MPOs: {mpos_with_trades}')
     return mpos_with_trades
 
 def generate_long_slow_charge_trade(flex: FlexibilityCalculation, mpos, endinterval_no):
     """
     Generates a multi-time-step trade, which ends at endinterval_no and previously
     takes as much charge power as possible until the min energy level is reached
     """
 
-    print(f'End interval: {endinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
+    # print(f'End interval: {endinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
     earliest_charge_start = 0 #len(flex.flex_with_mpo.allowed_min_power)
     startinterval_no = 0
     duration = endinterval_no+1
     # l=range(endinterval_no+1, -1, -1)
-    # print(l)
+    # # print(l)
     for interval_no in range(endinterval_no, -1, -1):
-        print(f'{interval_no} ',end='')
+        # print(f'{interval_no} ',end='')
         # verify charge is possible
         if flex.flex_with_mpo.allowed_max_power[interval_no] < 0 or \
             flex.flex_with_mpo.allowed_max_energy_delta[interval_no] < flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]:
             earliest_charge_start = interval_no+1
             startinterval_no = earliest_charge_start
             duration = endinterval_no - earliest_charge_start+1
-            print(f'\nEarliest charge start: {earliest_charge_start}')
+            # print(f'\nEarliest charge start: {earliest_charge_start}')
             break
     # generate multi-time-step trade
     trade_power = [0.0]*len(flex.flex_with_mpo.allowed_max_power)
     trade_energy_delta = [0.0]*(len(trade_power))
     trade_energy_delta[endinterval_no] = flex.flex_with_mpo.allowed_max_energy_delta[endinterval_no]
 
     if endinterval_no >= earliest_charge_start:
         for interval_no in range(endinterval_no, earliest_charge_start-1, -1):
-            print(f'{interval_no} ')
-            print(f'Trade energy start: {trade_energy_delta}')
-            print(f'Max Energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]}')
-            print(f'Min Energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]}')
+            # print(f'{interval_no} ')
+            # print(f'Trade energy start: {trade_energy_delta}')
+            # print(f'Max Energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]}')
+            # print(f'Min Energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]}')
             if interval_no > 0:
                 min_energy_delta_before = flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]
             elif interval_no == 0:
                 min_energy_delta_before = 0
-            print(f'Min energy delta beforce current interval: {min_energy_delta_before}')
+            # print(f'Min energy delta beforce current interval: {min_energy_delta_before}')
             if trade_energy_delta[interval_no] < min_energy_delta_before:
              # or trade_energy_delta[interval_no] < flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]:
                 # end trade if energy level exceeds limit
                 startinterval_no = interval_no+1
                 duration = endinterval_no - startinterval_no+1
-                print(f'Break due to invalid energy. Duration: {duration}')
-                print(f'Break trade power: {trade_power}')
+                # print(f'Break due to invalid energy. Duration: {duration}')
+                # print(f'Break trade power: {trade_power}')
                 break
 
             power_allowed_by_power = flex.flex_with_mpo.allowed_max_power[interval_no]
             power_allowed_by_energy = (trade_energy_delta[interval_no] - \
                 min_energy_delta_before) / 900*3600
 
             power_this_interval = min(power_allowed_by_power, power_allowed_by_energy)
-            print(f'Power this inverval: {power_this_interval}')
+            # print(f'Power this inverval: {power_this_interval}')
             if power_this_interval < flex.flex_with_mpo.allowed_min_power[interval_no]:
                 # end trade if power range is left
                 startinterval_no = interval_no+1
                 duration = endinterval_no - startinterval_no+1
-                print(f'Break due to invalid power. Duration: {duration}')
+                # print(f'Break due to invalid power. Duration: {duration}')
                 break
 
             # update trade_energy_delta
             trade_energy_delta[interval_no-1] = trade_energy_delta[interval_no] - power_this_interval*900/3600
 
-            print(f'Current trade power in {interval_no}: {power_this_interval}')
+            # print(f'Current trade power in {interval_no}: {power_this_interval}')
             trade_power[interval_no] = power_this_interval
             assert trade_power[interval_no] >= 0
 
-    print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
+    # print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
     mpos_with_trades = mpos.copy()
-    print('Start end', startinterval_no, endinterval_no)
-    print(mpos_with_trades, trade_power)
+    # print('Start end', startinterval_no, endinterval_no)
+    # print(mpos_with_trades, trade_power)
     for interval_no in range(startinterval_no, endinterval_no+1):
         mpos_with_trades[interval_no] = mpos_with_trades[interval_no] + trade_power[interval_no]
         # mpos_with_trades[interval_no] = trade_power[interval_no]
-    print(f'Final MPOs: {mpos_with_trades}')
+    # print(f'Final MPOs: {mpos_with_trades}')
 
     # validate_charge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
     return mpos_with_trades
 
 def generate_long_slow_discharge_trade(flex: FlexibilityCalculation, mpos, endinterval_no):
     """
     Generates a multi-time-step trade, which ends at endinterval_no and previously
     takes as much discharge power as possible until the max energy level is reached
     """
     # discharge trades
-    print(f'End interval: {endinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
+    # print(f'End interval: {endinterval_no}\nFlexibility: {flex.flex_with_mpo}\nMPOs: {mpos}')
     earliest_discharge_start = 0 #len(flex.flex_with_mpo.allowed_min_power)
     startinterval_no = 0
     duration = endinterval_no+1
     # l=range(endinterval_no+1, -1, -1)
-    # print(l)
+    # # print(l)
     for interval_no in range(endinterval_no, -1, -1):
-        print(f'{interval_no} ',end='')
+        # print(f'{interval_no} ',end='')
         # verify discharge is possible
         if flex.flex_with_mpo.allowed_min_power[interval_no] > 0 or \
             flex.flex_with_mpo.allowed_min_energy_delta[interval_no] > flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]:
             earliest_discharge_start = interval_no+1
             startinterval_no = earliest_discharge_start
             duration = endinterval_no - earliest_discharge_start+1
-            print(f'\nEarliest discharge start: {earliest_discharge_start}')
+            # print(f'\nEarliest discharge start: {earliest_discharge_start}')
             break
     # generate multi-time-step trade
     trade_power = [0.0]*len(flex.flex_with_mpo.allowed_min_power)
     trade_energy_delta = [0.0]*(len(trade_power))
     trade_energy_delta[endinterval_no] = flex.flex_with_mpo.allowed_min_energy_delta[endinterval_no]
 
     if endinterval_no >= earliest_discharge_start:
         for interval_no in range(endinterval_no, earliest_discharge_start-1, -1):
-            print(f'{interval_no} ')
-            print(f'Trade energy start: {trade_energy_delta}')
-            print(f'Max Energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]}')
-            print(f'Min Energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]}')
+            # print(f'{interval_no} ')
+            # print(f'Trade energy start: {trade_energy_delta}')
+            # print(f'Max Energy delta: {flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]}')
+            # print(f'Min Energy delta: {flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]}')
             if interval_no > 0:
                 max_energy_delta_before = flex.flex_with_mpo.allowed_max_energy_delta[interval_no-1]
             elif interval_no == 0:
                 max_energy_delta_before = 0
             if trade_energy_delta[interval_no] > max_energy_delta_before:
              # or trade_energy_delta[interval_no] < flex.flex_with_mpo.allowed_min_energy_delta[interval_no-1]:
                 # end trade if energy level exceeds limit
                 startinterval_no = interval_no+1
                 duration = endinterval_no - startinterval_no+1
-                print(f'Break due to invalid energy. Duration: {duration}')
+                # print(f'Break due to invalid energy. Duration: {duration}')
                 break
 
             power_allowed_by_power = flex.flex_with_mpo.allowed_min_power[interval_no]
             power_allowed_by_energy = (trade_energy_delta[interval_no] - \
                 max_energy_delta_before) / 900*3600
 
             power_this_interval = max(power_allowed_by_power, power_allowed_by_energy)
-            print(f'Power this inverval: {power_this_interval}')
+            # print(f'Power this inverval: {power_this_interval}')
             if power_this_interval > flex.flex_with_mpo.allowed_max_power[interval_no]:
                 # end trade if power range is left
                 startinterval_no = interval_no+1
                 duration = endinterval_no - startinterval_no+1
-                print(f'Break due to invalid power. Duration: {duration}')
+                # print(f'Break due to invalid power. Duration: {duration}')
                 break
 
             # update trade_energy_delta
             trade_energy_delta[interval_no-1] = trade_energy_delta[interval_no] - power_this_interval*900/3600
 
-            print(f'Current trade power in {interval_no}: {power_this_interval}')
+            # print(f'Current trade power in {interval_no}: {power_this_interval}')
             trade_power[interval_no] = power_this_interval
             assert trade_power[interval_no] <= 0
 
-    print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
+    # print(f'Final trade power: {trade_power}\nFinal start interval: {startinterval_no}, final duration: {duration}')
     mpos_with_trades = mpos.copy()
-    print('Start end', startinterval_no, endinterval_no)
-    print(mpos_with_trades, trade_power)
+    # print('Start end', startinterval_no, endinterval_no)
+    # print(mpos_with_trades, trade_power)
     for interval_no in range(startinterval_no, endinterval_no+1):
         mpos_with_trades[interval_no] = mpos_with_trades[interval_no] + trade_power[interval_no]
         # mpos_with_trades[interval_no] = trade_power[interval_no]
-    print(f'Final MPOs: {mpos_with_trades}')
+    # print(f'Final MPOs: {mpos_with_trades}')
 
     # validate_discharge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
     return mpos_with_trades
 
 def validate_charge_trade(flex, mpos_with_trades, startinterval_no, duration):
     # validate trade
@@ -346,15 +350,15 @@
         max_energy_delta = flex.flex_with_mpo.allowed_max_energy_delta[interval_no]
         min_energy_delta = flex.flex_with_mpo.allowed_min_energy_delta[interval_no]
         assert max_energy_delta >= max_energy + mpos_with_trades[interval_no]*900/3600 >= min_energy_delta, \
             f'Left allowed energy range: {mpos_with_trades}, in interval: {interval_no}\n' \
             f'Planned trade: {mpos_with_trades}, begin at index: {startinterval_no}\nFlexibility: {flex.flex_with_mpo}'
 
         max_energy = max_energy + mpos_with_trades[interval_no]*900/3600
-        print(max_energy)
+        # print(max_energy)
 
 def generate_long_medium_charge_trade(flex: FlexibilityCalculation, mpos, startinterval_no, duration):
     """
     Generate a multi-time-step trade, which starts at startinterval_no and of
     duration length, only if at all corresponding time intervals charging is
     allowed.
     The trade takes as much charge power as possible until a dip in the allowed
@@ -365,15 +369,15 @@
     charge_possible = True
     for d in range(duration):
         # verify charge is possible
         if flex.flex_with_mpo.allowed_max_power[startinterval_no+d] < 0:
             charge_possible = False
     # generate multi-time-step trade
     trade_power = [0.0]*duration
-    print(f'Charge possible: {charge_possible}')
+    # print(f'Charge possible: {charge_possible}')
     if charge_possible:
         trade_energy_delta = [0.0]*(duration+1)
         if startinterval_no == 0:
             trade_energy_delta[0] = 0
         else:
             trade_energy_delta[0] = flex.flex_with_mpo.allowed_min_energy_delta[startinterval_no-1]
         for interval_no in range(duration):
@@ -401,19 +405,19 @@
                 trade_power[interval_no] = to_be_used_power
             # update trade_energy_delta
             trade_energy_delta[interval_no+1] = trade_energy_delta[interval_no] + trade_power[interval_no]*900/3600
 
     mpos_with_trades = mpos.copy()
 
     if charge_possible:
-        print(f'Trade: {trade_power}')
+        # print(f'Trade: {trade_power}')
         for interval_no in range(duration):
             mpos_with_trades[startinterval_no+interval_no] = mpos_with_trades[startinterval_no+interval_no] + trade_power[interval_no]
             # mpos_with_trades[startinterval_no+interval_no] = trade_power[interval_no]
-        print(f'MPOs: {mpos_with_trades}')
+        # print(f'MPOs: {mpos_with_trades}')
         validate_charge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
     return mpos_with_trades
 
 def generate_long_medium_discharge_trade(flex: FlexibilityCalculation, mpos, startinterval_no, duration):
     """
     Generate a multi-time-step trade, which starts at startinterval_no and of
@@ -427,15 +431,15 @@
     discharge_possible = True
     for d in range(duration):
         # verify discharge is possible
         if flex.flex_with_mpo.allowed_min_power[startinterval_no+d] > 0:
             discharge_possible = False
     # generate multi-time-step trade
     trade_power = [0.0]*duration
-    print(f'Discharge possible: {discharge_possible}')
+    # print(f'Discharge possible: {discharge_possible}')
     if discharge_possible:
         trade_energy_delta = [0.0]*(duration+1)
         if startinterval_no == 0:
             trade_energy_delta[0] = 0
         else:
             trade_energy_delta[0] = flex.flex_with_mpo.allowed_max_energy_delta[startinterval_no-1]
         for interval_no in range(duration):
@@ -462,15 +466,15 @@
             else:
                 trade_power[interval_no] = to_be_used_power
             # update trade_energy_delta
             trade_energy_delta[interval_no+1] = trade_energy_delta[interval_no] + trade_power[interval_no]*900/3600
 
     mpos_with_trades = mpos.copy()
     if discharge_possible:
-        print(f'Trade: {trade_power}')
+        # print(f'Trade: {trade_power}')
         for interval_no in range(duration):
             mpos_with_trades[startinterval_no+interval_no] = mpos_with_trades[startinterval_no+interval_no] + trade_power[interval_no]
             # mpos_with_trades[startinterval_no+interval_no] = trade_power[interval_no]
-        print(f'MPOs: {mpos_with_trades}')
+        # print(f'MPOs: {mpos_with_trades}')
         validate_discharge_trade(flex, mpos_with_trades, startinterval_no, duration)
 
     return mpos_with_trades
```

### Comparing `amplify-model-0.1.1/amplify/tests/unit_tests/util/place_mpos.py` & `amplify_model-0.1.2/amplify/tests/unit_tests/util/place_mpos.py`

 * *Files identical despite different names*

### Comparing `amplify-model-0.1.1/pyproject.toml` & `amplify_model-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "amplify-model"
-version = "0.1.1"
+version = "0.1.2"
 description = "Amplify (abstract multi-purpose-limited flexibility) is a model for operational flexibility remaining after a primary application is fullfilled by distributed energy resources."
 authors = ["Paul Hendrik Tiemann <paul.hendrik.tiemann@uni-oldenburg.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "amplify"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pytest = "^7.1.2"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.group.dev.dependencies]
+plotly = "^5.10.0"
+pandas = "^1.4.4"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `amplify-model-0.1.1/PKG-INFO` & `amplify_model-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: amplify-model
-Version: 0.1.1
+Version: 0.1.2
 Summary: Amplify (abstract multi-purpose-limited flexibility) is a model for operational flexibility remaining after a primary application is fullfilled by distributed energy resources.
 License: Apache-2.0
 Author: Paul Hendrik Tiemann
 Author-email: paul.hendrik.tiemann@uni-oldenburg.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Amplify
 
 ## Getting started
 *Amplify* can be installed via `pip install amplify-model`. Then, the model can be used in an existing project by calling `from amplify.src.flex_calculation import FlexCalculator`.
```

