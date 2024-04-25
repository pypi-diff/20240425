# Comparing `tmp/diffedit-0.0.2rc6.tar.gz` & `tmp/diffedit-0.0.2rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffedit-0.0.2rc6.tar", max compression
+gzip compressed data, was "diffedit-0.0.2rc7.tar", max compression
```

## Comparing `diffedit-0.0.2rc6.tar` & `diffedit-0.0.2rc7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:54:24.248503 diffedit-0.0.2rc6/LICENSE
--rw-r--r--   0        0        0     5073 2024-04-24 19:54:24.248503 diffedit-0.0.2rc6/README.md
--rw-r--r--   0        0        0     5088 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/__init__.py
--rw-r--r--   0        0        0       57 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/constants.py
--rw-r--r--   0        0        0    10994 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/diff_edit_model.py
--rw-r--r--   0        0        0     2243 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/image_processing.py
--rw-r--r--   0        0        0     8789 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/mask_generation.py
--rw-r--r--   0        0        0      852 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/mask_inpainting.py
--rw-r--r--   0        0        0     3833 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/model/model_composer.py
--rw-r--r--   0        0        0     7551 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/scripts/image_edit.py
--rw-r--r--   0        0        0   434756 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/scripts/mask.png
--rw-r--r--   0        0        0   491401 2024-04-24 19:54:24.252503 diffedit-0.0.2rc6/src/diff_edit/scripts/result.png
--rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 diffedit-0.0.2rc6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/LICENSE
+-rw-r--r--   0        0        0     5073 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/README.md
+-rw-r--r--   0        0        0     4983 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/constants.py
+-rw-r--r--   0        0        0    10994 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/diff_edit_model.py
+-rw-r--r--   0        0        0     2243 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/image_processing.py
+-rw-r--r--   0        0        0     8789 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/mask_generation.py
+-rw-r--r--   0        0        0      852 2024-04-25 09:43:48.705318 diffedit-0.0.2rc7/src/diff_edit/model/mask_inpainting.py
+-rw-r--r--   0        0        0     3833 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/model/model_composer.py
+-rw-r--r--   0        0        0     7551 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/image_edit.py
+-rw-r--r--   0        0        0   434756 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/mask.png
+-rw-r--r--   0        0        0   491401 2024-04-25 09:43:48.709318 diffedit-0.0.2rc7/src/diff_edit/scripts/result.png
+-rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 diffedit-0.0.2rc7/PKG-INFO
```

### Comparing `diffedit-0.0.2rc6/LICENSE` & `diffedit-0.0.2rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/README.md` & `diffedit-0.0.2rc7/README.md`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/pyproject.toml` & `diffedit-0.0.2rc7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 [tool.poetry]
 name = "DiffEdit"
 # version_pattern = "MAJOR.MINOR.PATCH"
-version = "0.0.2rc6"
+version = "0.0.2rc7"
 description = "An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file."
 authors = ["Gennaro Farina"]
 readme = "README.md"
 packages = [
     { include = "diff_edit", from = "src" },
 ]
 license = "Apache-2.0"
 
 [project.scripts] # creates command-line scripts that call functions within your package.
 diff_edit = "diff_edit.scripts.image_edit:main"
 
 [tool.poetry.dependencies]
 python="^3.10"
-torch = "2.0.1"
+torch = ">=2.0.0, !=2.0.1, !=2.1.0"
 numpy = "1.26.2"
 tqdm = "*"
 transformers = "4.36.2"
 requests = "2.27.1"
 fastai = "2.7.13"
 opencv_python = "^4.9"
 diffusers = ">=0.25"
 accelerate = "0.26.1"
-
-
-# dev dependencies
 black = { version = "23.3.0", optional = true, extras = ["jupyter"] }
 ruff = { version = "0.0.264", optional = true }
 pre-commit = { version = "3.3.1", optional = true }
 docformatter = { version = "1.5.1", optional = true }
 docstr-coverage = { version = "2.2.0", optional = true }
 twine = { version = ">=4.0.0,<5", optional = true }
-
-# test dependencies
 pytest = { version = "7.3.1", optional = true }
 pytest-cov = { version = "4.0.0", optional = true }
-# beautify pytest output
 pytest-sugar = { version = "0.9.7", optional = true }
-# parallel test execution
 pytest-xdist = { version = "3.2.1", optional = true }
 setuptools = "^69.1.1"
 
 
 [tool.poetry.extras]
 dev = [
   "black",
@@ -172,23 +165,20 @@
 log_file_format = "%(asctime)s | %(levelname)-8s | %(module)-20s | %(funcName)-20s | %(thread)-8d ; %(message)s"
 log_file_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.mypy]
 python_version = "3.10"
 files = ["./src/**/*.py", "./tests/**/*.py"]
 exclude = [
-  'venv',
-  '.venv',
   'env',
   '.env',
   'docs',
   'bin',
   'lib',
   '.cicd',
-  "tests",
 ]
 # enables PEP 420 style namespace packages.
 namespace_packages = true
 # follows all imports normally and type checks all top level code
 # (as well as the bodies of all functions and methods with at least one type annotation in the signature).
 follow_imports = "normal"
 # raises an error whene imports cannot be resolved
```

### Comparing `diffedit-0.0.2rc6/src/diff_edit/model/diff_edit_model.py` & `diffedit-0.0.2rc7/src/diff_edit/model/diff_edit_model.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/model/image_processing.py` & `diffedit-0.0.2rc7/src/diff_edit/model/image_processing.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/model/mask_generation.py` & `diffedit-0.0.2rc7/src/diff_edit/model/mask_generation.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/model/mask_inpainting.py` & `diffedit-0.0.2rc7/src/diff_edit/model/mask_inpainting.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/model/model_composer.py` & `diffedit-0.0.2rc7/src/diff_edit/model/model_composer.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/scripts/image_edit.py` & `diffedit-0.0.2rc7/src/diff_edit/scripts/image_edit.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/scripts/mask.png` & `diffedit-0.0.2rc7/src/diff_edit/scripts/mask.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/src/diff_edit/scripts/result.png` & `diffedit-0.0.2rc7/src/diff_edit/scripts/result.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc6/PKG-INFO` & `diffedit-0.0.2rc7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiffEdit
-Version: 0.0.2rc6
+Version: 0.0.2rc7
 Summary: An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file.
 License: Apache-2.0
 Author: Gennaro Farina
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +24,15 @@
 Requires-Dist: pytest (==7.3.1) ; extra == "test"
 Requires-Dist: pytest-cov (==4.0.0) ; extra == "test"
 Requires-Dist: pytest-sugar (==0.9.7) ; extra == "test"
 Requires-Dist: pytest-xdist (==3.2.1) ; extra == "test"
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: ruff (==0.0.264) ; extra == "dev"
 Requires-Dist: setuptools (>=69.1.1,<70.0.0)
-Requires-Dist: torch (==2.0.1)
+Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
 Requires-Dist: tqdm
 Requires-Dist: transformers (==4.36.2)
 Requires-Dist: twine (>=4.0.0,<5) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # DiffEdit
 ___
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc6 Summary: An
+Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc7 Summary: An
 implementation of the DiffEdit algorithm for prompt-based mask creation and
 inpating. For more information, see the Readme file. License: Apache-2.0
 Author: Gennaro Farina Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev Provides-Extra: test Requires-Dist: accelerate (==0.26.1)
@@ -11,21 +11,21 @@
 Requires-Dist: docstr-coverage (==2.2.0) ; extra == "dev" Requires-Dist: fastai
 (==2.7.13) Requires-Dist: numpy (==1.26.2) Requires-Dist: opencv_python
 (>=4.9,<5.0) Requires-Dist: pre-commit (==3.3.1) ; extra == "dev" Requires-
 Dist: pytest (==7.3.1) ; extra == "test" Requires-Dist: pytest-cov (==4.0.0) ;
 extra == "test" Requires-Dist: pytest-sugar (==0.9.7) ; extra == "test"
 Requires-Dist: pytest-xdist (==3.2.1) ; extra == "test" Requires-Dist: requests
 (==2.27.1) Requires-Dist: ruff (==0.0.264) ; extra == "dev" Requires-Dist:
-setuptools (>=69.1.1,<70.0.0) Requires-Dist: torch (==2.0.1) Requires-Dist:
-tqdm Requires-Dist: transformers (==4.36.2) Requires-Dist: twine (>=4.0.0,<5) ;
-extra == "dev" Description-Content-Type: text/markdown # DiffEdit ___ [![pypi
-wheel](https://github.com/Gennaro-Farina/DiffEdit/actions/workflows/publish-
-wheel-pypi.yml/badge.svg)](https://github.com/Gennaro-Farina/DiffEdit/actions/
-workflows/publish-wheel-pypi.yml) [![Python package](https://github.com/
-Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml/
+setuptools (>=69.1.1,<70.0.0) Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
+Requires-Dist: tqdm Requires-Dist: transformers (==4.36.2) Requires-Dist: twine
+(>=4.0.0,<5) ; extra == "dev" Description-Content-Type: text/markdown #
+DiffEdit ___ [![pypi wheel](https://github.com/Gennaro-Farina/DiffEdit/actions/
+workflows/publish-wheel-pypi.yml/badge.svg)](https://github.com/Gennaro-Farina/
+DiffEdit/actions/workflows/publish-wheel-pypi.yml) [![Python package](https://
+github.com/Gennaro-Farina/DiffEdit/actions/workflows/python-package.yml/
 badge.svg?branch=main)](https://github.com/Gennaro-Farina/DiffEdit/actions/
 workflows/python-package.yml) An unofficial implementation of _D_i_f_f_E_d_i_t based on
 _ð__¤__ _H_u_g_g_i_n_g_ _F_a_c_e_ , _t_h_i_s_ _r_e_p_o and PyTorch. This methodology leverage the
 diffusion process to automatically extract a mask from an image given a prompt.
 The mask is then used to inpaint the image with the new content. To get a
 clearer overview of the process, you can take a look at the _D_i_f_f_E_d_i_t_._i_p_y_n_b
 notebook. ## Results
```

