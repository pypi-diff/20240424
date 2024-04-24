# Comparing `tmp/localstack-3.3.1.dev20240419073811.tar.gz` & `tmp/localstack-3.3.1.dev20240424163921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-3.3.1.dev20240419073811.tar", last modified: Fri Apr 19 07:41:27 2024, max compression
+gzip compressed data, was "localstack-3.3.1.dev20240424163921.tar", last modified: Wed Apr 24 16:44:26 2024, max compression
```

## Comparing `localstack-3.3.1.dev20240419073811.tar` & `localstack-3.3.1.dev20240424163921.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-19 07:41:27.321064 localstack-3.3.1.dev20240419073811/
--rw-rw-r--   0 runner    (1000) runner    (1001)       16 2024-04-19 07:37:13.000000 localstack-3.3.1.dev20240419073811/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1001)    13928 2024-04-19 07:41:27.321064 localstack-3.3.1.dev20240419073811/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)       24 2024-04-19 07:41:26.000000 localstack-3.3.1.dev20240419073811/VERSION
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-19 07:41:27.321064 localstack-3.3.1.dev20240419073811/localstack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)    13928 2024-04-19 07:41:27.000000 localstack-3.3.1.dev20240419073811/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      197 2024-04-19 07:41:27.000000 localstack-3.3.1.dev20240419073811/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-19 07:41:27.000000 localstack-3.3.1.dev20240419073811/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      141 2024-04-19 07:41:27.000000 localstack-3.3.1.dev20240419073811/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-19 07:41:27.000000 localstack-3.3.1.dev20240419073811/localstack.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-19 07:41:27.321064 localstack-3.3.1.dev20240419073811/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1564 2024-04-19 07:37:13.000000 localstack-3.3.1.dev20240419073811/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-24 16:44:26.962118 localstack-3.3.1.dev20240424163921/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       16 2024-04-24 16:38:53.000000 localstack-3.3.1.dev20240424163921/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1001)    13928 2024-04-24 16:44:26.962118 localstack-3.3.1.dev20240424163921/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)       24 2024-04-24 16:44:25.000000 localstack-3.3.1.dev20240424163921/VERSION
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-24 16:44:26.962118 localstack-3.3.1.dev20240424163921/localstack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)    13928 2024-04-24 16:44:26.000000 localstack-3.3.1.dev20240424163921/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      197 2024-04-24 16:44:26.000000 localstack-3.3.1.dev20240424163921/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-24 16:44:26.000000 localstack-3.3.1.dev20240424163921/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      141 2024-04-24 16:44:26.000000 localstack-3.3.1.dev20240424163921/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-24 16:44:26.000000 localstack-3.3.1.dev20240424163921/localstack.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-24 16:44:26.962118 localstack-3.3.1.dev20240424163921/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1564 2024-04-24 16:38:53.000000 localstack-3.3.1.dev20240424163921/setup.py
```

### Comparing `localstack-3.3.1.dev20240419073811/PKG-INFO` & `localstack-3.3.1.dev20240424163921/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 3.3.1.dev20240419073811
+Version: 3.3.1.dev20240424163921
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Requires-Dist: localstack-core
-Requires-Dist: localstack-ext==3.3.1.dev20240419073811
+Requires-Dist: localstack-ext==3.3.1.dev20240424163921
 Provides-Extra: runtime
 Requires-Dist: localstack-core[runtime]; extra == "runtime"
-Requires-Dist: localstack-ext[runtime]==3.3.1.dev20240419073811; extra == "runtime"
+Requires-Dist: localstack-ext[runtime]==3.3.1.dev20240424163921; extra == "runtime"
 
 <p align="center">
 :zap: We are thrilled to announce the release of <a href="https://discuss.localstack.cloud/t/localstack-release-v3-3-0/828">LocalStack 3.3</a> :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: localstack Version: 3.3.1.dev20240419073811
+Metadata-Version: 2.1 Name: localstack Version: 3.3.1.dev20240424163921
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Requires-Dist: localstack-core Requires-Dist:
-localstack-ext==3.3.1.dev20240419073811 Provides-Extra: runtime Requires-Dist:
+localstack-ext==3.3.1.dev20240424163921 Provides-Extra: runtime Requires-Dist:
 localstack-core[runtime]; extra == "runtime" Requires-Dist: localstack-ext
-[runtime]==3.3.1.dev20240419073811; extra == "runtime"
+[runtime]==3.3.1.dev20240424163921; extra == "runtime"
      :zap: We are thrilled to announce the release of _L_o_c_a_l_S_t_a_c_k_ _3_._3 :zap:
               [LocalStack - A fully functional local cloud stack]
 _[_C_i_r_c_l_e_C_I_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _P_u_l_l_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_B_a_c_k_e_r_s
   _o_n_ _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e_]_[_S_p_o_n_s_o_r_s_ _o_n_ _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e_]_[_P_y_P_I_ _L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:
                              _b_l_a_c_k_]_[_R_u_f_f_]_[_T_w_i_t_t_e_r_]
  LocalStack is a cloud software development framework to develop and test your
                            AWS applications locally.
```

### Comparing `localstack-3.3.1.dev20240419073811/localstack.egg-info/PKG-INFO` & `localstack-3.3.1.dev20240424163921/localstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 3.3.1.dev20240419073811
+Version: 3.3.1.dev20240424163921
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Requires-Dist: localstack-core
-Requires-Dist: localstack-ext==3.3.1.dev20240419073811
+Requires-Dist: localstack-ext==3.3.1.dev20240424163921
 Provides-Extra: runtime
 Requires-Dist: localstack-core[runtime]; extra == "runtime"
-Requires-Dist: localstack-ext[runtime]==3.3.1.dev20240419073811; extra == "runtime"
+Requires-Dist: localstack-ext[runtime]==3.3.1.dev20240424163921; extra == "runtime"
 
 <p align="center">
 :zap: We are thrilled to announce the release of <a href="https://discuss.localstack.cloud/t/localstack-release-v3-3-0/828">LocalStack 3.3</a> :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: localstack Version: 3.3.1.dev20240419073811
+Metadata-Version: 2.1 Name: localstack Version: 3.3.1.dev20240424163921
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Requires-Dist: localstack-core Requires-Dist:
-localstack-ext==3.3.1.dev20240419073811 Provides-Extra: runtime Requires-Dist:
+localstack-ext==3.3.1.dev20240424163921 Provides-Extra: runtime Requires-Dist:
 localstack-core[runtime]; extra == "runtime" Requires-Dist: localstack-ext
-[runtime]==3.3.1.dev20240419073811; extra == "runtime"
+[runtime]==3.3.1.dev20240424163921; extra == "runtime"
      :zap: We are thrilled to announce the release of _L_o_c_a_l_S_t_a_c_k_ _3_._3 :zap:
               [LocalStack - A fully functional local cloud stack]
 _[_C_i_r_c_l_e_C_I_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _P_u_l_l_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_B_a_c_k_e_r_s
   _o_n_ _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e_]_[_S_p_o_n_s_o_r_s_ _o_n_ _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e_]_[_P_y_P_I_ _L_i_c_e_n_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:
                              _b_l_a_c_k_]_[_R_u_f_f_]_[_T_w_i_t_t_e_r_]
  LocalStack is a cloud software development framework to develop and test your
                            AWS applications locally.
```

### Comparing `localstack-3.3.1.dev20240419073811/setup.py` & `localstack-3.3.1.dev20240424163921/setup.py`

 * *Files identical despite different names*

