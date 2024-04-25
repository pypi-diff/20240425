# Comparing `tmp/xspex-0.0.2.tar.gz` & `tmp/xspex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspex-0.0.2.tar", last modified: Thu Apr 18 18:22:19 2024, max compression
+gzip compressed data, was "xspex-0.0.3.tar", last modified: Thu Apr 25 14:47:04 2024, max compression
```

## Comparing `xspex-0.0.2.tar` & `xspex-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794935 xspex-0.0.2/
--rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.2/LICENSE
--rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.2/MANIFEST.in
--rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-18 18:22:19.794843 xspex-0.0.2/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      887 2024-04-18 18:21:14.000000 xspex-0.0.2/README.md
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.791562 xspex-0.0.2/helpers/
--rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/identify_xspec.py
--rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/report_xspec_version.cxx
--rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/template.py
--rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.2/pyproject.toml
--rw-r--r--   0 xuewc      (501) staff       (20)      787 2024-04-18 18:22:19.795273 xspex-0.0.2/setup.cfg
--rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-04-18 18:14:35.000000 xspex-0.0.2/setup.py
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.791753 xspex-0.0.2/src/
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.792003 xspex-0.0.2/src/include/
--rw-r--r--   0 xuewc      (501) staff       (20)    23356 2024-04-18 18:17:18.000000 xspex-0.0.2/src/include/xspex.hpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.792617 xspex-0.0.2/src/xspex/
--rw-r--r--   0 xuewc      (501) staff       (20)   338104 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     9303 2024-04-18 18:10:33.000000 xspex-0.0.2/src/xspex/primitive.py
--rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794549 xspex-0.0.2/src/xspex.egg-info/
--rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      523 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/SOURCES.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/dependency_links.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-17 17:48:09.000000 xspex-0.0.2/src/xspex.egg-info/not-zip-safe
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/requires.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/top_level.txt
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.793949 xspex-0.0.2/template/
--rw-r--r--   0 xuewc      (501) staff       (20)     4726 2024-04-17 10:50:41.000000 xspex-0.0.2/template/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.2/template/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794313 xspex-0.0.2/tests/
--rw-r--r--   0 xuewc      (501) staff       (20)     6286 2024-04-18 18:10:32.000000 xspex-0.0.2/tests/test_basic.py
--rw-r--r--   0 xuewc      (501) staff       (20)     7261 2024-04-18 18:10:32.000000 xspex-0.0.2/tests/test_primitive.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.941582 xspex-0.0.3/
+-rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.3/LICENSE
+-rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.3/MANIFEST.in
+-rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-25 14:47:04.941247 xspex-0.0.3/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)      887 2024-04-18 18:21:14.000000 xspex-0.0.3/README.md
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.935204 xspex-0.0.3/helpers/
+-rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/identify_xspec.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/report_xspec_version.cxx
+-rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/template.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.3/pyproject.toml
+-rw-r--r--   0 xuewc      (501) staff       (20)      787 2024-04-25 14:47:04.942344 xspex-0.0.3/setup.cfg
+-rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-04-25 14:45:58.000000 xspex-0.0.3/setup.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.935555 xspex-0.0.3/src/
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.936088 xspex-0.0.3/src/include/
+-rw-r--r--   0 xuewc      (501) staff       (20)    27131 2024-04-23 20:12:30.000000 xspex-0.0.3/src/include/xspex.hpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.936621 xspex-0.0.3/src/xspex/
+-rw-r--r--   0 xuewc      (501) staff       (20)   338104 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)    10035 2024-04-23 19:41:04.000000 xspex-0.0.3/src/xspex/primitive.py
+-rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.940551 xspex-0.0.3/src/xspex.egg-info/
+-rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)      523 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/SOURCES.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/dependency_links.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/not-zip-safe
+-rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/requires.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/top_level.txt
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.939348 xspex-0.0.3/template/
+-rw-r--r--   0 xuewc      (501) staff       (20)     4726 2024-04-17 10:50:41.000000 xspex-0.0.3/template/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.3/template/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.940024 xspex-0.0.3/tests/
+-rw-r--r--   0 xuewc      (501) staff       (20)     6286 2024-04-18 18:10:32.000000 xspex-0.0.3/tests/test_basic.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7538 2024-04-25 14:41:30.000000 xspex-0.0.3/tests/test_primitive.py
```

### Comparing `xspex-0.0.2/LICENSE` & `xspex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/PKG-INFO` & `xspex-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access Xspec models and corresponding JAX/XLA ops.
 Home-page: https://github.com/wcxve/xspex
 Author: Wang-Chen Xue
 Author-email: wcxuemail@gmail.com
 License: GNU GPL v3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `xspex-0.0.2/README.md` & `xspex-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/helpers/identify_xspec.py` & `xspex-0.0.3/helpers/identify_xspec.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/helpers/template.py` & `xspex-0.0.3/helpers/template.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/setup.cfg` & `xspex-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/setup.py` & `xspex-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
 sys.path.append(os.path.dirname(__file__))
 from helpers import template
 from helpers.identify_xspec import get_xspec_macros
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 # Check HEASARC is set up. The following does not provide a useful
 # message from 'pip install' so how do we make it more meaningful?
 #
 HEADAS = os.getenv('HEADAS')
 if HEADAS is None:
     sys.stderr.write('ERROR: unable to find HEADAS environment variable.\n')
```

### Comparing `xspex-0.0.2/src/include/xspex.hpp` & `xspex-0.0.3/src/include/xspex.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -558,61 +558,106 @@
     template <xsccCall model, int NumPars>
     void wrapper_con_C_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         float *mptr = reinterpret_cast<float *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const int batch = *reinterpret_cast<int *>(in[5]);
-        const string initStr = "";  //*reinterpret_cast<string *>(in[6]);
+        const int pbatch = *reinterpret_cast<int *>(in[5]);
+        const int mbatch = *reinterpret_cast<int *>(in[6]);
+        const string initStr = "";  //*reinterpret_cast<string *>(in[7]);
         float *optr = reinterpret_cast<float *>(out);
 
-        auto pars_ = std::vector<double>(NumPars);
+        int batch = std::max(1, std::max(pbatch, mbatch));
+        auto params_ = std::vector<double>(NumPars * batch);
+        auto model_ = std::vector<double>(nelem * batch);
+        double *pptr_ = params_.data();
+        double *mptr_ = model_.data();
+
+        if (pbatch >= 1 && mbatch == 1) {
+            float_to_double(pptr, pptr_, NumPars * batch);
+            for (int i = 0; i < batch; ++i) {
+                float_to_double(mptr, mptr_ + i * nelem, nelem);
+            }
+        } else if (pbatch == 1 && mbatch > 1) {
+            float_to_double(mptr, mptr_, nelem * batch);
+            for (int i = 0; i < batch; ++i) {
+                float_to_double(pptr, pptr_ + i * NumPars, NumPars);
+            }
+        } else {
+            if (pbatch > 1 && mbatch > 1 && pbatch == mbatch) {
+                float_to_double(pptr, pptr_, NumPars * batch);
+                float_to_double(mptr, mptr_, nelem * batch);
+            } else {
+                throw std::invalid_argument("Invalid batch sizes");
+            }
+        }
+
         auto energyArray_ = std::vector<double>(nelem + 1);
-        auto model_ = std::vector<double>(nelem);
         auto errors_ = std::vector<double>(nelem);
-        auto out_ = std::vector<double>(nelem);
 
-        double *pptr_ = pars_.data();
         double *eptr_ = energyArray_.data();
-        double *mptr_ = model_.data();
-        double *optr_ = out_.data();
         float_to_double(eptr, eptr_, nelem + 1);
-        float_to_double(mptr, mptr_, nelem + 1);
 
         for (int i = 0; i < batch; ++i) {
-            float *pptr_i = pptr + i * NumPars;
             float *optr_i = optr + i * nelem;
-            std::copy(mptr_, mptr_ + nelem, optr_);
-            float_to_double(pptr_i, pptr_, NumPars);
+            double *pptr_i = pptr_ + i * NumPars;
+            double *mptr_i = mptr_ + i * nelem;
             model(
-                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                eptr_, nelem, pptr_i, spectrumNumber, mptr_i,
                 errors_.data(), initStr.c_str()
             );
-            double_to_float(optr_, optr_i, nelem);
+            double_to_float(mptr_i, optr_i, nelem);
         }
     }
 
     template <xsccCall model, int NumPars>
     void wrapper_con_C_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         double *mptr = reinterpret_cast<double *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const int batch = *reinterpret_cast<int *>(in[5]);
-        const string initStr = "";  //*reinterpret_cast<string *>(in[6]);
+        const int pbatch = *reinterpret_cast<int *>(in[5]);
+        const int mbatch = *reinterpret_cast<int *>(in[6]);
+        const string initStr = "";  //*reinterpret_cast<string *>(in[7]);
         double *optr = reinterpret_cast<double *>(out);
 
+        int batch = std::max(1, std::max(pbatch, mbatch));
+        auto params_ = std::vector<double>(NumPars * batch);
+        auto model_ = std::vector<double>(nelem * batch);
+        double *pptr_ = params_.data();
+        double *mptr_ = model_.data();
+
+        if (pbatch >= 1 && mbatch == 1) {
+            std::copy(pptr, pptr + NumPars * batch, pptr_);
+            for (int i = 0; i < batch; ++i) {
+                std::copy(mptr, mptr + nelem, mptr_ + i * nelem);
+            }
+        } else if (pbatch == 1 && mbatch > 1) {
+            std::copy(mptr, mptr + nelem * batch, mptr_);
+            for (int i = 0; i < batch; ++i) {
+                std::copy(pptr, pptr + NumPars, pptr_ + i * NumPars);
+            }
+        } else {
+            if (pbatch > 1 && mbatch > 1 && pbatch == mbatch) {
+                std::copy(pptr, pptr + NumPars * batch, pptr_);
+                std::copy(mptr, mptr + nelem * batch, mptr_);
+            } else {
+                throw std::invalid_argument("Invalid batch sizes");
+            }
+        }
+
         auto errors_ = std::vector<double>(nelem);
 
         for (int i = 0; i < batch; ++i) {
-            double *pptr_i = pptr + i * NumPars;
+            double *pptr_i = pptr_ + i * NumPars;
+            double *mptr_i = mptr_ + i * nelem;
             double *optr_i = optr + i * nelem;
-            std::copy(mptr, mptr + nelem, optr_i);
+            std::copy(mptr_i, mptr_i + nelem, optr_i);
             model(
                 eptr, nelem, pptr_i, spectrumNumber, optr_i,
                 errors_.data(), initStr.c_str()
             );
         }
     }
 
@@ -620,60 +665,105 @@
     template <xsf77Call model, int NumPars>
     void wrapper_con_f_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         float *mptr = reinterpret_cast<float *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const int batch = *reinterpret_cast<int *>(in[5]);
+        const int pbatch = *reinterpret_cast<int *>(in[5]);
+        const int mbatch = *reinterpret_cast<int *>(in[6]);
         float *optr = reinterpret_cast<float *>(out);
 
+        int batch = std::max(1, std::max(pbatch, mbatch));
+        auto params_ = std::vector<float>(NumPars * batch);
+        auto model_ = std::vector<float>(nelem * batch);
+        float *pptr_ = params_.data();
+        float *mptr_ = model_.data();
+
+        if (pbatch >= 1 && mbatch == 1) {
+            std::copy(pptr, pptr + NumPars * batch, pptr_);
+            for (int i = 0; i < batch; ++i) {
+                std::copy(mptr, mptr + nelem, mptr_ + i * nelem);
+            }
+        } else if (pbatch == 1 && mbatch > 1) {
+            std::copy(mptr, mptr + nelem * batch, mptr_);
+            for (int i = 0; i < batch; ++i) {
+                std::copy(pptr, pptr + NumPars, pptr_ + i * NumPars);
+            }
+        } else {
+            if (pbatch > 1 && mbatch > 1 && pbatch == mbatch) {
+                std::copy(pptr, pptr + NumPars * batch, pptr_);
+                std::copy(mptr, mptr + nelem * batch, mptr_);
+            } else {
+                throw std::invalid_argument("Invalid batch sizes");
+            }
+        }
+
         auto errors_ = std::vector<float>(nelem);
 
         for (int i = 0; i < batch; ++i) {
             float *pptr_i = pptr + i * NumPars;
+            float *mptr_i = mptr_ + i * nelem;
             float *optr_i = optr + i * nelem;
-            std::copy(mptr, mptr + nelem, optr_i);
+            std::copy(mptr_i, mptr_i + nelem, optr_i);
             model(eptr, nelem, pptr_i, spectrumNumber, optr_i, errors_.data());
         }
     }
 
     template <xsf77Call model, int NumPars>
     void wrapper_con_f_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         double *mptr = reinterpret_cast<double *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const int batch = *reinterpret_cast<int *>(in[5]);
+        const int pbatch = *reinterpret_cast<int *>(in[5]);
+        const int mbatch = *reinterpret_cast<int *>(in[6]);
         double *optr = reinterpret_cast<double *>(out);
 
-        auto pars_ = std::vector<float>(NumPars);
+        int batch = std::max(1, std::max(pbatch, mbatch));
+        auto params_ = std::vector<float>(NumPars * batch);
+        auto model_ = std::vector<float>(nelem * batch);
+        float *pptr_ = params_.data();
+        float *mptr_ = model_.data();
+
+        if (pbatch >= 1 && mbatch == 1) {
+            double_to_float(pptr, pptr_, NumPars * batch);
+            for (int i = 0; i < batch; ++i) {
+                double_to_float(mptr, mptr_ + i * nelem, nelem);
+            }
+        } else if (pbatch == 1 && mbatch > 1) {
+            double_to_float(mptr, mptr_, nelem * batch);
+            for (int i = 0; i < batch; ++i) {
+                double_to_float(pptr, pptr_ + i * NumPars, NumPars);
+            }
+        } else {
+            if (pbatch > 1 && mbatch > 1 && pbatch == mbatch) {
+                double_to_float(pptr, pptr_, NumPars * batch);
+                double_to_float(mptr, mptr_, nelem * batch);
+            } else {
+                throw std::invalid_argument("Invalid batch sizes");
+            }
+        }
+
         auto energyArray_ = std::vector<float>(nelem + 1);
-        auto model_ = std::vector<float>(nelem);
         auto errors_ = std::vector<float>(nelem);
-        auto out_ = std::vector<float>(nelem);
 
-        float *pptr_ = pars_.data();
         float *eptr_ = energyArray_.data();
-        float *mptr_ = model_.data();
-        float *optr_ = out_.data();
         double_to_float(eptr, eptr_, nelem + 1);
-        double_to_float(mptr, mptr_, nelem + 1);
 
         for (int i = 0; i < batch; ++i) {
-            double *pptr_i = pptr + i * NumPars;
             double *optr_i = optr + i * nelem;
-            std::copy(mptr_, mptr_ + nelem, optr_);
-            double_to_float(pptr_i, pptr_, NumPars);
+            float *pptr_i = pptr_ + i * NumPars;
+            float *mptr_i = mptr_ + i * nelem;
             model(
-                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                eptr_, nelem, pptr_i, spectrumNumber, mptr_i,
                 errors_.data()
             );
-            float_to_double(optr_, optr_i, nelem);
+            float_to_double(mptr_i, optr_i, nelem);
         }
     }
 
 
     template <typename T>
     py::capsule EncapsulateFunction(T *fn) {
         return py::capsule((void *)fn, "xla._CUSTOM_CALL_TARGET");
```

### Comparing `xspex-0.0.2/src/xspex/__init__.py` & `xspex-0.0.3/src/xspex/__init__.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/src/xspex/primitive.py` & `xspex-0.0.3/src/xspex/primitive.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,18 @@
 
     def get_abstract_eval(self):
         name = self.name
         npar = self._nparam
 
         def abstract_eval(params, egrid, spec_num):
             params_shape = jnp.shape(params)
-            if params_shape[-1] != npar:
+            if params_shape == () or params_shape[-1] != npar:
                 raise ValueError(f'{name} params shape must be (..., {npar})')
             egrid_shape = jnp.shape(egrid)
-            if len(egrid_shape) > 1:
+            if len(egrid_shape) != 1:
                 raise ValueError('egrid must be 1D array')
             spec_num_shape = jnp.shape(spec_num)
             if len(spec_num_shape):
                 raise ValueError('spec_num must be a integer')
 
             shape = params_shape[:-1] + (egrid_shape[-1] - 1,)
             dtype = jax.dtypes.canonicalize_dtype(egrid.dtype)
@@ -94,20 +94,20 @@
         elif isinstance(etype, mlir.ir.F64Type):
             call_target_name = f'{self._model_name}_f64'
         else:
             raise NotImplementedError(f'unsupported dtype {etype}')
         out_shape = ctx.avals_out[0].shape
         out_type = mlir.ir.RankedTensorType.get(out_shape, etype)
         out_n = mlir.ir_constant(out_shape[-1])
-        batch_n = mlir.ir_constant(prod(out_shape[:-1]))
+        out_batch = mlir.ir_constant(prod(out_shape[:-1]))
         return custom_call(
             call_target_name,
             result_types=[out_type],
-            operands=[params, egrid, spec_num, out_n, batch_n],
-            operand_layouts=avals_to_layouts(ctx.avals_in) + [(), ()],
+            operands=[params, egrid, spec_num, out_n, out_batch],
+            operand_layouts=avals_to_layouts(ctx.avals_in) + [()] * 2,
             result_layouts=avals_to_layouts(ctx.avals_out)
         ).results
 
     def batching(self, vector_arg_values, batch_axes):
         if batch_axes[1] is not None:
             raise NotImplementedError('egrid batching is not implemented')
         if batch_axes[2] is not None:
@@ -157,63 +157,81 @@
 
     def get_abstract_eval(self):
         name = self.name
         npar = self._nparam
 
         def abstract_eval(params, egrid, flux, spec_num):
             params_shape = jnp.shape(params)
-            if params_shape[-1] != npar:
+            if params_shape == () or params_shape[-1] != npar:
                 raise ValueError(f'{name} params shape must be (..., {npar})')
             egrid_shape = jnp.shape(egrid)
-            if len(egrid_shape) > 1:
+            if len(egrid_shape) != 1:
                 raise ValueError('egrid must be 1D array')
             flux_shape = jnp.shape(flux)
-            if len(flux_shape) > 1:
-                raise ValueError('flux must be 1D array')
+            if flux_shape == () or flux_shape[-1] != egrid_shape[-1] - 1:
+                raise ValueError('flux shape must be (..., len(egrid) - 1)')
             spec_num_shape = jnp.shape(spec_num)
             if len(spec_num_shape):
                 raise ValueError('spec_num must be a integer')
 
-            shape = params_shape[:-1] + (egrid_shape[-1] - 1,)
+            if len(params_shape) > 1 and len(flux_shape) > 1:
+                if params_shape[:-1] != flux_shape[:-1]:
+                    raise ValueError(
+                        'params and flux should have the same batch size'
+                    )
+            if len(params_shape) >= len(flux_shape):
+                shape = params_shape[:-1] + (egrid_shape[-1] - 1,)
+            else:
+                shape = flux_shape[:-1] + (egrid_shape[-1] - 1,)
             dtype = jax.dtypes.canonicalize_dtype(egrid.dtype)
             return ShapedArray(shape=shape, dtype=dtype)
 
         return abstract_eval
 
     def lowering(self, ctx, params, egrid, flux, spec_num):
         egrid_type = mlir.ir.RankedTensorType(egrid.type)
         etype = egrid_type.element_type
         if isinstance(etype, mlir.ir.F32Type):
             call_target_name = f'{self._model_name}_f32'
         elif isinstance(etype, mlir.ir.F64Type):
             call_target_name = f'{self._model_name}_f64'
         else:
             raise NotImplementedError(f'unsupported dtype {etype}')
+
+        params_shape = ctx.avals_in[0].shape
+        params_batch = mlir.ir_constant(prod(params_shape[:-1]))
+
+        flux_shape = ctx.avals_in[2].shape
+        flux_batch = mlir.ir_constant(prod(flux_shape[:-1]))
+
         out_shape = ctx.avals_out[0].shape
         out_type = mlir.ir.RankedTensorType.get(out_shape, etype)
         out_n = mlir.ir_constant(out_shape[-1])
-        batch_n = mlir.ir_constant(prod(out_shape[:-1]))
+
         return custom_call(
             call_target_name,
             result_types=[out_type],
-            operands=[params, egrid, flux, spec_num, out_n, batch_n],
-            operand_layouts=avals_to_layouts(ctx.avals_in) + [(), ()],
+            operands=[
+                params, egrid, flux, spec_num, out_n, params_batch, flux_batch
+            ],
+            operand_layouts=avals_to_layouts(ctx.avals_in) + [()] * 3,
             result_layouts=avals_to_layouts(ctx.avals_out)
         ).results
 
     def batching(self, vector_arg_values, batch_axes):
         if batch_axes[1] is not None:
             raise NotImplementedError('egrid batching is not implemented')
-        if batch_axes[2] is not None:
-            raise NotImplementedError('flux batching is not implemented')
         if batch_axes[3] is not None:
             raise NotImplementedError('spec_num batching is not implemented')
 
         params, egrid, flux, spec_num = vector_arg_values
-        params = jnp.moveaxis(params, batch_axes[0], 0)
+        if batch_axes[0] is not None:
+            params = jnp.moveaxis(params, batch_axes[0], 0)
+        if batch_axes[2] is not None:
+            flux = jnp.moveaxis(flux, batch_axes[2], 0)
         return self(params, egrid, flux, spec_num), 0
 
 
 def get_primitive(
     model: str
 ) -> tuple[XspecPrimitive | XspecConvPrimitive, xspex.XspecModel]:
     """Return the primitive for the given Xspec model.
```

### Comparing `xspex-0.0.2/src/xspex.cpp` & `xspex-0.0.3/src/xspex.cpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/src/xspex.egg-info/PKG-INFO` & `xspex-0.0.3/src/xspex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspex
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access Xspec models and corresponding JAX/XLA ops.
 Home-page: https://github.com/wcxve/xspex
 Author: Wang-Chen Xue
 Author-email: wcxuemail@gmail.com
 License: GNU GPL v3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `xspex-0.0.2/src/xspex.egg-info/SOURCES.txt` & `xspex-0.0.3/src/xspex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/template/__init__.py` & `xspex-0.0.3/template/__init__.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/template/xspex.cpp` & `xspex-0.0.3/template/xspex.cpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/tests/test_basic.py` & `xspex-0.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.2/tests/test_primitive.py` & `xspex-0.0.3/tests/test_primitive.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,19 +204,24 @@
     mfunc = getattr(x, model)
 
     n = 5
     pars = np.column_stack([np.full(n, conv(p)) for p in info.parameters])
     y1 = np.array([mfunc(energies=egrid, pars=p, model=mvals) for p in pars])
     y2 = jax.vmap(p, in_axes=(0, None, None, None), out_axes=0)(pars, egrid, mvals, 1)
     y3 = jax.jit(jax.vmap(p, in_axes=(0, None, None, None), out_axes=0))(pars, egrid, mvals, 1)
+    mvals_n = np.tile(mvals, (n, 1))
+    y4 = jax.vmap(p, in_axes=(None, None, 0, None), out_axes=0)(pars[0], egrid, mvals_n, 1)
+    y5 = jax.vmap(p, in_axes=(0, None, 0, None), out_axes=0)(pars, egrid, mvals_n, 1)
 
     assert (y1 > 0).any()
     assert np.any(y1 != ymodel)
     assert np.allclose(y1, y2)
     assert np.allclose(y1, y3)
+    assert np.allclose(y1, y4)
+    assert np.allclose(y1, y5)
 
 
 # @pytest.mark.parametrize("model", MODELS_ADD + MODELS_MUL)
 # def test_jvp(model):
 #     p, info = x.get_primitive(model)
 #     if not info.can_cache:
 #         pytest.skip(f"Model {model} can not be cached.")
```

