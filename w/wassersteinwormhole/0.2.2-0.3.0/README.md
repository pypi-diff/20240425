# Comparing `tmp/wassersteinwormhole-0.2.2.tar.gz` & `tmp/wassersteinwormhole-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wassersteinwormhole-0.2.2.tar", max compression
+gzip compressed data, was "wassersteinwormhole-0.3.0.tar", max compression
```

## Comparing `wassersteinwormhole-0.2.2.tar` & `wassersteinwormhole-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      884 2024-04-06 20:42:04.006829 wassersteinwormhole-0.2.2/README.md
--rw-r--r--   0        0        0      382 2024-04-06 20:42:16.956757 wassersteinwormhole-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    15335 2024-04-06 20:41:25.158630 wassersteinwormhole-0.2.2/wassersteinwormhole/Wormhole.py
--rw-r--r--   0        0        0       30 2024-04-06 20:41:25.929478 wassersteinwormhole-0.2.2/wassersteinwormhole/__init__.py
--rw-r--r--   0        0        0     6997 2024-04-06 20:41:24.569044 wassersteinwormhole-0.2.2/wassersteinwormhole/utils_OT.py
--rw-r--r--   0        0        0     8357 2024-04-06 20:41:24.875511 wassersteinwormhole-0.2.2/wassersteinwormhole/utils_Transformer.py
--rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 wassersteinwormhole-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      852 2024-04-25 18:51:41.305312 wassersteinwormhole-0.3.0/README.md
+-rw-r--r--   0        0        0      382 2024-04-25 19:21:40.405227 wassersteinwormhole-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2656 2024-04-25 17:13:14.483313 wassersteinwormhole-0.3.0/wassersteinwormhole/DefaultConfig.py
+-rw-r--r--   0        0        0    16960 2024-04-25 17:27:05.475181 wassersteinwormhole-0.3.0/wassersteinwormhole/Wormhole.py
+-rw-r--r--   0        0        0       30 2024-04-25 17:27:07.725663 wassersteinwormhole-0.3.0/wassersteinwormhole/__init__.py
+-rw-r--r--   0        0        0     8343 2024-04-25 17:27:55.660813 wassersteinwormhole-0.3.0/wassersteinwormhole/_utils_Transformer.py
+-rw-r--r--   0        0        0     4036 2024-04-25 17:27:52.320398 wassersteinwormhole-0.3.0/wassersteinwormhole/_utils_WeightedAttention.py
+-rw-r--r--   0        0        0     9186 2024-04-25 17:27:38.887255 wassersteinwormhole-0.3.0/wassersteinwormhole/utils_OT.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 wassersteinwormhole-0.3.0/PKG-INFO
```

### Comparing `wassersteinwormhole-0.2.2/README.md` & `wassersteinwormhole-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-WassersteinWormhole for Python3
+WassersteinWormhole
 ======================
 
 Embedding point-clouds by presering Wasserstein distancse with the Wormhole.
 
 This implementation is written in Python3 and relies on FLAX, JAX, & JAX-OTT.
 
 
 To install JAX, simply run the command:
 
-    pip install --upgrade "jax[cuda11_pip]==0.4.23" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
 And to install WassersteinWormhole along with the rest of the requirements: 
 
     pip install wassersteinwormhole
 
 And running the Womrhole on your own set of point-clouds is as simple as:
     
     from wassersteinwormhole import Wormhole 
     WormholeModel = Wormhole(point_clouds = point_clouds)
     WormholeModel.train()
     Embeddings = WormholeModel.encode(WormholeModel.point_clouds, WormholeModel.masks)
-    
-For more details, follow tutorial at https://github.com/dpeerlab/WassersteinWormhole.
-    
+ 
+For more details, follow tutorial at https://wasserstienwormhole.readthedocs.io.
```

### Comparing `wassersteinwormhole-0.2.2/wassersteinwormhole/Wormhole.py` & `wassersteinwormhole-0.3.0/wassersteinwormhole/Wormhole.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,180 +2,220 @@
 import optax
 from flax import linen as nn
 from flax import struct
 from flax.training import train_state 
 
 import jax
 import jax.numpy as jnp
+import jax.scipy as jsp
 from jax import random, grad, jit, vmap
 from functools import partial
 import scipy.stats
 import numpy as np
 from tqdm import trange
 
-from wassersteinwormhole.utils_Transformer import * 
-from wassersteinwormhole.utils_OT import * 
-
+from wassersteinwormhole._utils_Transformer import * 
+import wassersteinwormhole.utils_OT as utils_OT
 
+from wassersteinwormhole.DefaultConfig import DefaultConfig
 
+    
+    
 def MaxMinScale(arr):
+    
+    """
+    :meta private:
+    """
+       
     min_arr = arr.min(axis = 0)
     max_arr = arr.max(axis = 0)
     
     arr = 2*(arr - arr.min(axis = 0, keepdims = True))/(arr.max(axis = 0, keepdims = True) - arr.min(axis = 0, keepdims = True))-1
     return(arr)
 
-def pad_pointclouds(point_clouds, max_shape = -1):
+def pad_pointclouds(point_clouds, weights, max_shape = -1):
+    """
+    :meta private:
+    """
+       
     if(max_shape == -1):
         max_shape = np.max([pc.shape[0] for pc in point_clouds])+1
     else:
         max_shape = max_shape + 1
-    weight_vec = np.asarray([np.concatenate((np.ones(pc.shape[0]), np.zeros(max_shape - pc.shape[0])), axis = 0) for pc in point_clouds])
+    weights_pad = np.asarray([np.concatenate((weight, np.zeros(max_shape - pc.shape[0])), axis = 0) for pc, weight in zip(point_clouds, weights)])
     point_clouds_pad = np.asarray([np.concatenate([pc, np.zeros([max_shape - pc.shape[0], pc.shape[-1]])], axis = 0) for pc in point_clouds])
     
+    weights_pad = weights_pad/weights_pad.sum(axis = 1, keepdims = True)
 
-    return(point_clouds_pad[:, :-1].astype('float32'), weight_vec[:, :-1].astype('float32'))
+    return(point_clouds_pad[:, :-1].astype('float32'), weights_pad[:, :-1].astype('float32'))
 
 class Wormhole():
-
-    def __init__(self, point_clouds, point_clouds_test = None, key = random.key(0), config = TransformerConfig):
     
-        self. config = config
+    """
+    Initializes Wormhole model and processes input point clouds 
+    
+    
+    :param point_clouds: (list of np.array) list of train-set point clouds to train Wormhole on
+    :param weights: (list of np.array) list of per point weight for each train-set point cloud (default None, indicating uniform weights)
+    :param point_clouds_test: (list of np.array) list of test-set point clouds (default None)
+    :param weights_test: (list of np.array)  list of per point weight for each test-set point cloud (default None, indicating uniform weights)
+    :param config: (flax struct.dataclass) object with parameters for Wormhole such as OT metric choice, emedding dimention, etc. See docs for 'DefaultConfig.py' and tutorial details. 
+    
+    :return: initialized Wormhole model
+    """ 
+        
+    def __init__(self, point_clouds, weights = None, point_clouds_test = None, weights_test = None, config = DefaultConfig):
+    
+        self.config = config
         self.point_clouds = point_clouds
+        
+        if(weights is None):
+            self.weights = [np.ones(pc.shape[0])/pc.shape[0] for pc in self.point_clouds]
+        else:
+            self.weights = weights
+        
         if(point_clouds_test is None):
-            self.point_clouds, self.masks = pad_pointclouds(self.point_clouds)
-            self.masks_normalized = self.masks/self.masks.sum(axis = 1, keepdims = True)
+            self.point_clouds, self.weights = pad_pointclouds(self.point_clouds, self.weights)
         else:
             self.point_clouds_test = point_clouds_test
+            
+            if(weights_test is None):
+                self.weights_test = [np.ones(pc.shape[0])/pc.shape[0] for pc in self.point_clouds_test]
+            else:
+                self.weights_test = weights_test
+                
+            
+            total_point_clouds, total_weights = pad_pointclouds(list(self.point_clouds) + list(self.point_clouds_test), list(self.weights) + list(self.weights_test))
+            self.point_clouds, self.weights = total_point_clouds[:len(list(self.point_clouds))], total_weights[:len(list(self.point_clouds))]
+            self.point_clouds_test, self.weights_test = total_point_clouds[len(list(self.point_clouds)):], total_weights[len(list(self.point_clouds)):]
 
-            total_point_clouds, total_masks = pad_pointclouds(list(self.point_clouds) + list(self.point_clouds_test))
-            self.point_clouds, self.masks = total_point_clouds[:len(list(self.point_clouds))], total_masks[:len(list(self.point_clouds))]
-            self.point_clouds_test, self.masks_test = total_point_clouds[len(list(self.point_clouds)):], total_masks[len(list(self.point_clouds)):]
-
-            self.masks_normalized = self.masks/self.masks.sum(axis = 1, keepdims = True)
-            self.masks_test_normalized = self.masks_test/self.masks_test.sum(axis = 1, keepdims = True)
+        
+        self.scale_weights = np.exp(-jsp.special.xlogy(self.weights, self.weights).sum(axis = 1).mean())
+        self.out_seq_len = int(jnp.exp(-jsp.special.xlogy(self.weights, self.weights).sum(axis = 1).mean()))
 
-        self.out_seq_len = int(jnp.median(jnp.sum(self.masks, axis = 1)))
         self.inp_dim = self.point_clouds.shape[-1]
 
 
 
         
         self.eps_enc = config.eps_enc
         self.eps_dec = config.eps_dec
 
         self.lse_enc = config.lse_enc
         self.lse_dec = config.lse_dec
 
         self.coeff_dec = config.coeff_dec
         
         self.dist_func_enc = config.dist_func_enc
-        if(self.dist_func_enc == 'W1'):
-            self.jit_dist_enc = jax.jit(jax.vmap(W1, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_enc == 'W2'):
-            self.jit_dist_enc = jax.jit(jax.vmap(W2, (0, 0, None, None), 0), static_argnums=[2,3])    
-        if(self.dist_func_enc == 'W2_norm'):
-            self.jit_dist_enc = jax.jit(jax.vmap(W2_norm, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_enc == 'GW'):
-            self.jit_dist_enc = jax.jit(jax.vmap(GW, (0, 0, None, None), 0), static_argnums=[2,3]) 
-        if(self.dist_func_enc == 'S1'):
-            self.jit_dist_enc = jax.jit(jax.vmap(S1, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_enc == 'S2'):
-            self.jit_dist_enc = jax.jit(jax.vmap(S2, (0, 0, None, None), 0), static_argnums=[2,3])    
-        if(self.dist_func_enc == 'S2_norm'):
-            self.jit_dist_enc = jax.jit(jax.vmap(S2_norm, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_enc == 'GS'):
-            self.jit_dist_enc = jax.jit(jax.vmap(GS, (0, 0, None, None), 0), static_argnums=[2,3]) 
-
         self.dist_func_dec = config.dist_func_dec
-        if(self.dist_func_dec == 'W1'):
-            self.jit_dist_dec = jax.jit(jax.vmap(W1_grad, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_dec == 'W2'):
-            self.jit_dist_dec = jax.jit(jax.vmap(W2_grad, (0, 0, None, None), 0), static_argnums=[2,3])    
-        if(self.dist_func_dec == 'W2_norm'):
-            self.jit_dist_dec = jax.jit(jax.vmap(W2_norm_grad, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_dec == 'GW'):
-            self.jit_dist_dec = jax.jit(jax.vmap(GW_grad, (0, 0, None, None), 0), static_argnums=[2,3]) 
-        if(self.dist_func_dec == 'S1'):
-            self.jit_dist_dec = jax.jit(jax.vmap(S1, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_dec == 'S2'):
-            self.jit_dist_dec = jax.jit(jax.vmap(S2, (0, 0, None, None), 0), static_argnums=[2,3])    
-        if(self.dist_func_dec == 'S2_norm'):
-            self.jit_dist_dec = jax.jit(jax.vmap(S2_norm, (0, 0, None, None), 0), static_argnums=[2,3])
-        if(self.dist_func_dec == 'GS'):
-            self.jit_dist_dec = jax.jit(jax.vmap(GS, (0, 0, None, None), 0), static_argnums=[2,3]) 
+        
+        self.jit_dist_enc = jax.jit(jax.vmap(getattr(utils_OT, self.dist_func_enc), (0, 0, None, None), 0), static_argnums=[2,3])
+        self.jit_dist_dec = jax.jit(jax.vmap(getattr(utils_OT, self.dist_func_dec), (0, 0, None, None), 0), static_argnums=[2,3])
+        
         if(self.coeff_dec < 0):
-            self.jit_dist_dec  = jax.jit(jax.vmap(Zeros, (0, 0, None, None), 0), static_argnums=[2,3]) 
-            self.coeff_dec = 0.0
-      
-
+            self.jit_dist_dec  = jax.jit(jax.vmap(utils_OT.Zeros, (0, 0, None, None), 0), static_argnums=[2,3]) 
+            self.coeff_dec = 0.0 
 
         self.scale = config.scale
         self.factor = config.factor
         self.point_clouds = self.scale_func(self.point_clouds) * self.factor
         if(point_clouds_test is not None):
             self.point_clouds_test = self.scale_func(self.point_clouds_test)*self.factor
         
       
-        self.pc_max_val = np.max(self.point_clouds[self.masks > 0])
-        self.pc_min_val = np.min(self.point_clouds[self.masks > 0])
-        self.scale_out = not np.isin(self.dist_func_dec, ['GS', 'GW'])
+        self.pc_max_val = np.max(self.point_clouds[self.weights > 0]) #* (1 + 1 * np.isin(self.dist_func_dec, ['GS', 'GW']))
+        self.pc_min_val = np.min(self.point_clouds[self.weights > 0]) #* (1 + 1 * np.isin(self.dist_func_dec, ['GS', 'GW']))
+        self.scale_out = True #not np.isin(self.dist_func_dec, ['GS', 'GW'])
         
         self.model = Transformer(self.config, out_seq_len = self.out_seq_len, inp_dim = self.inp_dim,
-                                 scale_out = self.scale_out, min_val = self.pc_min_val, max_val = self.pc_max_val)
+                                 scale_weights = self.scale_weights, scale_out = self.scale_out, min_val = self.pc_min_val, max_val = self.pc_max_val)
 
 
     def scale_func(self, point_clouds):
+            
+        """
+        :meta private:
+        """
+    
         if(self.scale == 'max_dist_total'):
             if(not hasattr(self, 'max_scale_num')):
                 max_dist = 0
                 for _ in range(10):
                     i,j = np.random.choice(np.arange(len(self.point_clouds)), 2,replace = False)
                     if(self.dist_func_enc == 'GW' or self.dist_func_enc == 'GS'):
-                        max_ij = np.max(scipy.spatial.distance.cdist(self.point_clouds[i], self.point_clouds[i])**2)
+                        max_ij = np.max(scipy.spatial.distance.cdist(self.point_clouds[i], self.point_clouds[i]))
                     else:
-                        max_ij = np.max(scipy.spatial.distance.cdist(self.point_clouds[i], self.point_clouds[j])**2)
+                        max_ij = np.max(scipy.spatial.distance.cdist(self.point_clouds[i], self.point_clouds[j]))
                     max_dist = np.maximum(max_ij, max_dist)
                 self.max_scale_num = max_dist
             else:
                 print("Using Calculated Max Dist Scaling Values") 
             return(point_clouds/self.max_scale_num)
         if(self.scale == 'max_dist_each'):
             print("Using Per Sample Max Dist") 
-            pc_scale = np.asarray([pc/np.max(scipy.spatial.distance.pdist(pc)**2) for pc in point_clouds])
+            pc_scale = np.asarray([pc/np.max(scipy.spatial.distance.pdist(pc)) for pc in point_clouds])
             return(pc_scale)
         if(self.scale == 'min_max_each'):
             print("Scaling Per Sample") 
             max_val = point_clouds.max(axis = 1, keepdims = True)
             min_val = point_clouds.min(axis = 1, keepdims = True)
             return(2 * (point_clouds - min_val)/(max_val - min_val) - 1)
         elif(self.scale == 'min_max_total'):
             if(not hasattr(self, 'max_val')):
                 self.max_val = self.point_clouds.max(axis = ((0,1)), keepdims = True)
                 self.min_val = self.point_clouds.min(axis = ((0,1)), keepdims = True)
             else:
                 print("Using Calculated Min Max Scaling Values") 
             return(2 * (point_clouds - self.min_val)/(self.max_val - self.min_val) - 1)
-        elif(isinstance(self.scale, (int, float, complex)) and not isinstance(self.scale, bool)):
-            print("Using Constant Scaling Value") 
-            return(point_clouds/self.scale)
+        elif(self.scale == 'min_max_total_all_axis'):
+            if(not hasattr(self, 'max_val')):
+                self.max_val = self.point_clouds.max(keepdims = True)
+                self.min_val = self.point_clouds.min(keepdims = True)
+            else:
+                print("Using Calculated Min Max Scaling Values") 
+            return(2 * (point_clouds - self.min_val)/(self.max_val - self.min_val) - 1)
+        else:
+            return(point_clouds)
     
-    def encode(self, pc, masks, max_batch = 256):
+    def encode(self, pc, weights, max_batch = 256):
+                
+        """
+        Encode point clouds with trained Wormhole model
+
+
+        :param pc: (np.array) array of point clouds to encode
+        :param weights: (np.array) point weigts for input point clouds. Wormhole calculates padding for train and test-set point clouds.
+        :param max_batch: (int) maximum size of batch during inference calls to Wormhole (default 256)
+
+        :return enc: per point cloud embeddings
+        """ 
+        
         if(pc.shape[0] < max_batch):
-            enc = self.model.bind({'params': self.params}).Encoder(pc, masks, deterministic = True)
+            enc = self.model.bind({'params': self.params}).Encoder(pc, weights, deterministic = True)
         else: # For when the GPU can't pass all point-clouds at once
             num_split = int(pc.shape[0]/max_batch)+1
             pc_split = np.array_split(pc, num_split)
-            mask_split = np.array_split(masks, num_split)
+            mask_split = np.array_split(weights, num_split)
             
             enc = np.concatenate([self.model.bind({'params': self.params}).Encoder(pc_split[split_ind], mask_split[split_ind], deterministic = True) for
                                   split_ind in range(num_split)], axis = 0)
         return enc
     
     def decode(self, enc, max_batch = 256):
+        
+        """
+        Decode embedding back into point clouds using Wormhole decoder
+
+
+        :param enc: (np.array) embeddings to decode
+        :param max_batch: (int) maximum size of batch during inference calls to Wormhole (default 256)
+
+        :return dec: decoded point clouds from embeddings
+        """ 
+        
         if(enc.shape[0]<max_batch):
             dec = self.model.bind({'params': self.params}).Decoder(enc, deterministic = True)
             if(self.scale_out):
                 dec = nn.sigmoid(dec) * (self.pc_max_val - self.pc_min_val) + self.pc_min_val
         else:
             num_split = int(enc.shape[0]/max_batch)+1
             enc_split = np.array_split(enc, num_split) 
@@ -183,119 +223,145 @@
                                   for split_ind in range(num_split)], axis = 0)
             if(self.scale_out):
                 dec_split = np.array_split(dec, num_split) 
                 dec = np.concatenate([nn.sigmoid(dec_split[split_ind]) * (self.pc_max_val - self.pc_min_val) + self.pc_min_val for split_ind in range(num_split)], axis = 0)
         return dec
     
     #@partial(jit, static_argnums=(0,4))
-    def call(self, pc, masks, deterministic = False, key = random.key(0)):
-        enc, dec = self.model.apply(self.variables, rngs = {'dropout': key}, deterministic = deterministic,
-                                    inputs = pc, masks = masks)
+    def call(self, pc, weights, deterministic = True, key = random.key(0)):
+                            
+        """
+        :meta private:
+        """
+    
+        enc, dec = self.model.apply(self.variables, inputs = pc, weights = weights, deterministic = deterministic, dropout_rng = key)
         return(enc, dec)
     
     #@partial(jit, static_argnums=(0,4))
-    def compute_losses(self, pc, masks, enc, dec):
+    def compute_losses(self, pc, weights, enc, dec):
+                      
+        """
+        :meta private:
+        """
     
-        
-        
-        mask_normalized = masks/jnp.sum(masks, axis = 1,keepdims = True)
-
-        pc_pairwise_dist = self.jit_dist_enc([pc[self.tri_u_ind[:, 0]], mask_normalized[self.tri_u_ind[:, 0]]],
-                                             [pc[self.tri_u_ind[:, 1]], mask_normalized[self.tri_u_ind[:, 1]]], 
+        pc_pairwise_dist = self.jit_dist_enc([pc[self.tri_u_ind[:, 0]], weights[self.tri_u_ind[:, 0]]],
+                                             [pc[self.tri_u_ind[:, 1]], weights[self.tri_u_ind[:, 1]]], 
                                              self.eps_enc, self.lse_enc)
        
         enc_pairwise_dist = jnp.mean(jnp.square(enc[self.tri_u_ind[:, 0]] - enc[self.tri_u_ind[:, 1]]), axis = 1)
-        
-        
-        pc_dec_dist = self.jit_dist_dec([pc, mask_normalized], [dec, self.pseudo_masks], 
+        pc_dec_dist = self.jit_dist_dec([pc, weights], [dec, self.pseudo_weights], 
                                         self.eps_dec, self.lse_dec)
         
         # pc_dec_dist = 0
         return(pc_pairwise_dist, enc_pairwise_dist, pc_dec_dist)
        
     
     def create_train_state(self, key = random.key(0), init_lr = 0.0001, decay_steps = 2000):
-        
+                      
+        """
+        :meta private:
+        """
+    
         key, subkey = random.split(key)
-        params = self.model.init(rngs = {'params': key, 'dropout': subkey}, deterministic = False,
-                                         inputs = self.point_clouds[0:1], masks = self.masks[0:1])['params']
+        params = self.model.init(rngs = {'params': key}, dropout_rng = subkey, deterministic = False,
+                                         inputs = self.point_clouds[0:1], weights = self.weights[0:1])['params']
         
-        lr_sched = optax.exponential_decay(0.0001, decay_steps, 0.9, staircase = True)
+        lr_sched = optax.exponential_decay(init_lr, decay_steps, 0.9, staircase = True)
         tx = optax.adam(lr_sched)#
         
         return(TrainState.create(
           apply_fn=self.model.apply, params=params, tx=tx,
           metrics=Metrics.empty()))
     
     @partial(jit, static_argnums=(0, ))
-    def train_step(self, state, pc, masks, key = random.key(0)):
-        """Train for a single step."""
-        
+    def train_step(self, state, pc, weights, key = random.key(0)):
+                      
+        """
+        :meta private:
+        """
+    
         def loss_fn(params):
-            enc, dec = state.apply_fn({'params':params}, inputs = pc, masks = masks, deterministic = False, rngs = {'dropout': key})
-            pc_pairwise_dist, enc_pairwise_dist, pc_dec_dist = self.compute_losses(pc, masks, enc, dec)
+            enc, dec = state.apply_fn({'params':params}, inputs = pc, weights = weights, deterministic = False, dropout_rng = key)
+            pc_pairwise_dist, enc_pairwise_dist, pc_dec_dist = self.compute_losses(pc, weights, enc, dec)
             
             enc_loss = jnp.mean(jnp.square(pc_pairwise_dist - enc_pairwise_dist))
             dec_loss = jnp.mean(pc_dec_dist)
             enc_corr = jnp.corrcoef(enc_pairwise_dist, pc_pairwise_dist)[0,1]
             return(enc_loss + self.coeff_dec * dec_loss, [enc_loss, dec_loss, enc_corr])
     
         grad_fn = jax.value_and_grad(loss_fn, has_aux = True)
         loss, grads = grad_fn(state.params)
         state = state.apply_gradients(grads=grads)
         return(state, loss)
     
     @partial(jit, static_argnums=(0, ))
-    def compute_metrics(self, state, pc, masks, key = random.key(0)):
-        enc, dec  = state.apply_fn({'params': state.params}, inputs = pc, masks = masks, deterministic = False, rngs = {'dropout': key})
-        pc_pairwise_dist, enc_pairwise_dist, pc_dec_dist = self.compute_losses(pc, masks, enc, dec)
+    def compute_metrics(self, state, pc, weights, key = random.key(0)):
+                      
+        """
+        :meta private:
+        """
+    
+        enc, dec  = state.apply_fn({'params': state.params}, inputs = pc, weights = weights, deterministic = False, dropout_rng = key)
+        pc_pairwise_dist, enc_pairwise_dist, pc_dec_dist = self.compute_losses(pc, weights, enc, dec)
         
         enc_loss = jnp.mean(jnp.square(pc_pairwise_dist - enc_pairwise_dist))
         dec_loss = jnp.mean(pc_dec_dist)
         enc_corr = jnp.corrcoef(enc_pairwise_dist, pc_pairwise_dist)[0,1]
         
     
         metric_updates = state.metrics.single_from_model_output(enc_loss = enc_loss, dec_loss = dec_loss, enc_corr = enc_corr)
         metrics = state.metrics.merge(metric_updates)
         state = state.replace(metrics=metrics)
         return(state)
 
-    def train(self, epochs = 10000, batch_size = 16, verbose = 8, init_lr = 0.0001, decay_steps = 2000, key = random.key(0)):
+    def train(self, training_steps = 10000, batch_size = 16, verbose = 8, init_lr = 0.0001, decay_steps = 2000, key = random.key(0)):
+          
+        """
+        Set up optimization parameters and train the ENVI moodel
+
+
+        :param training_steps: (int) number of gradient descent steps to train ENVI (default 10000)
+        :param batch_size: (int) size of train-set point clouds sampled for each training step  (default 16)
+        :param verbose: (int) amount of steps between each loss print statement (default 8)
+        :param init_lr: (float) initial learning rate for ADAM optimizer with exponential decay (default 1e-4)
+        :param decay_steps: (int) number of steps before each learning rate decay (default 2000)
+        :param key: (jax.random.key) random seed (default jax.random.key(0))
+
+        :return: nothing
+        """ 
+        
         batch_size = min(self.point_clouds.shape[0], batch_size)
         
         self.tri_u_ind = jnp.stack(jnp.triu_indices(batch_size, 1), axis =1)
-        self.pseudo_masks = jnp.ones([batch_size, self.out_seq_len])/self.out_seq_len
+        self.pseudo_weights = jnp.ones([batch_size, self.out_seq_len])/self.out_seq_len
 
         key, subkey = random.split(key)
         state = self.create_train_state(subkey, init_lr = init_lr, decay_steps = decay_steps)
         
         
 
         
-        tq = trange(epochs, leave=True, desc = "")
+        tq = trange(training_steps, leave=True, desc = "")
         enc_loss_mean, dec_loss_mean, enc_corr_mean, count = 0,0,0,0
-        for epoch in tq:
-            # time.sleep(1)
+        for training_step in tq:
             key, subkey = random.split(key)
 
-
-
             if(batch_size < self.point_clouds.shape[0]):
                 batch_ind = random.choice(key = subkey, a = self.point_clouds.shape[0], shape = [batch_size], replace = False)
-                point_clouds_batch, masks_batch = self.point_clouds[batch_ind], self.masks[batch_ind]
+                point_clouds_batch, weights_batch = self.point_clouds[batch_ind], self.weights[batch_ind]
             else:
-                point_clouds_batch, masks_batch = self.point_clouds, self.masks
+                point_clouds_batch, weights_batch = self.point_clouds, self.weights
 
             key, subkey = random.split(key)
-            state, loss = self.train_step(state, point_clouds_batch, masks_batch, subkey)
+            state, loss = self.train_step(state, point_clouds_batch, weights_batch, subkey)
             self.params = state.params
 
             enc_loss_mean, dec_loss_mean, enc_corr_mean, count = enc_loss_mean + loss[1][0], dec_loss_mean + loss[1][1], enc_corr_mean + loss[1][2], count + 1
 
-            if(epoch%verbose==0):
+            if(training_step%verbose==0):
                 print_statement = ''
                 for metric,value in zip(['enc_loss', 'dec_loss', 'enc_corr'], [enc_loss_mean, dec_loss_mean, enc_corr_mean]):
                     if(metric == 'enc_corr'):
                         print_statement = print_statement + ' ' + metric + ': {:.3f}'.format(value/count)
                     else:
                         print_statement = print_statement + ' ' + metric + ': {:.3e}'.format(value/count)
```

### Comparing `wassersteinwormhole-0.2.2/wassersteinwormhole/utils_Transformer.py` & `wassersteinwormhole-0.3.0/wassersteinwormhole/_utils_Transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,50 +11,28 @@
 
 from functools import partial
 import scipy.stats
 import numpy as np
 
 from typing import Callable, Any, Optional
 
+from wassersteinwormhole._utils_WeightedAttention import WeightedMultiheadAttention
+from wassersteinwormhole.DefaultConfig import DefaultConfig
+
 
-@struct.dataclass
-class TransformerConfig:
-    """Global hyperparameters used to minimize obnoxious kwarg plumbing."""
-    vocab_size: int
-    output_vocab_size: int
-    dtype: Any = jnp.float32
-    dist_func_enc: str = 'S2'
-    dist_func_dec: str = 'S2'
-    eps_enc: float = 0.1
-    eps_dec: float = 0.01
-    lse_enc: bool = False
-    lse_dec: bool = True
-    coeff_dec: float = 1
-    scale: str = 'min_max_total'
-    factor: float = 1.0
-    emb_dim: int = 128
-    num_heads: int = 4
-    num_layers: int = 3
-    qkv_dim: int = 128
-    mlp_dim: int = 512
-    max_len: int = 256
-    attention_dropout_rate: float = 0.1
-    kernel_init: Callable = nn.initializers.glorot_uniform()
-    bias_init: Callable = nn.initializers.zeros_init()
 
-    
 class Embedding(nn.Module):
     """Transformer embedding block.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     out_dim: optionally specify out dimension.
     """
 
-    config: TransformerConfig
+    config: DefaultConfig
 
     @nn.compact
     def __call__(self, inputs):
         config = self.config
         output = nn.Dense(
             config.emb_dim,
             dtype=config.dtype,
@@ -63,19 +41,19 @@
         )(inputs)
         return output
 
 class Unembedding(nn.Module):
     """Transformer embedding block.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     out_dim: optionally specify out dimension.
     """
 
-    config: TransformerConfig
+    config: DefaultConfig
     inp_dim: int
 
     @nn.compact
     def __call__(self, inputs):
         config = self.config
         output = nn.Dense(
             self.inp_dim,
@@ -85,19 +63,19 @@
         )(inputs)
         return output
     
 class Multiplyer(nn.Module):
     """Encoding multiplyer block.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     out_dim: optionally specify out dimension.
     """
 
-    config: TransformerConfig
+    config: DefaultConfig
     out_seq_len: int
 
     @nn.compact
     def __call__(self, inputs):
         config = self.config
         output = nn.Dense(
             config.emb_dim * self.out_seq_len,
@@ -107,187 +85,190 @@
         )(inputs)
         return output.reshape([inputs.shape[0], self.out_seq_len, config.emb_dim])
     
 class FeedForward(nn.Module):
     """Transformer MLP / feed-forward block.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     out_dim: optionally specify out dimension.
     """
 
-    config: TransformerConfig
+    config: DefaultConfig
 
     @nn.compact
     def __call__(self, inputs):
         config = self.config
         x = nn.Dense(
             config.mlp_dim,
             dtype=config.dtype,
             kernel_init=config.kernel_init,
             bias_init=config.bias_init,
         )(inputs)
         x = nn.relu(x)
-        x = nn.Dense(
+        output = nn.Dense(
             inputs.shape[-1],
             dtype=config.dtype,
             kernel_init=config.kernel_init,
             bias_init=config.bias_init,
         )(x) + inputs
-        output = nn.LayerNorm(dtype=config.dtype)(x)
         return output
 
+
     
 class EncoderBlock(nn.Module):
     """Transformer encoder layer.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     """
 
-    config: TransformerConfig
-
+    config: DefaultConfig
+    scale_weights: Optional[float] = 1
+    
     @nn.compact
-    def __call__(self, inputs, masks, deterministic):
+    def __call__(self, inputs, weights, deterministic, dropout_rng):
+        
         config = self.config
-
+        scale_weights = self.scale_weights
         # Attention block.
-        # x = nn.LayerNorm(dtype=config.dtype)(inputs)
-        x = nn.MultiHeadDotProductAttention(
-            num_heads=config.num_heads,
-            dtype=config.dtype,
-            qkv_features=config.qkv_dim,
-            kernel_init=config.kernel_init,
-            bias_init=config.bias_init,
-            use_bias=False,
-            broadcast_dropout=False,
-            dropout_rate=config.attention_dropout_rate,
-            deterministic=deterministic,
-        )(inputs, mask = masks[:, None, None, :]) + inputs
+   
+        x = WeightedMultiheadAttention(config, scale_weights)(x = inputs, 
+                                                             weights = weights, 
+                                                             deterministic = deterministic, 
+                                                             dropout_rng = dropout_rng) + inputs
 
-        #x = nn.Dropout(rate=config.attention_dropout_rate)(x, deterministic=deterministic)
-        x = x + inputs
         x = nn.LayerNorm(dtype=config.dtype)(x)
-        output = FeedForward(config=config)(x)
+        x = FeedForward(config=config)(x)
+        output = nn.LayerNorm(dtype=config.dtype)(x)
         return output
 
 class DecoderBlock(nn.Module):
     """Transformer decoder layer.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     """
 
-    config: TransformerConfig
+    config: DefaultConfig
 
     @nn.compact
-    def __call__(self, inputs, deterministic):
+    def __call__(self, inputs, deterministic, dropout_rng):
         config = self.config
 
         # Attention block.
-        x = nn.MultiHeadDotProductAttention(
-            num_heads=config.num_heads,
-            dtype=config.dtype,
-            qkv_features=config.qkv_dim,
-            kernel_init=config.kernel_init,
-            bias_init=config.bias_init,
-            use_bias=False,
-            broadcast_dropout=False,
-            dropout_rate=config.attention_dropout_rate,
-            deterministic=deterministic,
-        )(inputs) + inputs
+        x = WeightedMultiheadAttention(config)(x = inputs, 
+                                               deterministic = deterministic, 
+                                               dropout_rng = dropout_rng) + inputs
 
+        #x = nn.Dropout(rate=config.attention_dropout_rate)(x, deterministic=deterministic)
         x = nn.LayerNorm(dtype=config.dtype)(x)
-        output = FeedForward(config=config)(x)
-        
+        x = FeedForward(config=config)(x)
+        output = nn.LayerNorm(dtype=config.dtype)(x)
         return output
 
     
-class Encoder(nn.Module):
+class EncoderModel(nn.Module):
     """Transformer encoder network.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     """
-    config: TransformerConfig
+    config: DefaultConfig
+    scale_weights: Optional[float] = 1
     
     @nn.compact
-    def __call__(self, inputs, masks, deterministic):
+    def __call__(self, inputs, weights, deterministic, dropout_rng = random.key(0)):
 
         config = self.config
-
+        scale_weights = self.scale_weights
+        
         x = inputs#.astype('int32')
         x = Embedding(config)(x)
 
         for _ in range(config.num_layers):
-            x = EncoderBlock(config)(x, masks = masks, deterministic=deterministic)
-
-        x = jnp.sum(x * masks[:, :, None], axis = 1)/jnp.sum(masks, axis = 1, keepdims = True)
+            x = EncoderBlock(config, scale_weights)(inputs = x, 
+                                                    weights = weights, 
+                                                    deterministic = deterministic, 
+                                                    dropout_rng = dropout_rng)
+        x = jnp.sum(x * weights[:, :, None], axis = 1)/jnp.sum(weights, axis = 1, keepdims = True)
         output = FeedForward(config)(x)
         return output
 
-class Decoder(nn.Module):
+class DecoderModel(nn.Module):
     """Transformer decoder network.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     """
-    config: TransformerConfig
+    config: DefaultConfig
     out_seq_len: int
     imp_dim: int
     
     @nn.compact
-    def __call__(self, inputs, deterministic):
+    def __call__(self, inputs, deterministic, dropout_rng = random.key(0)):
 
         config = self.config
 
         x = inputs#.astype('int32')
         x = Multiplyer(config, self.out_seq_len)(x)
 
         for _ in range(config.num_layers):
-            x = DecoderBlock(config)(x, deterministic=deterministic)
+            x = DecoderBlock(config)(inputs = x, 
+                                    deterministic = deterministic, 
+                                    dropout_rng = dropout_rng)
         x = FeedForward(config)(x)
         output = Unembedding(config, self.imp_dim)(x)
         return output
     
 class Transformer(nn.Module):
     """Transformer autoencoder model.
 
     Attributes:
-    config: TransformerConfig dataclass containing hyperparameters.
+    config: DefaultConfig dataclass containing hyperparameters.
     """
     
-    config: TransformerConfig
+    config: DefaultConfig
     out_seq_len: int
     inp_dim : int
+    scale_weights: Optional[float] = 1
     scale_out: Optional[bool] = True
     min_val: Optional[Any] = -1
     max_val: Optional[Any] = 1
     
     def setup(self):
         config = self.config
         out_seq_len = self.out_seq_len
         inp_dim = self.inp_dim
+        scale_weights = self.scale_weights
         scale_out = self.scale_out
         min_val = self.min_val
         max_val = self.max_val
         
-        self.Encoder = Encoder(config)#(inputs, masks, deterministic=deterministic)
-        self.Decoder = Decoder(config, out_seq_len, inp_dim)#(enc, deterministic=deterministic)
+        self.Encoder = EncoderModel(config, scale_weights)#(inputs, weights, deterministic=deterministic)
+        self.Decoder = DecoderModel(config, out_seq_len, inp_dim)#(enc, deterministic=deterministic)
     
-    def __call__(self, inputs, masks, deterministic):
+    def __call__(self, inputs, weights, deterministic = True, dropout_rng = random.key(0)):
         config = self.config
         out_seq_len = self.out_seq_len
         inp_dim = self.inp_dim
         scale_out = self.scale_out
         min_val = self.min_val
         max_val = self.max_val
         
-        enc = self.Encoder(inputs, masks, deterministic=deterministic)
-        dec = self.Decoder(enc, deterministic=deterministic)
+
+        
+        enc = self.Encoder(inputs = inputs, 
+                            weights = weights, 
+                            deterministic = deterministic, 
+                            dropout_rng = dropout_rng)
+        
+        dec = self.Decoder(inputs = enc, 
+                            deterministic = deterministic, 
+                            dropout_rng = dropout_rng)
         
         if(scale_out):
             dec = nn.sigmoid(dec) * (max_val - min_val) + min_val        
         return(enc, dec)
```

### Comparing `wassersteinwormhole-0.2.2/PKG-INFO` & `wassersteinwormhole-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: wassersteinwormhole
-Version: 0.2.2
+Version: 0.3.0
 Summary: Transformer based embeddings for Wasserstein Distances
 License: MIT
 Author: Anon
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: clu (==0.0.10)
-Requires-Dist: flax (==0.7.5)
-Requires-Dist: ott-jax (==0.4.4)
-Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Requires-Dist: clu (==0.0.12)
+Requires-Dist: flax (==0.8.2)
+Requires-Dist: ott-jax (==0.4.6)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
-WassersteinWormhole for Python3
+WassersteinWormhole
 ======================
 
 Embedding point-clouds by presering Wasserstein distancse with the Wormhole.
 
 This implementation is written in Python3 and relies on FLAX, JAX, & JAX-OTT.
 
 
 To install JAX, simply run the command:
 
-    pip install --upgrade "jax[cuda11_pip]==0.4.23" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
 And to install WassersteinWormhole along with the rest of the requirements: 
 
     pip install wassersteinwormhole
 
 And running the Womrhole on your own set of point-clouds is as simple as:
     
     from wassersteinwormhole import Wormhole 
     WormholeModel = Wormhole(point_clouds = point_clouds)
     WormholeModel.train()
     Embeddings = WormholeModel.encode(WormholeModel.point_clouds, WormholeModel.masks)
-    
-For more details, follow tutorial at https://github.com/dpeerlab/WassersteinWormhole.
-    
+ 
+For more details, follow tutorial at https://wasserstienwormhole.readthedocs.io.
+
```

