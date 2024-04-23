# Comparing `tmp/berremueller-1.0.3.tar.gz` & `tmp/berremueller-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berremueller-1.0.3.tar", last modified: Wed Apr 17 22:36:02 2024, max compression
+gzip compressed data, was "berremueller-1.0.4.tar", last modified: Tue Apr 23 22:25:04 2024, max compression
```

## Comparing `berremueller-1.0.3.tar` & `berremueller-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:36:02.561865 berremueller-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1735 2024-04-17 22:36:02.561865 berremueller-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.0.3/README.md
--rw-rw-rw-   0        0        0      475 2024-04-17 22:35:48.000000 berremueller-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 22:36:02.563326 berremueller-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-16 23:09:45.000000 berremueller-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:36:02.493274 berremueller-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 22:36:02.541938 berremueller-1.0.3/src/berremueller/
--rw-rw-rw-   0        0        0        2 2024-04-16 23:07:11.000000 berremueller-1.0.3/src/berremueller/__init__.py
--rw-rw-rw-   0        0        0    45154 2024-04-16 23:15:34.000000 berremueller-1.0.3/src/berremueller/berreman_mueller.py
--rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.0.3/src/berremueller/cholesteric.py
--rw-rw-rw-   0        0        0    77860 2024-04-16 23:15:34.000000 berremueller-1.0.3/src/berremueller/dielectric_tensor.py
--rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.0.3/src/berremueller/field_plotting.py
--rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.0.3/src/berremueller/full_berreman.py
--rw-rw-rw-   0        0        0    60257 2024-04-17 20:54:46.000000 berremueller-1.0.3/src/berremueller/mueller.py
--rw-rw-rw-   0        0        0   157207 2024-04-16 23:15:34.000000 berremueller-1.0.3/src/berremueller/pyllama.py
--rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.0.3/src/berremueller/python_util.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:36:02.560598 berremueller-1.0.3/src/berremueller.egg-info/
--rw-rw-rw-   0        0        0     1735 2024-04-17 22:36:02.000000 berremueller-1.0.3/src/berremueller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2024-04-17 22:36:02.000000 berremueller-1.0.3/src/berremueller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:36:02.000000 berremueller-1.0.3/src/berremueller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-17 22:36:02.000000 berremueller-1.0.3/src/berremueller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-17 22:36:02.000000 berremueller-1.0.3/src/berremueller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.264253 berremueller-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1735 2024-04-23 22:25:04.262888 berremueller-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.0.4/README.md
+-rw-rw-rw-   0        0        0      475 2024-04-23 22:24:56.000000 berremueller-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:25:04.264253 berremueller-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-16 23:09:45.000000 berremueller-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.236427 berremueller-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.249103 berremueller-1.0.4/src/berremueller/
+-rw-rw-rw-   0        0        0        2 2024-04-16 23:07:11.000000 berremueller-1.0.4/src/berremueller/__init__.py
+-rw-rw-rw-   0        0        0    45413 2024-04-23 22:24:04.000000 berremueller-1.0.4/src/berremueller/berreman_mueller.py
+-rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.0.4/src/berremueller/cholesteric.py
+-rw-rw-rw-   0        0        0    77860 2024-04-16 23:15:34.000000 berremueller-1.0.4/src/berremueller/dielectric_tensor.py
+-rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.0.4/src/berremueller/field_plotting.py
+-rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.0.4/src/berremueller/full_berreman.py
+-rw-rw-rw-   0        0        0    60257 2024-04-17 20:54:46.000000 berremueller-1.0.4/src/berremueller/mueller.py
+-rw-rw-rw-   0        0        0   157207 2024-04-16 23:15:34.000000 berremueller-1.0.4/src/berremueller/pyllama.py
+-rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.0.4/src/berremueller/python_util.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:25:04.262888 berremueller-1.0.4/src/berremueller.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 22:25:04.000000 berremueller-1.0.4/src/berremueller.egg-info/top_level.txt
```

### Comparing `berremueller-1.0.3/LICENSE` & `berremueller-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/PKG-INFO` & `berremueller-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.3/README.md` & `berremueller-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/berreman_mueller.py` & `berremueller-1.0.4/src/berremueller/berreman_mueller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import copy
 
 import numpy as np
 from numpy.linalg import inv
 from numpy.linalg import multi_dot
-
 from berremueller import cholesteric
 from berremueller import  mueller
 from berremueller import pyllama
 from berremueller import dielectric_tensor as dt
 import warnings
-
+import pandas as pd
 
 '''Handling of Jones vectors and Mueller matrices, particularly those coming from
 numeric calculations
 
 Mostly an extension of mueller.py with specific focus on transfer/scattering matrix calcs
 
 Also includes functions for the construction of cavity systems for transfer/scattering matrix
 calcs 
 
 Convention: (1,1j) is LHP, keeping pyllama's convention (most of the rest of the codebase reverts this)
 '''
 
+
 def get_intensity_from_jones_vector(jones_vector):
     '''Jones vector converstion to intensity. Polarization axis must be 0'''
     return np.abs(jones_vector[0,...])**2+np.abs(jones_vector[1,...])**2
 
 def berre_dim_handling(berre_dim,reflection_matrix,transmission_matrix,input_vector):
     '''Converts jones reflection and transmission matrices of dimension 2-4 to transfer
     vectors for arbitrary polarization input'''
@@ -96,17 +96,17 @@
         input_n, input_a, input_b = np.array([1, 1]) / np.sqrt(2), np.array([1, 1j])/np.sqrt(2), np.array([1, -1j])/np.sqrt(2)
     else: input_n, input_a, input_b=  np.array([1,1])/np.sqrt(2),np.array([1,0]),np.array([0,1])
     input_all = np.vstack([input_n,input_a,input_b])
     trans_all = np.zeros((3,np.size(transmission_matrix,axis = -1)))
     refl_all = np.zeros((3,np.size(reflection_matrix,axis = -1)))
     for i in np.arange(np.size(input_all,axis =0)):
         if (style == "amplitude"):
-            refl_all[i,:], trans_all[i,:] = reflection_transmission_from_amplitude_matrices(reflection_matrix,transmission_matrix,input_all[i,:],kz_in = kz_in,kz_out = kz_out)
+            refl_all[i,:], trans_all[i,:] = reflection_transmission_from_amplitude_matrices(reflection_matrix,transmission_matrix,input_all[i,:])
         elif (style == "intensity"):
-            refl_all[i, :], trans_all[i, :] = reflection_transmission_from_intensity_matrices(reflection_matrix,transmission_matrix,input_all[i, :],kz_in = kz_in,kz_out = kz_out)
+            refl_all[i, :], trans_all[i, :] = reflection_transmission_from_intensity_matrices(reflection_matrix,transmission_matrix,input_all[i, :])
         else:
             raise ValueError("Invalid style")
     return refl_all, trans_all
 
 
 
 def reflection_transmission_from_intensity_matrices(reflection_matrix,transmission_matrix,input_vector):
@@ -117,15 +117,15 @@
     r_vec, t_vec = berre_dim_handling(berre_dim, reflection_matrix, transmission_matrix, input_vector)
     r_intensity = r_vec[0,...]+r_vec[1,...]
     t_intensity = t_vec[0,...]+t_vec[1,...]
     return r_intensity, t_intensity
 
 def kron_vectorized(a,b):
     '''
-    kronecker product implmented to take advantage of numpy
+    kronecker product implmented so as to take advantage of numpy
     vectorization when calculating a stack of products
     Much faster than a for loop caclulating each stack
     :param a: np.ndarray (shape (N,N,X))
     :param b:  np.ndarray (shape (N,N,X))
     :return:
     '''
     i,j,x = a.shape
@@ -450,15 +450,16 @@
     '''
     Provides strained dielectric tensor
     :param eps_constant:
     :param stress_tensor:
     :param elastic_material: dt.Elastic_Material
     :return:
     '''
-    strain_tensor = dt.strain_tensor_hookes_law_isotropic_from_stress(stress_tensor,elastic_material.get_stiffness_matrix())
+    strain_tensor = dt.strain_tensor_hookes_law_isotropic_from_stress(stress_tensor,
+                                                                     elastic_material.get_stiffness_matrix())
     electrostriction_params = dt.get_electrostriction_parameters(eps_constant,material_type="isotropic")
     eps_tensor = dt.strain_dielectric_tensor(eps_constant, strain_tensor, electrostriction_params)
     return eps_tensor
 
 def create_pyllama_spectrum_dict(cur_angle,model_args,**other_args):
     model_args = {**model_args,**other_args}
     model_args.update({"theta_in_rad": cur_angle})
@@ -491,14 +492,15 @@
                         wl_eps_set = wl_nm_list,eps_list =eps_total_list,thickness_nm_list = thick_total_list,
                         n_entry = n_entry,n_exit = n_exit,rotangle_rad= 0,rotaxis = "z"),**other_args)
         cur_spectrum = pyllama.Spectrum(spec_nm_set,model_type,
                                 model_args)
         cur_r,cur_t = get_refl_trans_matrix_spectra(cur_spectrum,coef_type=type,circ=  circ,talk= talk,method = "SM")
         r_matrix_set[:,:,:,i],t_matrix_set[:,:,:,i] = cur_r, cur_t
     return r_matrix_set,t_matrix_set
+
 def rotate_rank2_tensor_stack(rotation_matrix,tensor):
     '''
     :param rotation_matrix:
     :param tensor:
     :return:
     '''
     return np.einsum("ij,jkl->ikl", rotation_matrix,np.einsum("ijl,jk->ikl", tensor, np.transpose(rotation_matrix)))
@@ -623,15 +625,15 @@
         if (a==1):
             x_flip_rotation_matrix = np.array([[1,0,0],[0,-1,0],[0,0,-1]]) #flips object about its x axis
             material_stack_object.rotate_tensors(rotation_matrix=x_flip_rotation_matrix)
         for i in range(np.size(azimuthal_set)):
             cur_azimuthal_angle = azimuthal_set[i]
             for j in range(np.size(polar_angle_set)):
                 cur_polar_angle = polar_angle_set[j]
-                rotation_matrix = pyllama.euler_rotation_matrix(0,0,cur_polar_angle)
+                rotation_matrix = dt.euler_rotation_matrix(0,0,cur_polar_angle)
                 rotated_material_stack = material_stack_object.get_rotated_object(rotation_matrix)
                 if (model_type == "CholestericModel"):
                     other_args.update({'chole':chole,'eps':rotated_material_stack.eps_list[0],
                                        'wl_eps_set': rotated_material_stack.wl_nm_list[0],
                                        'eps_set': rotated_material_stack.eps_list[0]})
                 if (tensor_handling=="full"):
                     if (model_type == "StackModel"):
@@ -666,15 +668,25 @@
     def __init__(self,data,spec_nm,set_indicators):
         self.data = data
         self.spec_nm = spec_nm
         self.indicators = set_indicators
 
 
 
-def characterize_solo_sample_ps(dielectric_tensor,wl_nm_array,spec,thickness_nm,theta_in_rad = 0,talk = "True"):
+def characterize_solo_sample_ps(dielectric_tensor,wl_nm_array,spec,thickness_nm,theta_in_rad = 0,talk = "True",method="SM"):
+    '''
+    :param dielectric_tensor:
+    :param wl_nm_array:
+    :param spec:
+        spectrum (in eV) of sample
+    :param thickness_nm:
+    :param theta_in_rad:
+    :param talk:
+    :return:
+    '''
     eps_tensor_set = dielectric_tensor
     eps_tensor = dielectric_tensor[:, :, 0]
     wl_eps_set = dt.nm_to_eV(spec)
     n_entry = 1
     n_exit = 1
     spectrum = pyllama.Spectrum(wl_nm_array, "SlabModel",
                                 dict(eps_set=eps_tensor_set,
@@ -682,15 +694,15 @@
                                      eps=eps_tensor,
                                      thickness_nm=thickness_nm,
                                      n_entry=n_entry,
                                      n_exit=n_exit,
                                      theta_in_rad=theta_in_rad,
                                      rotangle_rad=0,
                                      rotaxis="z"))
-    spectrum.calculate_refl_trans_coefs(circ=False, method="SM", talk=talk)
+    spectrum.calculate_refl_trans_coefs(circ=False, method=method, talk=talk)
     r, t = spectrum.export_r_t_matrices(type="amplitude", matrix_type='ps')
     return r,t
 
 def characterize_solo_sample_intensity_ps(dielectric_tensor,wl_nm_array,spec,thickness_nm,theta_in_rad = 0,talk = "True"):
     eps_tensor_set = dielectric_tensor
     eps_tensor = dielectric_tensor[:, :, 0]
     wl_eps_set = dt.nm_to_eV(spec)
```

### Comparing `berremueller-1.0.3/src/berremueller/cholesteric.py` & `berremueller-1.0.4/src/berremueller/cholesteric.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/dielectric_tensor.py` & `berremueller-1.0.4/src/berremueller/dielectric_tensor.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/field_plotting.py` & `berremueller-1.0.4/src/berremueller/field_plotting.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/full_berreman.py` & `berremueller-1.0.4/src/berremueller/full_berreman.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/mueller.py` & `berremueller-1.0.4/src/berremueller/mueller.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/pyllama.py` & `berremueller-1.0.4/src/berremueller/pyllama.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller/python_util.py` & `berremueller-1.0.4/src/berremueller/python_util.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.3/src/berremueller.egg-info/PKG-INFO` & `berremueller-1.0.4/src/berremueller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.3/src/berremueller.egg-info/SOURCES.txt` & `berremueller-1.0.4/src/berremueller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

