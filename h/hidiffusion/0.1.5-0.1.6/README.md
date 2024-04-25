# Comparing `tmp/hidiffusion-0.1.5.tar.gz` & `tmp/hidiffusion-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidiffusion-0.1.5.tar", last modified: Tue Apr 23 14:21:35 2024, max compression
+gzip compressed data, was "hidiffusion-0.1.6.tar", last modified: Thu Apr 25 18:12:24 2024, max compression
```

## Comparing `hidiffusion-0.1.5.tar` & `hidiffusion-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-23 14:20:01.000000 hidiffusion-0.1.5/MANIFEST.in
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15069 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14776 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/README.md
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.213582 hidiffusion-0.1.5/hidiffusion/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/__init__.py
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   105456 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/hidiffusion.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/hidiffusion/sd_module_key/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/sd_module_key/sd15_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/sd_module_key/sdxl_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/utils.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/hidiffusion.egg-info/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15069 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      334 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/top_level.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/setup.cfg
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-23 14:20:54.000000 hidiffusion-0.1.5/setup.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    11357 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/LICENSE
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-25 18:11:43.000000 hidiffusion-0.1.6/MANIFEST.in
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15091 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14776 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/README.md
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/__init__.py
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   105548 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/hidiffusion.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion/sd_module_key/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/sd_module_key/sd15_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/sd_module_key/sdxl_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/utils.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion.egg-info/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15091 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      342 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/setup.cfg
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-25 18:11:34.000000 hidiffusion-0.1.6/setup.py
```

### Comparing `hidiffusion-0.1.5/PKG-INFO` & `hidiffusion-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.5
+Version: 0.1.6
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <!-- # 💡 HiDiffusion -->
 
 <div align="center">
   <img src="assets/hidiffusion_logo.jpg"  height=120>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.5 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.6 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown
+Jiajun Liang Description-Content-Type: text/markdown License-File: LICENSE
                          [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
```

### Comparing `hidiffusion-0.1.5/README.md` & `hidiffusion-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.5/hidiffusion/hidiffusion.py` & `hidiffusion-0.1.6/hidiffusion/hidiffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1746,15 +1746,16 @@
             
             if self.aggressive_raunet:
                 # self.T1 = min(int(self.max_timestep * self.T1_ratio), int(8/50 * self.max_timestep))
                 self.T1 = int(aggressive_step/50 * self.max_timestep)
             else:            
                 self.T1 = int(self.max_timestep * self.T1_ratio)
             if self.timestep < self.T1:
-                hidden_states = F.interpolate(hidden_states, scale_factor=2.0, mode='bicubic')
+                if ori_H != hidden_states.shape[2] and ori_W != hidden_states.shape[3]:
+                    hidden_states = F.interpolate(hidden_states, scale_factor=2.0, mode='bicubic')
             self.timestep += 1
             if self.timestep == self.max_timestep:
                 self.timestep = 0
             
             if old_diffusers:
                 if self.lora_layer is None:
                     # make sure to the functional Conv2D function as otherwise torch.compile's graph will break
```

### Comparing `hidiffusion-0.1.5/hidiffusion/sd_module_key/sd15_module_key.txt` & `hidiffusion-0.1.6/hidiffusion/sd_module_key/sd15_module_key.txt`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.5/hidiffusion/sd_module_key/sdxl_module_key.txt` & `hidiffusion-0.1.6/hidiffusion/sd_module_key/sdxl_module_key.txt`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.5/hidiffusion/utils.py` & `hidiffusion-0.1.6/hidiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.5/hidiffusion.egg-info/PKG-INFO` & `hidiffusion-0.1.6/hidiffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.5
+Version: 0.1.6
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <!-- # 💡 HiDiffusion -->
 
 <div align="center">
   <img src="assets/hidiffusion_logo.jpg"  height=120>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.5 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.6 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown
+Jiajun Liang Description-Content-Type: text/markdown License-File: LICENSE
                          [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
```

