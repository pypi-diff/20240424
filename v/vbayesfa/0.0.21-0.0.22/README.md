# Comparing `tmp/vbayesfa-0.0.21.tar.gz` & `tmp/vbayesfa-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbayesfa-0.0.21.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vbayesfa-0.0.22.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vbayesfa-0.0.21.tar` & `vbayesfa-0.0.22.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      234 2024-04-22 20:48:06.351350 vbayesfa-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.21/src/vbayesfa/.DS_Store
--rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.21/src/vbayesfa/__init__.py
--rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.21/src/vbayesfa/bayes_factors.py
--rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.21/src/vbayesfa/exp_families.py
--rw-r--r--   0        0        0     7482 2024-04-14 18:39:13.977771 vbayesfa-0.0.21/src/vbayesfa/finite_lpa.py
--rw-r--r--   0        0        0     4176 2024-04-11 18:23:10.081833 vbayesfa-0.0.21/src/vbayesfa/fit_finite_lpa.py
--rw-r--r--   0        0        0     3800 2024-04-15 14:08:40.305148 vbayesfa-0.0.21/src/vbayesfa/fit_lpa.py
--rw-r--r--   0        0        0     3893 2024-04-15 14:10:42.994079 vbayesfa-0.0.21/src/vbayesfa/fit_lpa2.py
--rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.21/src/vbayesfa/ibp/discrete_finite.py
--rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.21/src/vbayesfa/ibp/fit_ibp.py
--rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.21/src/vbayesfa/ibp/full_discrete_finite.py
--rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.21/src/vbayesfa/ibp/make_sim_data.py
--rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.21/src/vbayesfa/ibp/sparse_cont_finite.py
--rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.21/src/vbayesfa/ibp/sparse_pos_cont_finite.py
--rw-r--r--   0        0        0    10792 2024-04-14 18:38:41.582080 vbayesfa-0.0.21/src/vbayesfa/lpa.py
--rw-r--r--   0        0        0    20925 2024-04-10 19:09:07.425525 vbayesfa-0.0.21/src/vbayesfa/lpa_outcome_analysis.py
--rw-r--r--   0        0        0    35869 2024-04-14 18:50:12.079725 vbayesfa-0.0.21/src/vbayesfa/mixture_model.py
--rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.21/src/vbayesfa/old_lpa.py
--rw-r--r--   0        0        0    10712 2024-04-17 21:13:53.670539 vbayesfa-0.0.21/src/vbayesfa/simulate_data.py
--rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.21/src/vbayesfa/tests/.DS_Store
--rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.21/src/vbayesfa/tests/test_exp_families.py
--rw-r--r--   0        0        0     1633 2024-04-12 14:18:41.718223 vbayesfa-0.0.21/src/vbayesfa/tests/test_lpa.py
--rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.21/src/vbayesfa/tests/test_lpa_outcome_analysis.py
--rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0      234 2024-04-24 20:35:53.884246 vbayesfa-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.22/src/vbayesfa/.DS_Store
+-rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.22/src/vbayesfa/__init__.py
+-rw-r--r--   0        0        0    16841 2024-04-08 17:09:57.330242 vbayesfa-0.0.22/src/vbayesfa/bayes_factors.py
+-rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.22/src/vbayesfa/exp_families.py
+-rw-r--r--   0        0        0     7482 2024-04-14 18:39:13.977771 vbayesfa-0.0.22/src/vbayesfa/finite_lpa.py
+-rw-r--r--   0        0        0     4176 2024-04-11 18:23:10.081833 vbayesfa-0.0.22/src/vbayesfa/fit_finite_lpa.py
+-rw-r--r--   0        0        0     3800 2024-04-15 14:08:40.305148 vbayesfa-0.0.22/src/vbayesfa/fit_lpa.py
+-rw-r--r--   0        0        0     3893 2024-04-15 14:10:42.994079 vbayesfa-0.0.22/src/vbayesfa/fit_lpa2.py
+-rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.22/src/vbayesfa/ibp/discrete_finite.py
+-rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.22/src/vbayesfa/ibp/fit_ibp.py
+-rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.22/src/vbayesfa/ibp/full_discrete_finite.py
+-rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.22/src/vbayesfa/ibp/make_sim_data.py
+-rw-r--r--   0        0        0    11261 2024-04-04 15:36:07.290321 vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_cont_finite.py
+-rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_pos_cont_finite.py
+-rw-r--r--   0        0        0    10883 2024-04-24 20:20:51.773733 vbayesfa-0.0.22/src/vbayesfa/lpa.py
+-rw-r--r--   0        0        0    20925 2024-04-10 19:09:07.425525 vbayesfa-0.0.22/src/vbayesfa/lpa_outcome_analysis.py
+-rw-r--r--   0        0        0    35869 2024-04-24 20:25:44.549383 vbayesfa-0.0.22/src/vbayesfa/mixture_model.py
+-rw-r--r--   0        0        0    40897 2024-04-09 19:30:59.411472 vbayesfa-0.0.22/src/vbayesfa/old_lpa.py
+-rw-r--r--   0        0        0    10712 2024-04-17 21:13:53.670539 vbayesfa-0.0.22/src/vbayesfa/simulate_data.py
+-rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.22/src/vbayesfa/tests/.DS_Store
+-rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.22/src/vbayesfa/tests/test_exp_families.py
+-rw-r--r--   0        0        0     1633 2024-04-12 14:18:41.718223 vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa.py
+-rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa_outcome_analysis.py
+-rw-r--r--   0        0        0      180 1970-01-01 00:00:00.000000 vbayesfa-0.0.22/PKG-INFO
```

### Comparing `vbayesfa-0.0.21/src/vbayesfa/.DS_Store` & `vbayesfa-0.0.22/src/vbayesfa/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/bayes_factors.py` & `vbayesfa-0.0.22/src/vbayesfa/bayes_factors.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/exp_families.py` & `vbayesfa-0.0.22/src/vbayesfa/exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/finite_lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/finite_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/fit_finite_lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/fit_finite_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/fit_lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/fit_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/fit_lpa2.py` & `vbayesfa-0.0.22/src/vbayesfa/fit_lpa2.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/discrete_finite.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/fit_ibp.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/fit_ibp.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/full_discrete_finite.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/full_discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/make_sim_data.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/make_sim_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/sparse_cont_finite.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/ibp/sparse_pos_cont_finite.py` & `vbayesfa-0.0.22/src/vbayesfa/ibp/sparse_pos_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/lpa.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,16 @@
         # update distribution of stick-breaking lengths (V)
         for t in range(self.T):
             self.gamma1[t] = 1 + np.sum(self.phi[t,:])
             self.gamma2[t] = self.E_alpha + np.sum(self.phi[range(t+1,self.T),:])
             self.E_log_V[t] = digamma(self.gamma1[t]) - digamma(self.gamma1[t] + self.gamma2[t])
             self.E_log_1minusV[t] = digamma(self.gamma2[t]) - digamma(self.gamma1[t] + self.gamma2[t]) 
         for t in range(self.T):
-            self.E_log_pi[t] = self.E_log_V[t] + np.sum(self.E_log_1minusV[range(t-1)])
+            #self.E_log_pi[t] = self.E_log_V[t] + np.sum(self.E_log_1minusV[range(t-1)])
+            self.E_log_pi[t] = self.E_log_V[t] + np.sum(self.E_log_1minusV[range(t-1+1)])
         self.E_V = self.gamma1/(self.gamma1 + self.gamma2)
         product_term = np.concatenate([np.array([1]), np.cumprod(1 - self.E_V)[range(self.T-1)]])
         self.E_pi = self.E_V*product_term
         
     def _update_q_alpha(self):
         # update distribution of the Dirichlet process concentration parameter (alpha)
         self.w2 = self.prior_w2 - np.sum(self.E_log_1minusV[range(self.T - 1)]) # self.w1 stays constant, so we only update self.w2
```

### Comparing `vbayesfa-0.0.21/src/vbayesfa/lpa_outcome_analysis.py` & `vbayesfa-0.0.22/src/vbayesfa/lpa_outcome_analysis.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/mixture_model.py` & `vbayesfa-0.0.22/src/vbayesfa/mixture_model.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/old_lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/old_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/simulate_data.py` & `vbayesfa-0.0.22/src/vbayesfa/simulate_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/tests/.DS_Store` & `vbayesfa-0.0.22/src/vbayesfa/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/tests/test_exp_families.py` & `vbayesfa-0.0.22/src/vbayesfa/tests/test_exp_families.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/tests/test_lpa.py` & `vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.21/src/vbayesfa/tests/test_lpa_outcome_analysis.py` & `vbayesfa-0.0.22/src/vbayesfa/tests/test_lpa_outcome_analysis.py`

 * *Files identical despite different names*

