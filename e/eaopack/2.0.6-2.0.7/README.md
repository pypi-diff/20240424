# Comparing `tmp/eaopack-2.0.6.tar.gz` & `tmp/eaopack-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eaopack-2.0.6.tar", last modified: Sun Feb  4 12:24:27 2024, max compression
+gzip compressed data, was "eaopack-2.0.7.tar", last modified: Wed Apr 24 16:51:27 2024, max compression
```

## Comparing `eaopack-2.0.6.tar` & `eaopack-2.0.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:24:27.935056 eaopack-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-04 12:24:27.935056 eaopack-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-04 12:24:15.000000 eaopack-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:24:27.931056 eaopack-2.0.6/eaopack/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   152293 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14957 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/basic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/network_graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29189 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-02-04 12:24:15.000000 eaopack-2.0.6/eaopack/stoch_lin_prog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:24:27.935056 eaopack-2.0.6/eaopack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-04 12:24:27.000000 eaopack-2.0.6/eaopack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-04 12:24:27.000000 eaopack-2.0.6/eaopack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 12:24:27.000000 eaopack-2.0.6/eaopack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-04 12:24:27.000000 eaopack-2.0.6/eaopack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-04 12:24:27.935056 eaopack-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:24:27.935056 eaopack-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    62754 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_CHP_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_MIP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_TypedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)    27464 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_asset_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_new_asset_fnct.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_periodicity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_setting_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-02-04 12:24:15.000000 eaopack-2.0.6/tests/test_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:27.473539 eaopack-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 16:51:27.473539 eaopack-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-24 16:51:17.000000 eaopack-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:27.469539 eaopack-2.0.7/eaopack/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152293 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/basic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/network_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29189 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-24 16:51:17.000000 eaopack-2.0.7/eaopack/stoch_lin_prog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:27.473539 eaopack-2.0.7/eaopack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 16:51:27.000000 eaopack-2.0.7/eaopack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 16:51:27.000000 eaopack-2.0.7/eaopack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:51:27.000000 eaopack-2.0.7/eaopack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 16:51:27.000000 eaopack-2.0.7/eaopack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:51:27.000000 eaopack-2.0.7/eaopack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 16:51:27.473539 eaopack-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:27.473539 eaopack-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_CHP_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_MIP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_TypedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27464 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_asset_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_new_asset_fnct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_periodicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_setting_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-04-24 16:51:17.000000 eaopack-2.0.7/tests/test_tz.py
```

### Comparing `eaopack-2.0.6/PKG-INFO` & `eaopack-2.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: eaopack
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Framework for Optimizing Decentralized Portfolios and Green Supply
 Home-page: https://github.com/EnergyAssetOptimization/EAO
 Author: The EAO development Team
 Project-URL: Bug Tracker, https://github.com/EnergyAssetOptimization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: cvxpy
+Requires-Dist: cvxopt
+Requires-Dist: openpyxl
 
 
 [![CI](https://github.com/EnergyAssetOptimization/EAO/actions/workflows/unittests_doc.yml/badge.svg)](https://github.com/EnergyAssetOptimization/EAO/actions/workflows/unittests_doc.yml)
 
 # The Energy Asset Optimization (EAO) package
 
 The EAO package is a modular Python framework, designed to enable practitioners to use, build and optimize energy and commodity trading portfolios using linear or mixed integer programming as well as stochastic linear programming. It provides an implementation of
```

### Comparing `eaopack-2.0.6/README.md` & `eaopack-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/assets.py` & `eaopack-2.0.7/eaopack/assets.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/basic_classes.py` & `eaopack-2.0.7/eaopack/basic_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class StartEndValueDict(TypedDict):
     """ New type to contain info of the type start, end, value
         dict with
             start: array of datetime 
             end:   array of datetime (optional)
             values: array of floats """
     start:  Sequence[dt.datetime]
-    end:    Sequence[float]
+    end:    Sequence[dt.datetime]
     values: Sequence[float]
 
 class Unit:
     def __init__(self, volume:str='MWh', flow:str='MW', factor:float=1.):
         """ Defines the units used in a node and how to convert between volums and flows (volume/time)
 
         Args:
```

### Comparing `eaopack-2.0.6/eaopack/io.py` & `eaopack-2.0.7/eaopack/io.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/network_graphs.py` & `eaopack-2.0.7/eaopack/network_graphs.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/optimization.py` & `eaopack-2.0.7/eaopack/optimization.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/portfolio.py` & `eaopack-2.0.7/eaopack/portfolio.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/serialization.py` & `eaopack-2.0.7/eaopack/serialization.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack/stoch_lin_prog.py` & `eaopack-2.0.7/eaopack/stoch_lin_prog.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/eaopack.egg-info/PKG-INFO` & `eaopack-2.0.7/eaopack.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: eaopack
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Framework for Optimizing Decentralized Portfolios and Green Supply
 Home-page: https://github.com/EnergyAssetOptimization/EAO
 Author: The EAO development Team
 Project-URL: Bug Tracker, https://github.com/EnergyAssetOptimization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: cvxpy
+Requires-Dist: cvxopt
+Requires-Dist: openpyxl
 
 
 [![CI](https://github.com/EnergyAssetOptimization/EAO/actions/workflows/unittests_doc.yml/badge.svg)](https://github.com/EnergyAssetOptimization/EAO/actions/workflows/unittests_doc.yml)
 
 # The Energy Asset Optimization (EAO) package
 
 The EAO package is a modular Python framework, designed to enable practitioners to use, build and optimize energy and commodity trading portfolios using linear or mixed integer programming as well as stochastic linear programming. It provides an implementation of
```

### Comparing `eaopack-2.0.6/eaopack.egg-info/SOURCES.txt` & `eaopack-2.0.7/eaopack.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 eaopack/optimization.py
 eaopack/portfolio.py
 eaopack/serialization.py
 eaopack/stoch_lin_prog.py
 eaopack.egg-info/PKG-INFO
 eaopack.egg-info/SOURCES.txt
 eaopack.egg-info/dependency_links.txt
+eaopack.egg-info/requires.txt
 eaopack.egg-info/top_level.txt
 tests/test_CHP_asset.py
 tests/test_MIP.py
 tests/test_TypedDict.py
 tests/test_asset.py
 tests/test_asset_freq.py
 tests/test_io.py
```

### Comparing `eaopack-2.0.6/setup.cfg` & `eaopack-2.0.7/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 [metadata]
 name = eaopack
-version = 2.0.6
+version = 2.0.7
 author = The EAO development Team
 description = A Framework for Optimizing Decentralized Portfolios and Green Supply
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EnergyAssetOptimization/EAO
 project_urls = 
 	Bug Tracker = https://github.com/EnergyAssetOptimization/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.6
+install_requires = 
+	matplotlib
+	numpy
+	pandas
+	scipy
+	networkx
+	cvxpy
+	cvxopt
+	openpyxl
 
 [options.packages.find]
 exclude = 
 	tests
 	doc
 
 [egg_info]
```

### Comparing `eaopack-2.0.6/tests/test_CHP_asset.py` & `eaopack-2.0.7/tests/test_CHP_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -868,15 +868,16 @@
                                 min_cap=5., max_cap=10.)
         np.random.seed(2709)
         prices ={'rand_price': np.random.rand(timegrid.T)-0.5}
         op_o = a.setup_optim_problem(prices, timegrid=timegrid)
         res_o = op_o.optimize()
         x_power_o = np.around(res_o.x[:timegrid.T], decimals = 3) # round
         x_heat = np.around(res_o.x[timegrid.T:2*timegrid.T], decimals = 3) # round
-        self.assertTrue(all(x_heat==0))
+        # heat or power / exchangable --> need to look at sum
+        x_power_o += x_heat
 
         ## new: heat node is None
         a = eao.assets.CHPAsset(name='CHP', price='rand_price', 
                                 nodes = node_power,  # !!!!! heat node not given or None
                                 conversion_factor_power_heat = 0,  # use high number to assert I'd see effects if used
                                 min_cap=5., max_cap=10.,
                                 _no_heat = True)
@@ -997,15 +998,17 @@
                                 min_cap=5., max_cap=10.)
         np.random.seed(2709)
         prices ={'rand_price': np.random.rand(timegrid.T)-0.5}
         op_o = a.setup_optim_problem(prices, timegrid=timegrid)
         res_o = op_o.optimize()
         x_power_o = np.around(res_o.x[:timegrid.T], decimals = 3) # round
         x_heat = np.around(res_o.x[timegrid.T:2*timegrid.T], decimals = 3) # round
-        self.assertTrue(all(x_heat==0))
+        # heat or power / exchangable --> need to look at sum
+        x_power_o += x_heat
+        # self.assertTrue(all(x_heat==0))
 
         ## new: heat node is None
         a = eao.assets.Plant(name='CHP', price='rand_price', 
                                 nodes = node_power,  # !!!!! heat node not given or None
                                 min_cap=5., max_cap=10.)
         op = a.setup_optim_problem(prices, timegrid=timegrid)
         res = op.optimize()
@@ -1187,13 +1190,68 @@
         # self.assertAlmostEqual(out['dispatch'].sum().sum(),  0, 2)             
 
         # check serialization (new class...)
         s = eao.serialization.to_json(a)
         aa = eao.serialization.load_from_json(s)
 
 
+
+    def test_PP_check_start_ramp_vs_ramp(self):
+        """ What happens with ramp smaller / not equal start ramp? should be ignored
+        """
+        node_power = eao.assets.Node('node_power')
+        node_gas = eao.assets.Node('node_gas')
+
+        Start = dt.date(2022, 1, 1)
+        End = dt.date(2022, 1, 2)
+        timegrid = eao.assets.Timegrid(Start, End, freq='h')
+
+        #############################  test without heat node
+        #####################################################
+        # load test data
+        import os
+        myfile = os.path.join(os.path.join(os.path.dirname(__file__)),'plant_test_data.csv')
+        df = pd.read_csv(myfile)
+        df.set_index('date', inplace = True)
+        df = timegrid.prices_to_grid(df)
+        df['power_price'] = 1000
+        df['mincap'] = 6
+        # simple case, no min run time
+        a = eao.assets.Plant(name='PP',
+                                nodes=(node_power, node_gas),
+                                min_cap         = 'mincap',
+                                max_cap         = 'maxcap',
+                                start_costs     = 1.,
+                                running_costs   = 'runC',
+                                fuel_efficiency = 1,
+                                consumption_if_on= .1,
+                                start_fuel      = 1,
+                                min_downtime    = 2,
+                                ramp            = 1.1,
+                                time_already_running=0,
+                                time_already_off= 1,
+                                start_ramp_upper_bounds=[1,2,4,6,10],
+                                start_ramp_lower_bounds=[1,2,4,6,10],
+                                shutdown_ramp_upper_bounds=[1.1],
+                                shutdown_ramp_lower_bounds=[1.1],
+                                ramp_freq='h') 
+        b = eao.assets.SimpleContract(name = 'powerMarket', price='power_price', nodes = node_power, min_cap=-100, max_cap=100)
+        c = eao.assets.SimpleContract(name = 'gasMarket', price='gas_price', nodes = node_gas, min_cap=-100, max_cap=100)
+        portf = eao.portfolio.Portfolio([a, b, c])
+        op = portf.setup_optim_problem(df, timegrid=timegrid)
+        res = op.optimize()
+        out = eao.io.extract_output(portf, op, res, df)
+        # dispatch should follow start ramp and then add ramp
+        self.assertAlmostEqual(out['dispatch'].iloc[0,0],  0, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[1,0],  1, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[2,0],  2, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[3,0],  4, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[4,0],  6, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[5,0],  10, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[6,0],  11.1, 4) 
+        self.assertAlmostEqual(out['dispatch'].iloc[7,0],  12.2, 4) 
 ###########################################################################################################
 ###########################################################################################################
 ###########################################################################################################
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eaopack-2.0.6/tests/test_MIP.py` & `eaopack-2.0.7/tests/test_MIP.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_TypedDict.py` & `eaopack-2.0.7/tests/test_TypedDict.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_asset.py` & `eaopack-2.0.7/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_asset_freq.py` & `eaopack-2.0.7/tests/test_asset_freq.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_io.py` & `eaopack-2.0.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_new_asset_fnct.py` & `eaopack-2.0.7/tests/test_new_asset_fnct.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_optimization.py` & `eaopack-2.0.7/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_periodicity.py` & `eaopack-2.0.7/tests/test_periodicity.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_portfolio.py` & `eaopack-2.0.7/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_setting_params.py` & `eaopack-2.0.7/tests/test_setting_params.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_solvers.py` & `eaopack-2.0.7/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `eaopack-2.0.6/tests/test_tz.py` & `eaopack-2.0.7/tests/test_tz.py`

 * *Files identical despite different names*

