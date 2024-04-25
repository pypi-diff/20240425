# Comparing `tmp/celmech-1.4.0.tar.gz` & `tmp/celmech-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celmech-1.4.0.tar", last modified: Thu Feb  1 18:36:00 2024, max compression
+gzip compressed data, was "celmech-1.5.0.tar", last modified: Thu Apr 25 20:17:09 2024, max compression
```

## Comparing `celmech-1.4.0.tar` & `celmech-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-02-01 18:36:00.000000 celmech-1.4.0/
--rw-r--r--   0 shadden    (501) staff       (20)      815 2024-02-01 18:36:00.000000 celmech-1.4.0/PKG-INFO
--rw-r--r--   0 shadden    (501) staff       (20)    35149 2022-12-05 17:40:33.000000 celmech-1.4.0/LICENSE
-drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-02-01 18:36:00.000000 celmech-1.4.0/celmech/
--rw-r--r--   0 shadden    (501) staff       (20)    42720 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/poincare.py
--rw-r--r--   0 shadden    (501) staff       (20)    39109 2023-12-06 21:43:51.000000 celmech-1.4.0/celmech/maps.py
--rw-r--r--   0 shadden    (501) staff       (20)     8846 2022-05-19 20:35:02.000000 celmech-1.4.0/celmech/poisson_series.py
--rw-r--r--   0 shadden    (501) staff       (20)    15090 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/nbody_simulation_utilities.py
--rw-r--r--   0 shadden    (501) staff       (20)    17227 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/poisson_series_manipulate.py
--rw-r--r--   0 shadden    (501) staff       (20)    17808 2023-12-07 14:32:29.000000 celmech-1.4.0/celmech/planar_poincare.py
--rw-r--r--   0 shadden    (501) staff       (20)     3112 2020-09-08 19:07:09.000000 celmech-1.4.0/celmech/transformations.py
--rw-r--r--   0 shadden    (501) staff       (20)     5049 2020-01-28 16:42:51.000000 celmech-1.4.0/celmech/resonances.py
--rw-r--r--   0 shadden    (501) staff       (20)    48667 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/disturbing_function.py
--rw-r--r--   0 shadden    (501) staff       (20)     1676 2022-05-19 20:35:01.000000 celmech-1.4.0/celmech/__init__.py
--rw-r--r--   0 shadden    (501) staff       (20)    49321 2023-09-20 01:56:26.000000 celmech-1.4.0/celmech/secular.py
--rw-r--r--   0 shadden    (501) staff       (20)    57514 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/numerical_resonance_models.py
--rw-r--r--   0 shadden    (501) staff       (20)     1525 2017-08-31 19:32:04.000000 celmech-1.4.0/celmech/multiplanet_hamiltonian.py
--rw-r--r--   0 shadden    (501) staff       (20)    24979 2023-12-07 14:32:29.000000 celmech-1.4.0/celmech/miscellaneous.py
--rw-r--r--   0 shadden    (501) staff       (20)     3546 2024-02-01 18:31:53.000000 celmech-1.4.0/celmech/numerical_resonance_utils.py
--rw-r--r--   0 shadden    (501) staff       (20)    35161 2022-08-04 20:26:07.000000 celmech-1.4.0/celmech/canonical_transformations.py
--rw-r--r--   0 shadden    (501) staff       (20)     9401 2021-01-25 16:27:34.000000 celmech-1.4.0/celmech/rk_integrator.py
--rw-r--r--   0 shadden    (501) staff       (20)    20433 2023-09-20 01:56:26.000000 celmech-1.4.0/celmech/lie_transformations.py
--rw-r--r--   0 shadden    (501) staff       (20)    26888 2021-01-22 18:31:13.000000 celmech-1.4.0/celmech/symplectic_evolution_operators.py
--rw-r--r--   0 shadden    (501) staff       (20)    20332 2023-02-01 14:49:11.000000 celmech-1.4.0/celmech/hamiltonian.py
--rw-r--r--   0 shadden    (501) staff       (20)       87 2022-12-05 17:40:33.000000 celmech-1.4.0/MANIFEST.in
--rw-r--r--   0 shadden    (501) staff       (20)      665 2022-12-05 17:40:33.000000 celmech-1.4.0/README.md
--rw-r--r--   0 shadden    (501) staff       (20)     3308 2024-02-01 18:35:28.000000 celmech-1.4.0/setup.py
--rw-r--r--   0 shadden    (501) staff       (20)       38 2024-02-01 18:36:00.000000 celmech-1.4.0/setup.cfg
-drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-02-01 18:36:00.000000 celmech-1.4.0/src/
--rw-r--r--   0 shadden    (501) staff       (20)     4286 2024-02-01 18:35:28.000000 celmech-1.4.0/src/disturbing_function.c
--rw-r--r--   0 shadden    (501) staff       (20)     2494 2020-08-14 20:13:36.000000 celmech-1.4.0/src/nrutil.c
--rw-r--r--   0 shadden    (501) staff       (20)    10205 2024-02-01 18:31:53.000000 celmech-1.4.0/src/poisson_series.h
--rw-r--r--   0 shadden    (501) staff       (20)    15192 2021-02-09 14:23:17.000000 celmech-1.4.0/src/moid_v4_fun.f
--rw-r--r--   0 shadden    (501) staff       (20)      971 2022-05-19 20:01:57.000000 celmech-1.4.0/src/fmftPy.c
--rw-r--r--   0 shadden    (501) staff       (20)      494 2020-08-14 20:13:36.000000 celmech-1.4.0/src/nrutil.h
--rw-r--r--   0 shadden    (501) staff       (20)     1135 2020-07-10 17:45:01.000000 celmech-1.4.0/src/test.c
--rw-r--r--   0 shadden    (501) staff       (20)    18820 2020-08-14 20:13:36.000000 celmech-1.4.0/src/fmft.c
--rw-r--r--   0 shadden    (501) staff       (20)      483 2024-02-01 18:31:53.000000 celmech-1.4.0/src/poincare.c
--rw-r--r--   0 shadden    (501) staff       (20)     9536 2021-01-22 18:31:13.000000 celmech-1.4.0/src/poisson_series.c
-drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-02-01 18:36:00.000000 celmech-1.4.0/celmech.egg-info/
--rw-r--r--   0 shadden    (501) staff       (20)      815 2024-02-01 18:35:59.000000 celmech-1.4.0/celmech.egg-info/PKG-INFO
--rw-r--r--   0 shadden    (501) staff       (20)        1 2017-08-31 19:32:30.000000 celmech-1.4.0/celmech.egg-info/not-zip-safe
--rw-r--r--   0 shadden    (501) staff       (20)      960 2024-02-01 18:35:59.000000 celmech-1.4.0/celmech.egg-info/SOURCES.txt
--rw-r--r--   0 shadden    (501) staff       (20)      117 2024-02-01 18:35:59.000000 celmech-1.4.0/celmech.egg-info/requires.txt
--rw-r--r--   0 shadden    (501) staff       (20)       19 2024-02-01 18:35:59.000000 celmech-1.4.0/celmech.egg-info/top_level.txt
--rw-r--r--   0 shadden    (501) staff       (20)        1 2024-02-01 18:35:59.000000 celmech-1.4.0/celmech.egg-info/dependency_links.txt
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-04-25 20:17:09.686634 celmech-1.5.0/
+-rw-r--r--   0 shadden    (501) staff       (20)    35149 2022-12-05 17:40:33.000000 celmech-1.5.0/LICENSE
+-rw-r--r--   0 shadden    (501) staff       (20)       87 2022-12-05 17:40:33.000000 celmech-1.5.0/MANIFEST.in
+-rw-r--r--   0 shadden    (501) staff       (20)     1024 2024-04-25 20:17:09.685875 celmech-1.5.0/PKG-INFO
+-rw-r--r--   0 shadden    (501) staff       (20)      665 2022-12-05 17:40:33.000000 celmech-1.5.0/README.md
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-04-25 20:17:09.667032 celmech-1.5.0/celmech/
+-rw-r--r--   0 shadden    (501) staff       (20)     1676 2022-05-19 20:35:01.000000 celmech-1.5.0/celmech/__init__.py
+-rw-r--r--   0 shadden    (501) staff       (20)     8782 2024-04-02 19:46:49.000000 celmech-1.5.0/celmech/c_poisson_series.py
+-rw-r--r--   0 shadden    (501) staff       (20)    35161 2024-04-09 20:25:48.000000 celmech-1.5.0/celmech/canonical_transformations.py
+-rw-r--r--   0 shadden    (501) staff       (20)    48667 2024-02-01 18:31:53.000000 celmech-1.5.0/celmech/disturbing_function.py
+-rw-r--r--   0 shadden    (501) staff       (20)    20332 2023-02-01 14:49:11.000000 celmech-1.5.0/celmech/hamiltonian.py
+-rw-r--r--   0 shadden    (501) staff       (20)    20433 2023-09-20 01:56:26.000000 celmech-1.5.0/celmech/lie_transformations.py
+-rw-r--r--   0 shadden    (501) staff       (20)    39109 2023-12-06 21:43:51.000000 celmech-1.5.0/celmech/maps.py
+-rw-r--r--   0 shadden    (501) staff       (20)    26937 2024-04-03 15:47:40.000000 celmech-1.5.0/celmech/miscellaneous.py
+-rw-r--r--   0 shadden    (501) staff       (20)     1525 2017-08-31 19:32:04.000000 celmech-1.5.0/celmech/multiplanet_hamiltonian.py
+-rw-r--r--   0 shadden    (501) staff       (20)    15090 2024-02-01 18:31:53.000000 celmech-1.5.0/celmech/nbody_simulation_utilities.py
+-rw-r--r--   0 shadden    (501) staff       (20)    57514 2024-02-01 19:52:44.000000 celmech-1.5.0/celmech/numerical_resonance_models.py
+-rw-r--r--   0 shadden    (501) staff       (20)     3546 2024-02-01 19:52:44.000000 celmech-1.5.0/celmech/numerical_resonance_utils.py
+-rw-r--r--   0 shadden    (501) staff       (20)    17808 2023-12-07 14:32:29.000000 celmech-1.5.0/celmech/planar_poincare.py
+-rw-r--r--   0 shadden    (501) staff       (20)    42720 2024-02-01 18:31:53.000000 celmech-1.5.0/celmech/poincare.py
+-rw-r--r--   0 shadden    (501) staff       (20)    21240 2024-04-04 16:44:26.000000 celmech-1.5.0/celmech/poisson_series.py
+-rw-r--r--   0 shadden    (501) staff       (20)     5049 2020-01-28 16:42:51.000000 celmech-1.5.0/celmech/resonances.py
+-rw-r--r--   0 shadden    (501) staff       (20)     9401 2021-01-25 16:27:34.000000 celmech-1.5.0/celmech/rk_integrator.py
+-rw-r--r--   0 shadden    (501) staff       (20)    49323 2024-04-02 19:46:49.000000 celmech-1.5.0/celmech/secular.py
+-rw-r--r--   0 shadden    (501) staff       (20)    26890 2024-04-02 19:46:49.000000 celmech-1.5.0/celmech/symplectic_evolution_operators.py
+-rw-r--r--   0 shadden    (501) staff       (20)     3112 2020-09-08 19:07:09.000000 celmech-1.5.0/celmech/transformations.py
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-04-25 20:17:09.683943 celmech-1.5.0/celmech.egg-info/
+-rw-r--r--   0 shadden    (501) staff       (20)     1024 2024-04-25 20:17:08.000000 celmech-1.5.0/celmech.egg-info/PKG-INFO
+-rw-r--r--   0 shadden    (501) staff       (20)      951 2024-04-25 20:17:08.000000 celmech-1.5.0/celmech.egg-info/SOURCES.txt
+-rw-r--r--   0 shadden    (501) staff       (20)        1 2024-04-25 20:17:08.000000 celmech-1.5.0/celmech.egg-info/dependency_links.txt
+-rw-r--r--   0 shadden    (501) staff       (20)        1 2017-08-31 19:32:30.000000 celmech-1.5.0/celmech.egg-info/not-zip-safe
+-rw-r--r--   0 shadden    (501) staff       (20)      117 2024-04-25 20:17:08.000000 celmech-1.5.0/celmech.egg-info/requires.txt
+-rw-r--r--   0 shadden    (501) staff       (20)       19 2024-04-25 20:17:08.000000 celmech-1.5.0/celmech.egg-info/top_level.txt
+-rw-r--r--   0 shadden    (501) staff       (20)       38 2024-04-25 20:17:09.686998 celmech-1.5.0/setup.cfg
+-rw-r--r--   0 shadden    (501) staff       (20)     3308 2024-04-25 20:16:49.000000 celmech-1.5.0/setup.py
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2024-04-25 20:17:09.682864 celmech-1.5.0/src/
+-rw-r--r--   0 shadden    (501) staff       (20)     4286 2024-04-25 20:16:49.000000 celmech-1.5.0/src/disturbing_function.c
+-rw-r--r--   0 shadden    (501) staff       (20)    18820 2020-08-14 20:13:36.000000 celmech-1.5.0/src/fmft.c
+-rw-r--r--   0 shadden    (501) staff       (20)      971 2022-05-19 20:01:57.000000 celmech-1.5.0/src/fmftPy.c
+-rw-r--r--   0 shadden    (501) staff       (20)    15192 2021-02-09 14:23:17.000000 celmech-1.5.0/src/moid_v4_fun.f
+-rw-r--r--   0 shadden    (501) staff       (20)     2494 2020-08-14 20:13:36.000000 celmech-1.5.0/src/nrutil.c
+-rw-r--r--   0 shadden    (501) staff       (20)      494 2020-08-14 20:13:36.000000 celmech-1.5.0/src/nrutil.h
+-rw-r--r--   0 shadden    (501) staff       (20)      483 2024-02-01 18:31:53.000000 celmech-1.5.0/src/poincare.c
+-rw-r--r--   0 shadden    (501) staff       (20)     9536 2021-01-22 18:31:13.000000 celmech-1.5.0/src/poisson_series.c
+-rw-r--r--   0 shadden    (501) staff       (20)    10205 2024-02-01 18:31:53.000000 celmech-1.5.0/src/poisson_series.h
+-rw-r--r--   0 shadden    (501) staff       (20)     1135 2020-07-10 17:45:01.000000 celmech-1.5.0/src/test.c
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `celmech-1.4.0/PKG-INFO` & `celmech-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.4.0
+Version: 1.5.0
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
+Requires-Dist: exoplanet-core==0.3.0rc2
+Requires-Dist: pytensor>=2.18
+Requires-Dist: mpmath>=1.0.0
+Requires-Dist: sympy>=1.1.1
+Requires-Dist: rebound>=4.0.1
+Requires-Dist: reboundx>=4.0.0
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.2.0
```

### Comparing `celmech-1.4.0/LICENSE` & `celmech-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/poincare.py` & `celmech-1.5.0/celmech/poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/maps.py` & `celmech-1.5.0/celmech/maps.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/poisson_series.py` & `celmech-1.5.0/celmech/c_poisson_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from ctypes import *
 from .disturbing_function import  df_coefficient_C,evaluate_df_coefficient_dict,list_resonance_terms
 #from . import clibcelmech
-from celmech.disturbing_function import df_arguments_dictionary
 #libname = "/Users/shadden/Projects/celmech/src/libcelmech.so"
 #clibcelmech = CDLL(libname)
 from . import clibcelmech
 _rt2 = np.sqrt(2)
 _rt2_inv = 1  / _rt2
 
 class SeriesTerm(Structure):
```

### Comparing `celmech-1.4.0/celmech/nbody_simulation_utilities.py` & `celmech-1.5.0/celmech/nbody_simulation_utilities.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/poisson_series_manipulate.py` & `celmech-1.5.0/celmech/poisson_series.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,14 +36,25 @@
         return val
     # define scalar multiply
     def __mul__(self,val):
         # Scalar multiplication
         return PSTerm(val * self.C,self.k,self.kbar,self.p,self.q)
     # scalar multiply is commutative
     __rmul__ = __mul__
+    def as_series(self,**kwargs):
+        """
+        Get a :class:`.PoissonSeries` object representing a series comprised of
+        a single term.
+
+        Returns
+        -------
+        PoissonSeries
+            Series version of this term.
+        """
+        return PoissonSeries.from_PSTerms([self],**kwargs)
 
 class PoissonSeries():
     def __init__(self,N,M,**kwargs):
         r"""
         A class representing a Poisson series in :math:`N` complex canonically
         conjugate variables and :math:`M` angle-action pairs. Individual terms
         have form 
@@ -155,24 +166,34 @@
             new = PoissonSeries(self.N,self.M,**self._symbol_kwargs)
             new._terms_dict = self._terms_dict.copy()
             for key,val in ps._terms_dict.items():
                 new._terms_dict[key] += val
             return new
         else:
             raise TypeError("unsupported operand type(s) for +: '{}' and '{}'".format(PoissonSeries,type(ps)))
-    
+    #define multiplication by another poisson series
+    def _Pseries_multiply(self,pseries):
+        terms=[PSTerm(t1.C * t2.C, t1.k + t2.k, t1.kbar + t2.kbar,t1.p + t2.p,t1.q + t2.q) for t1 in self.terms for t2 in pseries.terms]
+        return PoissonSeries.from_PSTerms(terms)
     # define scalar multiply term-wise
     def __mul__(self,val):
+        if type(val)==type(self):
+            return self._Pseries_multiply(val)
         if len(self.terms)==0:
             return self
         return PoissonSeries.from_PSTerms([term * val for term in self.terms],**self._symbol_kwargs)
         # Scalar multiplication
     # scalar multiplication is commutative
     __rmul__ = __mul__
 
+    @property
+    def conj(self):
+        cterms = [PSTerm(np.conj(t.C),t.kbar,t.k,t.p,-1*t.q) for t in self.terms]
+        return PoissonSeries.from_PSTerms(cterms)
+        
     def Lie_deriv(self,ps):
         """
         Compute the Lie derivative of a Poisson series expression
         with respect to this Poisson series.
         """
         if type(ps)==PoissonSeries:
             return bracket(ps,self,**self._symbol_kwargs)
@@ -208,14 +229,29 @@
         for key,val in self._terms_dict.items():
             arr = np.array(key)
             k,kbar,q,p = arr[self.ki],arr[self.kbari],arr[self.qi],arr[self.pi]
             tot += val * np.prod(P**p) * np.prod(x**k) * np.prod(xbar**kbar) * np.exp(1j*q@Q)
         return tot
   
 def bracket(PSeries1,Pseries2,**kwargs):
+    """
+    Compute the Poisson bracket of a pair of Poisson series
+
+    Parameters
+    ----------
+    PSeries1 : PoissonSeries
+        First Poisson series
+    Pseries2 : PoissonSeries
+        Second Poisson series
+
+    Returns
+    -------
+    PoissonSeries
+        Poisson series representing the Poisson bracket of the input series.
+    """
     N,M = PSeries1.N,PSeries1.M
     
     assert Pseries2.N==N and Pseries2.M==M, \
     "Dimensions of poisson series {} and {} do not match!".format(PSeries1,Pseries2)
 
     result = PoissonSeries(N,M,**kwargs)
     for term1 in PSeries1.terms:
@@ -270,56 +306,128 @@
             chi_terms.append(PSTerm(amp,term.k,term.kbar,term.p,term.q))
         else:
             Hav_terms.append(term)
     chi = PoissonSeries.from_PSTerms(chi_terms,N,0)
     hav=PoissonSeries.from_PSTerms(Hav_terms,N,0)
     return chi,hav
 
-def do_perturbation_theory(omega_vec,H,lmax):
+def birkhoff_normalize(omega_vec,H,lmax,kres = []):
+    """
+    Given an input frequency vector and Hamiltonian, carry out the Birkhoff
+    normalization procedure up to maximum specified order.
+
+    Parameters
+    ----------
+    omega_vec : 1-d array
+        Frequency of 
+    H : dict
+        Dictionary containing terms of the Hamiltonian grouped by order. The
+        keys of the dictionary denote the order of the term in powers of complex
+        canonical variables. The values are PoissonSeries objects.
+    lmax : int
+        Order up to which the Birkhoff normalization should be carried out.
+    kres : list, optional
+        List of resonant wave vectors to retain in the transformed Hamiltonian.
+        Default is none.
+
+    Returns
+    -------
+    chi : dict
+        Dictionary containing terms of the generating function. The keys of the
+        dictionary denote the order of the term in powers of complex canonical
+        variables. The values are PoissonSeries objects.
+    Hav : dict
+        Dictionary containing terms of the averaged Hamiltonian. The keys of the
+        dictionary denote the order of the term in powers of complex canonical
+        variables. The values are PoissonSeries objects.
+    """
     N = len(omega_vec)
-    chi,Phi,Hav = [defaultdict(lambda: PoissonSeries(N,0)) for _ in range(3)]
+    chi,Upsilon,Hav = [defaultdict(lambda: PoissonSeries(N,0)) for _ in range(3)]
     Hav[2] += H[2]
     for l in range(2,lmax+1):
-        Phi[(0,l)] += H[l]
+        Upsilon[(0,l)] += H[l]
         Psi = PoissonSeries(N,0)
-        Psi+= Phi[(0,l)]        
+        Psi+= Upsilon[(0,l)]        
         for n in range(1,l-1):
             kmax = l+1-n if n>1 else l-n
             for k in range(3,kmax+1):
-                Phi[(n,l)]+=chi[k].Lie_deriv(Phi[(n-1,l+2-k)])
-            Psi += Phi[(n,l)]*(1/factorial(n))
+                Upsilon[(n,l)]+=chi[k].Lie_deriv(Upsilon[(n-1,l+2-k)])
+            Psi += Upsilon[(n,l)]*(1/factorial(n))
         if l>2:
-            chi[l],Hav[l] = Psi_to_chi_and_Hav(omega_vec,Psi,[])
-            Phi[(1,l)]+=chi[l].Lie_deriv(Phi[(0,2)])
-    return chi,Hav,Phi
+            chi[l],Hav[l] = Psi_to_chi_and_Hav(omega_vec,Psi,kres)
+            Upsilon[(1,l)]+=chi[l].Lie_deriv(Upsilon[(0,2)])
+    return chi,Hav
 
 def expL(f,chi,lmax=None):
+    """
+    Calculate a finite-order truncation of the exponential of the Lie derivative
+    operator applied to a function.
+
+    Parameters
+    ----------
+    f : dict
+        Dictionary containing terms in the expansion of the target function
+        grouped by order. The keys of the dictionary denote the order of the
+        term in powers of complex canonical variables. The values are
+        PoissonSeries objects.    
+    chi : dict 
+        Dictionary containing generating function terms grouped by order.
+    lmax : int, optional
+        maximum order of the finite-order truncation. Defaults to value set by
+        maximum order terms appearing in f and chi.
+
+    Returns
+    -------
+    dict
+        Dictionary containing terms of the expansion of the transformed function
+        grouped by order.
+    """
     kmin = min(chi.keys())
     k1min = min(f.keys())
-    Phi = defaultdict(chi.default_factory)
+    Upsilon = defaultdict(chi.default_factory)
     E = defaultdict(chi.default_factory)
     if not lmax:
         lmax = max(chi.keys()) + k1min - 2
     for l in range(k1min,lmax+1):
-        Phi[0,l] += f[l]
-        E[l] += Phi[0,l]
-        nmax = (l-2) // (kmin-2)
+        Upsilon[0,l] += f[l]
+        E[l] += Upsilon[0,l]
+        nmax = (l-k1min) // (kmin-2)
         lmin_n = k1min
         for n in range(1,nmax+1):
             kmax = l+2-lmin_n
             for k in range(kmin,kmax+1):
-                Phi[(n,l)]+=chi[k].Lie_deriv(Phi[(n-1,l+2-k)])
+                Upsilon[(n,l)]+=chi[k].Lie_deriv(Upsilon[(n-1,l+2-k)])
             lmin_n = kmin + lmin_n - 2 
-            E[l] += Phi[(n,l)] * (1/factorial(n))
+            E[l] += Upsilon[(n,l)] * (1/factorial(n))
     return E
 
 def expLinv(f,chi,lmax=None):
-    if not lmax:
-        lmax = max(chi.keys())    
-    lmin = min(chi.keys())
+    """
+    Calculate a finite-order truncation of the exponential of the inverse of the
+    Lie derivative operator applied to a function.
+
+    Parameters
+    ----------
+    f : dict
+        Dictionary containing terms in the expansion of the target function
+        grouped by order. The keys of the dictionary denote the order of the
+        term in powers of complex canonical variables. The values are
+        PoissonSeries objects.    
+    chi : dict 
+        Dictionary containing generating function terms grouped by order.
+    lmax : int, optional
+        maximum order of the finite-order truncation. Defaults to value set by
+        maximum order terms appearing in f and chi.
+
+    Returns
+    -------
+    dict
+        Dictionary containing terms of the expansion of the transformed function
+        grouped by order.
+    """
     nchi = defaultdict(chi.default_factory)
     for key,val in chi.items():
         nchi[key] = val * (-1.)
     return expL(f,nchi,lmax)
 
 def k_nu_l_to_PSindices(Npl,i,j,k_vec,nu_vec,l_vec):
     r"""
```

### Comparing `celmech-1.4.0/celmech/planar_poincare.py` & `celmech-1.5.0/celmech/planar_poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/transformations.py` & `celmech-1.5.0/celmech/transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/resonances.py` & `celmech-1.5.0/celmech/resonances.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/disturbing_function.py` & `celmech-1.5.0/celmech/disturbing_function.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/__init__.py` & `celmech-1.5.0/celmech/__init__.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/secular.py` & `celmech-1.5.0/celmech/secular.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from celmech.miscellaneous import getOmegaMatrix, _machine_eps
 from collections import defaultdict
 
 from celmech.disturbing_function import list_secular_terms
 from celmech.disturbing_function import df_coefficient_C, _add_dicts,_consolidate_dictionary_terms
 from celmech.disturbing_function import terms_list_to_HamiltonianCoefficients_dict
 from celmech.disturbing_function import resonant_secular_contribution_dictionary
-from celmech.poisson_series import DFTermSeries
+from celmech.c_poisson_series import DFTermSeries
 
 
 
 class LaplaceLagrangeSystem(Poincare):
     r"""
     A class for representing the classical Laplace-Lagrange secular
     solution for a planetary system.
```

### Comparing `celmech-1.4.0/celmech/numerical_resonance_models.py` & `celmech-1.5.0/celmech/numerical_resonance_models.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/multiplanet_hamiltonian.py` & `celmech-1.5.0/celmech/multiplanet_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/miscellaneous.py` & `celmech-1.5.0/celmech/miscellaneous.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,83 @@
     I = np.eye(n,dtype=int)
     return np.vstack(
         (
          np.concatenate([zeros,I]).T,
          np.concatenate([-I,zeros]).T
         )
     )
+####################################################
+################ Orbit linking #####################
+####################################################
+def EulerMatrix(Omega,inc,omega):
+    """
+    The Euler 3D rotation matrix for Euler angles (Omega,inc,omega). The (3,1,3)
+    convention is followed.
+
+    Parameters
+    ----------
+    Omega : float
+        First Euler angle (ascending node)
+    inc : float
+        Second Euler angle (inclination)
+    omega : float
+        Third Euler angle (argument of periapsis)
+
+    Returns
+    -------
+    numpy.array
+        3 x 3 rotation matrix
+    """
+    R = np.eye(3)
+    s,c = np.sin(omega),np.cos(omega)
+    R = np.array([[c,-s,0],[s,c,0],[0,0,1]]) @ R
+    s,c = np.sin(inc),np.cos(inc)
+    R = np.array([[1,0,0],[0,c,-s],[0,s,c]]) @ R
+    s,c = np.sin(Omega),np.cos(Omega)
+    R = np.array([[c,-s,0],[s,c,0],[0,0,1]]) @ R
+    return R
+
+def linking_l(orbit1,orbit2):
+    """
+    Computes the linking coefficient defined by `Kholshevnikov and Vassiliev
+    (1999) <https://ui.adsabs.harvard.edu/abs/1999CeMDA..75...67K/abstract>`_
+    for a pair of Keplerian orbits.
+
+    Parameters
+    ----------
+    orbit1 : rebound.Orbit
+        First orbit
+    orbit2 : rebound.Orbit
+        Second orbit
+
+    Returns
+    -------
+    float
+        The linking coefficient, :math:`l_1`, defined by Equation (1) of
+        Kholshevnikov and Vassiliev (1999)
+    """
+    mtrx1 = EulerMatrix(orbit1.Omega,orbit1.inc,orbit1.omega)
+    mtrx2 = EulerMatrix(orbit2.Omega,orbit2.inc,orbit2.omega)
+    P1,Q1,Z1 = mtrx1.T
+    P2,Q2,Z2 = mtrx2.T
+    wvec = np.cross(Z1,Z2)
+    w = np.linalg.norm(wvec)
+    a1,e1 = orbit1.a,orbit1.e
+    a2,e2 = orbit2.a,orbit2.e
+
+    p1 = a1 * (1 - e1*e1)
+    p2 = a2 * (1 - e2*e2)
+
+    R1 = p1 * w / (w - e1 * np.dot(P1,wvec))
+    R2 = p2 * w / (w - e2 * np.dot(P2,wvec))
+    r1 = p1 * w / (w + e1 * np.dot(P1,wvec))
+    r2 = p2 * w / (w + e2 * np.dot(P2,wvec))
+    return (r2-r1)*(R2-R1)
+
+
 ######################################################
 ################ AMD Calculation #####################
 ######################################################
 from scipy.optimize import brenth
 def _F(e,alpha,gamma):
     """Equation 35 of Laskar & Petit (2017)"""
     denom = np.sqrt(alpha*(1-e*e)+gamma*gamma*e*e)
```

### Comparing `celmech-1.4.0/celmech/numerical_resonance_utils.py` & `celmech-1.5.0/celmech/numerical_resonance_utils.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/canonical_transformations.py` & `celmech-1.5.0/celmech/canonical_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/rk_integrator.py` & `celmech-1.5.0/celmech/rk_integrator.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/lie_transformations.py` & `celmech-1.5.0/celmech/lie_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech/symplectic_evolution_operators.py` & `celmech-1.5.0/celmech/symplectic_evolution_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                 self.Lambda0In,
                 self.Lambda0Out
         )
         bvec = np.zeros(2)
         super(SecondOrderInclinationResonanceOperator,self).__init__(initial_state,indexIn,indexOut,res_vec,Amtrx,dt)
 
 
-from .poisson_series import DFTermSeries
+from .c_poisson_series import DFTermSeries
 from scipy.optimize import root
 from .disturbing_function import ResonanceTermsList, SecularTermsList
 
 class MeanMotionResonanceDFTermsEvolutionOperator(EvolutionOperator):
     """
     Evolution operator for a collection of disturbing function
     terms associated with a specific mean motion resonance between
```

### Comparing `celmech-1.4.0/celmech/hamiltonian.py` & `celmech-1.5.0/celmech/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/README.md` & `celmech-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/setup.py` & `celmech-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DCELMECHGITHASH="+ghash.strip()
 except:
-    ghash_arg = "-DCELMECHGITHASH=69d1a15b6297011a2ecbf7bb1ff282a329067f67" #GITHASHAUTOUPDATE
+    ghash_arg = "-DCELMECHGITHASH=b910cba8ae45ef1ce2c7ec289b3ced26bd49eb1f" #GITHASHAUTOUPDATE
 
 extra_link_args=[]
 if sys.platform == 'darwin':
     from distutils import sysconfig
     vars = sysconfig.get_config_vars()
     vars['LDSHARED'] = vars['LDSHARED'].replace('-bundle', '-shared')
     extra_link_args=['-Wl,-install_name,@rpath/libcelmech'+suffix]
@@ -45,15 +45,15 @@
     packages = ['exoplanet-core==0.3.0rc2','pytensor>=2.18' ,'sympy>=1.1.1', 'numpy', 'scipy>=1.2.0', 'reboundx>=4.0.0', 'rebound>=4.0.1', 'mpmath>=1.0.0']
     try:
         install_requires += packages
     except:
         install_requires = packages
 
 setup(name='celmech',
-    version='1.4.0',
+    version='1.5.0',
     description='Open source tools for celestial mechanics',
     url='http://github.com/shadden/celmech',
     author='Dan Tamayo, Sam Hadden',
     author_email='tamayo.daniel@gmail.com, shadden1107@gmail.com',
     license='GPL',
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `celmech-1.4.0/src/disturbing_function.c` & `celmech-1.5.0/src/disturbing_function.c`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #include <stdio.h>
 #include <assert.h>
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* celmech_build_str = __DATE__ " " __TIME__; // Date and time build string. 
-const char* celmech_version_str = "1.4.0";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* celmech_version_str = "1.5.0";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* celmech_githash_str = STRINGIFY(CELMECHGITHASH);             // This line gets updated automatically. Do not edit manually.
 
 double laplace(double s, int i, int j, double a);
 double GeneralOrderCoefficient(int res_j, int order, int epower,double a);
 
 int binomialCoeff(int n, int k)
 {
```

### Comparing `celmech-1.4.0/src/nrutil.c` & `celmech-1.5.0/src/nrutil.c`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/poisson_series.h` & `celmech-1.5.0/src/poisson_series.h`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/moid_v4_fun.f` & `celmech-1.5.0/src/moid_v4_fun.f`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/fmftPy.c` & `celmech-1.5.0/src/fmftPy.c`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/test.c` & `celmech-1.5.0/src/test.c`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/fmft.c` & `celmech-1.5.0/src/fmft.c`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/src/poisson_series.c` & `celmech-1.5.0/src/poisson_series.c`

 * *Files identical despite different names*

### Comparing `celmech-1.4.0/celmech.egg-info/PKG-INFO` & `celmech-1.5.0/celmech.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.4.0
+Version: 1.5.0
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
+Requires-Dist: exoplanet-core==0.3.0rc2
+Requires-Dist: pytensor>=2.18
+Requires-Dist: mpmath>=1.0.0
+Requires-Dist: sympy>=1.1.1
+Requires-Dist: rebound>=4.0.1
+Requires-Dist: reboundx>=4.0.0
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.2.0
```

### Comparing `celmech-1.4.0/celmech.egg-info/SOURCES.txt` & `celmech-1.5.0/celmech.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 celmech/__init__.py
+celmech/c_poisson_series.py
 celmech/canonical_transformations.py
 celmech/disturbing_function.py
 celmech/hamiltonian.py
 celmech/lie_transformations.py
 celmech/maps.py
 celmech/miscellaneous.py
 celmech/multiplanet_hamiltonian.py
 celmech/nbody_simulation_utilities.py
 celmech/numerical_resonance_models.py
 celmech/numerical_resonance_utils.py
 celmech/planar_poincare.py
 celmech/poincare.py
 celmech/poisson_series.py
-celmech/poisson_series_manipulate.py
 celmech/resonances.py
 celmech/rk_integrator.py
 celmech/secular.py
 celmech/symplectic_evolution_operators.py
 celmech/transformations.py
 celmech.egg-info/PKG-INFO
 celmech.egg-info/SOURCES.txt
```

