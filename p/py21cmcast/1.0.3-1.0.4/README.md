# Comparing `tmp/py21cmcast-1.0.3.tar.gz` & `tmp/py21cmcast-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py21cmcast-1.0.3.tar", last modified: Tue Mar  5 11:42:31 2024, max compression
+gzip compressed data, was "py21cmcast-1.0.4.tar", last modified: Wed Apr 24 06:15:01 2024, max compression
```

## Comparing `py21cmcast-1.0.3.tar` & `py21cmcast-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-05 11:42:31.709012 py21cmcast-1.0.3/
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    35149 2023-11-24 16:26:21.000000 py21cmcast-1.0.3/LICENSE
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)        0 2024-02-01 09:07:12.000000 py21cmcast-1.0.3/MANIFEST.in
--rw-r--r--   0 gfacchin (3003741) gfacchin (3003741)    45280 2024-03-05 11:42:31.708012 py21cmcast-1.0.3/PKG-INFO
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     3771 2024-02-02 10:21:03.000000 py21cmcast-1.0.3/README.md
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     1033 2024-03-05 11:42:13.000000 py21cmcast-1.0.3/pyproject.toml
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       38 2024-03-05 11:42:31.709012 py21cmcast-1.0.3/setup.cfg
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       37 2024-02-01 09:09:41.000000 py21cmcast-1.0.3/setup.py
-drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-05 11:42:31.630012 py21cmcast-1.0.3/src/
-drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-05 11:42:31.691012 py21cmcast-1.0.3/src/py21cmcast/
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      786 2024-02-15 15:06:05.000000 py21cmcast-1.0.3/src/py21cmcast/__init__.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       59 2024-02-01 09:17:54.000000 py21cmcast-1.0.3/src/py21cmcast/__main__.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    50742 2024-02-16 08:35:10.000000 py21cmcast-1.0.3/src/py21cmcast/core.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     5421 2024-02-15 13:51:30.000000 py21cmcast-1.0.3/src/py21cmcast/experiments.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    11671 2023-11-24 16:26:21.000000 py21cmcast-1.0.3/src/py21cmcast/power.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    22834 2024-02-15 14:25:50.000000 py21cmcast-1.0.3/src/py21cmcast/runs.py
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    27889 2024-02-14 15:07:42.000000 py21cmcast-1.0.3/src/py21cmcast/tools.py
-drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-05 11:42:31.706012 py21cmcast-1.0.3/src/py21cmcast.egg-info/
--rw-r--r--   0 gfacchin (3003741) gfacchin (3003741)    45280 2024-03-05 11:42:31.000000 py21cmcast-1.0.3/src/py21cmcast.egg-info/PKG-INFO
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      434 2024-03-05 11:42:31.000000 py21cmcast-1.0.3/src/py21cmcast.egg-info/SOURCES.txt
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)        1 2024-03-05 11:42:31.000000 py21cmcast-1.0.3/src/py21cmcast.egg-info/dependency_links.txt
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      129 2024-03-05 11:42:31.000000 py21cmcast-1.0.3/src/py21cmcast.egg-info/requires.txt
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       11 2024-03-05 11:42:31.000000 py21cmcast-1.0.3/src/py21cmcast.egg-info/top_level.txt
-drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-05 11:42:31.697012 py21cmcast-1.0.3/tests/
--rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      175 2024-02-01 16:16:41.000000 py21cmcast-1.0.3/tests/test.py
+drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-04-24 06:15:01.344017 py21cmcast-1.0.4/
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    35149 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/LICENSE
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)        0 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/MANIFEST.in
+-rw-r--r--   0 gfacchin (3003741) gfacchin (3003741)    45280 2024-04-24 06:15:01.342017 py21cmcast-1.0.4/PKG-INFO
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     3771 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/README.md
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     1033 2024-04-24 06:14:52.000000 py21cmcast-1.0.4/pyproject.toml
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       38 2024-04-24 06:15:01.344017 py21cmcast-1.0.4/setup.cfg
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       37 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/setup.py
+drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-04-24 06:15:01.318017 py21cmcast-1.0.4/src/
+drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-04-24 06:15:01.331017 py21cmcast-1.0.4/src/py21cmcast/
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      833 2024-04-15 11:52:07.000000 py21cmcast-1.0.4/src/py21cmcast/__init__.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       59 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/src/py21cmcast/__main__.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    54910 2024-04-15 15:12:47.000000 py21cmcast-1.0.4/src/py21cmcast/core.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)     5421 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/src/py21cmcast/experiments.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    11671 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/src/py21cmcast/power.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    24784 2024-04-15 14:36:14.000000 py21cmcast-1.0.4/src/py21cmcast/runs.py
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)    28534 2024-03-28 09:43:41.000000 py21cmcast-1.0.4/src/py21cmcast/tools.py
+drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-04-24 06:15:01.340017 py21cmcast-1.0.4/src/py21cmcast.egg-info/
+-rw-r--r--   0 gfacchin (3003741) gfacchin (3003741)    45280 2024-04-24 06:15:01.000000 py21cmcast-1.0.4/src/py21cmcast.egg-info/PKG-INFO
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      434 2024-04-24 06:15:01.000000 py21cmcast-1.0.4/src/py21cmcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)        1 2024-04-24 06:15:01.000000 py21cmcast-1.0.4/src/py21cmcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      129 2024-04-24 06:15:01.000000 py21cmcast-1.0.4/src/py21cmcast.egg-info/requires.txt
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)       11 2024-04-24 06:15:01.000000 py21cmcast-1.0.4/src/py21cmcast.egg-info/top_level.txt
+drwxrwxr-x   0 gfacchin (3003741) gfacchin (3003741)        0 2024-04-24 06:15:01.339017 py21cmcast-1.0.4/tests/
+-rw-rw-r--   0 gfacchin (3003741) gfacchin (3003741)      175 2024-03-07 10:03:18.000000 py21cmcast-1.0.4/tests/test.py
```

### Comparing `py21cmcast-1.0.3/LICENSE` & `py21cmcast-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py21cmcast-1.0.3/PKG-INFO` & `py21cmcast-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py21cmcast
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fisher forecasts with 21cm experiments
 Author-email: Gaétan Facchinetti <gaetanfacc@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py21cmcast-1.0.3/README.md` & `py21cmcast-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py21cmcast-1.0.3/pyproject.toml` & `py21cmcast-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py21cmcast"
-version = "1.0.3"
+version = "1.0.4"
 description = "Fisher forecasts with 21cm experiments"
 readme = "README.md"
 authors = [{ name = "Gaétan Facchinetti", email = "gaetanfacc@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `py21cmcast-1.0.3/src/py21cmcast/__init__.py` & `py21cmcast-1.0.4/src/py21cmcast/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     default_observation_set,
     extract_noise_from_fiducial,
 )
 
 from .runs import (
     init_runs,
     init_grid_runs,
-    read_grid_database,
-    find_in_grid_database,
+    init_random_runs,
     make_config_one_varying_param,
     run_lightcone_from_config,
 )
 
 from .tools import (
     read_config_params,
     write_config_params,
@@ -22,21 +21,24 @@
     plot_func_vs_z_and_k,
     plot_func,
     display_matrix,
     load_uv_luminosity_functions,
     prepare_plot,
     prepare_2subplots,
     prepare_triangle_plot,
+    confidence_ellipse,
+    ellipse_from_covariance,
 )
 
 from .power import (
     define_grid_modes_redshifts,
     generate_k_bins,
 )
 
 from .core import (
     evaluate_fisher_matrix,
+    print_tau_ion_var,
     Fiducial,
     Run,
     CombinedRuns,
     Parameter,
 )
```

### Comparing `py21cmcast-1.0.3/src/py21cmcast/core.py` & `py21cmcast-1.0.4/src/py21cmcast/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,18 @@
             # Compute the power spectrum and fetch global quantities
             self._get_power_spectra()    
             self._get_global_quantities()
 
             # Compute the optical depth to reionization
             if PY21CMFAST:
                 try: 
-                    self._tau_ion = p21f.compute_tau(redshifts=self._z_glob, global_xHI = self.xH_box, user_params=self._user_params, cosmo_params=self._cosmo_params)
+                    if np.all(self._xHIIdb == 0):
+                        self._tau_ion = p21f.compute_tau(redshifts=self._z_glob, global_xHI = self.xH_box, user_params=self._user_params, cosmo_params=self._cosmo_params)
+                    else:
+                        self._tau_ion = p21f.compute_tau(redshifts=self._z_glob, global_xHI = 1-self._xHIIdb, user_params=self._user_params, cosmo_params=self._cosmo_params)
                 except:
                     self._tau_ion = 0.0
                     if self._verbose:
                         warnings.warn("Impossible to compute the optical depth to reionization tau_ion")
                     
             else : 
                 ImportError("21cmFAST is needed to evaluate the optical depth to reionization")
@@ -260,56 +263,65 @@
             self._ps_poisson_noise = np.array([data['err_delta'] for data in _data_arr])
 
             _k_array = np.array([data['k'] for data in _data_arr])
             assert np.all(np.abs(np.diff(_k_array, axis=0)[0]/_k_array) <= 1e-3)
             self._k_array = _k_array[0]
 
         except Exception as e:
-            if self._verbose:
-                warnings.warn("Impossible to compute the power spectra: \n" + str(e))
 
             self._power_spectrum = np.array([])
             self._ps_poisson_noise = np.array([])
             self._k_array = np.array([])
             self._chunk_indices = np.array([])
+            
+            if self._verbose:
+                warnings.warn("Impossible to compute the power spectra: \n" + str(e))
 
 
     
     def _get_global_quantities(self):
 
         _lc_glob_redshifts = self._lightcone.node_redshifts
-        self._z_glob       = np.linspace(_lc_glob_redshifts[-1], _lc_glob_redshifts[0], 500)
+        self._z_glob       = np.linspace(_lc_glob_redshifts[-1], _lc_glob_redshifts[0], 200)
   
         _global_signal = self._lightcone.global_quantities.get('brightness_temp', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
         _xH_box        = self._lightcone.global_quantities.get('xH_box', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
+        _xHIIdb        = self._lightcone.global_quantities.get('xHIIdb', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
         _x_e_box       = self._lightcone.global_quantities.get('x_e_box', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
         _Ts_box        = self._lightcone.global_quantities.get('Ts_box', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
         _Tk_box        = self._lightcone.global_quantities.get('Tk_box', np.zeros(len(_lc_glob_redshifts), dtype=np.float64))
 
+        # constrain the value of the ionization fraction between 0 and 1
+        _xHIIdb[ _xHIIdb > 1.0 ] = 1.0
+        _xHIIdb[ _xHIIdb < 0.0 ] = 0.0
+
         self._global_signal = interpolate.interp1d(_lc_glob_redshifts, _global_signal)(self._z_glob)
         self._xH_box        = interpolate.interp1d(_lc_glob_redshifts, _xH_box)(self._z_glob)
+        self._xHIIdb        = interpolate.interp1d(_lc_glob_redshifts, _xHIIdb)(self._z_glob)
         self._x_e_box       = interpolate.interp1d(_lc_glob_redshifts, _x_e_box)(self._z_glob)
         self._Ts_box        = interpolate.interp1d(_lc_glob_redshifts, _Ts_box)(self._z_glob)
         self._Tk_box        = interpolate.interp1d(_lc_glob_redshifts, _Tk_box)(self._z_glob)
 
 
+
     def _save(self):
         """
         ##  Saves all the attributes of the class to be easily reload later if necessary
 
         numpy arrays are saved in an .npz format
         scalar parameters / attributes are saved in a dictionnary in a .pkl format
         """
 
         with open(self._filename_data, 'wb') as file: 
             np.savez(file, power_spectrum     = self.power_spectrum,
                             ps_poisson_noise  = self.ps_poisson_noise,
                             global_signal     = self.global_signal,
                             chunk_indices     = self.chunk_indices,
                             xH_box            = self.xH_box,
+                            xHIIdb            = self.xHIIdb,
                             x_e_box           = self.x_e_box,
                             Ts_box            = self.Ts_box,
                             Tk_box            = self.Tk_box,
                             z_array           = self.z_array if self.z_array is not None else np.array([]),
                             z_bins            = self.z_bins  if self.z_bins is not None else np.array([]),
                             k_bins            = self.k_bins  if self.k_bins is not None else np.array([]),
                             k_array           = self.k_array,
@@ -345,14 +357,15 @@
                 self._chunk_indices     = data['chunk_indices']
                 self._z_array           = data['z_array']
                 self._k_array           = data['k_array']
                 self._z_bins            = data['z_bins']
                 self._k_bins            = data['k_bins']  / units.Mpc
                 self._global_signal     = data['global_signal']
                 self._xH_box            = data['xH_box']
+                self._xHIIdb            = data['xHIIdb']
                 self._x_e_box           = data.get('x_e_box', None)
                 self._Ts_box            = data.get('Ts_box', None)
                 self._Tk_box            = data.get('Tk_box', None)
                 self._z_glob            = data['z_glob']
                 self._tau_ion           = data['tau_ion'].item()
 
 
@@ -412,14 +425,18 @@
         return self._xH_box
     
     @property
     def x_e_box(self):
         return self._x_e_box
     
     @property
+    def xHIIdb(self):
+        return self._xHIIdb
+    
+    @property
     def Ts_box(self):
         return self._Ts_box
 
     @property
     def Tk_box(self):
         return self._Tk_box
     
@@ -913,14 +930,15 @@
         self._k_bins  = self._fiducial.k_bins
         self._z_bins  = self._fiducial.z_bins
 
         if verbose is True: 
             print("Computing the derivatives of " + self._name)
 
         self.compute_ps_derivative()
+        self.compute_tau_ion_derivative()
 
         if verbose is True: 
             print("Derivative of " + self._name  + " computed")
             print("------------------------------------------")
             
         # Plotting the derivatives
         if self._plot is True:
@@ -1009,14 +1027,59 @@
             self._ps_derivative['left'] = [_der[iz][0] for iz, _ in enumerate(self._z_array)]
         
         if len(self._p_value) == 1 and self._p_value[0] > 0 :
             self._ps_derivative['right'] = [_der[iz][0] for iz, _ in enumerate(self._z_array)]
 
         
 
+    def compute_tau_ion_derivative(self):
+
+        _der = [None] * len(self._z_array)
+        
+        #_param_fid = self._astro_params[self._name]
+
+        # get all the parameters and sort them
+        _params = np.zeros(len(self._runs))
+
+        for irun, run in enumerate(self._runs):
+            _params[irun] = run.p
+
+        _params         = np.append(_params, self._param_fid)
+        _params_sorted  = np.sort(_params)
+        _mixing_params  = np.argsort(_params)
+
+
+        # loop over all the redshift bins
+    
+        # get an array of power spectra in the same order as the parameters
+        _tau_ion = [run.tau_ion for run in self._runs]
+        _tau_ion.append(self._fiducial.tau_ion)
+
+        # rearrange the power spectra in the same order of the parameters
+        _tau_ion_sorted = np.array(_tau_ion)[_mixing_params]        
+
+        # evaluate the derivative as a gradient
+        _der = np.gradient(_tau_ion_sorted, _params_sorted, axis=0)
+
+        # arrange the derivative whether they are left, right or centred
+        self._tau_ion_derivative  = {'left' : None, 'right' : None, 'centred' : None}
+
+        if len(self._p_value) == 2:
+            self._tau_ion_derivative['left']    = _der[0]
+            self._tau_ion_derivative['centred'] = _der[1]
+            self._tau_ion_derivative['right']   = _der[2]
+
+        if len(self._p_value) == 1 and self._p_value[0] < 0 :
+            self._tau_ion_derivative['left'] = _der[0]
+        
+        if len(self._p_value) == 1 and self._p_value[0] > 0 :
+            self._tau_ion_derivative['right'] = _der[0]
+
+
+
     def weighted_ps_derivative(self, kind: str ='centred'):
        
         """
         ## Weighted derivative of the power spectrum with respect to the parameter
         
         Params:
         -------
@@ -1067,14 +1130,49 @@
             der = self._ps_derivative.get('right', None)
 
         if _force_to_one_side is True and self._verbose is True:
             print("Weighted derivative computed from the one_sided derivative")
 
         # We sum (quadratically) the two errors
         return der / np.sqrt(ps_exp_noise**2 + ps_poisson_noise**2 + ps_modeling_noise**2)  
+    
+
+    def tau_ion_derivative(self, kind:str = 'centred'):
+        
+         # Initialize the derivative array to None
+        der = None
+
+        # If two sided derivative is asked then we are good here
+        if kind == 'centred' :
+            der = self._tau_ion_derivative.get('centred', None)
+        
+        # Value to check if we use the one sided derivative 
+        # by choice or because we cannot use the two-sided one
+        _force_to_one_side = False
+
+        # If there is no centred derivative
+        if der is None or kind == 'left':
+            if der is None and kind != 'left' and kind != 'right': 
+                # Means that we could not read a value yet 
+                # but not that we chose to use the left
+                _force_to_one_side = True
+            der = self._tau_ion_derivative.get('left', None)
+        
+        if der is None or kind == 'right':
+            if der is None and kind != 'right' and kind != 'left': 
+                # Means that we could not read a value yet 
+                # but not that we chose to use the right
+                _force_to_one_side = True
+            der = self._tau_ion_derivative.get('right', None)
+
+        if _force_to_one_side is True and self._verbose is True:
+            print("Weighted derivative computed from the one_sided derivative")
+
+        return der
+    
 
 
     def plot_ps_derivative(self):
 
         der_array = []
         for key in self._ps_derivative.keys():
             if self._ps_derivative[key] is not None:
@@ -1153,15 +1251,32 @@
     for i in range(0, n_params) :
         for j in range(0, n_params) :        
             fisher_matrix[i][j] = np.nansum(weighted_der[i] * weighted_der[j])
             
     return {'matrix' : fisher_matrix, 'name' : name_arr}
     
 
-    
+
+def print_tau_ion_var(params):
+
+    der = []
+    fid = []
+
+    res = ""
+
+    for ip, param in enumerate(params):
+        fid = param._param_fid
+        der = param.tau_ion_derivative() * fid
+        name = param.name
+
+        sign = "+" if np.sign(der) > 0 else "-"
+
+        res = res + sign + str(np.abs(der)) + "(" + name + "/" + str(fid) + ")" 
+
+    return res
 
 
 
 
 class CombinedRuns:
     """
     ## Smart collection of the same runs with different random seeds
```

### Comparing `py21cmcast-1.0.3/src/py21cmcast/experiments.py` & `py21cmcast-1.0.4/src/py21cmcast/experiments.py`

 * *Files identical despite different names*

### Comparing `py21cmcast-1.0.3/src/py21cmcast/power.py` & `py21cmcast-1.0.4/src/py21cmcast/power.py`

 * *Files identical despite different names*

### Comparing `py21cmcast-1.0.3/src/py21cmcast/runs.py` & `py21cmcast-1.0.4/src/py21cmcast/runs.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import configparser
 from copy import deepcopy
 import os
 
 from py21cmcast import tools as p21c_tools
 import warnings
 import numpy as np
-import pickle
+import random
 
 PY21CMFAST = True
 try:
     import py21cmfast as p21f
 except ImportError:
     PY21CMFAST = False
     p21f = None
@@ -258,135 +258,50 @@
     except configparser.NoSectionError:
         if verbose: 
             warnings.warn("No section global_quantities provided")
         global_q = {}    
 
 
 
-    extra_params = p21c_tools.read_config_params(config.items('extra_params'), int_type = False)
-    user_params  = p21c_tools.read_config_params(config.items('user_params'))
-    flag_options = p21c_tools.read_config_params(config.items('flag_options'))
-    astro_params = p21c_tools.read_config_params(config.items('astro_params'), int_type = False, allow_lists=True)
-    cosmo_params = p21c_tools.read_config_params(config.items('cosmo_params'), int_type = False, allow_lists=True)
-
+    extra_params      = p21c_tools.read_config_params(config.items('extra_params'), int_type = False)
+    user_params       = p21c_tools.read_config_params(config.items('user_params'))
+    flag_options      = p21c_tools.read_config_params(config.items('flag_options'))
+    astro_params  = p21c_tools.read_config_params(config.items('astro_params'), int_type = False, allow_lists=True)
+    cosmo_params  = p21c_tools.read_config_params(config.items('cosmo_params'), int_type = False, allow_lists=True)
 
-    params_array, params_single = collect_params_arrays(astro_params | cosmo_params)
 
     all_indices = set()
     params = []
     values = []
-
-    # Goes over all astro and cosmo params and makes set of all possible index combinations to get all possible values
     for param_key, param_values in (astro_params | cosmo_params).items():
         all_indices = indices_combinations(param_values, index_combinations=all_indices)
         params.append(param_key)
         values.append(param_values)
 
+    with open(output_run_dir + "/Database.txt", 'a') as file:
 
-    # Create and write the database in a human readable format
-    with open(output_run_dir + "/database.txt", 'a') as file:
-        
-        print("# DATAFILE", file = file)
-        print("##############################", file = file)
-        print("# Unvaried astro parameters", file = file)
-
-        for param in params_single:
-            if param in astro_params:
-                print(param + ' : ' + str(astro_params[param][0]) + ' | ', file = file, end ='')
-        
-        print("", file = file)
-        print("# Unvaried cosmo parameters", file = file)
-        for param in params_single:
-            if param in cosmo_params:
-                print(param + ' : ' + str(cosmo_params[param][0]) + ' | ', file = file, end ='')
-
-        print("", file = file)
-
-        print("##############################", file = file)
-        print("# Varied parameters", file = file) 
-        
-        print("# Index :", file = file, end = '') 
-
-        for param in params_array:
-            print(' | ' + param, file = file, end ='')
-
-        print("", file = file)
-
-        database = {param : [] for param in (astro_params | cosmo_params)}
-
-        for global_ind, indexes in enumerate(all_indices):
+        for iind, indexes in enumerate(all_indices):
             astro_params_print = {}
             cosmo_params_print = {}
             for ival, i in enumerate(indexes):
                 if params[ival] in astro_params:
                     astro_params_print = astro_params_print | {params[ival] :  values[ival][i]}
                 if params[ival] in cosmo_params:
                     cosmo_params_print = cosmo_params_print | {params[ival] :  values[ival][i]}
             
-                database[params[ival]].append(values[ival][i])
-            
-            p21c_tools.write_config_params(output_run_dir + '/Config_' + str(global_ind) + ".config", name, output_run_dir, cache_dir, 
-                                    lightcone_q, global_q, extra_params, user_params, flag_options, astro_params_print, cosmo_params_print, str(global_ind))
+            key = iind
+            p21c_tools.write_config_params(output_run_dir + '/Config_' + str(key) + ".config", name, output_run_dir, cache_dir, 
+                                    lightcone_q, global_q, extra_params, user_params, flag_options, astro_params_print, cosmo_params_print, str(key))
 
-            # ---------------------------- #
-            for param in params_array:
-                if param in astro_params:
-                    print(' ' + str(astro_params_print[param]), file=file, end='')
-                if param in cosmo_params:
-                    print(' ' + str(cosmo_params_print[param]), file=file, end='')
-            print("", file=file) 
-            # ---------------------------- #
-                
+            print(str(key) + ' : ' + str(astro_params_print) + ' | ' + str(cosmo_params_print), file=file)
         file.close()
-
-    # Write database in a machine readable format
-    with open(output_run_dir + "/database.pkl", 'wb') as file:
-        pickle.dump(database, file)
     
     print(str(len(all_indices)) + ' config files generated')
 
 
-def read_grid_database(dir_path:str):
-
-    with open(dir_path + '/database.pkl', 'rb') as file:
-        database = pickle.load(file)
-
-    return database
-
-
-def find_in_grid_database(database, **kwargs):
-
-    indices = []
-
-    for key, value in kwargs.items():
-        indices.append([i for i, j in enumerate(database[key]) if j == value])
-
-
-    common_indices = set(indices[0])  # Initialize with the first list
-    for sublist in indices[1:]:
-        common_indices = common_indices.intersection(sublist)
-
-    # Convert the set to a list if needed
-    return list(common_indices)
-
-
-
-def collect_params_arrays(params):
-
-    params_array = []
-    params_single = []
-
-    for key, value in params.items():
-        if len(value) > 1:
-            params_array.append(key)
-        else:
-            params_single.append(key)
-            
-    return params_array, params_single
-
 
 def indices_combinations(*arrays, index_combinations=None):    
     # Initialize index_combinations as an empty set for the first call
     if index_combinations is None:
         index_combinations = set()
 
     # Base case: if there are no more arrays, return the current set of index combinations
@@ -410,14 +325,126 @@
 
     # Recur with remaining arrays and the updated index_combinations
     return indices_combinations(*arrays[1:], index_combinations=index_combinations)
        
 
     
 
+def init_random_runs(config_file: str, *, n_sample = 1000, random_seed = None, clean_existing_dir: bool = False, verbose:bool = False) -> None:
+    
+    config = configparser.ConfigParser(delimiters=':')
+    config.optionxform = str
+
+    config.read(config_file)
+
+    name            = config.get('run', 'name')
+    output_dir      = config.get('run', 'output_dir')
+    cache_dir       = config.get('run', 'cache_dir')
+
+    output_run_dir = output_dir + "/" + name.upper() + "/"
+    existing_dir = p21c_tools.make_directory(output_run_dir, clean_existing_dir = clean_existing_dir)
+
+    if existing_dir is True:
+        print('WARNING: Cannot create a clean new folder because clean_existing_dir is False')
+        return 
+
+    try:
+        lightcone_q       = p21c_tools.read_config_params(config.items('lightcone_quantities'))
+    except configparser.NoSectionError:
+        if verbose: 
+            warnings.warn("No section lightcone_quantities provided")
+        lightcone_q = {}
+
+    try:
+        global_q       = p21c_tools.read_config_params(config.items('global_quantities'))
+    except configparser.NoSectionError:
+        if verbose: 
+            warnings.warn("No section global_quantities provided")
+        global_q = {}    
+
+
+    extra_params  = p21c_tools.read_config_params(config.items('extra_params'), int_type = False)
+    user_params   = p21c_tools.read_config_params(config.items('user_params'))
+    flag_options  = p21c_tools.read_config_params(config.items('flag_options'))
+    astro_params  = p21c_tools.read_config_params(config.items('astro_params'), int_type = False, allow_lists=True)
+    cosmo_params  = p21c_tools.read_config_params(config.items('cosmo_params'), int_type = False, allow_lists=True)
+
+
+    params_astro = []
+    params_cosmo = []
+    draws  = []
+
+    # set the random seed
+    random.seed(random_seed)
+
+    for i in range(0, n_sample): 
+
+        # Initialise the parameters
+        params_astro.append({ k : 0 for k in astro_params.keys()})
+        params_cosmo.append({ k : 0 for k in cosmo_params.keys()})
+        draws.append({ k : -1 for k in (astro_params | cosmo_params).keys()})
+
+        for param_key, param_values in (astro_params | cosmo_params).items():
+
+            # if the user enters a wrong input table
+            assert(len(param_values) < 3), "For random generator, can only define min and max values."
+
+            # parameter to randomly draw between min and max values
+            if len(param_values) == 2:
+                u = random.random()
+                if param_key in astro_params:
+                    params_astro[i][param_key] = (param_values[1] - param_values[0])*u  + param_values[0]
+                if param_key in cosmo_params:
+                    params_cosmo[i][param_key] = (param_values[1] - param_values[0])*u  + param_values[0]
+                draws[i][param_key] = u
+
+            # parameter fixed at a given value
+            if len(param_values) == 1:
+                if param_key in astro_params:
+                    params_astro[i][param_key] = param_values[0]
+                if param_key in cosmo_params:
+                    params_cosmo[i][param_key] = param_values[0]
+
+                # remove the parameter in the dictionnary of draws as nothing is drawn for that parameter
+                draws[i].pop(param_key)
+            
+        
+    with open(output_run_dir + "/Database.txt", 'a') as file:
+
+        print("# random seed = " + str(random_seed), file=file)
+
+        for i in range(0, n_sample): 
+            p21c_tools.write_config_params(output_run_dir + '/Config_' + str(i) + ".config", name, output_run_dir, cache_dir, 
+                                    lightcone_q, global_q, extra_params, user_params, flag_options, params_astro[i], params_cosmo[i], str(i))
+
+            print(str(i) + ' : ' + str(params_astro[i] | params_cosmo[i]), file=file)
+        
+        file.close()
+
+    with open(output_run_dir + "Database.npz", 'wb') as file:
+        np.savez(file, params_astro = params_astro, params_cosmo = params_cosmo, random_seed = random_seed)
+        file.close()
+
+    # Create a file containing the uniform distributions
+    with open(output_run_dir + "/Uniform.txt", 'a') as file:
+
+        print("# random seed = " + str(random_seed), file=file)
+
+        for i in range(0, n_sample): 
+            print(str(i) + ' : ' + str(draws[i]), file=file)
+
+        file.close()
+
+    with open(output_run_dir + "Uniform.npz", 'wb') as file:
+        np.savez(file, draws = draws, random_seed = random_seed)
+        file.close()
+    
+    print(str(n_sample) + ' config files generated with random seed : ' +  str(random_seed))
+    
+
 
 
 
 def make_config_one_varying_param(config_file: str, param_name: str, values, **kwargs):
 
     config = configparser.ConfigParser(delimiters=':')
     config.optionxform = str
@@ -531,14 +558,15 @@
 
     extra_params    = p21c_tools.read_config_params(config.items('extra_params'), int_type=False)
     user_params     = p21c_tools.read_config_params(config.items('user_params'))
     flag_options    = p21c_tools.read_config_params(config.items('flag_options'))
     astro_params    = p21c_tools.read_config_params(config.items('astro_params'), int_type=False)
     cosmo_params    = p21c_tools.read_config_params(config.items('cosmo_params'), int_type=False)
 
+
     # manually set the number of threads
     if n_omp is not None: 
         user_params['N_THREADS'] = int(n_omp)
 
     seed_str : str = ''
     if random_seed is not None:
         seed_str = 'rs' + str(random_seed) + '_'
```

### Comparing `py21cmcast-1.0.3/src/py21cmcast/tools.py` & `py21cmcast-1.0.4/src/py21cmcast/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                 cast_val = make_list(value, int_type)
             if allow_lists is False:
                 if int_type is True:
                     cast_val = int(value)
                 else:
                     cast_val = float(value)
         except:
+                
             if value == 'True':
                 cast_val =  True
             elif value == 'False':
                 cast_val =  False
             else:   
                 cast_val = value
     
@@ -328,18 +329,22 @@
     'DM_FHEAT_APPROX_PARAM_LOG10_F0' : {'tex_name' : r'\log_{10}[f_0]', 'min': -2, 'max': 1,  'ticks' : []},
     'DM_FHEAT_APPROX_PARAM_A'  : {'tex_name' : r'a', 'min': -2, 'max': 1,  'ticks' : []},
     'DM_FHEAT_APPROX_PARAM_B'  : {'tex_name' : r'b', 'min': -2, 'max': 1,  'ticks' : []},
     'LOG10_XION_at_Z_HEAT_MAX' : {'tex_name' : r'\log_{10}[\bar x_e^{\rm init}]', 'min': -2, 'max': 1,  'ticks' : []},
     'LOG10_TK_at_Z_HEAT_MAX'   : {'tex_name' : r'\log_{10}[\frac{\bar T_K^{\rm init}}{\rm K}]', 'min': -2, 'max': 1,  'ticks' : []},
     'OMm'   : {'tex_name' : r'\Omega_{\rm m}', 'min': -2, 'max': 1,  'ticks' : []},
     'OMb'   : {'tex_name' : r'\Omega_{\rm b}', 'min': -2, 'max': 1,  'ticks' : []},
+    'Omch2'   : {'tex_name' : r'\Omega_{\rm c}h^2', 'min': -2, 'max': 1,  'ticks' : []},
+    'Ombh2'   : {'tex_name' : r'\Omega_{\rm b}h^2', 'min': -2, 'max': 1,  'ticks' : []},
     'hlittle'   : {'tex_name' : r'h', 'min': -2, 'max': 1,  'ticks' : []},
+    'Ln_1010_As'   : {'tex_name' : r'\ln(10^{10} A_{\rm s})', 'min': -2, 'max': 1,  'ticks' : []},
     'SIGMA_8'   : {'tex_name' : r'\sigma_8', 'min': -2, 'max': 1,  'ticks' : []},
     'POWER_INDEX'   : {'tex_name' : r'n_{\rm s}', 'min': -2, 'max': 1,  'ticks' : []},
     'INVERSE_M_WDM'   : {'tex_name' : r'1/m_{\rm WDM}', 'min': -2, 'max': 1,  'ticks' : []},
+    'NEUTRINO_MASS_1'   : {'tex_name' : r'm_{\nu, 1} ~ [{\rm eV}]', 'min': -2, 'max': 1,  'ticks' : []},
     }
 
 
 def make_triangle_plot(covariance, fiducial_params, **kwargs) : 
 
     #####################################
     ## Choose the data we want to look at
@@ -428,15 +433,17 @@
                 x_min = val_min[i_name]
                 x_max = val_max[i_name]
                 y_min = val_min[j_name]
                 y_max = val_max[j_name]
 
                 axs[j_name][i_name].set_xlim([x_min, x_max])
 
-                if i != j :     
+                if i != j :   
+                    if y_min == np.NaN or y_min == np.Inf or y_max == np.NaN or y_max == np.Inf:
+                        print("Problem here: ", j_name, " ", i_name)
                     axs[j_name][i_name].set_ylim([y_min, y_max])
 
                 if i == j :
                     axs[i_name][i_name].set_ylim([0, 1.2])
 
 
                 ##############
@@ -721,14 +728,20 @@
         ax2.set_yscale('log')
 
     return fig, (ax1, ax2)
 
 
 
 
+def close_figure(fig):
+    """ close the figure fig """
+    plt.close(fig)
+    
+
+
 def plot_func(x, func, **kwargs) :
 
     """ 
         Function that plots simple functions of one variable on the same graph
 
         Params
         ------
```

### Comparing `py21cmcast-1.0.3/src/py21cmcast.egg-info/PKG-INFO` & `py21cmcast-1.0.4/src/py21cmcast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py21cmcast
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fisher forecasts with 21cm experiments
 Author-email: Gaétan Facchinetti <gaetanfacc@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

