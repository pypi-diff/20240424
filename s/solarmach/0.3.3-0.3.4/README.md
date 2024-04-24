# Comparing `tmp/solarmach-0.3.3.tar.gz` & `tmp/solarmach-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.3.3.tar", last modified: Fri Jan 12 10:06:20 2024, max compression
+gzip compressed data, was "solarmach-0.3.4.tar", last modified: Wed Apr 24 15:08:11 2024, max compression
```

## Comparing `solarmach-0.3.3.tar` & `solarmach-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.923547 solarmach-0.3.3/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.3/LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.3.3/MANIFEST.in
--rw-r--r--   0 jagies    (1000) jagies    (1000)     8230 2024-01-12 10:06:20.923547 solarmach-0.3.3/PKG-INFO
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     6505 2024-01-12 10:04:22.000000 solarmach-0.3.3/README.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.3.3/code_of_conduct.md
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.919547 solarmach-0.3.3/docs/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      634 2023-07-25 12:11:02.000000 solarmach-0.3.3/docs/Makefile
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1281 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/conf.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     2356 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/index.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      324 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/installation.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      800 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/make.bat
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      103 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/requirements.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      220 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/solarmach.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)       43 2024-01-12 10:04:22.000000 solarmach-0.3.3/docs/usage.nblink
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.919547 solarmach-0.3.3/examples/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)  4699075 2024-01-12 10:04:22.000000 solarmach-0.3.3/examples/example.ipynb
--rw-rw-r--   0 jagies    (1000) jagies    (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.3.3/examples/solarmach.png
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.923547 solarmach-0.3.3/licenses/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.3/licenses/LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.3.3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      133 2024-01-12 10:04:22.000000 solarmach-0.3.3/pyproject.toml
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      157 2024-01-12 10:04:22.000000 solarmach-0.3.3/requirements.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     2208 2024-01-12 10:06:20.923547 solarmach-0.3.3/setup.cfg
--rwxrwxr-x   0 jagies    (1000) jagies    (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.3.3/setup.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.923547 solarmach-0.3.3/solarmach/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)   103267 2024-01-12 10:04:22.000000 solarmach-0.3.3/solarmach/__init__.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)    24251 2024-01-12 10:04:22.000000 solarmach-0.3.3/solarmach/pfss_utilities.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.923547 solarmach-0.3.3/solarmach/tests/
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.3.3/solarmach/tests/__init__.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     4311 2024-01-12 10:04:22.000000 solarmach-0.3.3/solarmach/tests/test.py
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      345 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach/version.py
-drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-01-12 10:06:20.923547 solarmach-0.3.3/solarmach.egg-info/
--rw-r--r--   0 jagies    (1000) jagies    (1000)     8230 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      665 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.3.3/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 jagies    (1000) jagies    (1000)      263 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach.egg-info/requires.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)       10 2024-01-12 10:06:20.000000 solarmach-0.3.3/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 jagies    (1000) jagies    (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.3.3/tox.ini
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.4/LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.3.4/MANIFEST.in
+-rw-r--r--   0 jagies    (1000) jagies    (1000)     8273 2024-04-24 15:08:11.311487 solarmach-0.3.4/PKG-INFO
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     6505 2024-03-25 08:09:12.000000 solarmach-0.3.4/README.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.3.4/code_of_conduct.md
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/docs/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      634 2023-07-25 12:11:02.000000 solarmach-0.3.4/docs/Makefile
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1281 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/conf.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     2356 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/index.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      324 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/installation.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      800 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/make.bat
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      103 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/requirements.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      220 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/solarmach.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)       43 2024-03-25 08:09:12.000000 solarmach-0.3.4/docs/usage.nblink
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/examples/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)  4699075 2024-03-25 08:09:12.000000 solarmach-0.3.4/examples/example.ipynb
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.3.4/examples/solarmach.png
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.307487 solarmach-0.3.4/licenses/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.3.4/licenses/LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.3.4/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      133 2024-03-25 08:09:12.000000 solarmach-0.3.4/pyproject.toml
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      192 2024-03-25 08:09:12.000000 solarmach-0.3.4/requirements.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     2255 2024-04-24 15:08:11.311487 solarmach-0.3.4/setup.cfg
+-rwxrwxr-x   0 jagies    (1000) jagies    (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.3.4/setup.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)   104676 2024-04-24 13:54:06.000000 solarmach-0.3.4/solarmach/__init__.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)    24330 2024-03-25 08:09:12.000000 solarmach-0.3.4/solarmach/pfss_utilities.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach/tests/
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.3.4/solarmach/tests/__init__.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      230 2024-04-24 15:00:51.000000 solarmach-0.3.4/solarmach/tests/figure_hashes_mpl_353.json
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     6605 2024-04-24 13:56:25.000000 solarmach-0.3.4/solarmach/tests/test.py
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      345 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach/version.py
+drwxrwxr-x   0 jagies    (1000) jagies    (1000)        0 2024-04-24 15:08:11.311487 solarmach-0.3.4/solarmach.egg-info/
+-rw-r--r--   0 jagies    (1000) jagies    (1000)     8273 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      708 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.3.4/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)      274 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)       10 2024-04-24 15:08:11.000000 solarmach-0.3.4/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 jagies    (1000) jagies    (1000)     1305 2024-03-25 08:09:12.000000 solarmach-0.3.4/tox.ini
```

### Comparing `solarmach-0.3.3/LICENSE.rst` & `solarmach-0.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/PKG-INFO` & `solarmach-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.3.3
+Version: 0.3.4
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Project-URL: Documentation, https://solarmach.readthedocs.io
 Project-URL: Changelog, https://github.com/jgieseler/solarmach/releases
@@ -38,14 +38,15 @@
 Requires-Dist: sunpy
 Requires-Dist: zeep
 Provides-Extra: all
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mpl; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 solarmach
```

### Comparing `solarmach-0.3.3/README.rst` & `solarmach-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/code_of_conduct.md` & `solarmach-0.3.4/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/docs/Makefile` & `solarmach-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/docs/conf.py` & `solarmach-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/docs/index.rst` & `solarmach-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/docs/make.bat` & `solarmach-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/examples/example.ipynb` & `solarmach-0.3.4/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/examples/solarmach.png` & `solarmach-0.3.4/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/licenses/LICENSE.rst` & `solarmach-0.3.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.3.4/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/setup.cfg` & `solarmach-0.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,29 @@
 	drms
 	imageio>=2.31.6
 	Jinja2
 	lxml
 	matplotlib==3.5.3
 	numpy
 	pandas
-	pfsspy
+	pfsspy  # TODO: replace with sunkit_magex
 	plotly
 	python-dateutil
 	scipy
 	speasy>=1.2.0
 	sunpy
 	zeep
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
+	pytest-mpl
 docs = 
 	sphinx
 	sphinx-automodapi
 	numpydoc
 	sphinx_rtd_theme
 
 [tool:pytest]
```

### Comparing `solarmach-0.3.3/setup.py` & `solarmach-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.3.3/solarmach/__init__.py` & `solarmach-0.3.4/solarmach/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from pkg_resources import get_distribution, DistributionNotFound  # type: ignore
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     pass  # package is not installed
 
 import copy
-import dateutil.parser  # type: ignore
+# import dateutil.parser  # type: ignore
 import math
+import os
 
 import astropy.constants as aconst
 import astropy.units as u
 import datetime as dt
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import matplotlib.text
@@ -100,14 +101,17 @@
         measurements can be obtained. Default value 400.0
 
     Returns
     -------
     float
         solar wind bulk speed in km/s
     """
+    # disable unused speasy data provider before importing to speed it up
+    os.environ['SPEASY_CORE_DISABLED_PROVIDERS'] = "sscweb,archive,csa"
+
     try:
         import speasy as spz
     except ModuleNotFoundError:
         print(f"Couldn't load required module speasy, using default_vsw={default_vsw}. Install it with 'pip install speasy' to use this functionality.")
         return default_vsw
 
     try:
@@ -138,27 +142,26 @@
     if body in ['Earth', 'SEMB-L1']:
         print(f"Using 'ACE' measurements for '{body}'.")
         body = 'ACE'
     elif body not in dataset.keys():
         print(f"Body '{body}' not supported, assuming default Vsw value of {default_vsw} km/s.")
         return default_vsw
 
-    if type(dtime) == str:
-        try:
-            dtime = dateutil.parser.parse(dtime)
-        except dateutil.parser.ParserError:
-            print(f"Unable to extract datetime from '{dtime}'. Assuming default Vsw value of {default_vsw} km/s.")
-            return default_vsw
+    try:
+        dtime = parse_time(dtime).datetime  # dateutil.parser.parse(dtime)
+    except ValueError:  # dateutil.parser.ParserError:
+        print(f"Unable to extract datetime from '{dtime}'. Assuming default Vsw value of {default_vsw} km/s.")
+        return default_vsw
 
     try:
         if dataset[body].spz_provider() == 'amda':
             df = spz.get_data(dataset[body], dtime-dt.timedelta(hours=trange), dtime+dt.timedelta(hours=trange), output_format="CDF_ISTP").to_dataframe()
         elif dataset[body].spz_provider() == 'cda':
             df = spz.get_data(dataset[body], dtime-dt.timedelta(hours=trange), dtime+dt.timedelta(hours=trange)).to_dataframe()
-        df = df[sw_key[body]].resample('1H').mean()
+        df = df[sw_key[body]].resample('1h').mean()
         # drop NaN entries:
         df.dropna(inplace=True)
         if len(df) > 0:
             idx = df.iloc[df.index.get_indexer([dtime], method='nearest')]
             return idx.values[0]
         else:
             print(f"No Vsw data found for '{body}' on {dtime}, assuming default Vsw value of {default_vsw} km/s.")
@@ -209,27 +212,33 @@
         bodies = copy.deepcopy(body_dict)
 
         if coord_sys.lower().startswith('car'):
             coord_sys = 'Carrington'
         if coord_sys.lower().startswith('sto') or coord_sys.lower() == "earth":
             coord_sys = 'Stonyhurst'
 
-        self.date = date
+        # parse input date & time
+        self.date = parse_time(date)
+
         self.reference_long = reference_long
         self.reference_lat = reference_lat
         self.coord_sys = coord_sys
 
-        pos_E = get_horizons_coord(399, self.date, None)  # (lon, lat, radius) in (deg, deg, AU)
+        try:
+            pos_E = get_horizons_coord(399, self.date, None)  # (lon, lat, radius) in (deg, deg, AU)
+        except ValueError:
+            print('')
+            print('!!! No ephemeris found for Earth for date {self.date} - there probably is a problem with JPL HORIZONS.')
         if coord_sys=='Carrington':
             self.pos_E = pos_E.transform_to(frames.HeliographicCarrington(observer='Sun'))
         elif coord_sys=='Stonyhurst':
             self.pos_E = pos_E
 
         # standardize "undefined" vsw_list for further usage:
-        if type(vsw_list)==type(None) or vsw_list==False:
+        if type(vsw_list)==type(None) or vsw_list is False:
             vsw_list=[]
 
         # make deep copy of vsw_list bc. otherwise it doesn't get reset in a new init:
         vsw_list2 = copy.deepcopy(vsw_list)
 
         if len(vsw_list2) == 0:
             print('No solar wind speeds defined, trying to obtain measurements...')
@@ -490,20 +499,20 @@
         r_array = np.arange(0.007, (self.max_dist+0.1)/np.cos(np.deg2rad(self.max_dist_lat)) + 3.0, 0.001)
         # take into account solar differential rotation wrt. latitude. Thus move calculation of omega to the per-body section below
         # omega = np.radians(360. / (25.38 * 24 * 60 * 60))  # solar rot-angle in rad/sec, sidereal period
 
         E_long = self.pos_E.lon.value
 
         # catch old syntax
-        if numbered_markers==True and not markers:
+        if numbered_markers is True and not markers:
             markers='numbers'
             print('')
             print("WARNING: The usage of numbered_markers is deprecated and will be discontinued in the future! Use markers='numbers' instead.")
             print('')
-        
+
         if markers:
             if markers.lower() in ['n', 'number']:
                 markers='numbers'
             if markers.lower() in ['l', 'letter']:
                 markers='letters'
 
         if test_plotly:
@@ -534,17 +543,17 @@
                     if body_id[:6] == 'STEREO':
                         mark = str(body_id[-1])
                     else:
                         mark = str(body_id[0])
                 if markers.lower()=='numbers':
                     mark = i+1
                 ax.annotate(mark, xy=(np.deg2rad(body_long), dist_body*np.cos(np.deg2rad(body_lat))), color='white',
-                           fontsize="small", weight='heavy',
-                           horizontalalignment='center',
-                           verticalalignment='center')
+                            fontsize="small", weight='heavy',
+                            horizontalalignment='center',
+                            verticalalignment='center')
             else:
                 ax.plot(np.deg2rad(body_long), dist_body*np.cos(np.deg2rad(body_lat)), 's', color=body_color, label=body_lab)
 
             if plot_sun_body_line:
                 # ax.plot(alpha_ref[0], 0.01, 0)
                 ax.plot([np.deg2rad(body_long), np.deg2rad(body_long)], [0.01, dist_body*np.cos(np.deg2rad(body_lat))], ':', color=body_color)
             # plot the spirals
@@ -572,16 +581,17 @@
                         theta=[np.deg2rad(body_long), np.deg2rad(body_long)],
                         mode='lines',
                         name=f'{body_id} direct line',
                         showlegend=False,
                         line=dict(color=body_dict[body_id][2], dash='dot'),
                         thetaunit="radians"))
 
-                if numbered_markers:
-                    str_number = f'<b>{i+1}</b>'
+                if markers:
+                    if markers.lower()=='letters' or markers.lower()=='numbers':
+                        str_number = f'<b>{mark}</b>'
                 else:
                     str_number = None
 
                 pfig.add_trace(go.Scatterpolar(
                     r=[dist_body*np.cos(np.deg2rad(body_lat))],
                     theta=[np.deg2rad(body_long)],
                     mode='markers+text',
@@ -642,29 +652,42 @@
                         mode='lines',
                         name=f'field line connecting to<br>ref. long. (vsw={reference_vsw} km/s)',
                         showlegend=True,
                         line=dict(color=reference_color, dash="dash"),
                         thetaunit="radians"))
 
         if test_plotly:
-            if numbered_markers:
-                for i, body_id in enumerate(self.body_dict):
-                    if self.reference_long is not None:
-                        x_offset_ref = -0.035  # 0.004
-                        y_offset_ref = 0.081
-                        y_offset_per_i = -0.051
-                    else:
-                        x_offset_ref = 0.0
-                        y_offset_ref = 0.0
-                        y_offset_per_i = -0.0475
-                    x_offset = -0.11  # 0.05
-                    y_offset = 0.124  # -0.0064
-                    pfig.add_annotation(text=f'<b>{i+1}</b>', xref="paper", yref="paper", xanchor="center", yanchor="top",
-                                        x=test_plotly_legend[0]+x_offset+x_offset_ref, y=test_plotly_legend[1]+y_offset+y_offset_ref+y_offset_per_i*i,
-                                        showarrow=False, font=dict(color="white", size=14))
+            if markers:
+                if markers.lower()=='letters' or markers.lower()=='numbers':
+                    for i, body_id in enumerate(self.body_dict):
+                        if self.reference_long is not None:
+                            x_offset_ref = -0.035  # 0.004
+                            y_offset_ref = 0.081
+                            y_offset_per_i = -0.051
+                        else:
+                            x_offset_ref = 0.0
+                            y_offset_ref = 0.0
+                            y_offset_per_i = -0.0475
+                        # These offset numbers probably need to be updated; it seems the markers are now too much in the upper left direction.
+                        # They're not visible anymore for test_plotly_legend=[1.0, 1.0], so test for test_plotly_legend=[0.5, 0.5].
+                        # Note that the offset effect changes with the size of the plotly figure (i.e., when resizing the browser window)!
+                        x_offset = -0.11  # 0.05
+                        y_offset = 0.124  # -0.0064
+
+                        if markers.lower()=='letters':
+                            if body_id[:6] == 'STEREO':
+                                mark = str(body_id[-1])
+                            else:
+                                mark = str(body_id[0])
+                        if markers.lower()=='numbers':
+                            mark = i+1
+
+                        pfig.add_annotation(text=f'<b>{mark}</b>', xref="paper", yref="paper", xanchor="center", yanchor="top",
+                                            x=test_plotly_legend[0]+x_offset+x_offset_ref, y=test_plotly_legend[1]+y_offset+y_offset_ref+y_offset_per_i*i,
+                                            showarrow=False, font=dict(color="black", size=14))
 
             pfig.add_annotation(text='Solar-MACH', xref="paper", yref="paper",  # xanchor="center", yanchor="middle",
                                 x=test_plotly_logo[0], y=test_plotly_logo[1]+0.05,
                                 showarrow=False, font=dict(color="black", size=28, family='DejaVu Serif'), align="right")
             pfig.add_annotation(text='https://solar-mach.github.io', xref="paper", yref="paper",  # xanchor="center", yanchor="middle",
                                 x=test_plotly_logo[0], y=test_plotly_logo[1],
                                 showarrow=False, font=dict(color="black", size=18, family='DejaVu Serif'), align="right")
@@ -866,33 +889,33 @@
         # manually plot r-grid lines with different resolution depending on maximum distance body
         if self.max_dist < 2:
             ax.set_rgrids(np.arange(0, self.max_dist + 0.29, 0.5)[1:], angle=rlabel_pos)
         else:
             if self.max_dist < 10:
                 ax.set_rgrids(np.arange(0, self.max_dist + 0.29, 1.0)[1:], angle=rlabel_pos)
 
-        ax.set_title(str(self.date) + ' (UTC)\n', pad=30)
+        ax.set_title(str(self.date.to_value('iso', subfmt='date_hm')) + ' (UTC)\n', pad=30)
 
         plt.tight_layout()
         plt.subplots_adjust(bottom=0.15)
 
         if show_earth_centered_coord:
             print("The option 'show_earth_centered_coord' is deprecated! Please initialize SolarMACH with coord_sys='Stonyhurst' to get an Earth-centered coordinate system.")
             # pos1 = ax.get_position()  # get the original position of the polar plot
             # offset = 0.12
             # pos2 = [pos1.x0 - offset / 2, pos1.y0 - offset / 2, pos1.width + offset, pos1.height + offset]
             # ax2 = self._polar_twin(ax, E_long, pos2, long_offset)
 
         ax.tick_params(axis='x', pad=10)
 
         if not hide_logo:
-            ax.text(0.8, 0.16, 'Solar-MACH',
+            ax.text(0.83, 0.16, 'Solar-MACH',
                     fontfamily='DejaVu Serif', fontsize=23,
                     ha='right', va='bottom', transform=fig.transFigure)
-            ax.text(0.8, 0.12, 'https://solar-mach.github.io',
+            ax.text(0.83, 0.12, 'https://solar-mach.github.io',
                     fontfamily='DejaVu Sans', fontsize=13,
                     ha='right', va='bottom', transform=fig.transFigure)
 
         if transparent:
             fig.patch.set_alpha(0.0)
 
         if outfile != '':
@@ -979,20 +1002,20 @@
         # r_scaler scales distances from astronomical units to solar radii. unit = [solar radii / AU]
         r_scaler = (AU*1000)/sun_radius
 
         # carrington longitude of the Earth
         E_long = self.pos_E.lon.value
 
         # catch old syntax
-        if numbered_markers==True and not markers:
+        if numbered_markers is True and not markers:
             markers='numbers'
             print('')
             print("WARNING: The usage of numbered_markers is deprecated and will be discontinued in the future! Use markers='numbers' instead.")
             print('')
-        
+
         if markers:
             if markers.lower() in ['n', 'number']:
                 markers='numbers'
             if markers.lower() in ['l', 'letter']:
                 markers='letters'
 
         # save inital rcParams and update some of them:
@@ -1004,15 +1027,15 @@
         # init the figure and axes
         fig, ax = plt.subplots(subplot_kw=dict(projection='polar'), figsize=figsize, dpi=dpi)
 
         # maximum distance anything will be plotted
         r_max = r_scaler * 5  # 5 AU = 1075 in units of solar radii
 
         # setting the title
-        ax.set_title(str(self.date) + ' (UTC)\n', pad=30)  # , fontsize=26)
+        ax.set_title(str(self.date.to_value('iso', subfmt='date_hm')) + ' (UTC)\n', pad=30)  # , fontsize=26)
 
         # Plot the source_surface and solar surface
         full_circle_radians = 2*np.pi*np.linspace(0, 1, 200)
         ax.plot(full_circle_radians, np.ones(200)*rss, c='k', ls='--', zorder=3)
         ax.plot(full_circle_radians, np.ones(200), c='darkorange', lw=2.5, zorder=1)
 
         # Plot the 30 and 60 deg lines on the Sun
@@ -1060,15 +1083,15 @@
                 ax.plot(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), 'o', ms=15, color=body_color, label=body_lab)
                 if markers.lower()=='letters':
                     if body_id[:6] == 'STEREO':
                         mark = str(body_id[-1])
                     else:
                         mark = str(body_id[0])
                 if markers.lower()=='numbers':
-                    mark = i+1                
+                    mark = i+1
                 ax.annotate(mark, xy=(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat))), color='white',
                             fontsize="small", weight='heavy',
                             horizontalalignment='center',
                             verticalalignment='center')
             else:
                 ax.plot(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), 's', color=body_color, label=body_lab)
```

### Comparing `solarmach-0.3.3/solarmach/pfss_utilities.py` & `solarmach-0.3.4/solarmach/pfss_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import pickle
 
 import astropy.constants as aconst
 import astropy.units as u
 import matplotlib.pyplot as plt
 import numpy as np
-import pfsspy
+import pfsspy  # TODO: replace with "import sunkit_magex.pfss as pfsspy"
 import sunpy.map
 from astropy.coordinates import SkyCoord
 from sunpy.net import Fido
 from sunpy.net import attrs as a
 
 
 # @st_cache_decorator
@@ -68,15 +68,16 @@
     except FileNotFoundError:
         print("PFSS file not found.\nDownloading...")
         series = a.jsoc.Series('hmi.synoptic_mr_polfil_720s')
         crot = a.jsoc.PrimeKey('CAR_ROT', carrington_rot)
         result = Fido.search(time, series, crot, a.jsoc.Notify(email))
         files = Fido.fetch(result)
         hmi_map = sunpy.map.Map(files[0])
-        pfsspy.utils.fix_hmi_meta(hmi_map)
+        # pfsspy.utils.fix_hmi_meta(hmi_map)
+        
         print('Data shape: ', hmi_map.data.shape)
 
         hmi_map = hmi_map.resample([360, 180]*u.pix)
         print('New shape: ', hmi_map.data.shape)
 
         pfss_input = pfsspy.Input(hmi_map, nrho, rss)
         output = pfsspy.pfss(pfss_input)
@@ -328,24 +329,24 @@
 
     Returns:
     --------
     field_lines: FieldLine or list[FieldLine]
             A FieldLine object, or a list of them, if input coordinates were a list
 
     """
-    from pfsspy import tracing
+    # from pfsspy import tracing
 
     # if lat0 and lon0 are given in deg for some reason, transform them to rad
     if not rad:
         lat0 = np.deg2rad(lat0)
         lon0 = np.deg2rad(lon0)
 
     # Start tracing from a given height
     height = seedheight*aconst.R_sun
-    tracer = tracing.PythonTracer()
+    tracer = pfsspy.tracing.PythonTracer()
 
     # Add unit to longitude and latitude, so that SkyCoord understands them
     lon, lat = lon0*u.rad, lat0*u.rad
 
     # Seed the starting coordinate at the desired coordinates
     seed = SkyCoord(lon, lat, height, frame=hmimap.coordinate_frame)
```

### Comparing `solarmach-0.3.3/solarmach/tests/test.py` & `solarmach-0.3.4/solarmach/tests/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import astropy
 import astropy.units as u
 import datetime as dt
 import matplotlib
 import numpy as np
 import pandas
 import pfsspy
+import pytest
 import sunpy
-from solarmach import SolarMACH, print_body_list, get_gong_map, calculate_pfss_solution, sc_distance
+from pathlib import Path
+from solarmach import SolarMACH, print_body_list, get_gong_map, calculate_pfss_solution, sc_distance, get_sw_speed
 
 
 def test_print_body_list():
     df = print_body_list()
     assert isinstance(df, pandas.core.frame.DataFrame)
     assert df['Body'].loc['PSP'] == 'Parker Solar Probe'
 
 
 def test_solarmach_initialize():
-    body_list = ['STEREO-A']
+    body_list = ['STEREO-A', 'JUICE']
     vsw_list = [400]
     date = '2021-10-28 15:15:00'
     reference_long = 273
     reference_lat = 9
 
     sm = SolarMACH(date=date, body_list=body_list, vsw_list=vsw_list, reference_long=reference_long, reference_lat=reference_lat)
 
@@ -42,62 +44,106 @@
     assert np.round(sm.coord_table["Longitudinal separation between body's magnetic footpoint and reference_long"][0], 2) == 19.33
 
     # verify backwards compatibility: undefined coord_sys is interpreted as 'Carrington'
     assert sm.coord_sys == 'Carrington'
 
 
 def test_solarmach_get_sw_speed():
-    body_list = ['Earth', 'STEREO-A', 'BepiColombo']
-    date = '2021-10-28 15:15:00'
+    body_list = ['STEREO-A', 'SOHO', 'Parker Solar Probe', 'Solar Orbiter', 'Wind', 'ACE', 'Earth', 'BepiColombo']
+    date = '2023-02-28 15:00:00'
     sm = SolarMACH(date=date, body_list=body_list, coord_sys='Stonyhurst')
     try:
         import speasy as spz
-        vsw_stereoa = 365.0
+        vsw_stereoa = 636.0
+        vsw_soho = 655.0
+        vsw_psp = 476.0
+        vsw_solo = 496.0
+        vsw_wind = 597.0
+        vsw_ace = 616.0
     except ModuleNotFoundError:
         vsw_stereoa = 400.0
+        vsw_soho = 400.0
+        vsw_psp = 400.0
+        vsw_solo = 400.0
+        vsw_wind = 400.0
+        vsw_ace = 400.0
     assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='STEREO-A']['Vsw'].values[0]) == vsw_stereoa
+    assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='SOHO']['Vsw'].values[0]) == vsw_soho
+    assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='Parker Solar Probe']['Vsw'].values[0]) == vsw_psp
+    assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='Solar Orbiter']['Vsw'].values[0]) == vsw_solo
+    assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='Wind']['Vsw'].values[0]) == vsw_wind
+    assert np.round(sm.coord_table[sm.coord_table['Spacecraft/Body']=='ACE']['Vsw'].values[0]) == vsw_ace
+    assert sm.coord_table[sm.coord_table['Spacecraft/Body']=='Earth']['Vsw'].values[0] == sm.coord_table[sm.coord_table['Spacecraft/Body']=='ACE']['Vsw'].values[0]
     assert sm.coord_table[sm.coord_table['Spacecraft/Body']=='BepiColombo']['Vsw'].values[0] == 400.0
 
 
+def test_solarmach_wrong_datetime_format():
+    body_list = ['Earth', 'STEREO-A', 'BepiColombo']
+    date = '202110-28 15:15:00'
+    default_vsw = 999.9
+
+    # check only get_sw_speed
+    vsw_earth = get_sw_speed(body_list[0], date, trange=1, default_vsw=default_vsw)
+    assert vsw_earth == default_vsw
+
+    # check only sc_distance
+    distance = sc_distance(body_list[0], body_list[1], date)
+    assert np.isnan(distance.value)
+    assert distance.unit == u.AU
+
+    # check SolarMACH
+    with pytest.raises(ValueError):
+        sm = SolarMACH(date=date, body_list=body_list, coord_sys='Stonyhurst')
+
+
+"""
+Create/update hash library for the following matplotlib tests by running for example the following command from the base package dir:
+tox -e py310-test -- --mpl-generate-hash-library=solarmach/tests/figure_hashes_mpl_353.json --mpl-deterministic
+"""
+
+
+@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_353.json', deterministic=True)
 def test_solarmach_plot():
     body_list = ['STEREO-A']
     vsw_list = [400]
     date = '2021-10-28 15:15:00'
     reference_long = 273
     reference_lat = 9
     reference_vsw = 400
     filename = 'test.png'
     long_sector=[290, 328]
     long_sector_vsw=[400, 600]
     long_sector_color='red'
     background_spirals=[6, 600]
 
     sm = SolarMACH(date=date, body_list=body_list, vsw_list=vsw_list, reference_long=reference_long, reference_lat=reference_lat)
-    sm.plot(plot_spirals=True, plot_sun_body_line=True,
-            reference_vsw=reference_vsw, transparent=False,
-            show_earth_centered_coord=False, markers='numbers',
-            long_sector=long_sector, long_sector_vsw=long_sector_vsw, long_sector_color=long_sector_color,
-            background_spirals=background_spirals, outfile=filename)
-
+    fig, ax = sm.plot(plot_spirals=True, plot_sun_body_line=True,
+                      reference_vsw=reference_vsw, transparent=False,
+                      show_earth_centered_coord=False, markers='numbers',
+                      long_sector=long_sector, long_sector_vsw=long_sector_vsw, long_sector_color=long_sector_color,
+                      background_spirals=background_spirals, outfile=filename, return_plot_object=True)
     assert os.path.exists(os.getcwd()+os.sep+filename)
+    return fig
 
 
+@pytest.mark.mpl_image_compare(hash_library=Path(__file__).parent / 'figure_hashes_mpl_353.json', deterministic=True)
 def test_solarmach_pfss():
     date = '2021-4-1 1:00:00'
     body_list = ['Earth', 'STEREO-A']
     vsw_list = [400, 400]   # position-sensitive solar wind speed per body in body_list
     sm = SolarMACH(date, body_list, vsw_list, reference_long=100, reference_lat=10, coord_sys='Carrington')
     gong_map = get_gong_map(time=date, filepath=None)
     assert isinstance(gong_map, pfsspy.map.GongSynopticMap) or isinstance(gong_map, sunpy.map.sources.gong.GONGSynopticMap)
     pfss_solution = calculate_pfss_solution(gong_map=gong_map, rss=2.5, coord_sys='Carrington')
     assert isinstance(pfss_solution, pfsspy.output.Output)
     fig, ax = sm.plot_pfss(rss=2.5, pfss_solution=pfss_solution, vary=True, return_plot_object=True,
                            markers='numbers', long_sector=[290, 328], long_sector_vsw=[400, 600],
                            long_sector_color='red', reference_vsw=400.0)
     assert isinstance(fig, matplotlib.figure.Figure)
+    return fig
 
 
 def test_sc_distance():
     distance = sc_distance('SolO', 'PSP', "2020/12/12")
     assert np.round(distance.value, 8) == 1.45237361
     assert distance.unit == u.AU
     #
```

### Comparing `solarmach-0.3.3/solarmach.egg-info/PKG-INFO` & `solarmach-0.3.4/solarmach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.3.3
+Version: 0.3.4
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Project-URL: Documentation, https://solarmach.readthedocs.io
 Project-URL: Changelog, https://github.com/jgieseler/solarmach/releases
@@ -38,14 +38,15 @@
 Requires-Dist: sunpy
 Requires-Dist: zeep
 Provides-Extra: all
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mpl; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 solarmach
```

### Comparing `solarmach-0.3.3/solarmach.egg-info/SOURCES.txt` & `solarmach-0.3.4/solarmach.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 solarmach.egg-info/PKG-INFO
 solarmach.egg-info/SOURCES.txt
 solarmach.egg-info/dependency_links.txt
 solarmach.egg-info/not-zip-safe
 solarmach.egg-info/requires.txt
 solarmach.egg-info/top_level.txt
 solarmach/tests/__init__.py
+solarmach/tests/figure_hashes_mpl_353.json
 solarmach/tests/test.py
```

### Comparing `solarmach-0.3.3/tox.ini` & `solarmach-0.3.4/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tox]
 envlist =
-    py{36,37,38}-test
+    py{38,39,310}-test
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 
 [testenv]
 # Pass through the following environemnt variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
+passenv = HOME, WINDIR, LC_ALL, LC_CTYPE, CC, CI, TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # the package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructued with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
@@ -30,15 +30,15 @@
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     alldeps: all
 
 commands =
     pip freeze
-    pytest --pyargs solarmach {toxinidir}/docs --cov solarmach --cov-config={toxinidir}/setup.cfg {posargs}
+    pytest --pyargs solarmach {toxinidir}/docs --cov solarmach --cov-config={toxinidir}/setup.cfg {posargs} --mpl
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```

