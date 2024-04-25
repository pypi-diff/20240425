# Comparing `tmp/diffedit-0.0.2rc7.tar.gz` & `tmp/diffedit-0.0.2rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffedit-0.0.2rc7.tar", max compression
+gzip compressed data, was "diffedit-0.0.2rc8.tar", max compression
```

## Comparing `diffedit-0.0.2rc7.tar` & `diffedit-0.0.2rc8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/LICENSE
--rw-r--r--   0        0        0     5073 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/README.md
--rw-r--r--   0        0        0     4983 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/__init__.py
--rw-r--r--   0        0        0       57 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/constants.py
--rw-r--r--   0        0        0    10994 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/diff_edit_model.py
--rw-r--r--   0        0        0     2243 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/image_processing.py
--rw-r--r--   0        0        0     8789 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/mask_generation.py
--rw-r--r--   0        0        0      852 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/mask_inpainting.py
--rw-r--r--   0        0        0     3833 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/model/model_composer.py
--rw-r--r--   0        0        0     7551 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/image_edit.py
--rw-r--r--   0        0        0   434756 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/mask.png
--rw-r--r--   0        0        0   491401 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/result.png
--rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 diffedit-0.0.2rc7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/LICENSE
+-rw-r--r--   0        0        0     5062 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/README.md
+-rw-r--r--   0        0        0     4983 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/constants.py
+-rw-r--r--   0        0        0    10994 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/diff_edit_model.py
+-rw-r--r--   0        0        0     2243 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/image_processing.py
+-rw-r--r--   0        0        0     8789 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/mask_generation.py
+-rw-r--r--   0        0        0      852 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/mask_inpainting.py
+-rw-r--r--   0        0        0     3833 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/model/model_composer.py
+-rw-r--r--   0        0        0     7551 2024-04-25 10:07:43.361490 diffedit-0.0.2rc8/src/diff_edit/scripts/image_edit.py
+-rw-r--r--   0        0        0   434756 2024-04-25 10:07:43.365490 diffedit-0.0.2rc8/src/diff_edit/scripts/mask.png
+-rw-r--r--   0        0        0   491401 2024-04-25 10:07:43.365490 diffedit-0.0.2rc8/src/diff_edit/scripts/result.png
+-rw-r--r--   0        0        0     6581 1970-01-01 00:00:00.000000 diffedit-0.0.2rc8/PKG-INFO
```

### Comparing `diffedit-0.0.2rc7/LICENSE` & `diffedit-0.0.2rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/README.md` & `diffedit-0.0.2rc8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # DiffEdit
 ___
+
 [![pypi wheel](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml)
-[![Python package](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml)
+[![build and test](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/build_and_test.yml)
 
 An unofficial implementation of <a href="https://arxiv.org/abs/2210.11427"> DiffEdit</a> based on <a href="https://huggingface.co"> 🤗 Hugging Face </a>, <a href="https://github.com/johnrobinsn/diffusion_experiments/blob/main/DiffEdit.ipynb"> this repo</a> and PyTorch.
 This methodology leverage the diffusion process to automatically extract a mask from an image given a prompt. The mask is then used to inpaint the image with the new content.
 To get a clearer overview of the process, you can take a look at the <a href="https://github.com/Gennaro-Farina/diffusion-nbs/blob/master/DiffEdit.ipynb"> DiffEdit.ipynb</a> notebook.
 
 ## Results
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # DiffEdit ___ [![pypi wheel](https://github.com/Gennaro-Farina/DiffEdit/
 actions/workflows/publish-wheel-pypi.yml/badge.svg)](https://github.com/
-Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml) [![Python
-package](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-
-package.yml/badge.svg?branch=main)](https://github.com/Gennaro-Farina/DiffEdit/
-actions/workflows/python-package.yml) An unofficial implementation of _D_i_f_f_E_d_i_t
+Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml) [![build and
+test](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/
+build_and_test.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/
+actions/workflows/build_and_test.yml) An unofficial implementation of _D_i_f_f_E_d_i_t
 based on _ð__¤__ _H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage
 the diffusion process to automatically extract a mask from an image given a
 prompt. The mask is then used to inpaint the image with the new content. To get
 a clearer overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b
 notebook. ## Results
 "lion" â¶   [static/           [static/               [static/
 "dog"        ai_gen_lion.jpeg]  ai_gen_lion_mask.png]  ai_gen_lion_result.png]
```

### Comparing `diffedit-0.0.2rc7/pyproject.toml` & `diffedit-0.0.2rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "DiffEdit"
 # version_pattern = "MAJOR.MINOR.PATCH"
-version = "0.0.2rc7"
+version = "0.0.2rc8"
 description = "An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file."
 authors = ["Gennaro Farina"]
 readme = "README.md"
 packages = [
     { include = "diff_edit", from = "src" },
 ]
 license = "Apache-2.0"
```

### Comparing `diffedit-0.0.2rc7/src/diff_edit/model/diff_edit_model.py` & `diffedit-0.0.2rc8/src/diff_edit/model/diff_edit_model.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/model/image_processing.py` & `diffedit-0.0.2rc8/src/diff_edit/model/image_processing.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/model/mask_generation.py` & `diffedit-0.0.2rc8/src/diff_edit/model/mask_generation.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/model/mask_inpainting.py` & `diffedit-0.0.2rc8/src/diff_edit/model/mask_inpainting.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/model/model_composer.py` & `diffedit-0.0.2rc8/src/diff_edit/model/model_composer.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/scripts/image_edit.py` & `diffedit-0.0.2rc8/src/diff_edit/scripts/image_edit.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/scripts/mask.png` & `diffedit-0.0.2rc8/src/diff_edit/scripts/mask.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/src/diff_edit/scripts/result.png` & `diffedit-0.0.2rc8/src/diff_edit/scripts/result.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc7/PKG-INFO` & `diffedit-0.0.2rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiffEdit
-Version: 0.0.2rc7
+Version: 0.0.2rc8
 Summary: An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file.
 License: Apache-2.0
 Author: Gennaro Farina
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -32,16 +32,17 @@
 Requires-Dist: tqdm
 Requires-Dist: transformers (==4.36.2)
 Requires-Dist: twine (>=4.0.0,<5) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # DiffEdit
 ___
+
 [![pypi wheel](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/publish-wheel-pypi.yml)
-[![Python package](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml)
+[![build and test](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/build_and_test.yml)
 
 An unofficial implementation of <a href="https://arxiv.org/abs/2210.11427"> DiffEdit</a> based on <a href="https://huggingface.co"> 🤗 Hugging Face </a>, <a href="https://github.com/johnrobinsn/diffusion_experiments/blob/main/DiffEdit.ipynb"> this repo</a> and PyTorch.
 This methodology leverage the diffusion process to automatically extract a mask from an image given a prompt. The mask is then used to inpaint the image with the new content.
 To get a clearer overview of the process, you can take a look at the <a href="https://github.com/Gennaro-Farina/diffusion-nbs/blob/master/DiffEdit.ipynb"> DiffEdit.ipynb</a> notebook.
 
 ## Results
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc7 Summary: An
+Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc8 Summary: An
 implementation of the DiffEdit algorithm for prompt-based mask creation and
 inpating. For more information, see the Readme file. License: Apache-2.0
 Author: Gennaro Farina Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev Provides-Extra: test Requires-Dist: accelerate (==0.26.1)
@@ -16,23 +16,23 @@
 Requires-Dist: pytest-xdist (==3.2.1) ; extra == "test" Requires-Dist: requests
 (==2.27.1) Requires-Dist: ruff (==0.0.264) ; extra == "dev" Requires-Dist:
 setuptools (>=69.1.1,<70.0.0) Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
 Requires-Dist: tqdm Requires-Dist: transformers (==4.36.2) Requires-Dist: twine
 (>=4.0.0,<5) ; extra == "dev" Description-Content-Type: text/markdown #
 DiffEdit ___ [![pypi wheel](https://github.com/Gennaro-Farina/DiffEdit/actions/
 workflows/publish-wheel-pypi.yml/badge.svg)](https://github.com/Gennaro-Farina/
-DiffEdit/actions/workflows/publish-wheel-pypi.yml) [![Python package](https://
-github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml/
-badge.svg?branch=main)](https://github.com/Gennaro-Farina/DiffEdit/actions/
-workflows/python-package.yml) An unofficial implementation of _D_i_f_f_E_d_i_t based on
-_ð__¤__ _H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage the
-diffusion process to automatically extract a mask from an image given a prompt.
-The mask is then used to inpaint the image with the new content. To get a
-clearer overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b
-notebook. ## Results
+DiffEdit/actions/workflows/publish-wheel-pypi.yml) [![build and test](https://
+github.com/Gennaro-Farina/DiffEdit/actions/workflows/build_and_test.yml/
+badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/
+build_and_test.yml) An unofficial implementation of _D_i_f_f_E_d_i_t based on _ð__¤_
+_H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage the diffusion
+process to automatically extract a mask from an image given a prompt. The mask
+is then used to inpaint the image with the new content. To get a clearer
+overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b notebook. ##
+Results
 "lion" â¶   [static/           [static/               [static/
 "dog"        ai_gen_lion.jpeg]  ai_gen_lion_mask.png]  ai_gen_lion_result.png]
 "house" â¶  [static/           [static/               [static/
 "3-floor     ai_gen_house.jpeg] ai_gen_house_mask.png] ai_gen_house_result.png]
 hotel"
 "an F1 race" [static/           [static/               [static/
 â¶ "a       ai_gen_f1.jpeg]    ai_gen_f1_mask.png]    ai_gen_f1_result.png]
```

