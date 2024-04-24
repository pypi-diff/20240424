# Comparing `tmp/scenvi-0.3.1.tar.gz` & `tmp/scenvi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenvi-0.3.1.tar", max compression
+gzip compressed data, was "scenvi-0.3.2.tar", max compression
```

## Comparing `scenvi-0.3.1.tar` & `scenvi-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.1/LICENSE
--rw-r--r--   0        0        0     1802 2024-04-18 21:38:09.603472 scenvi-0.3.1/README.md
--rw-r--r--   0        0        0      434 2024-04-24 16:07:31.226023 scenvi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    22496 2024-04-24 16:01:33.330043 scenvi-0.3.1/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py
--rw-r--r--   0        0        0    22496 2024-04-24 16:01:33.330043 scenvi-0.3.1/scenvi/ENVI.py
--rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.3.1/scenvi/__init__.py
--rw-r--r--   0        0        0     1378 2024-04-24 15:39:07.613935 scenvi-0.3.1/scenvi/dists.py
--rw-r--r--   0        0        0     9530 2024-04-24 15:46:29.892026 scenvi-0.3.1/scenvi/utils.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 scenvi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1883 2024-04-24 20:34:08.461781 scenvi-0.3.2/README.md
+-rw-r--r--   0        0        0      434 2024-04-24 20:35:14.119255 scenvi-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    23379 2024-04-24 17:55:46.439378 scenvi-0.3.2/scenvi/ENVI.py
+-rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.3.2/scenvi/__init__.py
+-rw-r--r--   0        0        0     1652 2024-04-24 17:47:36.533143 scenvi-0.3.2/scenvi/_dists.py
+-rw-r--r--   0        0        0     8694 2024-04-24 17:47:36.533445 scenvi-0.3.2/scenvi/utils.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 scenvi-0.3.2/PKG-INFO
```

### Comparing `scenvi-0.3.1/LICENSE` & `scenvi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.1/README.md` & `scenvi-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,7 +41,8 @@
     sc_data.obsm['cell_type_niche'] = envi_model.sc_data.obsm['cell_type_niche']
     
 
 And to just compute COVET for spatial data:
 
     st_data.obsm['COVET'], st_data.obsm['COVET_SQRT'], st_data.uns['CovGenes'] = scenvi.compute_covet(st_data)
         
+Please read our documentation at https://scenvi.readthedocs.io/ for more details!
```

### Comparing `scenvi-0.3.1/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py` & `scenvi-0.3.2/scenvi/ENVI.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 from functools import partial
 import scipy.stats
 import numpy as np
 
 from typing import Callable, Any, Optional
 
 from scenvi.utils import *
-from scenvi.dists import *
+from scenvi._dists import *
 
 import tensorflow_probability.substrates.jax as jax_prob
 
 import scanpy as sc
 import pandas as pd
 from tqdm import trange
 
 
 class ENVI():
     
     """
     Initializes the ENVI model & computes COVET for spatial data
     
     
-    :param spatial_data (anndata): anndata with spatial data, with an obsm indicating spatial location of spot/segmented cell
-    :param sc_data (anndata): anndata with sinlge cell data
-    :param spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
-    :param batch_key (str): obs key name of batch/sample of spatial data (default 'batch' if in spatial_data.obs, else -1)
-    :param num_layers (int): number of neural network for decoders and encoders (default 3)
-    :param num_neurons (int): number of neurons in each layer (default 1024)
-    :param latent_dim (int): size of ENVI latent dimention (size 512)
-    :param k_nearest (int): number of physical neighbours to describe niche (default 8)
-    :param num_cov_genes (int): number of HVGs to compute niche covariance with default (64), if -1 uses all genes
-    :param cov_genes (list of str): manual genes to compute niche with (default [])
-    :param num_HVG (int): number of HVGs to keep for single cell data (default 2048)
-    :param sc_genes (list of str): manual genes to keep for sinlge cell data (default [])
+    :param spatial_data: (anndata) spatial transcriptomics data, with an obsm indicating spatial location of spot/segmented cell
+    :param sc_data: (anndata) complementary sinlge cell data
+    :param spatial_key: (str) obsm key name with physical location of spots/cells (default 'spatial')
+    :param batch_key: (str) obs key name of batch/sample of spatial data (default 'batch' if in spatial_data.obs, else -1)
+    :param num_layers: (int) number of neural network for decoders and encoders (default 3)
+    :param num_neurons: (int) number of neurons in each layer (default 1024)
+    :param latent_dim: (int) size of ENVI latent dimention (size 512)
+    :param k_nearest: (int) number of physical neighbours to describe niche (default 8)
+    :param num_cov_genes: (int) number of HVGs to compute niche covariance with (default ֿ64), if -1 uses all genes
+    :param cov_genes: (list of str) manual genes to compute niche with (default [])
+    :param num_HVG: (int) number of HVGs to keep for single cell data (default 2048)
+    :param sc_genes: (list of str) manual genes to keep for sinlge cell data (default [])
     :param spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb' or 'norm') 
-    :param sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb' or 'norm')
-    :param spatial_coeff (float): coefficient for spatial expression loss in total ELBO (default 1.0)
-    :param sc_coeff (float): coefficient for sinlge cell expression loss in total ELBO (default 1.0)
-    :param cov_coeff (float): coefficient for spatial niche loss in total ELBO (default 1.0)
-    :param kl_coeff (float): coefficient for latent prior loss in total ELBO (default 1.0)
-    :param log_input (float): if larger than zero, a log is applied to ENVI input with pseudocount of log_input (default 0.1)
-    :param stable_eps (float): added value to log probabilty calculations to avoid NaNs during training (default 1e-6)
+    :param sc_dist: (str) distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb' or 'norm')
+    :param spatial_coeff: (float) coefficient for spatial expression loss in total ELBO (default 1.0)
+    :param sc_coeff: (float) coefficient for sinlge cell expression loss in total ELBO (default 1.0)
+    :param cov_coeff: (float) coefficient for spatial niche loss in total ELBO (default 1.0)
+    :param kl_coeff: (float) coefficient for latent prior loss in total ELBO (default 1.0)
+    :param log_input: (float) if larger than zero, a log is applied to ENVI input with pseudocount of log_input (default 0.1)
+    :param stable_eps: (float) added value to log probabilty calculations to avoid NaNs during training (default 1e-6)
     
     :return: initialized ENVI model
     """ 
 
             
     def __init__(self,
                  spatial_data, 
@@ -160,19 +160,29 @@
                          n_output_exp = self.exp_dec_size,
                          n_output_cov = int(self.cov_gene_num * (self.cov_gene_num  + 1)/2))
                              
         
         print("Finished Initializing ENVI")
     
     def inp_log_fn(self, x):
+        
+        """
+        :meta private:
+        """
+            
         if(self.log_input > 0):
             return(jnp.log(x+self.log_input))
         return(x)
 
     def mean_sc(self, sc_inp):
+        
+        """
+        :meta private:
+        """
+        
         sc_inp = sc_inp[:, :self.dist_size_dict[self.sc_dist] * self.sc_data.shape[-1]]
         if(self.sc_dist == 'zinb'):
             sc_r, sc_p, sc_d = jnp.split(sc_inp, 3, axis = -1)
             return(nn.softplus(sc_r) * jnp.exp(sc_p) * (1 - nn.sigmoid(sc_d)))
         if(self.sc_dist == 'nb'):
             sc_r, sc_p = jnp.split(sc_inp, 2, axis = -1)
             return(nn.softplus(sc_r) * jnp.exp(sc_p))
@@ -180,14 +190,19 @@
             sc_l = sc_neurons
             return(sc_l)
         if(self.sc_dist == 'norm'):
             sc_l = sc_neurons
             return(sc_l)
     
     def mean_spatial(self, spatial_inp):
+        
+        """
+        :meta private:
+        """
+        
         if(self.spatial_dist == 'zinb' or self.spatial_dist == 'nb'):
             spatial_inp = jnp.concatenate([spatial_inp[:, :self.spatial_data.shape[-1]],
                                            spatial_inp[:, -(self.dist_size_dict[self.spatial_dist] - 1) * self.spatial_data.shape[-1]:]], axis = -1)
         else:
             spatial_inp = spatial_inp[:, :self.spatial_data.shape[-1]]
             
         if(self.spatial_dist == 'zinb'):
@@ -200,14 +215,19 @@
             spatial_l = spatial_inp
             return(spatial_l)
         if(self.spatial_dist == 'norm'):
             spatial_l = spatial_inp
             return(spatial_l)
         
     def factor_sc(self, sc_inp, dec_exp):
+        
+        """
+        :meta private:
+        """
+        
         sc_neurons = dec_exp[:, :self.dist_size_dict[self.sc_dist] * self.sc_data.shape[-1]]
         
         if(self.sc_dist == 'zinb'):
             sc_r, sc_p, sc_d = jnp.split(sc_neurons, 3, axis = -1)
             sc_like = jnp.mean(log_zinb_pdf(sc_inp, nn.softplus(sc_r)+self.eps, sc_p,  sc_d))
         if(self.sc_dist == 'nb'):
             sc_r, sc_p = jnp.split(sc_neurons, 2, axis = -1)
@@ -217,14 +237,19 @@
             sc_like = jnp.mean(log_pos_pdf(sc_inp, nn.softplus(sc_l)+self.eps))
         if(self.sc_dist == 'norm'):
             sc_l = sc_neurons
             sc_like = jnp.mean(log_normal_pdf(sc_inp, sc_l))
         return(sc_like)
     
     def factor_spatial(self, spatial_inp, dec_exp):
+        
+        """
+        :meta private:
+        """
+        
         if(self.spatial_dist == 'zinb' or self.spatial_dist == 'nb'):
             spatial_neurons = jnp.concatenate([dec_exp[:, :self.spatial_data.shape[-1]],
                                                dec_exp[:, -(self.dist_size_dict[self.spatial_dist] - 1) * self.spatial_data.shape[-1]:]], axis = -1)
         else:
             spatial_neurons = dec_exp[:, :self.spatial_data.shape[-1]]
         
         if(self.spatial_dist == 'zinb'):
@@ -238,19 +263,28 @@
             spatial_like = jnp.mean(log_pos_pdf(spatial_inp, nn.softplus(spatial_l)+self.eps))
         if(self.spatial_dist == 'norm'):
             spatial_l = spatial_neurons
             spatial_like = jnp.mean(log_normal_pdf(spatial_inp, spatial_l))
         return(spatial_like)     
     
     def grammian_cov(self, dec_cov):
+        
+        """
+        :meta private:
+        """
+        
         dec_cov = jax_prob.math.fill_triangular(dec_cov)
         return(jnp.matmul(dec_cov, dec_cov.transpose([0,2,1])))
         
     def create_train_state(self, key = random.key(0), init_lr = 0.0001, decay_steps = 4000):
         
+        """
+        :meta private:
+        """
+        
         key, subkey1, subkey2  = random.split(key, num = 3)
         params = self.model.init(rngs = {'params': subkey1},
                                 x = self.inp_log_fn(self.spatial_data.X[0:1]),
                                 mode = 'spatial',
                                 key = subkey2)['params']
 
         lr_sched = optax.exponential_decay(init_lr, decay_steps, 0.5, staircase = True)
@@ -259,14 +293,18 @@
         return(TrainState.create(
           apply_fn=self.model.apply, params=params, tx=tx,
           metrics=Metrics.empty()))
     
     @partial(jit, static_argnums=(0, ))
     def train_step(self, state, spatial_inp, spatial_COVET, sc_inp, key = random.key(0)):
         
+        """
+        :meta private:
+        """
+        
         key, subkey1, subkey2 = random.split(key, num = 3)
         
         def loss_fn(params):
             spatial_enc_mu, spatial_enc_logstd, spatial_dec_exp, spatial_dec_cov = state.apply_fn({'params':params}, 
                                                                                                   x = self.inp_log_fn(spatial_inp), 
                                                                                                   mode = 'spatial', 
                                                                                                   key = subkey1)
@@ -292,20 +330,20 @@
     
     def train(self, training_steps = 16000, batch_size = 128, verbose = 16, init_lr = 0.0001, decay_steps = 4000, key = random.key(0)):
   
         """
         Set up optimization parameters and train the ENVI moodel
 
 
-        :param training_steps (int): number of gradient descent steps to train ENVI (default 16000)
-        :param batch_size (int): size of spatial and single-cell profiles sampled for each training step  (default 128)
-        :param verbose (int): amount of steps between each loss print statement (default 16)
-        :param init_lr (float): initial learning rate for ADAM optimizer with exponential decay (default 1e-4)
-        :param decay_steps (int): number of steps before each learning rate decay (default 4000)
-        :param key (jax.random.key): random seed (default jax.random.key(0))
+        :param training_steps: (int) number of gradient descent steps to train ENVI (default 16000)
+        :param batch_size: (int) size of spatial and single-cell profiles sampled for each training step  (default 128)
+        :param verbose: (int) amount of steps between each loss print statement (default 16)
+        :param init_lr: (float) initial learning rate for ADAM optimizer with exponential decay (default 1e-4)
+        :param decay_steps: (int) number of steps before each learning rate decay (default 4000)
+        :param key: (jax.random.key) random seed (default jax.random.key(0))
 
         :return: nothing
         """ 
         
         batch_size = min(self.sc_data.shape[0], min(self.spatial_data.shape[0], batch_size))
 
         key, subkey = random.split(key)
@@ -345,26 +383,44 @@
                 tq.set_description(print_statement)
                 tq.refresh() # to show 
 
         self.latent_rep()
         
     @partial(jit, static_argnums=(0, ))
     def model_encoder(self, x):
+        
+        """
+        :meta private:
+        """
+        
         return(self.model.bind({'params': self.params}).encoder(x))
     
     @partial(jit, static_argnums=(0, ))
     def model_decoder_exp(self, x):
+        
+        """
+        :meta private:
+        """
+            
         return(self.model.bind({'params': self.params}).decoder_exp(x))
     
     @partial(jit, static_argnums=(0, ))
     def model_decoder_cov(self, x):
+        
+        """
+        :meta private:
+        """
         return(self.model.bind({'params': self.params}).decoder_cov(x))
     
     def encode(self, x, mode = 'spatial', max_batch = 256):
         
+        """
+        :meta private:
+        """
+            
         conf_const = 0 if mode == 'spatial' else 1 
         conf_neurons = jax.nn.one_hot(conf_const * jnp.ones(x.shape[0], dtype=jnp.int8), 2, dtype=jnp.float32)
         
         x_conf = jnp.concatenate([self.inp_log_fn(x), conf_neurons], axis = -1)
         
         
         if(x_conf.shape[0] < max_batch):
@@ -374,14 +430,18 @@
             x_conf_split = np.array_split(x_conf, num_split)
             enc = np.concatenate([jnp.split(self.model_encoder(x_conf_split[split_ind]), 2, axis = -1)[0] for
                                   split_ind in range(num_split)], axis = 0)
         return enc
     
     def decode_exp(self, x, mode = 'spatial', max_batch = 256):
         
+        """
+        :meta private:
+        """
+            
         conf_const = 0 if mode == 'spatial' else 1 
         conf_neurons = jax.nn.one_hot(conf_const * jnp.ones(x.shape[0], dtype=jnp.int8), 2, dtype=jnp.float32)
         
         x_conf = jnp.concatenate([x, conf_neurons], axis = -1)
         
         if(mode == 'spatial'):
             if(x_conf.shape[0] < max_batch):
@@ -399,14 +459,18 @@
                 x_conf_split = np.array_split(x_conf, num_split)
                 dec = np.concatenate([self.mean_sc(self.model_decoder_exp(x_conf_split[split_ind])) for
                                       split_ind in range(num_split)], axis = 0)
         return dec
     
     def decode_cov(self, x, max_batch = 256):
         
+        """
+        :meta private:
+        """
+            
         conf_const = 0
         conf_neurons = jax.nn.one_hot(conf_const * jnp.ones(x.shape[0], dtype=jnp.int8), 2, dtype=jnp.float32)
         
         x_conf = jnp.concatenate([x, conf_neurons], axis = -1)
         
         if(x_conf.shape[0] < max_batch):
             dec = self.grammian_cov(self.model_decoder_cov(x_conf))
@@ -414,51 +478,51 @@
             num_split = int(x_conf.shape[0]/max_batch)+1
             x_conf_split = np.array_split(x_conf, num_split)
             dec = np.concatenate([self.grammian_cov(self.model_decoder_cov(x_conf_split[split_ind])) for
                                   split_ind in range(num_split)], axis = 0)
         return(dec)
         
     def latent_rep(self): 
+        
         """
         Compute latent embeddings for spatial and single cell data, automatically performed after training
         
         :return: nothing, adds 'envi_latent' self.spatial_data.obsm and self.spatial_data.obsm
         """ 
     
         self.spatial_data.obsm['envi_latent'] = self.encode(self.spatial_data.X, mode = 'spatial')
         self.sc_data.obsm['envi_latent'] = self.encode(self.sc_data[:, self.spatial_data.var_names].X, mode = 'sc')
         
-
-    
     def impute_genes(self):
+        
         """
         Impute full transcriptome for spatial data
     
         :return: nothing adds 'imputation' to self.spatial_data.obsm
         """
-            
     
         self.spatial_data.obsm['imputation'] = pd.DataFrame(self.decode_exp(self.spatial_data.obsm['envi_latent'],  mode = 'sc'), 
                                                             columns = self.sc_data.var_names, 
                                                             index = self.spatial_data.obs_names)
         
         print("Finished imputing missing gene for spatial data! See 'imputation' in obsm of ENVI.spatial_data")
      
     def infer_niche_covet(self):
-        
+
         """
         Predict COVET representation for single-cell data
     
         :return: nothing adds 'COVET_SQRT' and 'COVET' to self.spatial_data.obsm
         """
 
         self.sc_data.obsm['COVET_SQRT'] = self.decode_cov(self.sc_data.obsm['envi_latent'])
         self.sc_data.obsm['COVET'] = np.matmul(self.sc_data.obsm['COVET_SQRT'], self.sc_data.obsm['COVET_SQRT'])
     
     def infer_niche_celltype(self, cell_type_key = 'cell_type'):
+        
         """
         Predict cell type abundence based one ENVI-inferred COVET representations 
         
         :param cell_type_key (string): key in spatial_data.obs where cell types are stored for environment composition (default 'cell_type')
         
         :return: nothing, adds 'niche_cell_type' to self.sc_data.obsm & self.spatial_data.obsm
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scenvi-0.3.1/scenvi/dists.py` & `scenvi-0.3.2/scenvi/_dists.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,32 +16,62 @@
 from typing import Callable, Any, Optional
 
 import tensorflow_probability.substrates.jax.distributions as jnd
 
 import scanpy as sc
 
 def KL(mean, log_std):
+    
+    """
+    :meta private:
+    """
+        
     KL = 0.5 * (jnp.square(mean) + jnp.square(jnp.exp(log_std)) - 2 * log_std)
     return(jnp.mean(KL, axis = -1))
     
 def log_pos_pdf(sample, l):
+    
+    """
+    :meta private:
+    """
+    
     log_prob = jnd.Poisson(rate=l).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
 
 def log_nb_pdf(sample, r, p):
+    
+    """
+    :meta private:
+    """
+    
     log_prob = jnd.NegativeBinomial(total_count=r, logits=p).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
 
 def log_zinb_pdf(sample, r, p, d):
+    
+    """
+    :meta private:
+    """
+    
     log_prob = jnd.Inflated(jnd.NegativeBinomial(total_count = r, logits = p), inflated_loc_logits = d).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
     
 def log_normal_pdf(sample, mean):
+    
+    """
+    :meta private:
+    """
+    
     log_prob = jnd.Normal(loc = mean, scale = 1).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
 
 def AOT_Distance(sample, mean):
+    
+    """
+    :meta private:
+    """
+    
     sample = jnp.reshape(sample, [sample.shape[0], -1])
     mean = jnp.reshape(mean, [mean.shape[0], -1])
     log_prob = - jnp.square(sample - mean)
     return(jnp.mean(log_prob, axis = -1))
```

### Comparing `scenvi-0.3.1/PKG-INFO` & `scenvi-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenvi
-Version: 0.3.1
+Version: 0.3.2
 Summary: Integration of scRNA-seq and spatial transcriptomics data
 License: MIT
 Author: Doron Haviv
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -62,8 +62,8 @@
     sc_data.obsm['cell_type_niche'] = envi_model.sc_data.obsm['cell_type_niche']
     
 
 And to just compute COVET for spatial data:
 
     st_data.obsm['COVET'], st_data.obsm['COVET_SQRT'], st_data.uns['CovGenes'] = scenvi.compute_covet(st_data)
         
-
+Please read our documentation at https://scenvi.readthedocs.io/ for more details!
```

