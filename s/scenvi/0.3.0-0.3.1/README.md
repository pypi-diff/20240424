# Comparing `tmp/scenvi-0.3.0.tar.gz` & `tmp/scenvi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenvi-0.3.0.tar", max compression
+gzip compressed data, was "scenvi-0.3.1.tar", max compression
```

## Comparing `scenvi-0.3.0.tar` & `scenvi-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.0/LICENSE
--rw-r--r--   0        0        0     1802 2024-04-18 21:38:09.603472 scenvi-0.3.0/README.md
--rw-r--r--   0        0        0      434 2024-04-18 21:41:34.069243 scenvi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    22052 2024-04-18 21:38:09.604781 scenvi-0.3.0/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py
--rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.3.0/scenvi/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.336812 scenvi-0.3.0/scenvi/.ipynb_checkpoints/dists-checkpoint.py
--rw-r--r--   0        0        0     9226 2024-04-18 21:38:09.605263 scenvi-0.3.0/scenvi/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0    22052 2024-04-18 21:38:09.605703 scenvi-0.3.0/scenvi/ENVI.py
--rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.3.0/scenvi/__init__.py
--rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.360992 scenvi-0.3.0/scenvi/dists.py
--rw-r--r--   0        0        0     9226 2024-04-18 21:38:09.606695 scenvi-0.3.0/scenvi/utils.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 scenvi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1802 2024-04-18 21:38:09.603472 scenvi-0.3.1/README.md
+-rw-r--r--   0        0        0      434 2024-04-24 16:07:31.226023 scenvi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    22496 2024-04-24 16:01:33.330043 scenvi-0.3.1/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py
+-rw-r--r--   0        0        0    22496 2024-04-24 16:01:33.330043 scenvi-0.3.1/scenvi/ENVI.py
+-rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.3.1/scenvi/__init__.py
+-rw-r--r--   0        0        0     1378 2024-04-24 15:39:07.613935 scenvi-0.3.1/scenvi/dists.py
+-rw-r--r--   0        0        0     9530 2024-04-24 15:46:29.892026 scenvi-0.3.1/scenvi/utils.py
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 scenvi-0.3.1/PKG-INFO
```

### Comparing `scenvi-0.3.0/LICENSE` & `scenvi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.0/README.md` & `scenvi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.0/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py` & `scenvi-0.3.1/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,40 +25,39 @@
 import pandas as pd
 from tqdm import trange
 
 
 class ENVI():
     
     """
-    ENVI Integrates spatial and single-cell data
+    Initializes the ENVI model & computes COVET for spatial data
     
-    Parameters: 
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        sc_data (anndata): anndata with sinlge cell data
-        spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
-        batch_key (str): obs key name of batch/sample of spatial data (default -1)
-        num_layers (int): number of neural network for decoders and encoders (default 3)
-        num_neurons (int): number of neurons in each layer (default 1024)
-        latent_dim (int): size of ENVI latent dimention (size 512)
-        k_nearest (int): number of physical neighbours to describe niche (default 8)
-        num_cov_genes (int): number of HVGs to compute niche covariance with default (64), if -1 takes all genes
-        cov_genes (list of str): manual genes to compute niche with (default [])
-        num_HVG (int): number of HVGs to keep for single cell data (default 2048)
-        sc_genes (list of str): manual genes to keep for sinlge cell data (default [])
-        spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm') 
-        sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm')
-        cov_dist (str): distribution used to describe niche covariance from spatial data (default OT, could be 'OT', 'wish' or 'norm')
-        prior_dist (str): prior distribution for latent (default normal)
-        comm_disp (bool): if True, spatial_dist and sc_dist share dispersion parameter(s) (default False)
-        const_disp (bool): if True, dispertion parameter(s) are only per gene, rather there per gene per sample (default False)
-        spatial_coeff (float): coefficient for spatial expression loss in total ELBO (default 1.0)
-        sc_coeff (float): coefficient for sinlge cell expression loss in total ELBO (default 1.0)
-        cov_coeff (float): coefficient for spatial niche loss in total ELBO (default 1.0)
-        kl_coeff (float): coefficient for latent prior loss in total ELBO (default 1.0)
-        log_input (float): if larger than zero, a log is applied to input with pseudocount of log_input (default 0.0)
+    
+    :param spatial_data (anndata): anndata with spatial data, with an obsm indicating spatial location of spot/segmented cell
+    :param sc_data (anndata): anndata with sinlge cell data
+    :param spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
+    :param batch_key (str): obs key name of batch/sample of spatial data (default 'batch' if in spatial_data.obs, else -1)
+    :param num_layers (int): number of neural network for decoders and encoders (default 3)
+    :param num_neurons (int): number of neurons in each layer (default 1024)
+    :param latent_dim (int): size of ENVI latent dimention (size 512)
+    :param k_nearest (int): number of physical neighbours to describe niche (default 8)
+    :param num_cov_genes (int): number of HVGs to compute niche covariance with default (64), if -1 uses all genes
+    :param cov_genes (list of str): manual genes to compute niche with (default [])
+    :param num_HVG (int): number of HVGs to keep for single cell data (default 2048)
+    :param sc_genes (list of str): manual genes to keep for sinlge cell data (default [])
+    :param spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb' or 'norm') 
+    :param sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb' or 'norm')
+    :param spatial_coeff (float): coefficient for spatial expression loss in total ELBO (default 1.0)
+    :param sc_coeff (float): coefficient for sinlge cell expression loss in total ELBO (default 1.0)
+    :param cov_coeff (float): coefficient for spatial niche loss in total ELBO (default 1.0)
+    :param kl_coeff (float): coefficient for latent prior loss in total ELBO (default 1.0)
+    :param log_input (float): if larger than zero, a log is applied to ENVI input with pseudocount of log_input (default 0.1)
+    :param stable_eps (float): added value to log probabilty calculations to avoid NaNs during training (default 1e-6)
+    
+    :return: initialized ENVI model
     """ 
 
             
     def __init__(self,
                  spatial_data, 
                  sc_data, 
                  spatial_key = 'spatial',
@@ -69,23 +68,20 @@
                  k_nearest = 8,
                  num_cov_genes = 64,
                  cov_genes = [],
                  num_HVG = 2048,
                  sc_genes = [],
                  spatial_dist = 'pois',
                  sc_dist = 'nb',
-                 comm_disp = False,
-                 const_disp = False,
                  spatial_coeff = 1,
                  sc_coeff = 1,
                  cov_coeff = 1,
                  kl_coeff = 0.3, 
                  log_input = 0.1,
-                 stable_eps = 1e-6,
-                 **kwargs):
+                 stable_eps = 1e-6):
         
 
         
         
         self.spatial_data = spatial_data
         self.sc_data = sc_data
         
@@ -152,15 +148,15 @@
         else:
             self.log_input = log_input
 
         
         self.eps = stable_eps
         
         
-        print("Initializing VAE")
+        print("Initializing CVAE")
         
         self.model = CVAE(n_layers = self.num_layers,
                          n_neurons = self.num_neurons,
                          n_latent = self.latent_dim,
                          n_output_exp = self.exp_dec_size,
                          n_output_cov = int(self.cov_gene_num * (self.cov_gene_num  + 1)/2))
                              
@@ -262,15 +258,14 @@
         
         return(TrainState.create(
           apply_fn=self.model.apply, params=params, tx=tx,
           metrics=Metrics.empty()))
     
     @partial(jit, static_argnums=(0, ))
     def train_step(self, state, spatial_inp, spatial_COVET, sc_inp, key = random.key(0)):
-        """Train for a single step."""
         
         key, subkey1, subkey2 = random.split(key, num = 3)
         
         def loss_fn(params):
             spatial_enc_mu, spatial_enc_logstd, spatial_dec_exp, spatial_dec_cov = state.apply_fn({'params':params}, 
                                                                                                   x = self.inp_log_fn(spatial_inp), 
                                                                                                   mode = 'spatial', 
@@ -291,54 +286,69 @@
         
         grad_fn = jax.value_and_grad(loss_fn, has_aux = True)
         loss, grads = grad_fn(state.params)
         state = state.apply_gradients(grads=grads)
         return(state, loss)
     
     
-    def train(self, epochs = 16000, batch_size = 128, verbose = 16, init_lr = 0.0001, decay_steps = 4000, key = random.key(0)):
-        batch_size = min(self.sc_data.shape[0], min(self.spatial_data.shape[0], batch_size))
+    def train(self, training_steps = 16000, batch_size = 128, verbose = 16, init_lr = 0.0001, decay_steps = 4000, key = random.key(0)):
+  
+        """
+        Set up optimization parameters and train the ENVI moodel
+
+
+        :param training_steps (int): number of gradient descent steps to train ENVI (default 16000)
+        :param batch_size (int): size of spatial and single-cell profiles sampled for each training step  (default 128)
+        :param verbose (int): amount of steps between each loss print statement (default 16)
+        :param init_lr (float): initial learning rate for ADAM optimizer with exponential decay (default 1e-4)
+        :param decay_steps (int): number of steps before each learning rate decay (default 4000)
+        :param key (jax.random.key): random seed (default jax.random.key(0))
+
+        :return: nothing
+        """ 
         
+        batch_size = min(self.sc_data.shape[0], min(self.spatial_data.shape[0], batch_size))
+
         key, subkey = random.split(key)
         state = self.create_train_state(subkey, init_lr = init_lr, decay_steps = decay_steps) 
         self.params = state.params
-        
-        tq = trange(epochs, leave=True, desc = "")
+
+        tq = trange(training_steps, leave=True, desc = "")
         sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = 0, 0, 0, 0, 0
-        
+
         sc_X = self.sc_data.X
         spatial_X =  self.spatial_data.X
         spatial_COVET =  self.spatial_data.obsm['COVET_SQRT']
-        
-        for epoch in tq:
+
+        for training_step in tq:
             key, subkey1, subkey2 = random.split(key, num = 3)
-            
+
             batch_spatial_ind = random.choice(key = subkey1, a = self.spatial_data.shape[0], shape = [batch_size], replace = False)
             batch_sc_ind = random.choice(key = subkey2, a = self.sc_data.shape[0], shape = [batch_size], replace = False)
-            
+
             batch_spatial_exp, batch_spatial_cov = spatial_X[batch_spatial_ind],  spatial_COVET[batch_spatial_ind]
             batch_sc_exp = sc_X[batch_sc_ind]
-            
+
             key, subkey = random.split(key)
-            
+
             state, loss = self.train_step(state, batch_spatial_exp, batch_spatial_cov, batch_sc_exp, key = subkey)
-            
+
             self.params = state.params
 
             sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = sc_loss_mean + loss[1][0], spatial_loss_mean + loss[1][1], cov_loss_mean + loss[1][2], kl_loss_mean + loss[1][3], count + 1
 
-            if(epoch%verbose==0):
+            if(training_step%verbose==0):
                 print_statement = ''
                 for metric,value in zip(['spatial', 'sc', 'cov', 'kl'], [spatial_loss_mean, sc_loss_mean, cov_loss_mean, kl_loss_mean]):
                     print_statement = print_statement + ' ' + metric + ': {:.3e}'.format(value/count)
 
                 sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = 0, 0, 0, 0, 0
                 tq.set_description(print_statement)
                 tq.refresh() # to show 
-                
+
         self.latent_rep()
         
     @partial(jit, static_argnums=(0, ))
     def model_encoder(self, x):
         return(self.model.bind({'params': self.params}).encoder(x))
     
     @partial(jit, static_argnums=(0, ))
@@ -405,56 +415,56 @@
             x_conf_split = np.array_split(x_conf, num_split)
             dec = np.concatenate([self.grammian_cov(self.model_decoder_cov(x_conf_split[split_ind])) for
                                   split_ind in range(num_split)], axis = 0)
         return(dec)
         
     def latent_rep(self): 
         """
-        Compute latent embeddings for spatial and single cell data
+        Compute latent embeddings for spatial and single cell data, automatically performed after training
         
-        Return:
-            no return, adds 'envi_latent' ENVI.spatial_data.obsm and ENVI.spatial_data.obsm
-        """
+        :return: nothing, adds 'envi_latent' self.spatial_data.obsm and self.spatial_data.obsm
+        """ 
     
         self.spatial_data.obsm['envi_latent'] = self.encode(self.spatial_data.X, mode = 'spatial')
         self.sc_data.obsm['envi_latent'] = self.encode(self.sc_data[:, self.spatial_data.var_names].X, mode = 'sc')
         
 
     
     def impute_genes(self):
         """
-        Imput full transcriptome for spatial data
+        Impute full transcriptome for spatial data
     
-        Return:
-            no return, adds 'imputation' to ENVI.spatial_data.obsm
+        :return: nothing adds 'imputation' to self.spatial_data.obsm
         """
             
     
         self.spatial_data.obsm['imputation'] = pd.DataFrame(self.decode_exp(self.spatial_data.obsm['envi_latent'],  mode = 'sc'), 
                                                             columns = self.sc_data.var_names, 
                                                             index = self.spatial_data.obs_names)
         
         print("Finished imputing missing gene for spatial data! See 'imputation' in obsm of ENVI.spatial_data")
      
     def infer_niche_covet(self):
-        """
-        Infer covariance niche composition for single cell data
         
-        Return:
-            no return, adds 'COVET_SQRT' and 'COVET' to ENVI.sc_data.obsm
         """
+        Predict COVET representation for single-cell data
+    
+        :return: nothing adds 'COVET_SQRT' and 'COVET' to self.spatial_data.obsm
+        """
+
         self.sc_data.obsm['COVET_SQRT'] = self.decode_cov(self.sc_data.obsm['envi_latent'])
         self.sc_data.obsm['COVET'] = np.matmul(self.sc_data.obsm['COVET_SQRT'], self.sc_data.obsm['COVET_SQRT'])
     
     def infer_niche_celltype(self, cell_type_key = 'cell_type'):
         """
         Predict cell type abundence based one ENVI-inferred COVET representations 
         
-        Return:
-            no return, adds 'niche_cell_type' to ENVI.sc_data.obsm & ENVI.spatial_data.obsm
+        :param cell_type_key (string): key in spatial_data.obs where cell types are stored for environment composition (default 'cell_type')
+        
+        :return: nothing, adds 'niche_cell_type' to self.sc_data.obsm & self.spatial_data.obsm
         """
          
         self.spatial_data.obsm['cell_type_niche'] = niche_cell_type(self.spatial_data, self.k_nearest, spatial_key = self.spatial_key, cell_type_key = cell_type_key, batch_key = self.batch_key)
         
         regression_model = sklearn.neighbors.KNeighborsRegressor(n_neighbors=5).fit(self.spatial_data.obsm['COVET_SQRT'].reshape([self.spatial_data.shape[0], -1]), 
                                                                                     self.spatial_data.obsm['cell_type_niche'])
```

### Comparing `scenvi-0.3.0/scenvi/.ipynb_checkpoints/dists-checkpoint.py` & `scenvi-0.3.1/scenvi/dists.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,13 @@
     log_prob = jnd.Inflated(jnd.NegativeBinomial(total_count = r, logits = p), inflated_loc_logits = d).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
     
 def log_normal_pdf(sample, mean):
     log_prob = jnd.Normal(loc = mean, scale = 1).log_prob(sample)
     return(jnp.mean(log_prob, axis = -1))
 
-
 def AOT_Distance(sample, mean):
     sample = jnp.reshape(sample, [sample.shape[0], -1])
     mean = jnp.reshape(mean, [mean.shape[0], -1])
     log_prob = - jnp.square(sample - mean)
     return(jnp.mean(log_prob, axis = -1))
```

### Comparing `scenvi-0.3.0/scenvi/.ipynb_checkpoints/utils-checkpoint.py` & `scenvi-0.3.1/scenvi/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from typing import Callable, Any, Optional
 import scanpy as sc
 
 import sklearn.neighbors
 
 class FeedForward(nn.Module):
-    """Transformer MLP / feed-forward block.
+    """MLP / feed-forward block.
 
     Attributes:
     config: TransformerConfig dataclass containing hyperparameters.
     out_dim: optionally specify out dimension.
     """
 
     n_layers: int
@@ -196,60 +196,63 @@
         
     DistanceMatWeighted = (ExpData.mean(axis = 0)[None, None, :] - ExpData[kNNGraphIndex[np.arange(ExpData.shape[0])]])
 
     CovMats = np.matmul(DistanceMatWeighted.transpose([0,2,1]), DistanceMatWeighted) / (kNN - 1)
     CovMats = CovMats + CovMats.mean() * 0.00001 * np.expand_dims(np.identity(CovMats.shape[-1]), axis=0) 
     return(CovMats)
 
+
+def niche_cell_type(spatial_data, kNN, spatial_key = 'spatial', cell_type_key = 'cell_type', batch_key = -1):
+    from sklearn.preprocessing import OneHotEncoder
+    
+    if(batch_key == -1):        
+        kNNGraph = sklearn.neighbors.kneighbors_graph(spatial_data.obsm[spatial_key], n_neighbors=kNN, mode='connectivity', n_jobs=-1).tocoo()
+        knn_index = np.reshape(np.asarray(kNNGraph.col), [spatial_data.obsm[spatial_key].shape[0], kNN])
+    else:
+        knn_index = BatchKNN(spatial_data.obsm[spatial_key], spatial_data.obs[batch_key], kNN)
+    
+    one_hot_enc = OneHotEncoder().fit(np.asarray(list(set(spatial_data.obs[cell_type_key]))).reshape([-1,1]))
+    cell_type_one_hot = one_hot_enc.transform(np.asarray(spatial_data.obs[cell_type_key]).reshape([-1,1])).reshape([spatial_data.obs['cell_type'].shape[0], -1]).todense()
+    
+    cell_type_niche = pd.DataFrame(cell_type_one_hot[knn_index].sum(axis = 1), index = spatial_data.obs_names, columns = list(one_hot_enc.categories_[0]))
+    return(cell_type_niche)
+
 def compute_covet(spatial_data, k = 8, g = 64, genes = [], spatial_key = 'spatial', batch_key = -1):
     
     """
-    Compte niche covariance matrices for spatial data
-
-    Args:
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        k (int): number of nearest neighbours to define niche
-        g (int): number of HVG to compute niche covariance matricies
-        genes (list of str): list of genes to keep for niche covariance
+    Compute niche covariance matrices for spatial data, run with scenvi.compute_covet
+        
+    :param spatial_data (anndata): anndata with spatial data, with an obsm indicating spatial location of spot/segmented cell
+    :param k (int): number of nearest neighbours to define niche (default 8)
+    :param g (int): number of HVG to compute COVET representation on (default 64)
+    :param genes (list of str): list of genes to keep for niche covariance (default []
+    :param spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
+    :param batch_key (str): obs key name of batch/sample of spatial data (default 'batch' if in spatial_data.obs, else -1)
+    
+    :return COVET: niche covariance matrices
+    :return COVET_SQRT: matrix square-root of niche covariance matrices for approximate OT
+    :return CovGenes: list of genes selected for COVET representation
+    """ 
 
-    Return:
-        CovMats: raw, untransformed niche covariance matrices
-        CovMatsTransformed: covariance matrices transformed into chosen cov_dist
-        NeighExp: Average geene expression in niche 
-        CovGenes: Genes used for niche covariance 
-    """
         
         
-
+    
     if(g == -1):
         CovGenes = spatial_data.var_names
     else:
         if 'highly_variable' not in spatial_data.var.columns:
             spatial_data.layers['log'] = np.log(spatial_data.X+1)
             sc.pp.highly_variable_genes(spatial_data, n_top_genes = g, layer = 'log')
         
         
         CovGenes = np.asarray(spatial_data.var_names[spatial_data.var.highly_variable])
         if(len(genes) > 0):
             CovGenes = np.union1d(CovGenes, genes)
     
-    CovMats = CalcCovMats(spatial_data, k, genes = CovGenes, spatial_key = spatial_key, batch_key = batch_key)
-    CovMatsTransformed = MatSqrt(CovMats)
-
-    
-    return(CovMats.astype('float32'), CovMatsTransformed.astype('float32'), np.asarray(CovGenes).astype('str'))
-
+    if batch_key not in spatial_data.obs.columns:
+        batch_key = -1
+            
+    COVET = CalcCovMats(spatial_data, k, genes = CovGenes, spatial_key = spatial_key, batch_key = batch_key)
+    COVET_SQRT = MatSqrt(COVET)
 
-def niche_cell_type(spatial_data, kNN, spatial_key = 'spatial', cell_type_key = 'cell_type', batch_key = -1):
-    from sklearn.preprocessing import OneHotEncoder
     
-    if(batch_key == -1):        
-        kNNGraph = sklearn.neighbors.kneighbors_graph(spatial_data.obsm[spatial_key], n_neighbors=kNN, mode='connectivity', n_jobs=-1).tocoo()
-        knn_index = np.reshape(np.asarray(kNNGraph.col), [spatial_data.obsm[spatial_key].shape[0], kNN])
-    else:
-        knn_index = BatchKNN(spatial_data.obsm[spatial_key], spatial_data.obs[batch_key], kNN)
-    
-    one_hot_enc = OneHotEncoder().fit(np.asarray(list(set(spatial_data.obs[cell_type_key]))).reshape([-1,1]))
-    cell_type_one_hot = one_hot_enc.transform(np.asarray(spatial_data.obs[cell_type_key]).reshape([-1,1])).reshape([spatial_data.obs['cell_type'].shape[0], -1]).todense()
-    
-    cell_type_niche = pd.DataFrame(cell_type_one_hot[knn_index].sum(axis = 1), index = spatial_data.obs_names, columns = list(one_hot_enc.categories_[0]))
-    return(cell_type_niche)
+    return(COVET.astype('float32'), COVET_SQRT.astype('float32'), np.asarray(CovGenes).astype('str'))
```

### Comparing `scenvi-0.3.0/scenvi/ENVI.py` & `scenvi-0.3.1/scenvi/ENVI.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,40 +25,39 @@
 import pandas as pd
 from tqdm import trange
 
 
 class ENVI():
     
     """
-    ENVI Integrates spatial and single-cell data
+    Initializes the ENVI model & computes COVET for spatial data
     
-    Parameters: 
-        spatial_data (anndata): anndata with spatial data, with obsm 'spatial' indicating spatial location of spot/segmented cell
-        sc_data (anndata): anndata with sinlge cell data
-        spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
-        batch_key (str): obs key name of batch/sample of spatial data (default -1)
-        num_layers (int): number of neural network for decoders and encoders (default 3)
-        num_neurons (int): number of neurons in each layer (default 1024)
-        latent_dim (int): size of ENVI latent dimention (size 512)
-        k_nearest (int): number of physical neighbours to describe niche (default 8)
-        num_cov_genes (int): number of HVGs to compute niche covariance with default (64), if -1 takes all genes
-        cov_genes (list of str): manual genes to compute niche with (default [])
-        num_HVG (int): number of HVGs to keep for single cell data (default 2048)
-        sc_genes (list of str): manual genes to keep for sinlge cell data (default [])
-        spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm') 
-        sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb', 'norm' or 'full_norm')
-        cov_dist (str): distribution used to describe niche covariance from spatial data (default OT, could be 'OT', 'wish' or 'norm')
-        prior_dist (str): prior distribution for latent (default normal)
-        comm_disp (bool): if True, spatial_dist and sc_dist share dispersion parameter(s) (default False)
-        const_disp (bool): if True, dispertion parameter(s) are only per gene, rather there per gene per sample (default False)
-        spatial_coeff (float): coefficient for spatial expression loss in total ELBO (default 1.0)
-        sc_coeff (float): coefficient for sinlge cell expression loss in total ELBO (default 1.0)
-        cov_coeff (float): coefficient for spatial niche loss in total ELBO (default 1.0)
-        kl_coeff (float): coefficient for latent prior loss in total ELBO (default 1.0)
-        log_input (float): if larger than zero, a log is applied to input with pseudocount of log_input (default 0.0)
+    
+    :param spatial_data (anndata): anndata with spatial data, with an obsm indicating spatial location of spot/segmented cell
+    :param sc_data (anndata): anndata with sinlge cell data
+    :param spatial_key (str): obsm key name with physical location of spots/cells (default 'spatial')
+    :param batch_key (str): obs key name of batch/sample of spatial data (default 'batch' if in spatial_data.obs, else -1)
+    :param num_layers (int): number of neural network for decoders and encoders (default 3)
+    :param num_neurons (int): number of neurons in each layer (default 1024)
+    :param latent_dim (int): size of ENVI latent dimention (size 512)
+    :param k_nearest (int): number of physical neighbours to describe niche (default 8)
+    :param num_cov_genes (int): number of HVGs to compute niche covariance with default (64), if -1 uses all genes
+    :param cov_genes (list of str): manual genes to compute niche with (default [])
+    :param num_HVG (int): number of HVGs to keep for single cell data (default 2048)
+    :param sc_genes (list of str): manual genes to keep for sinlge cell data (default [])
+    :param spatial_dist (str): distribution used to describe spatial data (default pois, could be 'pois', 'nb', 'zinb' or 'norm') 
+    :param sc_dist (str): distribution used to describe sinlge cell data (default nb, could be 'pois', 'nb', 'zinb' or 'norm')
+    :param spatial_coeff (float): coefficient for spatial expression loss in total ELBO (default 1.0)
+    :param sc_coeff (float): coefficient for sinlge cell expression loss in total ELBO (default 1.0)
+    :param cov_coeff (float): coefficient for spatial niche loss in total ELBO (default 1.0)
+    :param kl_coeff (float): coefficient for latent prior loss in total ELBO (default 1.0)
+    :param log_input (float): if larger than zero, a log is applied to ENVI input with pseudocount of log_input (default 0.1)
+    :param stable_eps (float): added value to log probabilty calculations to avoid NaNs during training (default 1e-6)
+    
+    :return: initialized ENVI model
     """ 
 
             
     def __init__(self,
                  spatial_data, 
                  sc_data, 
                  spatial_key = 'spatial',
@@ -69,23 +68,20 @@
                  k_nearest = 8,
                  num_cov_genes = 64,
                  cov_genes = [],
                  num_HVG = 2048,
                  sc_genes = [],
                  spatial_dist = 'pois',
                  sc_dist = 'nb',
-                 comm_disp = False,
-                 const_disp = False,
                  spatial_coeff = 1,
                  sc_coeff = 1,
                  cov_coeff = 1,
                  kl_coeff = 0.3, 
                  log_input = 0.1,
-                 stable_eps = 1e-6,
-                 **kwargs):
+                 stable_eps = 1e-6):
         
 
         
         
         self.spatial_data = spatial_data
         self.sc_data = sc_data
         
@@ -152,15 +148,15 @@
         else:
             self.log_input = log_input
 
         
         self.eps = stable_eps
         
         
-        print("Initializing VAE")
+        print("Initializing CVAE")
         
         self.model = CVAE(n_layers = self.num_layers,
                          n_neurons = self.num_neurons,
                          n_latent = self.latent_dim,
                          n_output_exp = self.exp_dec_size,
                          n_output_cov = int(self.cov_gene_num * (self.cov_gene_num  + 1)/2))
                              
@@ -262,15 +258,14 @@
         
         return(TrainState.create(
           apply_fn=self.model.apply, params=params, tx=tx,
           metrics=Metrics.empty()))
     
     @partial(jit, static_argnums=(0, ))
     def train_step(self, state, spatial_inp, spatial_COVET, sc_inp, key = random.key(0)):
-        """Train for a single step."""
         
         key, subkey1, subkey2 = random.split(key, num = 3)
         
         def loss_fn(params):
             spatial_enc_mu, spatial_enc_logstd, spatial_dec_exp, spatial_dec_cov = state.apply_fn({'params':params}, 
                                                                                                   x = self.inp_log_fn(spatial_inp), 
                                                                                                   mode = 'spatial', 
@@ -291,54 +286,69 @@
         
         grad_fn = jax.value_and_grad(loss_fn, has_aux = True)
         loss, grads = grad_fn(state.params)
         state = state.apply_gradients(grads=grads)
         return(state, loss)
     
     
-    def train(self, epochs = 16000, batch_size = 128, verbose = 16, init_lr = 0.0001, decay_steps = 4000, key = random.key(0)):
-        batch_size = min(self.sc_data.shape[0], min(self.spatial_data.shape[0], batch_size))
+    def train(self, training_steps = 16000, batch_size = 128, verbose = 16, init_lr = 0.0001, decay_steps = 4000, key = random.key(0)):
+  
+        """
+        Set up optimization parameters and train the ENVI moodel
+
+
+        :param training_steps (int): number of gradient descent steps to train ENVI (default 16000)
+        :param batch_size (int): size of spatial and single-cell profiles sampled for each training step  (default 128)
+        :param verbose (int): amount of steps between each loss print statement (default 16)
+        :param init_lr (float): initial learning rate for ADAM optimizer with exponential decay (default 1e-4)
+        :param decay_steps (int): number of steps before each learning rate decay (default 4000)
+        :param key (jax.random.key): random seed (default jax.random.key(0))
+
+        :return: nothing
+        """ 
         
+        batch_size = min(self.sc_data.shape[0], min(self.spatial_data.shape[0], batch_size))
+
         key, subkey = random.split(key)
         state = self.create_train_state(subkey, init_lr = init_lr, decay_steps = decay_steps) 
         self.params = state.params
-        
-        tq = trange(epochs, leave=True, desc = "")
+
+        tq = trange(training_steps, leave=True, desc = "")
         sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = 0, 0, 0, 0, 0
-        
+
         sc_X = self.sc_data.X
         spatial_X =  self.spatial_data.X
         spatial_COVET =  self.spatial_data.obsm['COVET_SQRT']
-        
-        for epoch in tq:
+
+        for training_step in tq:
             key, subkey1, subkey2 = random.split(key, num = 3)
-            
+
             batch_spatial_ind = random.choice(key = subkey1, a = self.spatial_data.shape[0], shape = [batch_size], replace = False)
             batch_sc_ind = random.choice(key = subkey2, a = self.sc_data.shape[0], shape = [batch_size], replace = False)
-            
+
             batch_spatial_exp, batch_spatial_cov = spatial_X[batch_spatial_ind],  spatial_COVET[batch_spatial_ind]
             batch_sc_exp = sc_X[batch_sc_ind]
-            
+
             key, subkey = random.split(key)
-            
+
             state, loss = self.train_step(state, batch_spatial_exp, batch_spatial_cov, batch_sc_exp, key = subkey)
-            
+
             self.params = state.params
 
             sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = sc_loss_mean + loss[1][0], spatial_loss_mean + loss[1][1], cov_loss_mean + loss[1][2], kl_loss_mean + loss[1][3], count + 1
 
-            if(epoch%verbose==0):
+            if(training_step%verbose==0):
                 print_statement = ''
                 for metric,value in zip(['spatial', 'sc', 'cov', 'kl'], [spatial_loss_mean, sc_loss_mean, cov_loss_mean, kl_loss_mean]):
                     print_statement = print_statement + ' ' + metric + ': {:.3e}'.format(value/count)
 
                 sc_loss_mean, spatial_loss_mean, cov_loss_mean, kl_loss_mean, count = 0, 0, 0, 0, 0
                 tq.set_description(print_statement)
                 tq.refresh() # to show 
-                
+
         self.latent_rep()
         
     @partial(jit, static_argnums=(0, ))
     def model_encoder(self, x):
         return(self.model.bind({'params': self.params}).encoder(x))
     
     @partial(jit, static_argnums=(0, ))
@@ -405,56 +415,56 @@
             x_conf_split = np.array_split(x_conf, num_split)
             dec = np.concatenate([self.grammian_cov(self.model_decoder_cov(x_conf_split[split_ind])) for
                                   split_ind in range(num_split)], axis = 0)
         return(dec)
         
     def latent_rep(self): 
         """
-        Compute latent embeddings for spatial and single cell data
+        Compute latent embeddings for spatial and single cell data, automatically performed after training
         
-        Return:
-            no return, adds 'envi_latent' ENVI.spatial_data.obsm and ENVI.spatial_data.obsm
-        """
+        :return: nothing, adds 'envi_latent' self.spatial_data.obsm and self.spatial_data.obsm
+        """ 
     
         self.spatial_data.obsm['envi_latent'] = self.encode(self.spatial_data.X, mode = 'spatial')
         self.sc_data.obsm['envi_latent'] = self.encode(self.sc_data[:, self.spatial_data.var_names].X, mode = 'sc')
         
 
     
     def impute_genes(self):
         """
-        Imput full transcriptome for spatial data
+        Impute full transcriptome for spatial data
     
-        Return:
-            no return, adds 'imputation' to ENVI.spatial_data.obsm
+        :return: nothing adds 'imputation' to self.spatial_data.obsm
         """
             
     
         self.spatial_data.obsm['imputation'] = pd.DataFrame(self.decode_exp(self.spatial_data.obsm['envi_latent'],  mode = 'sc'), 
                                                             columns = self.sc_data.var_names, 
                                                             index = self.spatial_data.obs_names)
         
         print("Finished imputing missing gene for spatial data! See 'imputation' in obsm of ENVI.spatial_data")
      
     def infer_niche_covet(self):
-        """
-        Infer covariance niche composition for single cell data
         
-        Return:
-            no return, adds 'COVET_SQRT' and 'COVET' to ENVI.sc_data.obsm
         """
+        Predict COVET representation for single-cell data
+    
+        :return: nothing adds 'COVET_SQRT' and 'COVET' to self.spatial_data.obsm
+        """
+
         self.sc_data.obsm['COVET_SQRT'] = self.decode_cov(self.sc_data.obsm['envi_latent'])
         self.sc_data.obsm['COVET'] = np.matmul(self.sc_data.obsm['COVET_SQRT'], self.sc_data.obsm['COVET_SQRT'])
     
     def infer_niche_celltype(self, cell_type_key = 'cell_type'):
         """
         Predict cell type abundence based one ENVI-inferred COVET representations 
         
-        Return:
-            no return, adds 'niche_cell_type' to ENVI.sc_data.obsm & ENVI.spatial_data.obsm
+        :param cell_type_key (string): key in spatial_data.obs where cell types are stored for environment composition (default 'cell_type')
+        
+        :return: nothing, adds 'niche_cell_type' to self.sc_data.obsm & self.spatial_data.obsm
         """
          
         self.spatial_data.obsm['cell_type_niche'] = niche_cell_type(self.spatial_data, self.k_nearest, spatial_key = self.spatial_key, cell_type_key = cell_type_key, batch_key = self.batch_key)
         
         regression_model = sklearn.neighbors.KNeighborsRegressor(n_neighbors=5).fit(self.spatial_data.obsm['COVET_SQRT'].reshape([self.spatial_data.shape[0], -1]), 
                                                                                     self.spatial_data.obsm['cell_type_niche'])
```

### Comparing `scenvi-0.3.0/PKG-INFO` & `scenvi-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenvi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Integration of scRNA-seq and spatial transcriptomics data
 License: MIT
 Author: Doron Haviv
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

