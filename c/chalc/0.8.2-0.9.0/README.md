# Comparing `tmp/chalc-0.8.2.tar.gz` & `tmp/chalc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalc-0.8.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "chalc-0.9.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `chalc-0.8.2.tar` & `chalc-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1135 2022-11-09 12:37:21.000000 chalc-0.8.2/.gitignore
--rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 chalc-0.8.2/.gitmodules
--rw-r--r--   0        0        0     4449 2022-11-09 12:37:21.000000 chalc-0.8.2/CMakeLists.txt
--rw-r--r--   0        0        0    35148 2022-11-09 12:37:21.000000 chalc-0.8.2/COPYING
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 chalc-0.8.2/README.md
--rwxr-xr-x   0        0        0      298 2022-11-09 12:37:21.000000 chalc-0.8.2/build_docs.sh
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 chalc-0.8.2/build_stubs.sh
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/API.rst
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/Makefile
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_static/css/custom.css
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1253 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_templates/autosummary/function.rst
--rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_templates/autosummary/method.rst
--rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     3490 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/conf.py
--rw-r--r--   0        0        0 13185814 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/example.ipynb
--rw-r--r--   0        0        0     4865 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/exts/autosummary_customise.py
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/index.rst
--rw-r--r--   0        0        0     3006 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/installation.rst
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/license.rst
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/make.bat
--rw-r--r--   0        0        0     2463 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/references.bib
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/requirements.txt
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/stubgen.py
--rw-r--r--   0        0        0     4700 2022-11-09 12:37:21.000000 chalc-0.8.2/docs/theory.rst
--rw-r--r--   0        0        0     1754 2022-11-09 12:37:21.000000 chalc-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/.git
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/.gitmodules
--rw-r--r--   0        0        0    35148 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/COPYING
--rw-r--r--   0        0        0     7651 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/COPYING.LESSER
--rw-r--r--   0        0        0    10094 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/ConstrainedMiniball.h
--rw-r--r--   0        0        0     1667 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/README.md
--rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/example.cpp
--rw-r--r--   0        0        0     6761 2022-11-09 12:37:21.000000 chalc-0.8.2/src/ConstrainedMiniball/test.cpp
--rw-r--r--   0        0        0      719 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/__init__.py
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/_utils.py
--rw-r--r--   0        0        0    21767 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/chromatic/chromatic.cxx
--rw-r--r--   0        0        0     2239 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/chromatic/chromatic.h
--rw-r--r--   0        0        0     4531 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/chromatic.pyi
--rw-r--r--   0        0        0     5170 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/chromatic_py.cxx
--rw-r--r--   0        0        0     1897 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/common.h
--rw-r--r--   0        0        0    17085 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/filtration/filtration.cxx
--rw-r--r--   0        0        0     8847 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/filtration/filtration.h
--rw-r--r--   0        0        0     7467 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/filtration.pyi
--rw-r--r--   0        0        0     8679 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/filtration_py.cxx
--rw-r--r--   0        0        0    11797 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/plotting.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/py.typed
--rw-r--r--   0        0        0    14445 2022-11-09 12:37:21.000000 chalc-0.8.2/src/chalc/sixpack.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/.git
--rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/README.md
--rw-r--r--   0        0        0    18527 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/changelog
--rw-r--r--   0        0        0    35146 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/copying.txt
--rw-r--r--   0        0        0     4852 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/example/example.cpp
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/example/makefile
--rw-r--r--   0        0        0   124054 2022-11-09 12:37:21.000000 chalc-0.8.2/src/mpreal/mpreal.h
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 chalc-0.8.2/vcpkg.json
--rw-r--r--   0        0        0    42459 2022-11-09 12:37:21.000000 chalc-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1135 2022-11-09 12:37:21.000000 chalc-0.9.0/.gitignore
+-rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 chalc-0.9.0/.gitmodules
+-rw-r--r--   0        0        0     4449 2022-11-09 12:37:21.000000 chalc-0.9.0/CMakeLists.txt
+-rw-r--r--   0        0        0    35148 2022-11-09 12:37:21.000000 chalc-0.9.0/COPYING
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 chalc-0.9.0/README.md
+-rwxr-xr-x   0        0        0      298 2022-11-09 12:37:21.000000 chalc-0.9.0/build_docs.sh
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 chalc-0.9.0/build_stubs.sh
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/API.rst
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1253 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_templates/autosummary/method.rst
+-rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0 13185814 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/example.ipynb
+-rw-r--r--   0        0        0     4865 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/exts/autosummary_customise.py
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0     3006 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/installation.rst
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/license.rst
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0     2463 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/references.bib
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/stubgen.py
+-rw-r--r--   0        0        0     4700 2022-11-09 12:37:21.000000 chalc-0.9.0/docs/theory.rst
+-rw-r--r--   0        0        0     1754 2022-11-09 12:37:21.000000 chalc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/.git
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/.gitmodules
+-rw-r--r--   0        0        0    35148 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/COPYING
+-rw-r--r--   0        0        0     7651 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/COPYING.LESSER
+-rw-r--r--   0        0        0    10094 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/ConstrainedMiniball.h
+-rw-r--r--   0        0        0     1667 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/README.md
+-rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/example.cpp
+-rw-r--r--   0        0        0     6761 2022-11-09 12:37:21.000000 chalc-0.9.0/src/ConstrainedMiniball/test.cpp
+-rw-r--r--   0        0        0      719 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/__init__.py
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/_utils.py
+-rw-r--r--   0        0        0    21767 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/chromatic/chromatic.cxx
+-rw-r--r--   0        0        0     2239 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/chromatic/chromatic.h
+-rw-r--r--   0        0        0     4577 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/chromatic.pyi
+-rw-r--r--   0        0        0     5218 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/chromatic_py.cxx
+-rw-r--r--   0        0        0     1897 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/common.h
+-rw-r--r--   0        0        0    17085 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/filtration/filtration.cxx
+-rw-r--r--   0        0        0     8847 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/filtration/filtration.h
+-rw-r--r--   0        0        0     7454 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/filtration.pyi
+-rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/filtration_py.cxx
+-rw-r--r--   0        0        0    12004 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/plotting.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/py.typed
+-rw-r--r--   0        0        0    15182 2022-11-09 12:37:21.000000 chalc-0.9.0/src/chalc/sixpack.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/.git
+-rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/README.md
+-rw-r--r--   0        0        0    18527 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/changelog
+-rw-r--r--   0        0        0    35146 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/copying.txt
+-rw-r--r--   0        0        0     4852 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/example/example.cpp
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/example/makefile
+-rw-r--r--   0        0        0   124054 2022-11-09 12:37:21.000000 chalc-0.9.0/src/mpreal/mpreal.h
+-rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 chalc-0.9.0/vcpkg.json
+-rw-r--r--   0        0        0    42459 2022-11-09 12:37:21.000000 chalc-0.9.0/PKG-INFO
```

### Comparing `chalc-0.8.2/.gitignore` & `chalc-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/CMakeLists.txt` & `chalc-0.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/COPYING` & `chalc-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/README.md` & `chalc-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/Makefile` & `chalc-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/_templates/autosummary/class.rst` & `chalc-0.9.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/_templates/autosummary/module.rst` & `chalc-0.9.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/conf.py` & `chalc-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 master_doc = "index"
 templates_path = ['_templates']
 exclude_patterns = [
     '_build', 
     '_templates', 
     'exts', 
     '_static',
-    # 'example.ipynb'
+    'example.ipynb'
 ]
 
 extensions = [
     'sphinx.ext.autosectionlabel',
     'sphinx.ext.napoleon',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
@@ -65,15 +65,14 @@
 
 # autosectionlabel options
 autosectionlabel_prefix_document = True
 
 # napoleon options
 napolean_include_init_with_doc = True
 napoleon_attr_annotations = True
-napolean_use_keyword = True
 
 # autodoc options
 autodoc_default_options = {
     'special-members': '',
     'undoc-members': False,
     'private-members': False,
     'imported-members': False,
```

### Comparing `chalc-0.8.2/docs/example.ipynb` & `chalc-0.9.0/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/exts/autosummary_customise.py` & `chalc-0.9.0/docs/exts/autosummary_customise.py`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/index.rst` & `chalc-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/installation.rst` & `chalc-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/license.rst` & `chalc-0.9.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/make.bat` & `chalc-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/references.bib` & `chalc-0.9.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/docs/theory.rst` & `chalc-0.9.0/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/pyproject.toml` & `chalc-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "scikit-build-core>=0.6.0",
     "pybind11==2.11",
 ]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "chalc"
-version = "0.8.2"
+version = "0.9.0"
 authors = [
     {name = "Abhinav Natarajan", email = "natarajan@maths.ox.ac.uk"},
 ]
 description = "Persistent homology of chromatic alpha complexes"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 license = {file = "COPYING"}
```

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/COPYING` & `chalc-0.9.0/src/ConstrainedMiniball/COPYING`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/COPYING.LESSER` & `chalc-0.9.0/src/ConstrainedMiniball/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/ConstrainedMiniball.h` & `chalc-0.9.0/src/ConstrainedMiniball/ConstrainedMiniball.h`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/README.md` & `chalc-0.9.0/src/ConstrainedMiniball/README.md`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/example.cpp` & `chalc-0.9.0/src/ConstrainedMiniball/example.cpp`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/ConstrainedMiniball/test.cpp` & `chalc-0.9.0/src/ConstrainedMiniball/test.cpp`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/__init__.py` & `chalc-0.9.0/src/chalc/__init__.py`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/_utils.py` & `chalc-0.9.0/src/chalc/_utils.py`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/chromatic/chromatic.cxx` & `chalc-0.9.0/src/chalc/chromatic/chromatic.cxx`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/chromatic/chromatic.h` & `chalc-0.9.0/src/chalc/chromatic/chromatic.h`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/chromatic.pyi` & `chalc-0.9.0/src/chalc/chromatic.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 Returns:
                     The chromatic alpha complex and a boolean flag to indicate if numerical issues were encountered. In case of numerical issues, a warning is also raised.
     
                 Raises:
                     ValueError: If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
     
                 See Also:
-                    delrips, delcech
+                    :func:`delrips`, :func:`delcech`
     """
 def delaunay(x: typing.Annotated[numpy.ndarray, numpy.float64, pybind11_stubgen.typing_ext.DynamicSize('m', 'n')]) -> chalc.filtration.FilteredComplex:
     """
                 Returns the Delaunay triangulation of a point cloud in Euclidean space.
     
                 Args:
                     x : Numpy matrix whose columns are points in the point cloud.
@@ -53,15 +53,15 @@
                 Raises:
                     ValueError : If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
     
                 Notes:
                     The chromatic Delaunay-Cech complex of the point cloud has the same set of simplices as the chromatic alpha complex, but with Cech filtration times.
     
                 See Also:
-                    alpha, delrips
+                    :func:`alpha`, :func:`delrips`
     """
 def delrips(x: typing.Annotated[numpy.ndarray, numpy.float64, pybind11_stubgen.typing_ext.DynamicSize('m', 'n')], colours: list[int]) -> tuple[chalc.filtration.FilteredComplex, bool]:
     """
                 Computes the chromatic Delaunay-Rips complex of a coloured point cloud.
     
                 Args:
                     x : Numpy matrix whose columns are points in the point cloud.
@@ -70,13 +70,13 @@
                 Returns:
                     The chromatic Delaunay-Rips complex and a boolean flag to indicate if numerical issues were encountered. In case of numerical issues, a warning is also raised.
     
                 Raises:
                     ValueError: If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
     
                 Notes:
-                    The chromatic Delaunay-Rips complex of the point cloud has the same set of simplices as the chromatic alpha complex, but with Vietoris-Rips filtration times. The convention used is that the filtration time of a simplex is half the maximum edge length in that simplex. With this convention, the chromatic Delaunay-Rips complex and chromatic alpha complex have a visually similar persistence diagrams.
+                    The chromatic Delaunay-Rips complex of the point cloud has the same set of simplices as the chromatic alpha complex, but with Vietoris-Rips filtration times. The convention used is that the filtration time of a simplex is half the maximum edge length in that simplex. With this convention, the chromatic Delaunay-Rips complex and chromatic alpha complex have visually similar persistence diagrams.
     
                 See Also:
-                    alpha, delcech
+                    :func:`alpha`, :func:`delcech`
     """
 MaxColoursChromatic: int = 64
```

### Comparing `chalc-0.8.2/src/chalc/chromatic_py.cxx` & `chalc-0.9.0/src/chalc/chromatic_py.cxx`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             Raises:
                 ValueError: If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
 
             Notes:
                 The chromatic Delaunay-Rips complex of the point cloud has the same set of simplices as the chromatic alpha complex, but with Vietoris-Rips filtration times. The convention used is that the filtration time of a simplex is half the maximum edge length in that simplex. With this convention, the chromatic Delaunay-Rips complex and chromatic alpha complex have visually similar persistence diagrams.
 
             See Also:
-                alpha, delcech
+                :func:`alpha`, :func:`delcech`
         )docstring",
         py::arg("x"), py::arg("colours"))
     .def("alpha",
         [log_warn](const Eigen::MatrixXd& points, const vector<index_t>& colours) {
             std::ostringstream ostream;
             auto res = alpha(points, colours, ostream);
             bool issues = false;
@@ -75,15 +75,15 @@
             Returns:
                 The chromatic alpha complex and a boolean flag to indicate if numerical issues were encountered. In case of numerical issues, a warning is also raised.
 
             Raises:
                 ValueError: If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
 
             See Also:
-                delrips, delcech
+                :func:`delrips`, :func:`delcech`
         )docstring",
         py::arg("x"), py::arg("colours"))
     .def("delcech",
         [log_warn](const Eigen::MatrixXd& points, const vector<index_t>& colours) {
             std::ostringstream ostream;
             auto res = delcech(points, colours, ostream);
             bool issues = false;
@@ -106,11 +106,11 @@
             Raises:
                 ValueError : If any value in ``colours`` is >= :attr:`MaxColoursChromatic <chalc.chromatic.MaxColoursChromatic>` or < 0, or if the length of ``colours`` does not match the number of points.
 
             Notes:
                 The chromatic Delaunay-Cech complex of the point cloud has the same set of simplices as the chromatic alpha complex, but with Cech filtration times.
 
             See Also:
-                alpha, delrips
+                :func:`alpha`, :func:`delrips`
         )docstring",
         py::arg("x"), py::arg("colours"));
 }
```

### Comparing `chalc-0.8.2/src/chalc/common.h` & `chalc-0.9.0/src/chalc/common.h`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/filtration/filtration.cxx` & `chalc-0.9.0/src/chalc/filtration/filtration.cxx`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/filtration/filtration.h` & `chalc-0.9.0/src/chalc/filtration/filtration.h`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/chalc/filtration.pyi` & `chalc-0.9.0/src/chalc/filtration.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     def __repr__(self) -> str:
         ...
     def add_simplex(self, vertices: list[int], filt_value: float) -> bool:
         """
         				Add a simplex to a filtered simplicial complex.
         
         				Args:
-        					vertices : List of vertex labels corresponding to existing vertices
-        					in the complex.
+        					vertices : List of vertex labels corresponding to existing vertices in the complex.
         					filt_value : Filtration value to associate to the new simplex.
         
         				Note:
         					Faces of the added simplex that are already present in the simplicial complex will have their filtration values reduced if necessary.
         """
     def get_label_from_vertex_labels(self, vertices: list[int]) -> int:
         """
```

### Comparing `chalc-0.8.2/src/chalc/filtration_py.cxx` & `chalc-0.9.0/src/chalc/filtration_py.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 	filtered_complex.def(py::init<const index_t, const index_t>(),
 		py::arg("n"), py::arg("k"))
 		.def("add_simplex", &FilteredComplex::add_simplex,
 			R"docstring(
 				Add a simplex to a filtered simplicial complex.
 
 				Args:
-					vertices : List of vertex labels corresponding to existing vertices
-					in the complex.
+					vertices : List of vertex labels corresponding to existing vertices in the complex.
 					filt_value : Filtration value to associate to the new simplex.
 
 				Note:
 					Faces of the added simplex that are already present in the simplicial complex will have their filtration values reduced if necessary.
 			)docstring",
 			py::arg("vertices"), py::arg("filt_value"))
 		.def_property_readonly("num_simplices",
```

### Comparing `chalc-0.8.2/src/chalc/plotting.py` & `chalc-0.9.0/src/chalc/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-from __future__ import annotations
-
-from matplotlib.figure import Figure
-from matplotlib.axes import Axes
-import matplotlib.pyplot as plt
-import matplotlib.animation as animation
-import numpy as np
-from itertools import product
-from typing import Annotated
-from pandas import DataFrame
-import seaborn as sns
-from .sixpack import DiagramEnsemble, _num_colours_in_bitmask, _bitmask_to_colours, _colours_are_subset, _colours_to_bitmask
-from chalc.filtration import FilteredComplex # absolute import because of a bug in scikit-build-core v0.6.0
-from ._utils import interpolate_docstring
+from   __future__           import annotations
+from   collections.abc      import Collection, Sequence
+from   itertools            import product
+from   typing               import Annotated
+
+import matplotlib.animation as     animation
+from   matplotlib.axes      import Axes
+from   matplotlib.figure    import Figure
+import matplotlib.pyplot    as     plt
+import numpy                as     np
+from   pandas               import DataFrame
+import seaborn              as     sns
+
+from   chalc.filtration     import FilteredComplex
+
+from   ._utils              import interpolate_docstring
+from   .sixpack             import (
+	DiagramEnsemble,
+	_bitmask_to_colours,
+	_colours_are_subset,
+	_colours_to_bitmask,
+	_num_colours_in_bitmask,
+)
 
 plt.rcParams["animation.html"] = "jshtml"
 
 __doc__ = 'Plotting and visualisation utilities.'
 
 def plot_sixpack(
 	dgms                  : DiagramEnsemble,
-	*,
 	truncation            : float | None = None,
 	max_diagram_dimension : int   | None = None,
 	tolerance             : float        = 0,
 	) -> tuple[Figure, Annotated[np.ndarray, "Axes"]] :
 
 	"""
 	Plots the 6-pack of persistence diagrams returned by :func:`compute <.sixpack.compute>`.
 
 	Args:
-		dgms : The 6-pack of persistence diagrams.
-
-	Keyword Args:
-		truncation : The maximum entrance time upto which features are plotted. A sensible default will be calculated if not provided.
+		dgms                  : The 6-pack of persistence diagrams.
+		truncation            : The maximum entrance time upto which features are plotted. A sensible default will be calculated if not provided.
 		max_diagram_dimension : The maximum homological dimension for which to plot features. If not provided, all dimensions will be included in the plots.
-		tolerance: Only features with persistence greater than this value will be plotted.
+		tolerance             : Only features with persistence greater than this value will be plotted.
 	"""
 	if max_diagram_dimension is None:
 		max_diagram_dimension = max(dgms.dimensions)
 	dim_shift = { name : (1 if name == 'ker' else 0) for name in DiagramEnsemble.diagram_names }
 	max_dim = { name : (max_diagram_dimension if name != 'rel' else max_diagram_dimension + 1) for name in DiagramEnsemble.diagram_names }
 	plot_pos = { name : (val[1], val[0]) for name, val in zip(DiagramEnsemble.diagram_names, product((0, 1, 2), (0, 1))) }
 	plot_titles = {
@@ -83,32 +89,29 @@
 	fig.legend(handles=legends.values(), loc = 'upper center', bbox_to_anchor = (0.5, 0.05), ncol = 5)
 	return fig, axes
 
 @interpolate_docstring()
 def plot_diagram(
 	dgms                  : DiagramEnsemble,
 	diagram_name          : str,
-	*,
 	truncation            : float | None = None,
 	max_diagram_dimension : int   | None = None,
 	ax                    : Axes  | None = None,
 	tolerance             : float        = 0
-	) -> tuple[Figure, Axes] :
+	) -> Axes :
 	"""
 	Plot a specific diagram from a 6-pack.
 
 	Args:
-		dgms : The 6-pack of persistence diagrams.
-		diagram_name : One of ``${str(DiagramEnsemble.diagram_names)}``.
-
-	Keyword Args:
-		truncation : The maximum entrance time for which the diagrams are plotted. A sensible default will be calculated if not provided.
+		dgms                  : The 6-pack of persistence diagrams.
+		diagram_name          : One of ``${str(DiagramEnsemble.diagram_names)}``.
+		truncation            : The maximum entrance time for which the diagrams are plotted. A sensible default will be calculated if not provided.
 		max_diagram_dimension : The maximum homological dimension for which to plot points. If not provided, all dimensions will be included in the plots.
-		ax : A matplotlib axes object. If provided then the diagram will be plotted on the given axes.
-		tolerance: Only features with persistence greater than this value will be plotted.
+		ax                    : A matplotlib axes object. If provided then the diagram will be plotted on the given axes.
+		tolerance             : Only features with persistence greater than this value will be plotted.
 	"""
 	if not diagram_name in DiagramEnsemble.diagram_names:
 		raise KeyError("Invalid diagram name!")
 	titles = {
 		'ker': 'Kernel',
 		'cok': 'Cokernel',
 		'im' : 'Image',
@@ -120,31 +123,29 @@
 		max_diagram_dimension = max(dgms.dimensions)
 	if truncation is None:
 		et = [dgms.entrance_times[d]
 			for _, d in getattr(dgms, diagram_name).paired
 			if dgms.dimensions[d] <= max_diagram_dimension]
 		truncation = _get_truncation(et)
 	if ax is None:
-		fig, ax = plt.subplots()
-	else:
-		fig = ax.get_figure()
+		_, ax = plt.subplots()
 	_plot_diagram(
 		getattr(dgms, diagram_name),
 		dgms.entrance_times,
 		dgms.dimensions,
 		truncation,
 		ax            = ax,
 		dim_shift     = 1 if diagram_name == 'ker' else 0,
 		points_legend = True,
 		lines_legend  = True,
 		title         = titles[diagram_name],
 		max_dim       = max_diagram_dimension,
 		tolerance     = tolerance
 	)
-	return fig, ax
+	return ax
 
 def _plot_diagram(
 	diagram,
 	entrance_times,
 	dimensions,
 	truncation,
 	max_dim       = 2,
@@ -206,33 +207,30 @@
 	if lines_legend:
 		handle.legend()
 
 def draw_filtration(
 	K               : FilteredComplex,
 	points          : Annotated[np.ndarray, np.float64],
 	time            : float,
-	*,
-	include_colours : list[int] | None = None
+	include_colours : Collection[int] | None = None
 	) -> tuple[Figure, Axes] :
 	"""
 	Visualise a filtration at given time, optionally including only certain colours.
 
 	Args:
-		K : A filtered complex.
-		points : The vertices of ``K`` as a :math:`2\\times N` numpy matrix.
-		time : Filtration times for which to draw simplices.
-
-	Keyword Args:
-		include_colours : Optional list of colours to include. If not specified then all colours will be drawn.
+		K               : A filtered complex.
+		points          : The vertices of ``K`` as a :math:`2\\times N` numpy matrix.
+		time            : Filtration times for which to draw simplices.
+		include_colours : Optional collection of colours to include. If not specified then all colours will be drawn.
 	"""
 	if len(points.shape) != 2:
 		raise NotImplementedError
 
 	if include_colours is None:
-		include_colours = list(set([_bitmask_to_colours(vertex.colours)[0] for vertex in K.simplices[0].values()]))
+		include_colours = set([_bitmask_to_colours(vertex.colours)[0] for vertex in K.simplices[0].values()])
 
 	include_colours_bitmask = _colours_to_bitmask(include_colours)
 
 	fig : Figure
 	ax : Axes
 	fig, ax = plt.subplots()
 	plot_colours = np.array(plt.rcParams['axes.prop_cycle'].by_key()['color'])
@@ -271,26 +269,24 @@
 	# ax.set_xlabel('Time = ' + f"{0.0:.4f}")
 
 	return fig, ax
 
 def animate_filtration(
 	K                : FilteredComplex,
 	points           : Annotated[np.ndarray, np.float64],
-	*,
-	filtration_times : list[float],
-	animation_length : float) -> animation.FuncAnimation :
+	filtration_times : Sequence[float],
+	animation_length : float
+	) -> animation.FuncAnimation :
 	"""
 	Create animation of 2-skeleton of filtered simplicial complex.
 
-	Args :
-		K : A filtered complex.
-		points : The vertices of ``K`` as a :math:`2\\times N` numpy matrix.
-
-	Keyword Args:
-		filtration_times : List of filtration times for which to draw animation frames.
+	Args:
+		K                : A filtered complex.
+		points           : The vertices of ``K`` as a :math:`2\\times N` numpy matrix.
+		filtration_times : Sequence of filtration times for which to draw animation frames.
 		animation_length : Total length of the animation in seconds.
 	"""
 	if len(points.shape) != 2:
 		raise NotImplementedError
 
 	fig : Figure
 	ax : Axes
```

### Comparing `chalc-0.8.2/src/chalc/sixpack.py` & `chalc-0.9.0/src/chalc/sixpack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from __future__ import annotations
+from   __future__       import annotations
+from   collections.abc  import Collection, Sequence
+from   dataclasses      import dataclass,  field,    fields
+from   typing           import Annotated,  Callable, ClassVar, overload
+
+from   h5py             import Dataset,    Group
+import numpy            as     np
+from   phimaker         import compute_ensemble
 
-__doc__ = "Routines for computing 6-packs of persistence diagrams."
+from   chalc.chromatic  import alpha,      delcech,  delrips
+from   chalc.filtration import FilteredComplex
 
-from chalc.chromatic import alpha, delcech, delrips # absolute import because of a bug in scikit-build-core v0.6.0
-from chalc.filtration import FilteredComplex # absolute import because of a bug in scikit-build-core v0.6.0
-from ._utils import interpolate_docstring
-import numpy as np
-from typing import Optional, Callable, ClassVar, overload, Annotated
-from phimaker import compute_ensemble
-from dataclasses import dataclass, field, fields
-from h5py import Group, Dataset
+from   ._utils          import interpolate_docstring
 
+__doc__ = "Routines for computing 6-packs of persistence diagrams."
 __all__ = ["from_filtration", "compute", "SimplexPairings", "DiagramEnsemble", "save_diagrams", "load_diagrams"]
 
 ChromaticMethod = {
 	"chromatic alpha"   : alpha,
 	"chromatic delcech" : delcech,
 	"chromatic delrips" : delrips
 }
 
 BdMatType = list[tuple[bool, int, list[int]]]
 
 # bitmask that represents a list of colours
-def _colours_to_bitmask(colours : list[int]) -> int :
+def _colours_to_bitmask(colours : Collection[int]) -> int :
 	return sum(2**i for i in colours)
 
 # list of colours represented by a bitmask
 def _bitmask_to_colours(b : int) -> list[int] :
 	i = 0
 	res = []
 	while (b) :
@@ -47,17 +49,17 @@
 def _get_diagrams(
 	K               : FilteredComplex,
 	check_in_domain : Callable[[int], bool],
 	max_dgm_dim     : int,
 	tolerance       : float = 0,
 	) -> DiagramEnsemble :
 	# Build up the matrix
-	matrix:         BdMatType   = []
-	entrance_times: list[float] = []
-	dimensions:     list[int]   = []
+	matrix         : BdMatType   = []
+	entrance_times : list[float] = []
+	dimensions     : list[int]   = []
 	for column in K.serialised():
 		facet_idxs = column[0]
 		dimension = max(0, len(facet_idxs) - 1)
 		# Only need k-skeleton for k <= max_dgm_dim + 1
 		if dimension > max_dgm_dim + 1: break
 		dimensions.append(dimension)
 		entrance_times.append(column[2])
@@ -73,34 +75,32 @@
 		entrance_times,
 		dimensions)
 	return dgms.threshold(tolerance)
 
 @interpolate_docstring()
 def from_filtration(
 	K                     : FilteredComplex,
-	*,
-	dom                   : list[int] | None = None,
-	k                     : int | None       = None,
-	max_diagram_dimension : int              = 2,
-	tolerance             : float            = 0
+	dom                   : Collection[int] | int | None = None,
+	k                     : int | None                   = None,
+	max_diagram_dimension : int                          = 2,
+	tolerance             : float                        = 0
 	) -> DiagramEnsemble :
 	"""
 	Compute the 6-pack of persistence diagrams filtered simplicial complex with coloured vertices.
 
 	Given a filtered chromatic simplicial complex :math:`K` and a subcomplex :math:`L` of :math:`K`, this function computes the 6-pack of persistence diagram associated with the inclusion map :math:`f : L \\hookrightarrow K`. The subcomplex is specified by
 	the colours of its vertices, or by an integer :math:`k` wherein all simplices with :math:`k` or fewer colours are considered part of the subcomplex.
 
 	Args:
-		K : A filtered chromatic simplicial complex.
+		K                     : A filtered chromatic simplicial complex.
 
-	Keyword Args:
-		dom : List of integers describing the colours of the points in the domain (the subcomplex :math:`L`).
-		k : If not ``None``, then the domain is taken to be the :math:`k`-chromatic subcomplex of :math:`K`, i.e., the subcomplex of simplices having at most :math:`k` colours.
+		dom                   : Integer or collection of integers describing the colours of the points in the domain (the subcomplex :math:`L`).
+		k                     : If not ``None``, then the domain is taken to be the :math:`k`-chromatic subcomplex of :math:`K`, i.e., the subcomplex of simplices having at most :math:`k` colours.
 		max_diagram_dimension : Maximum homological dimension for which the persistence diagrams are computed.
-		tolerance : Retain only points with persistence strictly greater than this value.
+		tolerance             : Retain only points with persistence strictly greater than this value.
 
 	Returns:
 		Diagrams corresponding to the following persistence modules (where :math:`H_*` is the persistent homology functor and :math:`f_*` is the induced map on persistent homology):
 
 		#. :math:`H_*(L)` (domain)
 		#. :math:`H_*(K)` (codomain)
 		#. :math:`\\ker(f_*)` (kernel)
@@ -109,52 +109,52 @@
 		#. :math:`H_*(K, L)` (relative homology)
 
 		Each diagram is represented by sets of paired and unpaired simplices,
 		and contain simplices of all dimensions. ``dgms`` also contains the
 		entrance times of the simplices and their dimensions.
 	"""
 	if dom is not None and k is None:
+		if isinstance(dom, int): dom = [dom,]
 		colours_bitmask = _colours_to_bitmask(dom)
 		check_in_domain = lambda b : _colours_are_subset(b, colours_bitmask)
 	elif k is not None and dom is None:
 		check_in_domain = lambda b: _num_colours_in_bitmask(b) <= k # k-chromatic simplex
+	elif k is None and dom is None:
+		raise RuntimeError("At least one of k or dom must be provided")
 	else:
 		raise RuntimeError("Only one of k or dom is allowed")
 	# if(K, L) is a pair of simplicial complexes where dim(L) <= dim(K) = d
 	# then all of the sixpack diagrams except for the relative homology
 	# can be non-zero upt dimension d, and relative can be nontrivial upto dim = d+1
 	max_diagram_dimension = min(max_diagram_dimension, K.dimension + 1)
 	return _get_diagrams(K, check_in_domain, max_diagram_dimension, tolerance)
 
 @interpolate_docstring()
 def compute(
 	x                     : Annotated[np.ndarray, np.float64],
-	colours               : list[int],
-	*, # rest are keyword only
-	dom                   : Optional[list[int]] = None,
-	k                     : Optional[int]       = None,
-	method                : str                 = "chromatic alpha",
-	max_diagram_dimension : int                 = 2,
-	tolerance             : float               = 0
+	colours               : Sequence[int],
+	dom                   : Collection[int] | int | None = None,
+	k                     : int | None                   = None,
+	method                : str                          = "chromatic alpha",
+	max_diagram_dimension : int                          = 2,
+	tolerance             : float                        = 0
 	) -> DiagramEnsemble :
 	"""
 	Compute the 6-pack of persistence diagrams of a coloured point-cloud.
 
 	This function constructs a filtered chromatic simplicial complex :math:`K` from the point cloud, and computes the 6-pack of persistence diagrams associated with the inclusion :math:`f : L \\hookrightarrow K` where :math:`L` is some filtered subcomplex of :math:`K`.
 
 	Args:
-		x : Numpy matrix whose columns are points.
-		colours : List of integers describing the colours of the points.
-
-	Keyword Args:
-		dom : List of integers describing the colours of the points in the domain (the subcomplex :math:`L`).
-		k : If not ``None``, then the domain is taken to be the :math:`k`-chromatic subcomplex of :math:`K`, i.e., the subcomplex of simplices having at most :math:`k` colours.
-		method: Filtration used to construct the chromatic complex. Must be one of ``${str(list(ChromaticMethod.keys()))}``.
+		x                     : Numpy matrix whose columns are points.
+		colours               : Sequence of integers describing the colours of the points.
+		dom                   : Integer or collection of integers describing the colours of the points in the domain (the subcomplex :math:`L`).
+		k                     : If not ``None``, then the domain is taken to be the :math:`k`-chromatic subcomplex of :math:`K`, i.e., the subcomplex of simplices having at most :math:`k` colours.
+		method                : Filtration used to construct the chromatic complex. Must be one of ``${str(list(ChromaticMethod.keys()))}``.
 		max_diagram_dimension : Maximum homological dimension for which the persistence diagrams are computed.
-		tolerance : Retain only points with persistence strictly greater than this value.
+		tolerance             : Retain only points with persistence strictly greater than this value.
 
 	Returns :
 		Diagrams corresponding to the following persistence modules (where :math:`H_*` is the persistent homology functor and :math:`f_*` is the induced map on persistent homology):
 
 		#. :math:`H_*(L)` (domain)
 		#. :math:`H_*(K)` (codomain)
 		#. :math:`\\ker(f_*)` (kernel)
@@ -164,19 +164,22 @@
 
 		Each diagram is represented by lists of paired and unpaired simplices,
 		and contains simplices of all dimensions. ``dgms`` also contains the
 		entrance times of the simplices and their dimensions.
 	"""
 	if dom is not None and k is None:
 		# new colours: 1 -> domain, 0 -> codomain
-		new_colours = list(np.isin(colours, dom).astype(np.int64))
+		if isinstance(dom, int): dom = [dom,]
+		new_colours = list(np.isin(colours, list(dom)).astype(np.int64))
 		check_in_domain = lambda b : b == 2
 	elif k is not None and dom is None:
 		check_in_domain = lambda b: _num_colours_in_bitmask(b) <= k # k-chromatic simplex
-		new_colours = colours
+		new_colours = list(colours)
+	elif k is None and dom is None:
+		raise RuntimeError("At least one of k or dom must be provided")
 	else:
 		raise RuntimeError("Only one of k or dom is allowed")
 	# can have non-zero homology upto dimension d for everything except rel
 	# rel can have non-zero homology in dimension d+1
 	max_diagram_dimension = min(max_diagram_dimension, x.shape[0])
 	# Compute chromatic complex
 	if method in ChromaticMethod.keys():
@@ -188,30 +191,30 @@
 @dataclass
 class SimplexPairings:
 	"""
 	Persistence diagram object, represented by a
 	list of simplex pairings and a list of unpaired simplices.
 	"""
 	#: Set of tuples of indices of paired simplices.
-	paired: list[tuple[int, int]] = field(default_factory=list)
+	paired   : list[tuple[int, int]] = field(default_factory=list)
 	#: Set of indices of unpaired simplices.
-	unpaired: list[int] = field(default_factory=list)
+	unpaired : list[int] = field(default_factory=list)
 
 	@classmethod
 	def _fromPhimaker(cls, obj) -> SimplexPairings :
 		return cls(list(obj.paired), list(obj.unpaired))
 
 	def __str__(self):
 		return f"Paired: {self.paired}\nUnpaired: {self.unpaired}"
 
 	@classmethod
 	def _from_matrices(cls, p : Annotated[np.ndarray, np.int64], u : Annotated[np.ndarray, np.int64]) -> SimplexPairings :
 		if p.shape[1] != 2:
 			raise ValueError(f"p must be a (m, 2) matrix, but received a matrix of size {p.shape}")
-		paired : list[tuple[int, int]] = [tuple(p[i, :]) for i in range(p.shape[0])]
+		paired : list[tuple[int, int]] = [(p[i, 0], p[i, 1]) for i in range(p.shape[0])]
 		unpaired = list(u)
 		return cls(paired, unpaired)
 
 	def paired_as_matrix(self) -> Annotated[np.ndarray, np.int64] :
 		return np.concatenate(list(self.paired)).reshape((-1, 2))
 
 	def __eq__(self, other) -> bool :
@@ -222,31 +225,31 @@
 
 @dataclass
 class DiagramEnsemble:
 	"""
 	6-pack of persistence diagrams.
 	"""
 	# List of matrices
-	diagram_names : ClassVar[list[str]] = ['ker', 'cok', 'dom', 'cod', 'im', 'rel']
+	diagram_names  : ClassVar[tuple[str,...]] = ('ker', 'cok', 'dom', 'cod', 'im', 'rel')
 	#: Kernel
-	ker: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	ker            : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Cokernel
-	cok: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	cok            : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Domain
-	dom: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	dom            : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Codomain
-	cod: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	cod            : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Image
-	im: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	im             : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Relative
-	rel: SimplexPairings = field(default_factory = lambda : SimplexPairings())
+	rel            : SimplexPairings          = field(default_factory = lambda : SimplexPairings())
 	#: Entrance times of the simplices
-	entrance_times : list[float] = field(default_factory = lambda : [])
+	entrance_times : list[float]              = field(default_factory = lambda : [])
 	#: Dimensions of the simplices
-	dimensions: list[int] = field(default_factory = lambda : [])
+	dimensions     : list[int]                = field(default_factory = lambda : [])
 
 	def __eq__(self, other) -> bool :
 		if isinstance(other, DiagramEnsemble):
 			return all(getattr(self, f.name) == getattr(other, f.name) for f in fields(DiagramEnsemble))
 		else:
 			return NotImplemented
 
@@ -268,15 +271,15 @@
 	@interpolate_docstring({'diagram_names' : diagram_names})
 	def get(self, diagram_name, dim = None):
 		"""
 		Get a specific diagram as a matrix of birth and death times.
 
 		Args:
 			diagram_name : One of ``${str(diagram_names)}``.
-			dim : Dimension(s) of the diagram desired. If a list is provided then a list of matrices is returned, with the order of matrices respecting the order of entries of `dim`. If `dim` is not provided then the returned matrix will contain persistent features from all homological dimensions from zero to ``max(self.dimensions)``.
+			dim          : Dimension(s) of the diagram desired. If a list is provided then a list of matrices is returned, with the order of matrices respecting the order of entries of `dim`. If `dim` is not provided then the returned matrix will contain persistent features from all homological dimensions from zero to ``max(self.dimensions)``.
 
 		Returns:
 			An :math:`m \\times 2` matrix whose rows are a pair of birth and death times, or a list of such matrices.
 		"""
 		if dim is None:
 			dim = list(range(max(set(self.dimensions))))
 		if isinstance(dim, int):
```

### Comparing `chalc-0.8.2/src/mpreal/README.md` & `chalc-0.9.0/src/mpreal/README.md`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/mpreal/changelog` & `chalc-0.9.0/src/mpreal/changelog`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/mpreal/copying.txt` & `chalc-0.9.0/src/mpreal/copying.txt`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/mpreal/example/example.cpp` & `chalc-0.9.0/src/mpreal/example/example.cpp`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/src/mpreal/mpreal.h` & `chalc-0.9.0/src/mpreal/mpreal.h`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/vcpkg.json` & `chalc-0.9.0/vcpkg.json`

 * *Files identical despite different names*

### Comparing `chalc-0.8.2/PKG-INFO` & `chalc-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalc
-Version: 0.8.2
+Version: 0.9.0
 Summary: Persistent homology of chromatic alpha complexes
 Keywords: topological data analysis TDA chromatic alpha complex persistent homology
 Author-Email: Abhinav Natarajan <natarajan@maths.ox.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

