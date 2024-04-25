# Comparing `tmp/elisa_lib-0.0.1.dev1.tar.gz` & `tmp/elisa_lib-0.1.0.tar.gz`

## Comparing `elisa_lib-0.0.1.dev1.tar` & `elisa_lib-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,56 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/.DS_Store
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/.readthedocs.yaml
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/.DS_Store
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/Makefile
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/conf.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/make.bat
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/docs/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/.DS_Store
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/data/__init__.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/data/grouping.py
--rw-r--r--   0        0        0    37128 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/data/ogip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/inference/__init__.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/inference/fit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/inference/gof.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/inference/likelihood.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/inference/lrt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/__init__.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/add.py
--rw-r--r--   0        0        0    25425 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/base.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/con.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/integral.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/mul.py
--rw-r--r--   0        0        0    27645 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/model/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/src/elisa/plot/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/base.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/fit.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/quick_start.ipynb
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/sampling_test.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/test.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/test_ogip.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/transform_test.py
--rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/tests/xspec.ipynb
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/__init__.py
--rw-r--r--   0        0        0    25973 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/data.py
--rw-r--r--   0        0        0    72442 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/inference.py
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/likelihood.py
--rw-r--r--   0        0        0    31164 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/plot.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/requirements.txt
--rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/sampling.py
--rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/test.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/test2.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/.DS_Store
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/__init__.py
--rw-r--r--   0        0        0    41653 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/base.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/flux_model.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/model.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/xspec/.DS_Store
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/xspec/__init__.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/xspec/base.py
--rw-r--r--   0        0        0   259903 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/xspec/model.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/v0/model/xspec/xs.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/LICENSE
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/README.md
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 elisa_lib-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/noxfile.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/modules.rst
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/__about__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/__init__.py
+-rw-r--r--   0        0        0    21847 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/grouping.py
+-rw-r--r--   0        0        0    55530 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/ogip.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/data.py
+-rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/fit.py
+-rw-r--r--   0        0        0    33616 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/helper.py
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/likelihood.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/lrt.py
+-rw-r--r--   0        0        0    19964 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/nested_sampling.py
+-rw-r--r--   0        0        0    67863 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/results.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/__init__.py
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/add.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/conv.py
+-rw-r--r--   0        0        0    55905 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/model.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/mul.py
+-rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/parameter.py
+-rw-r--r--   0        0        0    14335 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/xspec.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/tables/generate_xsect_table.py
+-rw-r--r--   0        0        0  3172880 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/tables/xsect.hdf5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/__init__.py
+-rw-r--r--   0        0        0    30171 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/data.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/errorbars.py
+-rw-r--r--   0        0        0     9438 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/misc.py
+-rw-r--r--   0        0        0    51692 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/plotter.py
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/residuals.py
+-rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/scale.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/util.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/__init__.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/bslogu.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/config.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/integrate.py
+-rw-r--r--   0        0        0    14312 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/misc.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/scipy_nquad.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/model/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/model/test_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/parameter/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/parameter/test_name.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/README.md
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/PKG-INFO
```

### Comparing `elisa_lib-0.0.1.dev1/docs/Makefile` & `elisa_lib-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.0.1.dev1/src/elisa/data/ogip.py` & `elisa_lib-0.1.0/src/elisa/data/ogip.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,134 @@
-"""Handle OGIP/92-007 format data loading."""
+"""Containers of OGIP/92-007 format data."""
+
 from __future__ import annotations
 
 import re
 import warnings
+from typing import TYPE_CHECKING
 
+import matplotlib.pyplot as plt
 import numpy as np
 from astropy.io import fits
-from .grouping import (
+from scipy.sparse import coo_array, csc_array
+
+from elisa.data.grouping import (
     group_const,
     group_min,
-    group_sig,
-    group_pos,
     group_opt,
-    group_optmin,
-    group_optsig
+    group_optsig_gv,
+    group_optsig_lima,
+    group_optsig_normal,
+    group_sig_gv,
+    group_sig_lima,
+    group_sig_normal,
 )
 
-__all__ = ['Data']
-# TODO: support creating Data object from array
+if TYPE_CHECKING:
+    from elisa.util.typing import NumPyArray as NDArray
 
-NDArray = np.ndarray
+# TODO: support multiple response in a single data object
+# TODO: support creating Data object from array
 
 
 class Data:
-    """Class to load observation data stored in OGIP/92-007 format.
+    """Handle observation data in OGIP standards [1]_ [2]_.
 
     Load the observation spectrum, the telescope response and the possible
     background, and handle the grouping of spectrum and response.
 
     Parameters
     ----------
     erange : array_like
         Energy range of interest in keV, e.g., ``erange=[(0.5, 2), (5, 200)]``.
     specfile : str
         Spectrum file path. For type II pha file, the row specifier must be
-        given in the end of path, e.g., ``specfile="./spec.pha2{1}"``.
+        given in the end of path, e.g., ``specfile='spec.pha2{1}'``.
     backfile : str or None, optional
         Background file path. Read from the `specfile` header if None.
         For type II pha file, the row specifier must be given in the end of
-        path, e.g., ``backfile="./back.pha2{1}"``.
+        path, e.g., ``backfile='back.pha2{1}'``.
     respfile : str or None, optional
         Response file path. Read from the `specfile` header if None.
         The path must be given if ``RESPFILE`` is undefined in the header.
     ancrfile : str or None, optional
         Ancillary response path. Read from the `specfile` header if None.
+
+    Other Parameters
+    ----------------
     name : str or None, optional
         Data name. Read from the `specfile` header if None. The name must
         be given if ``DETNAM``, ``INSTRUME`` and ``TELESCOP`` are all
         undefined in the header.
     group : str or None, optional
         Method to group spectrum and background adaptively, these options are
         available so that each channel group has:
-            * const: `scale` number channels
-            * min: counts >= `scale` for src + bkg
-            * sig: src significance >= `scale`-sigma
-            * opt: optimal binning, see Kaastra & Bleeker (2016, A&A)
-            * optmin: opt with counts >= `scale` for src + bkg
-            * optsig: opt with src significance >= `scale`-sigma
-            * bmin: counts >= `scale` for bkg (useful for W-stat)
-            * bpos: bkg < 0 with probability < `scale` (useful for PG-stat)
+
+            * ``'const'``: `scale` number channels
+            * ``'min'``: total (source + background) counts >= `scale`
+            * ``'sig'``: source significance >= `scale` sigma
+            * ``'bmin'``: background counts >= `scale`, used to avoid bias when
+              using ``wstat`` to simultaneously fit the source and background
+            * ``'bsig'``: background significance >= `scale` sigma, used to
+              avoid bias when using ``pgstat`` to simultaneously fit the source
+              and background
+            * ``'opt'``: optimal binning, see Kaastra & Bleeker (2016) [3]_
+            * ``'optmin'``: optimal binning with total counts >= `scale`
+            * ``'optsig'``: optimal binning with source significance >= `scale`
+              sigma
+            * ``'optbmin'``: optimal binning with background counts >= `scale`
+            * ``'optbsig'``: optimal binning with background significance
+              >= `scale` sigma
+
+        The default is None.
     scale : float or None, optional
-        Grouping scale. Only takes effect if `group` is not None.
+        Grouping scale for the method specified in `group`.
     spec_poisson : bool or None, optional
         Whether the spectrum data follows counting statistics, reading from
         the `specfile` header. This value must be set if ``POISSERR`` is
         undefined in the header.
     back_poisson : bool or None, optional
         Whether the background data follows counting statistics, reading
         from the `backfile` header. This value must be set if ``POISSERR``
         is undefined in the header.
     ignore_bad : bool, optional
-        Whether to ignore channels whose ``QUALITY`` are 5.
-        The default is True. The possible values for ``QUALITY`` are
-            *  0: good
-            *  1: defined bad by software
-            *  2: defined dubious by software
-            *  5: defined bad by user
-            * -1: reason for bad flag unknown
+        Whether to ignore channels with ``QUALITY==5``.
+        The default is True. The possible values for spectral ``QUALITY`` are
+
+            * ``0``: good
+            * ``1``: defined bad by software
+            * ``2``: defined dubious by software
+            * ``5``: defined bad by user
+            * ``-1``: reason for bad flag unknown
+
     record_channel : bool, optional
         Whether to record channel information in the label of grouped
         channel. Only takes effect if `group` is not None or spectral data
         has ``GROUPING`` defined. The default is False.
+    resp_sparse : bool, optional
+        Whether the response matrix is sparse. The default is False.
     corrfile : str or None, optional
         Correction file applied to `specfile`. Read from the `specfile`
         header if None. The default is None.
     corrnorm : float or None, optional
         Scaling factor to be applied to `corrfile`. Read from the
         `specfile` header if None. The default is None.
 
     Notes
     -----
     Reading and applying correction to data is not yet supported.
 
+    References
+    ----------
+    .. [1] `The OGIP Spectral File Format <https://heasarc.gsfc.nasa.gov/docs/heasarc/ofwg/docs/spectra/ogip_92_007/ogip_92_007.html>`__
+            and `Addendum: Changes log <https://heasarc.gsfc.nasa.gov/docs/heasarc/ofwg/docs/spectra/ogip_92_007a/ogip_92_007a.html>`__
+    .. [2] `The Calibration Requirements for Spectral Analysis (Definition of
+            RMF and ARF file formats) <https://heasarc.gsfc.nasa.gov/docs/heasarc/caldb/docs/memos/cal_gen_92_002/cal_gen_92_002.html>`__
+            and `Addendum: Changes log <https://heasarc.gsfc.nasa.gov/docs/heasarc/caldb/docs/memos/cal_gen_92_002a/cal_gen_92_002a.html>`__
+    .. [3] `Kaastra & Bleeker 2016, A&A, 587, A151 <https://doi.org/10.1051/0004-6361/201527395>`__
     """
 
     def __init__(
         self,
         erange: list | tuple,
         specfile: str,
         backfile: str | None = None,
@@ -104,18 +137,36 @@
         name: str | None = None,
         group: str | None = None,
         scale: float | int | None = None,
         spec_poisson: bool | None = None,
         back_poisson: bool | None = None,
         ignore_bad: bool = True,
         record_channel: bool = False,
-        corrfile: str | None = None,
-        corrnorm: str | None = None
+        resp_sparse: bool = False,
+        corrfile: bool | None = None,
+        corrnorm: bool | None = None,
     ):
-        spec = Spectrum(specfile, spec_poisson)
+        erange = np.array(erange, dtype=np.float64, order='C', ndmin=2)
+
+        # check if erange is increasing
+        if np.any(np.diff(erange, axis=1) <= 0.0):
+            raise ValueError('erange must be increasing')
+
+        # check if erange is overlapped
+        erange = erange[erange[:, 0].argsort()]
+        if np.any(np.diff(np.hstack(erange)) <= 0.0):
+            raise ValueError('erange must not be overlapped')
+
+        try:
+            spec = Spectrum(specfile, spec_poisson)
+        except PoissonFlagNotFoundError as err:
+            raise PoissonFlagNotFoundError(
+                '"POISSERR" is undefined in spectrum header, `spec_poisson` '
+                'must be set in Data(..., spec_poisson=True/False)'
+            ) from err
 
         # check data name
         if name:
             name = str(name)
         elif spec.name:
             name = spec.name
         else:
@@ -130,48 +181,64 @@
             resp = Response(respfile, ancrfile)
         elif spec.respfile:
             resp = Response(spec.respfile, ancrfile)
         else:
             raise ValueError('respfile is required for data')
 
         if len(spec._raw_counts) != len(resp._raw_channel):
-            msg = f'specfile ({specfile}) and respfile ({respfile}) are not '
-            msg += 'matched'
-            raise ValueError(msg)
+            raise ValueError(
+                f'specfile ({specfile}) and respfile ({respfile}) are not '
+                'matched'
+            )
 
         # check background file
-        if backfile:
-            back = Spectrum(backfile, back_poisson)
-        elif spec.backfile:
-            back = Spectrum(spec.backfile, back_poisson)
-        else:
-            back = None
+        try:
+            if backfile:
+                back = Spectrum(backfile, back_poisson)
+            elif spec.backfile:
+                back = Spectrum(spec.backfile, back_poisson)
+            else:
+                back = None
+        except PoissonFlagNotFoundError as err:
+            raise PoissonFlagNotFoundError(
+                '"POISSERR" is undefined in background header, `back_poisson` '
+                'must be set in Data(..., back_poisson=True/False)'
+            ) from err
 
         if back and len(spec._raw_counts) != len(back._raw_counts):
-            msg = f'specfile ({specfile}) and backfile ({backfile}) are not '
-            msg += 'matched'
-            raise ValueError(msg)
+            raise ValueError(
+                f'specfile ({specfile}) and backfile ({backfile}) are not '
+                'matched'
+            )
 
         # bad quality
         bad = (1, 5) if ignore_bad else (1,)
 
-        # check if quality of spectrum and background are matched
+        # check if the quality of spectrum and background are matched
         good_quality = ~np.isin(spec.quality, bad)
         if back:
             back_good = ~np.isin(back.quality, bad)
             if not np.all(good_quality == back_good):
                 good_quality &= back_good
-                msg = 'ignore bad channels defined by the union of spectrum '
-                msg += 'and background quality'
-                warnings.warn(msg, Warning, stacklevel=2)
+                warnings.warn(
+                    'ignore bad channels defined by the union of spectrum '
+                    f'({specfile})and background ({backfile}) quality',
+                    Warning,
+                    stacklevel=2,
+                )
+        if not np.any(good_quality):
+            raise RuntimeError(f'no good channel is found for {name} data')
 
-        # corrfile and corrnorm not supported yet
+        # corrfile and corrnorm are not supported yet
         if corrfile or corrnorm:
-            msg = 'correction to data is not yet supported.'
-            warnings.warn(msg, Warning, stacklevel=2)
+            warnings.warn(
+                'correction to data is not yet supported',
+                Warning,
+                stacklevel=2,
+            )
 
         # check correction file
         # use poisson=True to bypass stat_err check, which takes no effect
         # if corrfile:
         #     corr = Spectrum(corrfile, True)
         # elif spec.corrfile:
         #     corr = Spectrum(spec.corrfile, True)
@@ -185,196 +252,305 @@
 
         self._spec = spec
         self._resp = resp
         self._back = back
         # self._corr = corr
 
         self._name = name
-        self._erange = np.array(erange, dtype=np.float64, order='C', ndmin=2)
+        self._erange = erange
         self._good_quality = good_quality
         self._record_channel = bool(record_channel)
 
         # response attributes
+        self._resp_sparse = bool(resp_sparse)
         self._ph_egrid = resp.ph_egrid
         self._channel = None
         self._ch_emin = None
         self._ch_emax = None
         self._ch_emid = None
         self._ch_mean = None
         self._ch_width = None
         self._ch_error = None
         self._resp_matrix = None
 
-        # NOTE:
-        # grouping of area/background scale is not supported currently,
-        # so we hard code effexpo here, but it should be moved into _set_data
-        # once grouping of area/background scale is implemented.
-
         # spectrum attributes
         self._spec_exposure = spec.exposure
-        self._spec_effexpo = spec.exposure * spec.area_scale * spec.back_scale
         self._spec_poisson = spec.poisson
         self._spec_counts = None
         self._spec_error = None
 
         self._has_back = True if back else False
 
         # background attributes
         if self._has_back:
             self._back_exposure = back.exposure
-            self._back_effexpo = back.exposure*back.area_scale*back.back_scale
             self._back_poisson = back.poisson
+            self._back_ratio = (
+                spec.exposure * spec.area_scale * spec.back_scale
+            ) / (back.exposure * back.area_scale * back.back_scale)
         else:
             self._back_exposure = None
-            self._back_effexpo = None
             self._back_poisson = None
+            self._back_ratio = None
         self._back_counts = None
         self._back_error = None
 
         # net spectrum attributes
         self._net_counts = None
-        self._net_spec = None
         self._net_error = None
+        self._ce = None
+        self._ce_error = None
 
         # other attributes
         self._grouping = None
         self._ch_mask = None
 
         if group:
             # group spectrum and set the other attributes therein
             self.group(group, scale)
         else:
             # set the other attributes
             self._set_data(spec.grouping)
 
-    def group(self, method: str, scale: float | int):
-        """Adaptively group the spectrum.
+    def group(self, method: str, scale: float | int | None):
+        """Group the spectrum.
 
         Parameters
         ----------
         method : str
             Method to group spectrum and background adaptively, these options
             are available so that each channel group has:
-                * const: `scale` number channels
-                * min: counts >= `scale` for src + bkg
-                * sig: src significance >= `scale`-sigma
-                * opt: optimal binning, see Kaastra & Bleeker (2016, A&A)
-                * optmin: opt with counts >= `scale` for src + bkg
-                * optsig: opt with src significance >= `scale`-sigma
-                * bmin: counts >= `scale` for bkg (useful for W-stat)
-                * bpos: bkg < 0 with probability < `scale` (useful for PG-stat)
-        scale : float
-            Grouping scale.
 
-        Warns
-        -----
-        GroupWarning
-            Warn if grouping scale is not met for any channel.
+            * ``'const'``: `scale` number channels
+            * ``'min'``: total (source + background) counts >= `scale`
+            * ``'sig'``: source significance >= `scale` sigma
+            * ``'bmin'``: background counts >= `scale`, used to avoid bias when
+              using ``wstat`` to simultaneously fit the source and background
+            * ``'bsig'``: background significance >= `scale` sigma, used to
+              avoid bias when using ``pgstat`` to simultaneously fit the source
+              and background
+            * ``'opt'``: optimal binning, see Kaastra & Bleeker (2016) [1]_
+            * ``'optmin'``: optimal binning with total counts >= `scale`
+            * ``'optsig'``: optimal binning with source significance >= `scale`
+              sigma
+            * ``'optbmin'``: optimal binning with background counts >= `scale`
+            * ``'optbsig'``: optimal binning with background significance
+              >= `scale` sigma
+
+        scale : float, int or None
+            Grouping scale.
 
         Raises
         ------
         NotImplementedError
             Grouping is not yet implemented for spectrum with ``AREASCAL``
             and/or ``BACKSCAL`` array.
 
+        Warns
+        -----
+        GroupWarning
+            Warn if grouping scale is not met for any channel.
+
         Notes
         -----
         If there are ignored channels in a channel group, this may cause an
-        inconsistency in a spectral plot, i.e., the error bar of a channel
-        group will cover these bad channels, whilst these bad channels are
-        never used in fitting.
+        inconsistency in a spectral plot. That is to say, the error bar of a
+        channel group will cover these bad channels, whilst these bad channels
+        are never used in fitting.
 
+        References
+        ----------
+        .. [1] `Kaastra & Bleeker 2016, A&A, 587, A151 <https://doi.org/10.1051/0004-6361/201527395>`__
         """
+        method = str(method)
+        scale = float(scale) if scale is not None else None
+
+        if method != 'opt' and scale is None:
+            raise ValueError(f'scale must be given for {method} grouping')
+
+        if method.startswith('opt'):
+            fwhm = self._resp.ch_fwhm
+        else:
+            fwhm = None
+
         ch_emin, ch_emax = self._resp._raw_channel_egrid.T
         ch_mask = self._channel_mask(ch_emin, ch_emax)  # shape = (nchan, 2)
         spec_counts = self._spec._raw_counts
-        # spec_error = self._spec._raw_error
+        spec_errors = self._spec._raw_error
+        if self.has_back:
+            back_ratio = self.back_ratio
+            back_counts = self._back._raw_counts
+            back_errors = self._back._raw_error
+            berr = back_ratio * back_errors
+            net_counts = spec_counts - back_ratio * back_counts
+            net_errors = np.sqrt(spec_errors * spec_errors + berr * berr)
+        else:
+            back_ratio = None
+            back_counts = None
+            back_errors = None
+            net_counts = spec_counts
+            net_errors = spec_errors
+
         grouping = np.full(len(spec_counts), 1, dtype=np.int64)
 
-        def apply_grouping(group_func, mask, *args):
-            """function operating the grouping array defined above."""
-            data = (i[mask] * self._good_quality[mask] for i in args)
+        def apply_grouping(group_func, mask, args, all_good=()):
+            """Apply the grouping array defined above."""
+            data = []
+            for i, j in enumerate(args):
+                if np.shape(j) == ():  # scalar
+                    data.append(j)
+                else:
+                    if i not in all_good:
+                        data.append(j[mask] * self._good_quality[mask])
+                    else:
+                        data.append(j[mask])
             grouping_flag, grouping_success = group_func(*data, scale)
             grouping[mask] = grouping_flag
             return grouping_success
 
-        def apply_map(func, *args):
-            """map the apply function and return success flag."""
+        def apply_map(func, *args, all_good=()):
+            """Map the apply function and return a success flag."""
             return all(
-                map(
-                    lambda mask: apply_grouping(func, mask, *args),
-                    ch_mask
-                )
+                apply_grouping(func, mask, args, all_good) for mask in ch_mask
             )
 
         if method == 'const':
-            success = group_const()
+            success = apply_map(group_const, len(spec_counts))
 
         elif method == 'min':
             success = apply_map(group_min, spec_counts)
 
         elif method == 'sig':
-            success = group_sig()
+            if self.spec_poisson:
+                if self.back_poisson:
+                    fn = group_sig_lima
+                    args = (spec_counts, back_counts, back_ratio)
+                    all_good = (2,)
+                else:
+                    fn = group_sig_gv
+                    args = (spec_counts, back_counts, back_errors, back_ratio)
+                    all_good = (3,)
+            else:
+                fn = group_sig_normal
+                args = (net_counts, net_errors)
+                all_good = ()
+            success = apply_map(fn, *args, all_good=all_good)
+
+        elif method == 'bmin':
+            if not (self.has_back and self.back_poisson):
+                raise ValueError(
+                    'Poisson background is required for "bmin" method'
+                )
+            success = apply_map(group_min, back_counts)
+
+        elif method == 'bsig':
+            if not self.has_back:
+                raise ValueError(
+                    'background data is required for "bsig" method'
+                )
+            success = apply_map(group_sig_normal, back_counts, back_errors)
 
         elif method == 'opt':
-            success = group_opt()
+            success = apply_map(group_opt, fwhm, net_counts, all_good=(0, 1))
 
         elif method == 'optmin':
-            success = group_optmin()
+            success = apply_map(
+                group_opt, fwhm, net_counts, spec_counts, all_good=(0, 1)
+            )
 
         elif method == 'optsig':
-            success = group_optsig()
-
-        elif method == 'bmin':
-            if self.has_back and self.back_poisson:
-                back_counts = self._back._raw_counts
+            if self.spec_poisson:
+                if self.back_poisson:
+                    fn = group_optsig_lima
+                    args = (
+                        fwhm,
+                        net_counts,
+                        spec_counts,
+                        back_counts,
+                        back_ratio,
+                    )
+                else:
+                    fn = group_optsig_gv
+                    args = (
+                        fwhm,
+                        net_counts,
+                        spec_counts,
+                        back_counts,
+                        back_errors,
+                        back_ratio,
+                    )
             else:
-                msg = 'Poisson background is required for "bmin" method'
-                raise ValueError(msg)
-            success = apply_map(group_min, back_counts)
-
-        elif method == 'bpos':
-            if self.has_back:
-                back_counts = self._back._raw_counts
-                back_error = self._back._raw_error
-            else:
-                msg = 'background data is required for "bpos" method'
-                raise ValueError(msg)
+                fn = group_optsig_normal
+                args = (fwhm, net_counts, net_counts, net_errors)
+            success = apply_map(fn, *args, all_good=(0, 1))
+
+        elif method == 'optbmin':
+            if not (self.has_back and self.back_poisson):
+                raise ValueError(
+                    'Poisson background is required for "optbmin" method'
+                )
+            success = apply_map(
+                group_opt, fwhm, net_counts, back_counts, all_good=(0, 1)
+            )
 
-            success = apply_map(group_pos, back_counts, back_error)
+        elif method == 'optbsig':
+            if not self.has_back:
+                raise ValueError(
+                    'background data is required for "optbsig" method'
+                )
+            success = apply_map(
+                group_optsig_normal,
+                fwhm,
+                net_counts,
+                back_counts,
+                back_errors,
+                all_good=(0, 1),
+            )
 
         else:
             supported = (
-                'const', 'min', 'sig', 'opt', 'optmin', 'optsig', 'bmin',
-                'bpos'
+                'const',
+                'min',
+                'bmin',
+                'bsig',
+                'sig',
+                'opt',
+                'optmin',
+                'optsig',
+                'optbmin',
+                'optbsig',
+            )
+            raise ValueError(
+                f'supported grouping method are: {", ".join(supported)}'
             )
-            msg = f'supported grouping method are: {", ".join(supported)}'
-            raise ValueError(msg)
 
         if not success:
-            msg = f'"{method}" grouping failed in some {self._name} channels'
-            warnings.warn(msg, GroupWaring)
+            warnings.warn(
+                f'"{method}" grouping failed in some {self._name} channels',
+                GroupingWaring,
+            )
 
         self._set_data(grouping)
 
     def _set_data(self, grouping: NDArray):
         """Set data according to quality, grouping, and energy range."""
         self._spec.group(grouping, self._good_quality)
         self._resp.group(grouping, self._good_quality)
         self._grouping = grouping
 
+        ch = self._spec._header.get('CHANTYPE', 'Ch')
         if self._record_channel:
             groups_channel = np.array(
-                [f'{self.name}_Ch{"+".join(c)}' for c in self._resp.channel]
+                [f'{self.name}_{ch}_{"+".join(c)}' for c in self._resp.channel]
             )
         else:
-            grp_idx = np.flatnonzero(grouping == 1)  # transform to index
+            grp_idx = np.flatnonzero(grouping != -1)  # transform to index
             non_empty = np.add.reduceat(self._good_quality, grp_idx) != 0
             groups_channel = np.array(
-                [f'{self.name}_Ch{c}' for c in np.flatnonzero(non_empty)]
+                [f'{self.name}_{ch}_{c}' for c in np.flatnonzero(non_empty)]
             )
 
         ch_emin = self._resp.ch_emin
         ch_emax = self._resp.ch_emax
         ch_mask = self._channel_mask(ch_emin, ch_emax)  # shape = (nchan, 2)
         ch_mask = np.any(ch_mask, axis=0)
 
@@ -383,58 +559,69 @@
         self._ch_emin = ch_emin[ch_mask]
         self._ch_emax = ch_emax[ch_mask]
         resp = self._resp
         self._ch_emid = resp.ch_emid[ch_mask]
         self._ch_mean = resp.ch_mean[ch_mask]
         self._ch_width = resp.ch_width[ch_mask]
         self._ch_error = resp.ch_error[:, ch_mask]
-        self._resp_matrix = resp.matrix[:, ch_mask]
+        self._resp_matrix = resp.sparse_matrix.tocsc()[:, ch_mask]
 
         # spectrum attribute
         spec = self._spec
         self._spec_counts = spec.counts[ch_mask]
         self._spec_error = spec.error[ch_mask]
 
         # background attribute
         if self._has_back:
             self._back.group(grouping, self._good_quality)
-            back = self._back
-            self._back_counts = back.counts[ch_mask]
-            self._back_error = back.error[ch_mask]
+            self._back_counts = self._back.counts[ch_mask]
+            self._back_error = self._back.error[ch_mask]
 
         # net spectrum attribute
         unit = 1.0 / (self._ch_width * self._spec_exposure)
         if self._has_back:
-            ratio = self._spec_effexpo / self._back_effexpo
-            net = self._spec_counts - ratio * self._back_counts
-            spec = net * unit
+            net = self._spec_counts - self._back_ratio * self._back_counts
             var = np.square(self._spec_error)
-            var += np.square(ratio * self._back_error)
-            var *= np.square(unit)
+            var += np.square(self._back_ratio * self._back_error)
+            net_error = np.sqrt(var)
+            ce = net * unit
+            ce_error = net_error * unit
             self._net_counts = net
-            self._net_spec = spec
-            self._net_error = np.sqrt(var)
+            self._net_error = net_error
+            self._ce = ce
+            self._ce_error = ce_error
 
         else:
             self._net_counts = self._spec_counts
-            self._net_spec = self._net_counts * unit
-            self._net_error = self._spec_error * unit
+            self._net_error = self._spec_error
+            self._ce = self._net_counts * unit
+            self._ce_error = self._spec_error * unit
 
         # correction attribute
         # if self._corr:
         #     self._corr.group(grouping, self._good_quality)
 
     def _channel_mask(self, ch_emin: NDArray, ch_emax: NDArray) -> NDArray:
         """Return channel mask given energy grid and erange of interest."""
         emin = np.expand_dims(self._erange[:, 0], axis=1)
         emax = np.expand_dims(self._erange[:, 1], axis=1)
         mask1 = np.less_equal(emin, ch_emin)
         mask2 = np.less_equal(ch_emax, emax)
         return np.bitwise_and(mask1, mask2)
 
+    def plot_matrix(self, hatch: bool = True) -> None:
+        """Plot the response matrix.
+
+        Parameters
+        ----------
+        hatch : bool, optional
+            Whether to add hatches in the ignored region. The default is True.
+        """
+        self._resp.plot(self._erange if hatch else None)
+
     @property
     def name(self) -> str:
         """Data name."""
         return self._name
 
     @property
     def spec_counts(self) -> NDArray:
@@ -448,22 +635,22 @@
 
     @property
     def spec_poisson(self) -> bool:
         """Whether spectrum data follows counting statistics."""
         return self._spec_poisson
 
     @property
-    def spec_exposure(self) -> float:
+    def spec_exposure(self) -> np.float64:
         """Spectrum exposure."""
         return self._spec_exposure
 
     @property
-    def spec_effexpo(self) -> float | NDArray:
-        """Effective exposure of spectrum."""
-        return self._spec_effexpo
+    def area_factor(self) -> np.float64 | NDArray:
+        """Area scaling factor."""
+        return self._spec.area_scale
 
     @property
     def has_back(self) -> bool:
         """Whether spectrum data includes background."""
         return self._has_back
 
     @property
@@ -478,106 +665,121 @@
 
     @property
     def back_poisson(self) -> bool | None:
         """Whether background data follows counting statistics."""
         return self._back_poisson
 
     @property
-    def back_exposure(self) -> float | None:
+    def back_exposure(self) -> np.float64 | None:
         """Background exposure."""
         return self._back_exposure
 
     @property
-    def back_effexpo(self) -> float | NDArray | None:
-        """Effective exposure of background."""
-        return self._back_effexpo
+    def back_ratio(self) -> np.float64 | NDArray | None:
+        """Ratio of spectrum to background effective exposure."""
+        return self._back_ratio
 
     @property
     def net_counts(self) -> NDArray:
         """Net counts in each measuring channel."""
         return self._net_counts
 
     @property
-    def net_spec(self) -> NDArray:
+    def net_error(self) -> NDArray:
+        """Uncertainty of net counts in each measuring channel."""
+        return self._net_error
+
+    @property
+    def ce(self) -> NDArray:
         """Net counts per second per keV."""
-        return self._net_spec
+        return self._ce
 
     @property
-    def net_error(self) -> NDArray:
-        """Uncertainty of net spectrum."""
-        return self._net_error
+    def ce_error(self) -> NDArray:
+        """Uncertainty of net counts per second per keV."""
+        return self._ce_error
 
     @property
     def ph_egrid(self) -> NDArray:
         """Photon energy grid of response matrix."""
         return self._ph_egrid
 
     @property
     def channel(self) -> NDArray:
-        """Measured channel information."""
+        """Measurement channel information."""
         return self._channel
 
     @property
     def ch_emin(self) -> NDArray:
-        """Left edge of measured energy grid."""
+        """Left edge of measurement energy grid."""
         return self._ch_emin
 
     @property
     def ch_emax(self) -> NDArray:
-        """Right edge of measured energy grid."""
+        """Right edge of measurement energy grid."""
         return self._ch_emax
 
     @property
     def ch_emid(self) -> NDArray:
-        """Middle of measured energy grid."""
+        """Middle of measurement energy grid."""
         return self._ch_emid
 
     @property
     def ch_width(self) -> NDArray:
-        """Width of measured energy grid."""
+        """Width of measurement energy grid."""
         return self._ch_width
 
     @property
     def ch_mean(self) -> NDArray:
-        """Geometric mean of measured energy grid."""
+        """Geometric mean of measurement energy grid."""
         return self._ch_mean
 
     @property
     def ch_error(self) -> NDArray:
         """Width between left/right and geometric mean of channel grid."""
         return self._ch_error
 
     @property
     def resp_matrix(self) -> NDArray:
         """Response matrix."""
+        return self._resp_matrix.todense()
+
+    @property
+    def sparse_resp_matrix(self) -> coo_array:
+        """Sparse response matrix."""
         return self._resp_matrix
 
+    @property
+    def resp_sparse(self) -> bool:
+        """Whether the response matrix is sparse."""
+        return self._resp_sparse
+
 
 class Spectrum:
-    """Class to handle spectrum data in OGIP standard.
+    """Handle spectral data in OGIP standards [1]_.
 
     Parameters
     ----------
     specfile : str
         Spectrum file path. For type II pha file, the row specifier must be
-        given in the end of path, e.g., ``specfile="./spec.pha2{1}"``.
+        given in the end of path, e.g., ``specfile='spec.pha2{1}'``.
     poisson : bool or None, optional
         Whether the spectrum data follows counting statistics, reading from
         the `specfile` header. This value must be set if ``POISSERR`` is
         undefined in the header.
 
+    References
+    ----------
+    .. [1] `The OGIP Spectral File Format <https://heasarc.gsfc.nasa.gov/docs/heasarc/ofwg/docs/spectra/ogip_92_007/ogip_92_007.html>`__
+            and `Addendum: Changes log <https://heasarc.gsfc.nasa.gov/docs/heasarc/ofwg/docs/spectra/ogip_92_007a/ogip_92_007a.html>`__
     """
 
-    def __init__(
-        self,
-        specfile: str,
-        poisson: bool | None = None
-    ):
+    def __init__(self, specfile: str, poisson: bool | None = None):
         # test if file is '/path/to/specfile{n}'
-        match = re.compile(r'(.+){(\d+)}').match(specfile)
+        match = re.compile(r'(.+){(.+)}').match(specfile)
         if match:
             file = match.group(1)
             type_ii = True  # spectrum file is of type II
             spec_id = int(match.group(2)) - 1  # row specifier to index
         else:
             file = specfile
             type_ii = False
@@ -586,35 +788,38 @@
         with fits.open(file) as hdul:
             header = hdul['SPECTRUM'].header
             data = hdul['SPECTRUM'].data
 
         # TODO: more robust way to detect a type II data
         # check if data is type II
         if not type_ii:
-            msg = f'row id must be provided for type II spectrum {specfile}'
+            msg = 'row id must be provided for type II spectrum, e.g., '
+            msg += f"'{specfile}{{1}}'"
 
             nchan = len(data)
             if int(header.get('DETCHANS', nchan)) != nchan:
                 raise ValueError(msg)
 
             if header.get('HDUCLAS4', '') == 'TYPE:II':
                 raise ValueError(msg)
 
         else:
-            data = data[spec_id].array  # set data to the specified row
+            data = data[spec_id : spec_id + 1]  # set data to the specified row
 
         # check if COUNTS or RATE exists
         if 'COUNTS' not in data.names and 'RATE' not in data.names:
             raise ValueError(f'"COUNTS" or "RATE" not found in {specfile}')
 
         # get poisson flag
         poisson = header.get('POISSERR', poisson)
         if poisson is None:
-            msg = '`poisson` must be set if "POISSERR" is undefined in header'
-            raise ValueError(msg)
+            raise PoissonFlagNotFoundError(
+                '"POISSERR" is undefined in header, `poisson` must be set in '
+                'Spectrum(..., poisson=True/False)'
+            )
 
         # check if STAT_ERR exists for non-Poisson spectrum
         if not poisson and 'STAT_ERR' not in data.names:
             raise ValueError(f'"STAT_ERR" not found in {specfile}')
 
         def get_field(field, default=None, excluded=None):
             """Get value of specified field, return default if not found."""
@@ -648,16 +853,19 @@
         else:
             stat_err = get_field('STAT_ERR')
             stat_err = np.array(stat_err, dtype=np.float64, order='C')
             if 'RATE' in data.names:
                 stat_err *= exposure
 
                 if 'COUNTS' in data.names:
-                    msg = f'"STAT_ERR" in {specfile} is assumed for "RATE"'
-                    warnings.warn(msg, Warning, stacklevel=3)
+                    warnings.warn(
+                        f'"STAT_ERR" in {specfile} is assumed for "RATE"',
+                        Warning,
+                        stacklevel=3,
+                    )
 
         # get fractional systematic error of counts
         sys_err = get_field('SYS_ERR', 0)
         if np.shape(sys_err) == () and sys_err == 0:
             sys_err = np.zeros(len(counts))
         else:
             sys_err = np.array(sys_err, dtype=np.float64, order='C')
@@ -672,41 +880,54 @@
         # get grouping flag
         grouping = get_field('GROUPING', 0)
         if np.shape(grouping) == () and grouping == 0:
             grouping = np.ones(len(counts), np.int64)
         else:
             grouping = np.array(grouping, dtype=np.int64, order='C')
 
-        if poisson:  # check if counts are integers
+        # check data
+        if poisson:
+            # check if counts are integers
             diff = np.abs(counts - np.round(counts))
             if np.any(diff > 1e-8 * counts):
-                msg = f'spectrum ({specfile}) has non-integer counts, '
-                msg += 'which may lead to wrong result'
-                warnings.warn(msg, Warning, stacklevel=3)
-
-        # check if statistical error are positive
-        mask = stat_err < 0.0
-        if np.any(mask):
-            stat_err[mask] = 0.0
-            msg = f'spectrum ({specfile}) has some statistical errors < 0, '
-            msg += 'which are reset to 0'
-            warnings.warn(msg, Warning, stacklevel=3)
-
-        # check if systematic error are positive
-        mask = sys_err < 0.0
-        if np.any(mask):
-            sys_err[mask] = 0.0
-            msg = f'spectrum ({specfile}) has some systematic errors < 0, '
-            msg += 'which are reset to 0'
-            warnings.warn(msg, Warning, stacklevel=3)
+                warnings.warn(
+                    f'poisson spectrum ({specfile}) has non-integer counts, '
+                    'which may lead to wrong result',
+                    Warning,
+                    stacklevel=3,
+                )
+        else:
+            # check if statistical errors are positive
+            if np.any(stat_err < 0.0):
+                raise ValueError(
+                    f'spectrum ({specfile}) has negative statistical errors'
+                )
+
+            if np.any(stat_err == 0.0):
+                warnings.warn(
+                    f'spectrum ({specfile}) has zero statistical errors, '
+                    'which may lead to wrong result under Gaussian statistics,'
+                    ' consider to group the spectrum',
+                    Warning,
+                    stacklevel=3,
+                )
+
+            # check if systematic errors are non-negative
+            if np.any(sys_err < 0.0):
+                raise ValueError(
+                    f'spectrum ({specfile}) has systematic errors < 0'
+                )
 
         # total error of counts
-        stat_var = np.square(stat_err)
-        sys_var = np.square(sys_err * counts)
-        error = np.sqrt(stat_var + sys_var)
+        if not poisson:
+            stat_var = np.square(stat_err)
+            sys_var = np.square(sys_err * counts)
+            error = np.sqrt(stat_var + sys_var)
+        else:
+            error = stat_err
 
         # search name in header
         excluded_name = ('', 'none', 'unknown')
         for key in ('DETNAM', 'INSTRUME', 'TELESCOP'):
             name = str(header.get(key, ''))
             if name.lower() not in excluded_name:
                 break
@@ -724,40 +945,39 @@
 
         # get ancrfile
         self._ancrfile = get_field('ANCRFILE', '', excluded_file)
 
         # get corrfile
         self._corrfile = get_field('CORRFILE', '', excluded_file)
 
-        # get background scaling factor
+        # get the background scaling factor
         back_scale = np.float64(get_field('BACKSCAL', 1.0))
-        if isinstance(back_scale, NDArray):
+        if isinstance(back_scale, np.ndarray):
             back_scale = np.array(back_scale, dtype=np.float64, order='C')
         else:
             back_scale = np.float64(back_scale)
         self._back_scale = back_scale
 
-        # get area scaling factor
+        # get the area scaling factor
         area_scale = get_field('AREASCAL', 1.0)
-        if isinstance(area_scale, NDArray):
+        if isinstance(area_scale, np.ndarray):
             area_scale = np.array(area_scale, dtype=np.float64, order='C')
         else:
             area_scale = np.float64(area_scale)
         self._area_scale = area_scale
 
-        # get correction scaling factor
+        # get the correction scaling factor
         self._corr_scale = np.float64(get_field('CORRSCAL', 0.0))
 
         self._header = header
         self._data = data
         self._counts = self._raw_counts = counts
         self._error = self._raw_error = error
         self._grouping = grouping
         self._exposure = exposure
-        self._eff_exposure = exposure * area_scale * back_scale
         self._poisson = poisson
         self._quality = quality
 
     def group(self, grouping: NDArray, noticed: NDArray | None):
         """Group spectrum channel.
 
         Parameters
@@ -773,39 +993,46 @@
         NotImplementedError
             Grouping is not yet implemented for spectrum with ``AREASCAL``
             and/or ``BACKSCAL`` array.
 
         Notes
         -----
         If there are ignored channels in a channel group, this may cause an
-        inconsistency in a spectral plot, i.e., the error bar of a channel
-        group will cover these bad channels, whilst these bad channels are
-        never used in fitting.
-
+        inconsistency in a spectral plot. That is to say, the error bar of a
+        channel group will cover these bad channels, whilst these bad channels
+        are never used in fitting.
         """
+        # TODO:
+        #   * area_scale array grouping info can be hardcode into grouped
+        #     response matrix when calculating model
+        #   * back_scale array grouping info can be ...? using average?
+        #   * net counts and model folding calculation should be re-implemented
+        #     in likelihood and helper modules
         if not () == np.shape(self.area_scale) == np.shape(self.back_scale):
-            msg = 'grouping is not implemented yet for the spectrum with '
-            msg += '``AREASCAL`` and/or ``BACKSCAL`` array'
-            raise NotImplementedError(msg)
+            raise NotImplementedError(
+                'grouping is not implemented yet for the spectrum with '
+                '``AREASCAL`` and/or ``BACKSCAL`` array'
+            )
 
         l0 = len(self._raw_counts)
         if noticed is None:
             noticed = np.full(l0, True)
         else:
             l1 = len(grouping)
             l2 = len(noticed)
             if not l0 == l1 == l2:
-                msg = f'length of grouping ({l1}) and noticed ({l2}) must be '
-                msg += f'matched to spectrum channel ({l0})'
-                raise ValueError(msg)
+                raise ValueError(
+                    f'length of grouping ({l1}) and noticed ({l2}) must be '
+                    f'matched to spectrum channel ({l0})'
+                )
 
             noticed = np.array(noticed, dtype=bool)
 
         factor = noticed.astype(np.float64)
-        grp_idx = np.flatnonzero(grouping == 1)  # transform to index
+        grp_idx = np.flatnonzero(grouping != -1)  # transform to index
         non_empty = np.add.reduceat(factor, grp_idx) != 0
 
         counts = np.add.reduceat(factor * self._raw_counts, grp_idx)
         counts = counts[non_empty]
 
         var = factor * self._raw_error * self._raw_error
         var = np.add.reduceat(var, grp_idx)[non_empty]
@@ -831,24 +1058,19 @@
 
     @property
     def quality(self) -> NDArray:
         """Quality flag indicating which channel to be used in analysis."""
         return self._quality
 
     @property
-    def exposure(self) -> float:
+    def exposure(self) -> np.float64:
         """Exposure time of the spectrum, in unit of second."""
         return self._exposure
 
     @property
-    def eff_exposure(self) -> float | NDArray:
-        """Effective exposure, corrected with area and background scaling."""
-        return self._eff_exposure
-
-    @property
     def poisson(self) -> bool:
         """Whether the spectrum data follows counting statistics."""
         return self._poisson
 
     @property
     def name(self) -> str:
         """``DETNAM``, ``INSTRUME`` or ``TELESCOP`` in `specfile` header."""
@@ -871,215 +1093,464 @@
 
     @property
     def corrfile(self) -> str:
         """Correction file."""
         return self._corrfile
 
     @property
-    def back_scale(self) -> float | NDArray:
+    def back_scale(self) -> np.float64 | NDArray:
         """Background scaling factor."""
         return self._back_scale
 
     @property
-    def area_scale(self) -> float | NDArray:
+    def area_scale(self) -> np.float64 | NDArray:
         """Area scaling factor."""
         return self._area_scale
 
     @property
-    def corr_scale(self) -> float:
+    def corr_scale(self) -> np.float64:
         """Correction scaling factor."""
         return self._corr_scale
 
 
 class Response:
-    """Class to store and group telescope response.
+    """Handle telescope response in OGIP standards [1]_.
 
     Parameters
     ----------
     respfile : str
         Response file path.
     ancrfile : str or None, optional
         Ancillary response path. The default is None.
 
+    References
+    ----------
+    .. [1] `The Calibration Requirements for Spectral Analysis (Definition of
+            RMF and ARF file formats) <https://heasarc.gsfc.nasa.gov/docs/heasarc/caldb/docs/memos/cal_gen_92_002/cal_gen_92_002.html>`__
+            and `Addendum: Changes log <https://heasarc.gsfc.nasa.gov/docs/heasarc/caldb/docs/memos/cal_gen_92_002a/cal_gen_92_002a.html>`__
     """
 
+    _fwhm: NDArray | None = None
+    _ch_fwhm: NDArray | None = None
+
     def __init__(self, respfile: str, ancrfile: str | None = None):
-        with fits.open(respfile) as rsp_hdul:
-            ebounds = rsp_hdul['EBOUNDS'].data
+        if ancrfile is None:
+            ancrfile = ''
+
+        self._respfile = respfile
+        self._ancrfile = ancrfile
+
+        # test if file is '/path/to/respfile{n}'
+        match = re.compile(r'(.+){(.+)}').match(respfile)
+        if match:  # respfile file is of type II
+            file = match.group(1)
+            resp_id = int(match.group(2))
+        else:
+            file = respfile
+            resp_id = 1
 
+        with fits.open(file) as rsp_hdul:
             if 'MATRIX' in rsp_hdul:
-                resp = rsp_hdul['MATRIX'].data
+                if ancrfile is None:
+                    warnings.warn(
+                        f'{file} is probably a rmf, '
+                        'ancrfile (arf) maybe needed but not provided',
+                        Warning,
+                    )
+
+                ext = ('MATRIX', resp_id)
+
             elif 'SPECRESP MATRIX' in rsp_hdul:
-                resp = rsp_hdul['SPECRESP MATRIX'].data
+                ext = ('SPECRESP MATRIX', resp_id)
 
-        channel = ebounds['CHANNEL']
+            else:
+                raise ValueError(
+                    f'cannot read response matrix data from {respfile}'
+                )
 
-        # assume ph_egrid is continuous
-        ph_egrid = np.append(resp['ENERG_LO'], resp['ENERG_HI'][-1])
-        ph_egrid = np.asarray(ph_egrid, dtype=np.float64, order='C')
-        ch_egrid = np.column_stack((ebounds['E_MIN'], ebounds['E_MAX']))
+            self._read_ebounds(rsp_hdul['EBOUNDS'].data)
+            self._read_resp(rsp_hdul[ext].header, rsp_hdul[ext].data)
+
+        self._read_ancrfile()
+        # self._drop_zeros()
+
+    def _read_ebounds(self, ebounds_data):
+        ch_emin = ebounds_data['E_MIN']
+        ch_emax = ebounds_data['E_MAX']
+        if np.any(ch_emin > ch_emax):
+            raise ValueError(
+                f'respfile ({self._respfile}) channel energy grids are not '
+                'increasing'
+            )
+        ch_egrid = np.column_stack((ch_emin, ch_emax))
         ch_egrid = np.asarray(ch_egrid, dtype=np.float64, order='C')
+        self._channel_egrid = self._raw_channel_egrid = ch_egrid
+
+    def _read_resp(self, resp_header, resp_data):
+        # check and read photon energy grid
+        if not np.allclose(
+            resp_data['ENERG_LO'][1:], resp_data['ENERG_HI'][:-1]
+        ):
+            raise ValueError(
+                f'respfile ({self._respfile}) photon energy grids exist '
+                'discontinuity'
+            )
+
+        if np.any(resp_data['ENERG_LO'] > resp_data['ENERG_HI']):
+            raise ValueError(
+                f'respfile ({self._respfile}) photon energy grids are not '
+                'increasing'
+            )
+
+        ph_egrid = np.append(resp_data['ENERG_LO'], resp_data['ENERG_HI'][-1])
+        ph_egrid = np.asarray(ph_egrid, dtype=np.float64, order='C')
+        self._ph_egrid = ph_egrid
 
-        # extract response matrix
-        matrix = resp['MATRIX']
+        # check and read response matrix
+        nchan = resp_header.get('DETCHANS', None)
+        if nchan is None:
+            raise ValueError(
+                f'keyword "DETCHANS" not found in "{self._respfile}" header'
+            )
+        else:
+            nchan = int(nchan)
 
-        # wrap around N/A of matrix
-        nch = len(ch_egrid)
-        nch_matrix = np.array([len(i) for i in matrix])
-        if np.any(nch_matrix != nch):
-            # inhomogeneous matrix is due to zero elements being discarded
-            # here we put zeros back in
-            mask = np.less(np.arange(nch), nch_matrix[:, None])
-            matrix_flatten = np.concatenate(matrix, dtype=np.float64)
-            matrix = np.zeros(mask.shape)
-            matrix[mask] = matrix_flatten
+        fchan_idx = resp_data.names.index('F_CHAN') + 1
+        # set the first channel number to 1 if not found
+        first_chan = int(resp_header.get(f'TLMIN{fchan_idx}', 1))
+
+        channel = tuple(str(c) for c in range(first_chan, first_chan + nchan))
+        self._raw_channel = channel
+        self._channel = tuple((c,) for c in channel)
+
+        n_grp = resp_data['N_GRP']
+        f_chan = resp_data['F_CHAN'] - first_chan
+        n_chan = resp_data['N_CHAN']
+
+        # if ndim == 1 and dtype is 'O', it is an array of array
+        if f_chan.ndim == 1 and f_chan.dtype != np.dtype('O'):
+            # f_chan is scalar in each row, make it an array
+            f_chan = f_chan[:, None]
+
+        if n_chan.ndim == 1 and n_chan.dtype != np.dtype('O'):
+            # n_chan is scalar in each row, make it an array
+            n_chan = n_chan[:, None]
+
+        # the last channel numbers
+        e_chan = f_chan + n_chan
+
+        rows = np.hstack(
+            tuple(np.full(round(n.sum()), i) for i, n in enumerate(n_chan))
+        )
+        cols = []
+        for i in range(len(resp_data)):
+            n = int(n_grp[i])  # n channel subsets
+            if n > 0:
+                f = f_chan[i].astype(int)  # first channel numbers of subsets
+                e = e_chan[i].astype(int)  # last channel numbers of subsets
+                cols.extend(map(np.arange, f, e))
+        cols = np.hstack(cols)
+
+        matrix = resp_data['MATRIX'].ravel()
+        if matrix.dtype != np.dtype('O'):
+            reduced_matrix = matrix
+        else:
+            reduced_matrix = np.hstack(matrix)
+        self._sparse_matrix = coo_array(
+            (reduced_matrix, (rows, cols)), shape=(len(resp_data), nchan)
+        )
+        self._sparse_matrix.eliminate_zeros()
+        self._matrix = self._sparse_matrix
+
+    def _read_ancrfile(self):
+        ancrfile = self._ancrfile
 
-        # read in ancrfile if exists
         if ancrfile:
             with fits.open(ancrfile) as arf_hdul:
                 arf = arf_hdul['SPECRESP'].data['SPECRESP']
 
-            if len(arf) != len(matrix):
-                msg = f'rmf ({respfile}) and arf ({ancrfile}) are not matched'
-                raise ValueError(msg)
+            if len(arf) != self._sparse_matrix.shape[0]:
+                respfile = self._respfile
+                raise ValueError(
+                    f'rmf ({respfile}) and arf ({ancrfile}) are not matched'
+                )
 
-            matrix *= arf[:, None]
+            self._sparse_matrix *= arf[:, None]
+            self._matrix = self._sparse_matrix
 
-        # drop the zero entries at the beginning or end of photon energy grid
-        zero_mask = np.all(np.less_equal(matrix, 0.0), axis=1)
+    def _drop_zeros(self):
+        """Remove leading or trailing rows filled with 0 from the matrix."""
+        matrix = self._sparse_matrix
+        ph_egrid = self._ph_egrid
+        nonzero_rows = np.unique(matrix.nonzero()[0])
+        nonzero_mask = np.isin(range(matrix.shape[0]), nonzero_rows)
+        zero_mask = np.bitwise_not(nonzero_mask)
         if zero_mask.any():
             n_entries = len(ph_egrid) - 1
             last_idx = len(ph_egrid) - 2
             idx = np.flatnonzero(zero_mask)
             diff = np.diff(idx)
             if len(diff) == 0:  # only one zero entry
                 idx = idx[0]
-                if idx in (0, last_idx):  # the beginning/end of grid
-                    matrix = matrix[~zero_mask]
+                if idx in (0, last_idx):  # check if idx is leading or trailing
                     if idx == 0:
                         ph_egrid = ph_egrid[1:]
                     else:
                         ph_egrid = ph_egrid[:-1]
             else:
                 splits = np.split(idx, np.nonzero(np.diff(idx) > 1)[0] + 1)
                 zeros_mask2 = np.full(n_entries, False)
                 for s in splits:
                     if np.isin(s, (0, last_idx)).any():
-                        # drop only if at beginning or ending part of the grid
+                        # only drop leading or trailing part of grids
                         zeros_mask2[s] = True
 
                 elo = ph_egrid[:-1][~zeros_mask2]
                 ehi = ph_egrid[1:][~zeros_mask2]
                 ph_egrid = np.append(elo, ehi[-1])
 
+        self._sparse_matrix = self._matrix = matrix.tocsr()[~zero_mask]
         self._ph_egrid = ph_egrid
-        self._channel = self._raw_channel = channel
-        self._channel_egrid = self._raw_channel_egrid = ch_egrid
-        self._matrix = self._raw_matrix = matrix
 
     def group(self, grouping: NDArray, noticed: NDArray | None = None):
         """Group response matrix.
 
         Parameters
         ----------
         grouping : ndarray
             Channel with a grouping flag of 1 with all successive channels
             with grouping flags of -1 are combined.
         noticed : ndarray or None, optional
             Flag indicating which channel to be used in grouping.
-
         """
         l0 = len(self._raw_channel)
 
         if noticed is None:
             noticed = np.full(l0, True)
 
         l1 = len(grouping)
         l2 = len(noticed)
         if not l0 == l1 == l2:
-            msg = f'length of grouping ({l1}) and good ({l2}) must match to '
-            msg += f'original channel ({l0})'
-            raise ValueError(msg)
+            raise ValueError(
+                f'length of grouping ({l1}) and good ({l2}) must match to '
+                f'original channel ({l0})'
+            )
 
-        grp_idx = np.flatnonzero(grouping == 1)  # transform to index
+        grp_idx = np.flatnonzero(grouping != -1)  # transform to index
 
         if len(grp_idx) == l0:  # case of no group, apply good mask
-            self._channel = self._raw_channel[noticed]
-            self._channel_egrid = self._raw_channel_egrid[noticed]
-            self._matrix = self._raw_matrix[:, noticed]
+            if np.count_nonzero(noticed) != noticed.size:
+                channel = np.array(self._raw_channel)[noticed]
+                self._channel = tuple((c,) for c in channel)
+                self._channel_egrid = self._raw_channel_egrid[noticed]
+                self._matrix = self._sparse_matrix.tocsc()[:, noticed]
 
         else:
-            non_empty = np.add.reduceat(noticed, grp_idx) != 0
+            non_empty = np.greater(np.add.reduceat(noticed, grp_idx), 0)
 
             edge_indices = np.append(grp_idx, l0)
             channel = self._raw_channel
             emin, emax = self._raw_channel_egrid.T
             group_channel = []
             group_emin = []
             group_emax = []
 
             for i in range(len(grp_idx)):
                 if not non_empty[i]:
                     continue
                 slice_i = slice(edge_indices[i], edge_indices[i + 1])
                 quality_slice = noticed[slice_i]
-                channel_slice = channel[slice_i]
-                group_channel.append(channel_slice[quality_slice].astype(str))
+                channel_slice = np.array(channel[slice_i])[quality_slice]
+                group_channel.append(tuple(channel_slice))
                 group_emin.append(min(emin[slice_i]))
                 group_emax.append(max(emax[slice_i]))
 
-            self._channel = tuple(map(lambda g: tuple(g), group_channel))
+            self._channel = tuple(group_channel)
             self._channel_egrid = np.column_stack([group_emin, group_emax])
 
             a = np.where(noticed, 1.0, 0.0)
-            matrix = np.add.reduceat(a * self._raw_matrix, grp_idx, axis=1)
-            self._matrix = matrix[:, non_empty]
+            n = self._sparse_matrix.shape[1]
+            idx = np.arange(n)
+            ptr = np.append(grp_idx, n)
+            grouping_matrix = csc_array((a, idx, ptr))
+            matrix = self._sparse_matrix.dot(grouping_matrix)
+            self._matrix = matrix.tocsc()[:, non_empty]
+
+    def plot(self, hatch_range: NDArray | None = None):
+        """Plot the response matrix.
+
+        Parameters
+        ----------
+        hatch_range : ndarray, optional
+            Energy range to add hatches.
+        """
+        ch_emin, ch_emax = self._raw_channel_egrid.T
+        matrix = self._sparse_matrix.todense()
+
+        # some response matrix has discontinuity in channel energy grid,
+        # insert np.nan to handle this
+        idx = np.flatnonzero(ch_emin[1:] - ch_emax[:-1])
+        if len(idx) > 0:
+            ch_emin = np.insert(ch_emin, idx + 1, ch_emax[idx])
+            ch_emax = np.insert(ch_emax, idx + 1, ch_emin[idx + 1])
+            matrix = np.insert(matrix, idx + 1, np.nan, axis=1)
+
+        ch_egrid = np.append(ch_emin, ch_emax[-1])
+        ch, ph = np.meshgrid(ch_egrid, self._ph_egrid)
+        plt.figure()
+        plt.pcolormesh(ch, ph, matrix, cmap='jet')
+        plt.xlabel('Measurement Energy [keV]')
+        plt.ylabel('Photon Energy [keV]')
+        plt.colorbar(label='Effective Area [cm$^2$]')
+        plt.xscale('log')
+        plt.yscale('log')
+
+        if hatch_range is not None:
+            hatch_range = np.atleast_2d(hatch_range)
+            emin = np.expand_dims(hatch_range[:, 0], axis=1)
+            emax = np.expand_dims(hatch_range[:, 1], axis=1)
+            mask1 = np.less_equal(emin, ch_emin)
+            mask2 = np.less_equal(ch_emax, emax)
+            idx = [np.flatnonzero(i) for i in np.bitwise_and(mask1, mask2)]
+
+            ignored = []
+            if ch_emin[idx[0][0]] > ch_emin[0]:
+                ignored.append((ch_emin[0], ch_emin[idx[0][0]]))
+            for i in range(len(idx) - 1):
+                this_noticed_right = ch_emax[idx[i][-1]]
+                next_noticed_left = ch_emin[idx[i + 1][0]]
+                ignored.append((this_noticed_right, next_noticed_left))
+            if ch_emax[idx[-1][-1]] < ch_emax[-1]:
+                ignored.append((ch_emax[idx[-1][-1]], ch_emax[-1]))
+
+            y = (self._ph_egrid[0], self._ph_egrid[-1])
+            for i in ignored:
+                plt.fill_betweenx(y, *i, alpha=0.4, color='w', hatch='x')
+
+        plt.show()
 
     @property
     def ph_egrid(self) -> NDArray:
-        """Photon energy grid."""
+        """Monte Carlo photon energy grid."""
         return self._ph_egrid
 
     @property
     def channel(self) -> tuple:
-        """Measured channel numbers."""
+        """Measurement channel numbers."""
         return self._channel
 
     @property
     def ch_emin(self) -> NDArray:
-        """Left edge of measured energy grid."""
+        """Left edge of measurement energy grid."""
         return self._channel_egrid[:, 0]
 
     @property
     def ch_emax(self) -> NDArray:
-        """Right edge of measured energy grid."""
+        """Right edge of measurement energy grid."""
         return self._channel_egrid[:, 1]
 
     @property
     def ch_emid(self) -> NDArray:
-        """Middle of measured energy grid."""
+        """Middle of measurement energy grid."""
         return np.mean(self._channel_egrid, axis=1)
 
     @property
     def ch_width(self) -> NDArray:
-        """Width of measured energy grid."""
+        """Width of measurement energy grid."""
         return self._channel_egrid[:, 1] - self._channel_egrid[:, 0]
 
     @property
     def ch_mean(self) -> NDArray:
-        """Geometric mean of measured energy grid."""
+        """Geometric mean of measurement energy grid."""
         return np.sqrt(np.prod(self._channel_egrid, axis=1))
 
     @property
     def ch_error(self) -> NDArray:
         """Width between left/right and geometric mean of energy grid."""
         mean = self.ch_mean
         return np.abs([self.ch_emin - mean, self.ch_emax - mean])
 
     @property
     def matrix(self) -> NDArray:
         """Response matrix."""
+        return self._matrix.todense()
+
+    @property
+    def sparse_matrix(self):
+        """Sparse representation of the response matrix."""
         return self._matrix
 
+    @property
+    def fwhm(self) -> NDArray:
+        """Estimated Full Width at Half Maximum (FWHM) in photon energy space.
+
+        .. note::
+            The calculation code is translated from ``heasp``. This does assume
+            that the response has a well-defined main peak and operates by the
+            simple method of stepping out from the peak in both directions till
+            the response falls below half the maximum. A better solution would
+            obviously be to fit a gaussian.
+        """
+        if self._fwhm is not None:
+            return self._fwhm
+
+        matrix = self._sparse_matrix
+        csr_matrix = matrix.tocsr()
+        nE, nC = matrix.shape
+        row_idx = np.arange(nE)
+        argmax = np.squeeze(matrix.argmax(axis=1))
+        max_value = csr_matrix[row_idx, argmax]
+        half_max = 0.5 * max_value
+        i, j = np.nonzero(matrix <= half_max[:, None])
+        idx_low_high = np.column_stack([argmax - 1, argmax + 1])
+        for iE in range(nE):
+            imax = argmax[iE]
+            idx = j[i == iE]  # rsp elements of iE row at idx are <= half_max
+            if idx.size:
+                mask = idx < imax
+                # find the right-most lower index
+                k = np.flatnonzero(mask)
+                lower = idx[k[-1]] if k.size else imax - 1
+                # find the left-most upper index
+                k = np.flatnonzero(~mask)
+                upper = idx[k[0]] if k.size else imax + 1
+                idx_low_high[iE] = [lower, upper]
+        ilow, ihigh = np.clip(idx_low_high, 0, nC - 1).T
+        good_low = csr_matrix[row_idx, [0] * nE] <= half_max
+        good_high = csr_matrix[row_idx, [-1] * nE] <= half_max
+        fwhm = np.full(nE, 0)
+        fwhm[good_high] += ihigh[good_high] - argmax[good_high]
+        fwhm[good_low] += argmax[good_low] - ilow[good_low]
+        fwhm[(good_high & (~good_low)) | ((~good_high) & good_low)] *= 2
+        fwhm = np.clip(fwhm, 1, None)  # set minimum FWHM to 1
+        fwhm[~(good_high | good_low)] = -1
+        self._fwhm = fwhm
+        return self._fwhm
+
+    @property
+    def ch_fwhm(self) -> NDArray:
+        """Estimated Full Width at Half Maximum (FWHM) in channel energy space.
+
+        .. note::
+            The calculation code is translated from ``heasp``. The calculation
+            interpolates the `estimated_fwhm` using the nominal channel energy
+            to give the FWHM for each channel. Assuming that FWHM does not
+            change significantly over the channel, so just find the FWHM at the
+            center energy of the channel.
+        """
+        if self._ch_fwhm is not None:
+            return self._ch_fwhm
+
+        fwhm = self.fwhm
+        ch_emid = self._raw_channel_egrid.mean(1)
+        idx = np.searchsorted(self.ph_egrid, ch_emid) - 1
+        idx = np.clip(idx, 0, len(fwhm) - 1)
+        self._ch_fwhm = fwhm[idx]
+        return self._ch_fwhm
+
+
+class GroupingWaring(Warning):
+    """Issued by grouping scale not being met for all channel groups."""
+
 
-class GroupWaring(Warning):
-    """Issued by grouping scale not being met for all channels."""
+class PoissonFlagNotFoundError(RuntimeError):
+    """Issued by ``POISSERR`` not found in spectrum header."""
```

### Comparing `elisa_lib-0.0.1.dev1/src/elisa/model/base.py` & `elisa_lib-0.1.0/src/elisa/models/parameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,898 +1,1061 @@
-"""Module to handle model construction."""
-# TODO:
-#    - model construction and parameter binding should be separated
-#    - transformable to other PPL libs
-#    - time-dependent model
+"""The parameter."""
+
 from __future__ import annotations
 
-from abc import ABC, ABCMeta, abstractmethod
-from typing import Callable, Union
+from abc import ABC, abstractmethod
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, NamedTuple, get_args
 
 import jax.numpy as jnp
 from numpyro.distributions import Distribution, LogUniform, Uniform
 
-from .node import (
-    LabelSpace,
-    ModelNode,
-    ModelOperationNode,
-    ParameterNode,
-    ParameterOperationNode,
-)
+from elisa.util.integrate import AdaptQuadMethod, make_integral_factory
+from elisa.util.misc import build_namespace
 
-ModelNodeType = Union[ModelNode, ModelOperationNode]
-ParameterNodeType = Union[ParameterNode, ParameterOperationNode]
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from typing import Any, Callable, Literal
+
+    # from tinygp import kernels, means, noise
+    from elisa.util.integrate import IntegralFactory
+    from elisa.util.typing import (
+        CompID,
+        CompParamName,
+        JAXArray,
+        JAXFloat,
+        ParamID,
+        ParamIDStrMapping,
+        ParamIDValMapping,
+    )
+
+
+class AssignmentTracker:
+    """Track component assignment of a parameter."""
+
+    def __init__(self):
+        self._history = []
+
+    def append(self, cid: CompID, pname: CompParamName) -> None:
+        """Append a new assignment record."""
+        record = (cid, pname)
+        if record not in self._history:
+            self._history.append((cid, pname))
+
+    def remove(self, cid: CompID, pname: CompParamName) -> None:
+        """Remove an assignment record."""
+        self._history.remove((cid, pname))
 
-# __all__ = ['UniformParameter', ]
+    def get_comp_param(
+        self,
+        comp_ids: Iterable[CompID],
+    ) -> tuple[CompID, CompParamName] | None:
+        """Get the earliest component assignment record within comp_ids."""
+        id_set = set(comp_ids)
+        flag = [i[0] in id_set for i in self._history]
+        if any(flag):
+            return self._history[flag.index(True)]
+        else:
+            return None
 
 
-class Parameter:
-    """Prototype parameter class.
+class ParamInfo(NamedTuple):
+    """Parameter information."""
 
-    Parameters
-    ----------
-    node : ParameterNode, or ParameterOperationNode
-        The base parameter node.
+    name: str | Callable[[ParamIDStrMapping], str]
+    """Plain name of the parameter.
 
+    It is a getter function for composite parameter.
     """
 
-    def __init__(self, node: ParameterNodeType):
-        if not isinstance(node, (ParameterNode, ParameterOperationNode)):
-            raise ValueError(
-                "node must be ParameterNode or ParameterOperationNode"
+    latex: str | Callable[[ParamIDStrMapping], str]
+    r""":math:`\LaTeX` format of the parameter.
+
+    It is a getter function for composite parameter.
+    """
+
+    default: Any
+    """Default value of the parameter."""
+
+    bound: str
+    """Value bound expression of the parameter."""
+
+    prior: str
+    """Prior distribution expression of the parameter."""
+
+    log: bool
+    """Whether the parameter is parameterized in a logarithmic scale."""
+
+    fixed: bool
+    """Whether the parameter is fixed."""
+
+    tracker: AssignmentTracker
+    """Component assignment tracker."""
+
+    id_to_value: Callable[[ParamIDValMapping], JAXFloat]
+    """Mapping function from id to value."""
+
+    dist: Distribution | None = None
+    """NumPyro distribution for the parameter."""
+
+    composite: bool = False
+    """Whether the parameter is composite."""
+
+    integrate: IntegralFactory | bool = False
+    """Integration factory for the parameter for interval parameter.
+
+    For composite parameter composed by interval parameter, this is True.
+    """
+
+
+class Parameter(ABC):
+    """Parameter base."""
+
+    _id: ParamID
+    _tracker: AssignmentTracker
+    _nodes_id: tuple[ParamID, ...]
+
+    def __init__(self):
+        self._id = hex(id(self))[2:]
+        self._tracker = AssignmentTracker()
+        self._nodes_id = (self._id,)
+
+    def _id_to_label(
+        self,
+        mapping: ParamIDStrMapping,
+        label_type: Literal['name', 'latex'],
+    ) -> str:
+        """Get the label of the parameter."""
+        if label_type not in {'name', 'latex'}:
+            raise ValueError(f'unknown label type: {label_type}')
+
+        return mapping[self._id]
+
+    @property
+    def _id_to_value(self) -> Callable[[ParamIDValMapping], JAXFloat]:
+        """Gets the mapping function from id to value."""
+        pid = self._id
+        default = self.default
+
+        def id_to_value(mapping: ParamIDValMapping) -> JAXFloat:
+            """Get the value of the parameter from mapping."""
+            return mapping.get(pid, default)
+
+        return id_to_value
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """Plain name of the parameter."""
+        pass
+
+    @property
+    @abstractmethod
+    def latex(self) -> str:
+        r""":math:`\LaTeX` format of the parameter."""
+        pass
+
+    @property
+    @abstractmethod
+    def default(self) -> JAXFloat:
+        """Default value of the parameter."""
+        pass
+
+    @property
+    @abstractmethod
+    def log(self) -> bool:
+        """Whether the parameter is parameterized in a logarithmic scale."""
+        pass
+
+    @property
+    @abstractmethod
+    def fixed(self) -> bool:
+        """Whether the parameter is fixed."""
+        pass
+
+    @property
+    @abstractmethod
+    def _info(self) -> dict[ParamID, ParamInfo]:
+        """Parameter information."""
+        pass
+
+    def __str__(self) -> str:
+        return self.name
+
+    def __repr__(self) -> str:
+        return self.name
+
+    def __add__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(self, other, '+')
+
+    def __radd__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(other, self, '+')
+
+    def __sub__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(self, other, '-')
+
+    def __rsub__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(other, self, '-')
+
+    def __mul__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(self, other, '*')
+
+    def __rmul__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(other, self, '*')
+
+    def __truediv__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(self, other, '/')
+
+    def __rtruediv__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(other, self, '/')
+
+    def __pow__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(self, other, '^')
+
+    def __rpow__(self, other: Parameter) -> CompositeParameter:
+        return self._make_composite_parameter(other, self, '^')
+
+    @staticmethod
+    def _make_composite_parameter(
+        lhs: Parameter,
+        rhs: Parameter,
+        op: Literal['+', '-', '*', '/', '^'],
+    ) -> CompositeParameter:
+        # check if the type of lhs and rhs are both parameter
+        if not (isinstance(lhs, Parameter) and isinstance(rhs, Parameter)):
+            raise TypeError(
+                f'unsupported operand types for {op}: '
+                f"'{type(lhs).__name__}' and '{type(rhs).__name__}'"
             )
 
-        self._node = node
+        op_symbol = op
+
+        if op == '+':
+            op = jnp.add
+            op_name = '{} + {}'
+            op_latex = '{{{}}} + {{{}}}'
+        elif op == '-':
+            op = jnp.subtract
+            op_name = '{} - {}'
+            op_latex = '{{{}}} - {{{}}}'
+        elif op == '*':
+            op = jnp.multiply
+            op_name = '{} * {}'
+            op_latex = r'{{{}}} \times {{{}}}'
+        elif op == '/':
+            op = jnp.divide
+            op_name = '{} / {}'
+            op_latex = r'{{{}}} / {{{}}}'
+        elif op == '^':
+            op = jnp.power
+            op_name = '{}^{}'
+            op_latex = r'{{{}}}^{{{}}}'
+        else:
+            raise NotImplementedError(f'op {op}')
+
+        return CompositeParameter(
+            params=[lhs, rhs],
+            op=op,
+            op_name=op_name,
+            op_latex=op_latex,
+            op_symbol=op_symbol,
+        )
+
+
+class ParameterHelper(Parameter):
+    """Handle name, latex, and default value of a parameter."""
+
+    def __init__(
+        self,
+        name: str,
+        latex: str | None,
+        default: Any | None = None,
+    ):
+        if latex is None:
+            latex = name
+
+        self._name = name
+        self.latex = latex
+
+        if default is not None:
+            self.default = default
+
+        super().__init__()
 
-    def __repr__(self):
-        return self._node.attrs['name']
+    @property
+    def name(self) -> str:
+        return self._name
 
-    def __add__(self, other: Parameter) -> SuperParameter:
-        return SuperParameter(self, other, '+')
+    @property
+    def latex(self) -> str:
+        return self._latex
 
-    def __mul__(self, other: Parameter) -> SuperParameter:
-        return SuperParameter(self, other, '*')
+    @latex.setter
+    def latex(self, latex):
+        self._latex = str(latex)
 
     @property
-    def default(self) -> float:
-        """Parameter default value."""
-        return self._node.default
+    @abstractmethod
+    def default(self) -> Any:
+        pass
 
     @default.setter
-    def default(self, value: float):
-        """Parameter default value."""
-        self._node.default = value
+    @abstractmethod
+    def default(self, value: Any):
+        pass
 
 
-class SuperParameter(Parameter):
-    """Class to handle operation on parameters.
+class DistParameter(ParameterHelper):
+    r"""Parameter definition given a distribution.
 
     Parameters
     ----------
-    lh: Parameter
-        Left-hand parameter.
-    rh: Parameter
-        Right-hand parameter.
-    op : {'+', '*'}
-        Operation to perform.
-
+    name : str
+        Parameter name.
+    dist : Distribution
+        Numpyro distribution to which the parameter is sampled.
+    default : float
+        Parameter default value.
+    min : float, optional
+        Parameter minimum value, for display purpose only. The default is None.
+    max : float, optional
+        Parameter maximum value, for display purpose only. The default is None.
+    log : bool, optional
+        Whether the parameter is parameterized in a logarithmic scale.
+        The default is False.
+    fixed : bool, optional
+        Whether the parameter is fixed. The default is False.
+    latex : str, optional
+        :math:`\LaTeX` format of the parameter. The default is as `name`.
     """
 
-    def __init__(self, lh: Parameter, rh: Parameter, op: str):
-        if op not in {'+', '*'}:
-            raise TypeError(f'operator "{op}" is not supported')
-
-        if not isinstance(lh, Parameter):
-            raise TypeError(f'{lh} is not a valid parameter')
-
-        if not isinstance(rh, Parameter):
-            raise TypeError(f'{rh} is not a valid parameter')
+    def __init__(
+        self,
+        name: str,
+        dist: Distribution,
+        default: float,
+        *,
+        min: float | None = None,
+        max: float | None = None,
+        log: bool = False,
+        fixed: bool = False,
+        latex: str | None = None,
+    ):
+        if not isinstance(dist, Distribution):
+            raise ValueError('prior must be a numpyro distribution')
 
-        self._op = op
-        self._lh = lh
-        self._rh = rh
+        if jnp.shape(default) != ():
+            raise ValueError('default must be a scalar')
 
-        if op == '+':
-            node = lh._node + rh._node
-        else:  # op == '*'
-            node = lh._node * rh._node
+        if not bool(dist._validate_sample(default)):
+            raise ValueError('default should be within the prior support')
 
-        super().__init__(node)
+        self._dist = dist
+        self._default = jnp.asarray(default, float)
 
-    def __repr__(self):
-        if isinstance(self._lh, UniformParameter):
-            lh = self._lh._node.attrs['name']
+        if min is None:
+            self._min = None
         else:
-            lh = repr(self._lh)
+            if jnp.shape(min) != ():
+                raise ValueError('min must be a scalar')
+            self._min = jnp.asarray(min, float)
 
-        if isinstance(self._rh, UniformParameter):
-            rh = self._rh._node.attrs['name']
+        if max is None:
+            self._max = None
         else:
-            rh = repr(self._rh)
+            if jnp.shape(max) != ():
+                raise ValueError('max must be a scalar')
+            self._max = jnp.asarray(max, float)
+
+        self._log = bool(log)
+        self._fixed = bool(fixed)
+
+        super().__init__(name, latex, default)
+
+    @property
+    def default(self) -> JAXFloat:
+        return self._default
+
+    @default.setter
+    def default(self, default: float):
+        if jnp.shape(default) != ():
+            raise ValueError('default must be a scalar')
 
-        op = self._op
+        if not bool(self._dist._validate_sample(default)):
+            raise ValueError('default should be within the dist support')
 
-        if op == '*':
-            if getattr(self._lh, '_op', '') == '+':
-                lh = f'({lh})'
+        self._default = jnp.asarray(default, float)
 
-            if getattr(self._rh, '_op', '') == '+':
-                rh = f'({rh})'
+    @property
+    def log(self) -> bool:
+        return self._log
 
-        return f'{lh} {op} {rh}'
+    @property
+    def fixed(self) -> bool:
+        return self._fixed
 
     @property
-    def default(self) -> float:
-        """Parameter default value, get only."""
-        return self._node.default
+    def _dist_expr(self) -> str:
+        dist = self._dist
+        name = dist.__class__.__name__
+        args = [
+            f'{arg}={getattr(dist, arg):.4g}'
+            for arg in self._dist.arg_constraints
+        ]
+        args = ', '.join(args)
+        return f'{name}({args})'
 
     @property
-    def expression(self) -> str:
-        """Expression of the super parameter."""
-        return repr(self)
+    def _info(self) -> dict[ParamID, ParamInfo]:
+        vmin = f'{self._min:.4g}' if self._min is not None else '???'
+        vmax = f'{self._max:.4g}' if self._max is not None else '???'
+        if vmin == '???' or vmax == '???':
+            bound_expr = str(self._dist.support)
+        else:
+            bound_expr = f'({vmin}, {vmax})'
 
+        info = ParamInfo(
+            name=self.name,
+            latex=self.latex,
+            default=self.default,
+            bound='' if self.fixed else bound_expr,
+            prior='' if self.fixed else self._dist_expr,
+            log=self.log,
+            fixed=self.fixed,
+            tracker=self._tracker,
+            id_to_value=self._id_to_value,
+            dist=None if self.fixed else self._dist,
+        )
+
+        return {self._id: info}
 
-class UniformParameter(Parameter):
-    """The default class to handle parameter definition.
+
+class UniformParameter(DistParameter):
+    r"""Define the parameter by a uniform distribution.
 
     Parameters
     ----------
     name : str
         Parameter name.
-    fmt : str
-        Parameter Tex.
     default : float
         Parameter default value.
     min : float
         Parameter minimum value.
     max : float
         Parameter maximum value.
-    frozen : bool
-        Whether parameter is fixed.
-    log : bool
-        Whether parameter is parameterized into log scale, only for positive
-        valued parameter.
-
+    log : bool, optional
+        Whether the parameter is logarithmically uniform. The default is False.
+    fixed : bool, optional
+        Whether the parameter is fixed. The default is False.
+    latex : str, optional
+        :math:`\LaTeX` format of the parameter. The default is as `name`.
     """
 
     def __init__(
         self,
         name: str,
-        fmt: str,
         default: float,
         min: float,
         max: float,
-        frozen: bool = False,
-        log: bool = False
+        *,
+        log: bool = False,
+        fixed: bool = False,
+        latex: str | None = None,
     ):
-        self._config = {
-            'default': float(default),
-            'min': float(min),
-            'max': float(max),
-            'frozen': bool(frozen),
-            'log': bool(log)
-        }
-
-        self._check_and_set_values()
+        self._log = bool(log)
 
-        distribution, deterministic = self._get_distribution_deterministic()
-        node = ParameterNode(name, fmt, default, distribution, deterministic)
-        super().__init__(node)
+        self._check_and_set_values(default, min, max)
 
-    def __repr__(self):
-        name = self._node.attrs["name"]
-        default = self._config["default"]
+        super().__init__(
+            name,
+            self._dist,
+            default,
+            min=min,
+            max=max,
+            log=log,
+            fixed=fixed,
+            latex=latex,
+        )
 
-        if self._config['frozen']:
-            s = f'{name} = {default}'
+    def __repr__(self) -> str:
+        if self._fixed:
+            return f'{self.name} = {self.default:.4g}'
+        elif self._log:
+            return f'{self.name} ~ LogUniform({self.min:.4g}, {self.max:.4g})'
         else:
-            min = self._config["min"]
-            max = self._config["max"]
-
-            if self._config['log']:
-                dist = f'LogUniform(min={min}, max={max}, default={default})'
-            else:
-                dist = f'Uniform(min={min}, max={max}, default={default})'
-
-            s = f'{name} ~ {dist}'
+            return f'{self.name} ~ Uniform({self.min:.4g}, {self.max:.4g})'
 
-        return s
+    @property
+    def name(self) -> str:
+        return self._name
 
     @property
-    def fmt(self) -> str:
-        """Parameter Tex."""
-        return self._node.attrs['fmt']
+    def latex(self) -> str:
+        return self._latex
 
-    @fmt.setter
-    def fmt(self, value):
-        """Parameter Tex."""
-        self._node.attrs['fmt'] = str(value)
+    @latex.setter
+    def latex(self, latex: str):
+        self._latex = str(latex)
 
     @property
-    def default(self) -> float:
-        """Parameter default value."""
-        return self._config['default']
+    def default(self) -> JAXFloat:
+        return self._default
 
     @default.setter
-    def default(self, value):
-        """Parameter default value."""
-        self._check_and_set_values(default=value)
+    def default(self, default: float):
+        self._check_and_set_values(default=default)
 
     @property
-    def min(self) -> float:
-        """Parameter minimum."""
-        return self._config['min']
+    def min(self) -> JAXFloat:
+        """Parameter minimum value."""
+        return self._min
 
     @min.setter
-    def min(self, value):
-        """Parameter minimum."""
-        self._check_and_set_values(min=value)
+    def min(self, min: float):
+        self._check_and_set_values(min=min)
 
     @property
-    def max(self) -> float:
-        """Parameter maximum."""
-        return self._config['max']
+    def max(self) -> JAXFloat:
+        """Parameter maximum value."""
+        return self._max
 
     @max.setter
-    def max(self, value):
-        """Parameter maximum."""
-        self._check_and_set_values(max=value)
-
-    @property
-    def frozen(self) -> bool:
-        """Parameter frozen status."""
-        return self._config['frozen']
-
-    @frozen.setter
-    def frozen(self, value):
-        """Parameter frozen status."""
-        flag = bool(value)
-
-        if self._config['frozen'] != flag:
-            self._config['frozen'] = flag
-            self._reset_distribution_deterministic()
+    def max(self, max: float):
+        self._check_and_set_values(max=max)
 
     @property
     def log(self) -> bool:
-        """Whether parameter is in log scale."""
-        return self._config['log']
+        """Whether the parameter is logarithmically uniform."""
+        return self._log
 
     @log.setter
-    def log(self, value):
-        """Whether parameter is in log scale."""
-        log_flag = bool(value)
-
-        config = self._config
-        if config['log'] != log_flag:
-            if log_flag and config['min'] <= 0.0:
-                raise ValueError(
-                    'parameterization into log-uniform failed due to '
-                    'non-positive minimum'
-                )
+    def log(self, log: bool):
+        log = bool(log)
+        if self._log != log:
+            self._log = log
 
-            config['log'] = log_flag
+            if log:
+                self._dist = LogUniform(self._min, self._max)
+            else:
+                self._dist = Uniform(self._min, self._max)
+
+    @property
+    def fixed(self) -> bool:
+        return self._fixed
 
-            self._reset_distribution_deterministic()
+    @fixed.setter
+    def fixed(self, fixed: bool):
+        self._fixed = bool(fixed)
 
-    def _check_and_set_values(self, default=None, min=None, max=None) -> None:
-        """Check and set parameter configure."""
-        config = self._config
+    @property
+    def _dist_expr(self) -> str:
+        if self._log:
+            return f'LogUniform({self.min:.4g}, {self.max:.4g})'
+        else:
+            return f'Uniform({self.min:.4g}, {self.max:.4g})'
 
+    def _check_and_set_values(
+        self,
+        default: float | None = None,
+        min: float | None = None,
+        max: float | None = None,
+    ) -> None:
+        """Check and set parameter configuration."""
         if default is None:
-            _default = config['default']
+            _default = self._default
         else:
-            _default = float(default)
+            if jnp.shape(default) != ():
+                raise ValueError('default must be a scalar')
+            _default = jnp.asarray(default, float)
 
         if min is None:
-            _min = config['min']
+            _min = self._min
         else:
-            _min = float(min)
+            if jnp.shape(min) != ():
+                raise ValueError('min must be a scalar')
+            _min = jnp.asarray(min, float)
 
         if max is None:
-            _max = config['max']
+            _max = self._max
         else:
-            _max = float(max)
+            if jnp.shape(max) != ():
+                raise ValueError('max must be a scalar')
+            _max = jnp.asarray(max, float)
 
-        if _min <= 0.0 and config['log']:
-            raise ValueError(
-                f'min ({_min}) must be positive for LogUniform'
-            )
+        if _min <= 0.0 and self._log:
+            raise ValueError(f'min ({_min}) must be positive for log uniform')
 
-        if _min > _max:
-            raise ValueError(
-                f'min ({_min}) must not larger than max ({_max})'
-            )
+        if _min >= _max:
+            raise ValueError(f'min ({_min}) must less than max ({_max})')
 
-        if _default < _min:
+        if _default <= _min:
             raise ValueError(
-                f'default value ({_default}) is smaller than min ({_min})'
+                f'default ({_default}) must greater than min ({_min})'
             )
 
-        if _default > _max:
+        if _default >= _max:
             raise ValueError(
-                f'default value ({_default}) is larger than max ({_max})'
+                f'default ({_default}) must less than max ({_max})'
             )
 
         if default is not None:
-            config['default'] = float(default)
-            self._node.attrs['default'] = float(default)
+            self._default = _default
 
         if min is not None:
-            config['min'] = float(min)
+            self._min = _min
 
         if max is not None:
-            config['max'] = float(max)
+            self._max = _max
 
-        if (min is not None) or (max is not None):
-            self._reset_distribution_deterministic()
+        if min is not None or max is not None:
+            if self.log:
+                self._dist = LogUniform(self._min, self._max)
+            else:
+                self._dist = Uniform(self._min, self._max)
 
-    def _get_distribution_deterministic(self) -> tuple:
-        """Get distribution and deterministic for :class:`ParameterNode`."""
-        config = self._config
 
-        if config['frozen']:
-            distribution = config['default']  # TODO: use a Delta distribution?
-        else:
-            if config['log']:
-                distribution = LogUniform(config['min'], config['max'])
-            else:
-                distribution = Uniform(config['min'], config['max'])
+class ConstantParameter(ParameterHelper):
+    r"""Constant parameter.
 
-        if not config['frozen'] and config['log']:
-            deterministic = ((r'\ln({name})',), lambda p: jnp.log(p))
-        else:
-            deterministic = None
+    Parameters
+    ----------
+    name : str
+        Parameter name.
+    value : array_like
+        The constant value of parameter.
+    latex : str, optional
+        :math:`\LaTeX` format of the parameter. The default is as `name`.
+    """
+
+    def __init__(self, name: str, value: Any, latex: str | None = None):
+        super().__init__(name, latex, value)
 
-        return distribution, deterministic
+    @property
+    def log(self) -> bool:
+        """Constant parameter is not logarithmically parameterized."""
+        return False
 
-    def _reset_distribution_deterministic(self) -> None:
-        """Reset distribution and deterministic after configuring parameter."""
-        distribution, deterministic = self._get_distribution_deterministic()
-        self._node.attrs['distribution'] = distribution
-        self._node.attrs['deterministic'] = deterministic
+    @property
+    def fixed(self) -> bool:
+        """Constant parameter is fixed."""
+        return True
 
 
-class Model(ABC):
-    """Prototype model class.
+class ConstantValue(ConstantParameter):
+    r"""Parameter with a fixed value.
 
     Parameters
     ----------
-    node : ModelNode, or ModelOperationNode
-        The base model node.
-    params : dict, or None
-        A :class:`str`-:class:`Parameter` mapping that contains the parameters
-        of the model. It should be None when initializing :class:`SuperModel`.
-
+    name: str
+        Parameter name.
+    value: float
+        Parameter value.
+    latex : str, optional
+        :math:`\LaTeX` format of the parameter. The default is as `name`.
     """
 
-    def __init__(
-        self,
-        node: ModelNodeType,
-        params: dict[str, Parameter] | None
-    ):
-        if not isinstance(node, (ModelNode, ModelOperationNode)):
-            raise ValueError(
-                'node must be ModelNode or ModelOperationNode'
-            )
-
-        if isinstance(node, ModelNode) and not (
-            isinstance(params, dict)
-            and all(map(lambda k: isinstance(k, str), params.keys()))
-            and all(map(lambda v: isinstance(v, Parameter), params.values()))
-        ):
-            raise ValueError(
-                'params must be dict of str-Parameter mapping for model'
-            )
+    def __init__(self, name: str, value: float, latex: str | None = None):
+        super().__init__(name, value, latex)
 
-        self._node = node
-        self._label = LabelSpace(node)
+    def __repr__(self) -> str:
+        return f'{self.name} = {self.default:.4g}'
 
-        if params is not None:
-            for key, value in params.items():
-                setattr(self, key, value)
+    @property
+    def default(self) -> JAXFloat:
+        return self._default
 
-            self._comps = {node.name: self}  # use name_id to mark model
-            self._params = params
-            self._params_name = tuple(params.keys())
+    @default.setter
+    def default(self, default: float):
+        if jnp.shape(default) != ():
+            raise ValueError('default must be a scalar')
 
-    def __repr__(self):
-        return self._label.name
+        self._default = jnp.asarray(default, float)
 
-    def __add__(self, other: Model) -> SuperModel:
-        return SuperModel(self, other, '+')
+    @property
+    def _info(self) -> dict[ParamID, ParamInfo]:
+        info = ParamInfo(
+            name=self.name,
+            latex=self.latex,
+            default=self.default,
+            bound='',  # this is not supposed to be used
+            prior='',  # this is not supposed to be used
+            log=self.log,
+            fixed=self.fixed,
+            tracker=self._tracker,
+            id_to_value=self._id_to_value,
+        )
 
-    def __mul__(self, other: Model) -> SuperModel:
-        return SuperModel(self, other, '*')
+        return {self._id: info}
 
-    def __setattr__(self, key, value):
-        if hasattr(self, '_params_name') \
-                and self._params_name is not None \
-                and key in self._params_name:
-            self._set_param(key, value)
 
-        super().__setattr__(key, value)
+class ConstantInterval(ConstantParameter):
+    r"""Constant parameter to be integrated over a given interval.
 
-    def __getitem__(self, name: str) -> Parameter:
-        if name not in self._params:
-            raise ValueError(
-                f'{self} has no "{name}" parameter'
-            )
+    Parameters
+    ----------
+    name: str
+        Parameter name.
+    interval: array_like
+        The interval, a 2-element sequence.
+    method : {'quadgk', 'quadcc', 'quadts', 'romberg', 'rombergts'}, optional
+        Numerical integration method used to integrate over the parameter.
+        Available options are:
+
+            * ``'quadgk'``: global adaptive quadrature by Gauss-Konrod rule
+            * ``'quadcc'``: global adaptive quadrature by Clenshaw-Curtis rule
+            * ``'quadts'``: global adaptive quadrature by trapz tanh-sinh rule
+            * ``'romberg'``: Romberg integration
+            * ``'rombergts'``: Romberg integration by tanh-sinh
+              (a.k.a. double exponential) transformation
+
+        The default is ``'quadgk'``.
+    latex : str, optional
+        :math:`\LaTeX` format of the parameter. The default is as `name`.
+    kwargs : dict, optional
+        Extra kwargs passed to integration methods. See [1]_ for details.
 
-        return self._params[name]
+    References
+    ----------
+    .. [1] `quadax docs <https://quadax.readthedocs.io/en/latest/api.html#adaptive-integration-of-a-callable-function-or-method>`__
+    """
 
-    def __setitem__(self, name: str, param: Parameter):
-        if name not in self._params:
-            raise ValueError(
-                f'{self} has no "{name}" parameter'
-            )
+    def __init__(
+        self,
+        name: str,
+        interval: Sequence[float],
+        method: AdaptQuadMethod = 'quadgk',
+        latex: str | None = None,
+        **kwargs,
+    ):
+        super().__init__(name, interval, latex)
+        self.method = method
+        self._integrate_kwargs = {'epsabs': 0.0, 'epsrel': 1.4e-8} | kwargs
 
-        setattr(self, name, param)
+    def __repr__(self) -> str:
+        return f'{self.name} = [{self.default[0]:.4g}, {self.default[1]:.4g}]'
 
     @property
-    def type(self) -> str:
-        """Model type."""
-        return self._node.attrs['mtype']
+    def default(self) -> JAXArray:
+        return self._default
 
-    def _set_param(self, name: str, param: Parameter) -> None:
-        """Set parameter.
+    @default.setter
+    def default(self, default):
+        if jnp.shape(default) != (2,):
+            raise ValueError('interval must be a 2-element sequence')
 
-        Parameters
-        ----------
-        name : str
-            Parameter name.
-        param : Parameter
-            Parameter instance.
+        self._default = jnp.asarray(default, float)
 
-        """
-        if not isinstance(self._node, ModelNode):
-            raise TypeError('SuperModel does not support setting parameter')
+    @property
+    def method(self) -> AdaptQuadMethod:
+        """Numerical integration method."""
+        return self._method
+
+    @method.setter
+    def method(self, value: AdaptQuadMethod):
+        supported = get_args(AdaptQuadMethod)
+        if value not in supported:
+            raise ValueError(f'method must be one of {supported}')
 
-        type_error = False
+        self._method = value
 
-        if isinstance(param, Parameter):
-            self._params[name] = param
-            idx = self._params_name.index(name)
-            self._node.predecessor[idx] = param._node
+    @property
+    def _info(self) -> dict[ParamID, ParamInfo]:
+        factory = make_integral_factory(
+            param_id=self._id,
+            interval=self.default,
+            method=self.method,
+            kwargs=self._integrate_kwargs,
+        )
 
-        else:
-            if isinstance(param, (float, int)):
-                p = self._params[name]
-                if isinstance(p, UniformParameter):
-                    p.frozen = True
-                    p.default = param
-                else:
-                    type_error = True
-            else:
-                type_error = True
+        info = ParamInfo(
+            name=self.name,
+            latex=self.latex,
+            default=self.default,
+            bound='',  # this is not supposed to be used
+            prior='',  # this is not supposed to be used
+            log=self.log,
+            fixed=self.fixed,
+            tracker=self._tracker,
+            integrate=factory,
+            id_to_value=self._id_to_value,
+        )
 
-        if type_error:  # other input types are not supported yet
-            type_name = type(param).__name__
-            raise TypeError(
-                f'got {repr(param)} ({type_name}) for '
-                f'{self}.{name}, which is not supported'
-            )
+        return {self._id: info}
 
-    @property
-    def _wrapped_func(self) -> Callable:
-        """Model evaluation function."""
-        f = self._node.generate_func(self._label.mapping['name'])
-
-        # TODO: eliminate *args and **kwargs
-        def func(egrid, params, *args, **kwargs):
-            """Model function wrapper."""
-            return f(params, egrid, *args, **kwargs)
-
-        return func
-
-    @property
-    def _model_info(self) -> dict:
-        """Model information.
-
-        Returns sample and deterministic site information of :mod:`numpyro`,
-        model parameter configure based on site, model function and id mapping.
-        """
-        info = dict(
-            site=self._node.site,
-            params=self._node.params,
-            func=self._wrapped_func,
-            mapping=self._label.mapping,
-        )
-        return info
 
-    # def set_params(self, params: dict[str, Parameter]) -> None:
-    #     """Set parameters."""
-    #
-    #     params_in = set(params.keys())
-    #     params_all = set(self._params_name)
-    #
-    #     if not params_in <= params_all:
-    #         diff = params_all - params_in
-    #         raise ValueError(f'input params {diff} not included in {self}')
-    #
-    #     if not all(map(lambda v: isinstance(v, Parameter), params.values())):
-    #         raise ValueError('Parameter type is required')
-    #
-    #     params = self._params | params
-    #     params_node = list(map(lambda v: v._node, params.values()))
-    #     self._params = params
-    #     self._node.predecessor = params_node
-    #
-    # @property
-    # def additives(self):
-    #     return ...
-    #
-    # def flux(self):
-    #     ...
-    #
-    # def ne(self):
-    #     ...
-    #
-    # def ene(self):
-    #     ...
-    #
-    # def eene(self):
-    #     ...
-    #
-    # def ce(self):
-    #     ...
-    #
-    # def counts(self):
-    #     ...
-    #
-    # def fmt(self):
-    #     ...
+# class DependentInterval(Parameter):
+#     """Interval whose bounds are defined by function of parameters."""
 
 
-class SuperModel(Model):
-    """Class to handle operation on models.
+class CompositeParameter(Parameter):
+    r"""Compose parameters into a new parameter.
 
     Parameters
     ----------
-    lh: Model
-        Left-hand parameter.
-    rh: Model
-        Right-hand parameter.
-    op : {'+', '*'}
-        Operation to perform.
-
+    params : Parameter, or sequence of Parameter
+        Parameters to be composed.
+    op : callable
+        Function to be applied to `params`.
+    op_name : str
+        Name of the composition operator `op`.
+    op_latex : str, optional
+        :math:`\LaTeX` format of the composition operator `op`. The default is
+        as `op_name`.
     """
 
-    def __init__(self, lh: Model, rh: Model, op: str):
-        if op not in {'+', '*'}:
-            raise TypeError(f'operator "{op}" is not supported')
+    _params: tuple[Parameter, ...]
+    _has_interval: bool
 
-        if not isinstance(lh, Model):
-            raise TypeError(f'{lh} is not a valid model')
+    def __init__(
+        self,
+        params: Parameter | Sequence[Parameter],
+        op: Callable[..., JAXFloat],
+        op_name: str,
+        op_latex: str,
+        *,
+        op_symbol: Literal['+', '-', '*', '/', '^'] | None = None,
+    ):
+        # check if the type of params is parameter or sequence
+        if not isinstance(params, (Parameter, Sequence)):
+            raise TypeError(
+                'parameters must be a Parameter or a sequence of Parameter'
+            )
 
-        if not isinstance(rh, Model):
-            raise TypeError(f'{rh} is not a valid model')
+        # make params a list
+        if isinstance(params, Parameter):
+            params = [params]
+        else:
+            params = list(params)
 
-        self._op = op
-        self._lh = lh
-        self._rh = rh
+        # check if params are all parameters
+        if not all(isinstance(i, Parameter) for i in params):
+            raise TypeError(
+                'parameters must be a Parameter or a sequence of Parameter'
+            )
 
-        if op == '+':
-            node = lh._node + rh._node
-        else:  # op == '*'
-            node = lh._node * rh._node
-
-        super().__init__(node, None)
-
-        comps = {**lh._comps, **rh._comps}
-        names = self._label.mapping['name']
-        for k in names:
-            setattr(self, names[k], comps[k])
-        self._comps = comps
-        self._comps_name = tuple(names.values())
-
-    def __setattr__(self, key, value):
-        if hasattr(self, '_comps_name') and key in self._comps_name:
-            raise AttributeError(f"can't set attribute '{key}'")
+        if op_symbol not in {'+', '-', '*', '/', '^', None}:
+            raise ValueError('`op_symbol` is for internal use only')
 
-        super().__setattr__(key, value)
+        super().__init__()
 
-    def __getitem__(self, name: str) -> Model:
-        if name not in self._comps_name:
-            raise ValueError(
-                f'{self} has no "{name}" component'
-            )
+        self._op = op
+        self._op_name = str(op_name)
+        self._op_latex = self._op_name if op_latex is None else str(op_latex)
+        self._op_symbol = op_symbol
+        self._params = tuple(params)
+
+        for p in self._params:
+            if isinstance(p, ConstantInterval) or (
+                isinstance(p, CompositeParameter) and p._has_interval
+            ):
+                self._has_interval = True
+                break
+        else:
+            self._has_interval = False
 
-        return getattr(self, name)
+        # correct Parameter's _nodes_id attribute
+        nodes = []
+        for p in self._params:
+            stack = [p]
+            while stack:
+                node = stack.pop(0)
+                if isinstance(node, CompositeParameter):
+                    stack = list(node._params) + stack
+                elif node not in nodes:
+                    nodes.append(node)
+        self._nodes = tuple(nodes)
+        self._nodes_id = tuple(p._id for p in self._nodes)
+
+        pid_to_pname = dict(
+            zip(
+                self._nodes_id,
+                build_namespace([p.name for p in self._nodes], prime=True)[
+                    'namespace'
+                ],
+            )
+        )
+        self._name = self._id_to_label(pid_to_pname, 'name')
 
-    def __setitem__(self, name, value):
-        raise TypeError('item assignment not supported')
+    def _id_to_label(
+        self,
+        mapping: dict[ParamID, str],
+        label_type: Literal['name', 'latex'],
+    ) -> str:
+        if label_type not in {'name', 'latex'}:
+            raise ValueError(f'unknown label type: {label_type}')
 
+        if self._id in mapping:
+            return mapping[self._id]
+        else:
+            if self._op_symbol:
+                op = self._op_symbol
+                lhs, rhs = self._params
+
+                if op == '+':
+                    lhs_fmt = rhs_fmt = '{}'
+
+                elif op == '-':
+                    lhs_fmt = '{}'
+
+                    if isinstance(
+                        rhs, CompositeParameter
+                    ) and rhs._op_symbol not in {'*', '/', '^'}:
+                        rhs_fmt = '({})'
+                    else:
+                        rhs_fmt = '{}'
+
+                elif op == '*':
+                    if isinstance(
+                        lhs, CompositeParameter
+                    ) and lhs._op_symbol not in {'*', '/', '^'}:
+                        lhs_fmt = '({})'
+                    else:
+                        lhs_fmt = '{}'
+
+                    if isinstance(
+                        rhs, CompositeParameter
+                    ) and rhs._op_symbol not in {'*', '/', '^'}:
+                        rhs_fmt = '({})'
+                    else:
+                        rhs_fmt = '{}'
+
+                elif op == '/':
+                    if isinstance(
+                        lhs, CompositeParameter
+                    ) and lhs._op_symbol not in {'*', '/', '^'}:
+                        lhs_fmt = '({})'
+                    else:
+                        lhs_fmt = '{}'
+
+                    rhs_fmt = '({})'
+
+                elif op == '^':
+                    if isinstance(lhs, CompositeParameter):
+                        lhs_fmt = '({})'
+                    else:
+                        lhs_fmt = '{}'
+
+                    if isinstance(rhs, CompositeParameter):
+                        rhs_fmt = '({})'
+                    else:
+                        rhs_fmt = '{}'
 
-class ComponentMeta(ABCMeta):
-    """Metaclass to avoid cumbersome code for ``__init__`` of subclass."""
+                else:
+                    raise NotImplementedError(f'op_symbol: {op}')
 
-    def __init__(cls, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # if subclass has ``default`` defined correctly, override its __init__
-        if hasattr(cls, '_default') and isinstance(cls._default, tuple):
-            name = cls.__name__.lower()
-
-            # >>> construct __init__ function >>>
-            default = cls._default
-            init_def = 'self, '
-            init_body = ''
-            par_body = '('
-            for cfg in default:
-                init_def += cfg[0] + '=None, '
-                init_body += f'{cfg[0]}={cfg[0]}, '
-                par_body += f'{cfg[0]}, '
-            par_body += ')'
-
-            par_def = str(init_def)
-
-            init_def += 'fmt=None'
-            init_body += f'fmt=fmt'
-
-            if hasattr(cls, '_extra_kw') and isinstance(cls._extra_kw, tuple):
-                for kw in cls._extra_kw:
-                    # FIXME: repr may fail!
-                    init_def += f', {kw[0]}={repr(kw[1])}'
-                    init_body += f', {kw[0]}={kw[0]}'
-
-            func_code = f'def __init__({init_def}):\n    '
-            func_code += f'super(type(self), type(self))'
-            func_code += f'.__init__(self, {init_body})\n'
-            func_code += f'def {name}({par_def}):\n    '
-            func_code += f'return {par_body}'
-            # <<< construct __init__ function <<<
-
-            # now create and set __init__ function
-            tmp = {}
-            exec(func_code, tmp)
-            init_func = tmp['__init__']
-            init_func.__qualname__ = f'{name}.__init__'
-            cls.__init__ = init_func
-            cls._get_args = tmp[name]
-
-
-class Component(Model, ABC, metaclass=ComponentMeta):
-    """The abstract spectral component class."""
-
-    def __init__(self, fmt=None, **params):
-        if fmt is None:
-            fmt = self.__class__.__name__.lower()
-
-        # parse parameters
-        params_dict = {}
-        for cfg in self._default:
-            param_name = cfg[0]
-            param = params[param_name]
-
-            if param is None:
-                # use default configure
-                params_dict[param_name] = UniformParameter(*cfg)
-
-            elif isinstance(param, Parameter):
-                # specified by user
-                params_dict[param_name] = param
-
-            elif isinstance(param, (float, int)):
-                # frozen to the value given by user
-                p = UniformParameter(*cfg)
-                p.default = param
-                p.frozen = True
-                params_dict[param_name] = p
+                labels = (
+                    lhs_fmt.format(lhs._id_to_label(mapping, label_type)),
+                    rhs_fmt.format(rhs._id_to_label(mapping, label_type)),
+                )
 
             else:
-                # other input types are not supported yet
-                cls_name = type(self).__name__
-                type_name = type(param).__name__
-                raise TypeError(
-                    f'got {type_name} type {repr(param)} for '
-                    f'{cls_name}.{param_name}, which is not supported'
+                labels = tuple(
+                    (
+                        '({})' if isinstance(p, CompositeParameter) else '{}'
+                    ).format(p._id_to_label(mapping, label_type))
+                    for p in self._params
                 )
 
-        if self.type == 'ncon':  # normalization convolution type
-            mtype = 'con'
-            is_ncon = True
-        else:
-            mtype = self.type
-            is_ncon = False
-
-        component = ModelNode(
-            name=type(self).__name__.lower(),
-            fmt=fmt,
-            mtype=mtype,
-            params={k: v._node for k, v in params_dict.items()},
-            func_generator=self._func_generator,
-            is_ncon=is_ncon
-        )
-
-        super().__init__(component, params_dict)
-
-    @abstractmethod
-    def _func_generator(self, func_name: str) -> Callable:
-        """Model function generator, overriden by subclass."""
-        pass
-
-    @property
-    @abstractmethod
-    def type(self) -> str:
-        """Model type, overriden by subclass."""
-        pass
+            temp = self._op_name if label_type == 'name' else self._op_latex
+            return temp.format(*labels)
 
     @property
-    @abstractmethod
-    def _default(self) -> tuple:
-        """Default configuration of parameters, overriden by subclass.
+    def _id_to_value(self) -> Callable[[ParamIDValMapping], JAXFloat]:
+        fns = [param._id_to_value for param in self._params]
 
-        Configuration format should be ``((name: str, fmt: str, default: float,
-        min: float, max: float, frozen: bool, log: bool), ...)``.
+        def id_to_value(mapping: ParamIDValMapping) -> JAXFloat:
+            """Get the value of the composite parameter."""
+            return self._op(*[fn(mapping) for fn in fns])
 
-        """
-        pass
+        return id_to_value
 
     @property
-    def _extra_kw(self) -> tuple:
-        """Extra keywords passed to ``__init__``, overriden by subclass.
+    def name(self) -> str:
+        return self._name
 
-        Note that Element of inner tuple should respect :py:func:`repr`, or
-        ``__init__`` of :class:`ComponentMeta` may fail.
-        """
-        return tuple()
-
-
-def generate_parameter(
-    name: str,
-    fmt: str,
-    default: float,
-    distribution: Distribution,
-) -> Parameter:
-    """Create :class:`Parameter` instance.
+    @property
+    def latex(self) -> str:
+        nodes_latex = [p.latex for p in self._nodes]
+        latex = build_namespace(nodes_latex, True, True)['namespace']
+        pid_to_latex = dict(zip(self._nodes_id, latex))
+        return self._id_to_label(pid_to_latex, 'latex')
 
-    Parameters
-    ----------
-    name : str
-        Name of the parameter.
-    fmt : str
-        Tex format of the parameter.
-    default : float
-        Default value of the parameter.
-    distribution : Distribution
-        Instance of :class:`numpyro.distributions.Distribution`.
-
-    Returns
-    -------
-    Parameter
-        The generated parameter.
+    @property
+    def default(self) -> JAXFloat:
+        if self._has_interval:
+            raise RuntimeError(
+                'cannot get default value of a composite interval'
+            )
 
-    """
-    node = ParameterNode(name, fmt, default, distribution, None)
+        return self._op(*[i.default for i in self._params])
 
-    return Parameter(node)
+    @property
+    def log(self) -> bool:
+        """If any of the sub-parameters is logarithmically parameterized."""
+        return all(i.log for i in self._params)
 
+    @property
+    def fixed(self) -> bool:
+        """If all the sub-parameters are fixed."""
+        return all(i.fixed for i in self._params)
 
-def generate_model(
-    name: str,
-    fmt: str,
-    mtype: str,
-    params: dict[str, Parameter],
-    func: Callable,
-    is_ncon: bool
-) -> Model:
-    """Create :class:`Model` instance.
+    @property
+    def _info(self) -> dict[ParamID, ParamInfo]:
+        info = {
+            self._id: ParamInfo(
+                name=lambda mapping: self._id_to_label(mapping, 'name'),
+                latex=lambda mapping: self._id_to_label(mapping, 'latex'),
+                default=jnp.nan,  # this is not supposed to be used
+                bound='',  # this is not supposed to be used
+                prior='',  # this is not supposed to be used
+                log=self.log,
+                fixed=self.fixed,
+                tracker=self._tracker,
+                id_to_value=self._id_to_value,
+                integrate=self._has_interval,
+                composite=True,
+            )
+        }
 
-    Parameters
-    ----------
-    name : str
-        Name of the model.
-    fmt : str
-        Tex format of the model.
-    mtype : {'add', 'mul', 'con'}
-        Model type.
-    params : dict
-        A :class:`str`-:class:`Parameter` mapping that defines the parameters
-        of the model.
-    func : callable
-        Evaluation function of the model.
-    is_ncon : bool
-        Whether the model is normalization convolution type.
-
-    Returns
-    -------
-    Model
-        The generated model.
-
-    Notes
-    -----
-    The signature of `func` should be ``func(egrid, par1, ...)``, where
-    `func` is expected to return ndarray of length ``len(egrid) - 1`` (i.e.,
-    integrating over `egrid`), and ``par1, ...`` matches `params`.
-
-    If the function is convolution type, operating on flux (con) or norm
-    (ncon), then corresponding signature of `func` should be
-    ``func(egrid, flux, par1, ...)`` or ``func(flux_func, flux, par1, ...)``,
-    where `flux` is ndarray of length ``len(egrid) - 1``, and `flux_func` has
-    the same signature and returns as aforementioned.
+        for p in self._params:
+            info |= p._info
 
-    """
-    params_node = {k: v._node for k, v in params.items()}
-    model_node = ModelNode(name, fmt, mtype, params_node, func, is_ncon)
+        return info
 
-    return Model(model_node, params)
 
+# class GPParameter(ParameterHelper):
+#     """Parameter sampled from a Gaussian process."""
 #
+#     def __init__(
+#         self,
+#         name: str,
+#         kernel: kernels.Kernel,
+#         x: JAXFloat,
+#         *,
+#         diag: JAXFloat | None = None,
+#         noise: noise.Noise | None = None,
+#         mean: means.MeanBase | Callable | JAXFloat | None = None,
+#         log: bool = False,
+#         latex: str | None = None,
+#     ):
+#         self._log = bool(log)
+#         super().__init__(name, latex, None)
 #
-# class Model(metaclass=ComponentMeta):
-#     def _get_param(self, key):
-#         """Check and return component and parameter key."""
-#
-#         if '.' not in key:
-#             raise ValueError('key format should be "component.parameter"')
-#
-#         c, p = key.split('.')
-#
-#         name_map = {v: k for k, v in self._label._label_map['name'].items()}
-#
-#         if c not in name_map:
-#             raise ValueError(f'No component "{c}" in model "{self}"')
-#
-#         return self._node.comps[name_map[c]], p
+#     def _fn(self, name: str | None, rng_key: PRNGKey | None) -> JAXFloat:
+#         """Sample from the Gaussian process."""
+#         raise NotImplementedError
 #
 #     @property
-#     def comps(self):
-#         """Additive type of compositions of subcomponents."""
-#
-#         if self.type != 'add':
-#             raise TypeError(
-#                 f'"{self.type}" model has no additive sub-components'
-#             )
-#         else:
-#             if not self._comps:
-#                 raise NotImplementedError
+#     def default(self) -> None:
+#         return None
 #
-#             return self._comps
-#
-#     # def flux(self, params, e_range, energy=True, ngrid=1000, log=True):
-#     #     """Evaluate model by
-#     #         * analytic expression
-#     #         * trapezoid or Simpson's 1/3 rule given :math:`N_E`
-#     #         * Xspec model library
-#     #
-#     #     TODO: docstring
-#     #
-#     #     """
-#     #
-#     #     if self.type != 'add':
-#     #         raise TypeError(
-#     #             f'flux is undefined for "{self.type}" type model "{self}"'
-#     #         )
-#     #
-#     #     if log:  # evenly spaced grid in log space
-#     #         egrid = np.geomspace(*e_range, ngrid)
-#     #     else:  # evenly spaced grid in linear space
-#     #         egrid = np.linspace(*e_range, ngrid)
-#     #
-#     #     if energy:  # energy flux
-#     #         flux = np.sum(self.ENE(pars, ebins) * np.diff(ebins), axis=-1)
-#     #     else:  # photon flux
-#     #         flux = np.sum(self.NE(pars, ebins) * np.diff(ebins), axis=-1)
-#     #
-#     #     return flux
-#
-#     def _build_prior(self) -> Callable:
-#         """Get the prior function which will be used in numpyro."""
-#
-#         def prior():
-#             """This should be called inside numpyro."""
-#             self
-#             ...
-#
-#         return prior
-#
-#     def __call__(self, egrid, flux=None):
-#         # TODO:
-#         return self.eval(egrid, flux)
+#     @property
+#     def log(self) -> bool:
+#         return self._log
 #
-#     def eval(self, *args, **kwargs):
-#         """TODO"""
-#         if self.type != 'con':
-#             ...
-#         else:
-#             ...
+#     @property
+#     def fixed(self) -> bool:
+#         return False
 #
+#     @property
+#     def _info(self) -> dict[ParamID, ParamInfo]:
+#         return ...
```

### Comparing `elisa_lib-0.0.1.dev1/.gitignore` & `elisa_lib-0.1.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-### Example user template template
-### Example user template
+### JupyterNotebooks template
+# gitignore template for Jupyter Notebooks
+# website: http://jupyter.org/
+
+.ipynb_checkpoints
+*/.ipynb_checkpoints/*
+
+# IPython
+profile_default/
+ipython_config.py
+
+# Remove previous ipynb_checkpoints
+#   git rm -r .ipynb_checkpoints/
 
-# IntelliJ project files
-.idea
-*.iml
-out
-gen
 ### Python template
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
-*.dylib
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -76,26 +81,20 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/apidoc
 
 # PyBuilder
 .pybuilder/
 target/
 
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
 #   intended to run in multiple environments; otherwise, check them in:
 # .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
@@ -105,15 +104,15 @@
 #Pipfile.lock
 
 # poetry
 #   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
 #   This is especially recommended for binary packages to ensure reproducibility, and is more
 #   commonly ignored for libraries.
 #   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-poetry.lock
+#poetry.lock
 
 # pdm
 #   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
 #pdm.lock
 #   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
 #   in version control.
 #   https://pdm.fming.dev/#use-with-ide
```

### Comparing `elisa_lib-0.0.1.dev1/LICENSE` & `elisa_lib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.0.1.dev1/pyproject.toml` & `elisa_lib-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "elisa-lib"
 dynamic = ["version"]
-description = "An efficient and fast library for spectral analysis in X/γ-ray astrophysics."
+description = "An efficient library for spectral analysis in high-energy astrophysics."
 readme = "README.md"
 requires-python = ">=3.9, <3.12"
 license = "GPL-3.0-or-later"
 keywords = []
 authors = [
     { name = "Wang-Chen Xue", email = "wcxuemail@gmail.com" },
 ]
@@ -18,34 +18,47 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "arviz",
-    "astropy",
-    "jax",
+    "astropy>=5.3",
+    "corner>=2.2.2",
+    "h5py",
+    "iminuit",
+    "jax>=0.4.5",
+    "jaxns>=2.4.8",
+    "matplotlib",
     "numpy",
-#    "numpy<=1.24.4 ; sys_platform != 'darwin' or platform_machine != 'arm64'",
-#    "numpy @ https://github.com/numpy/numpy/releases/download/v1.24.4/numpy-1.24.4.tar.gz ; sys_platform == 'darwin' and platform_machine == 'arm64'",
     "numpyro",
+    "optimistix",
+    "prettytable",
+    "quadax>=0.2.1",
+    "scipy>=1.11.0, <=1.12.0",
+    "seaborn",
+    "tinygp",
     "tqdm",
-    "corner>=2.2.2"
 ]
 
 
 [project.optional-dependencies]
-xspec = ['xspex']
-test = []
+xspec = ["xspex"]
+test = ["pytest", "pytest-cov", "coverage[toml]"]
 docs = [
     "sphinx",
-    "sphinx_rtd_theme",
-    "numpydoc"
+    "sphinx-autodoc-typehints",
+    "sphinx-book-theme",
+    "sphinx-copybutton",
+    "sphinx-design",
+    "myst-nb",
+    "numba",
+    "numpydoc",
 ]
-dev = ['ipython', 'black', 'ruff']
+dev = ["pre-commit>=3.6.0", "ruff>=2.0"]
 
 
 [project.urls]
 Documentation = "https://github.com/wcxve/elisa#readme"
 Issues = "https://github.com/wcxve/elisa/issues"
 Source = "https://github.com/wcxve/elisa"
 
@@ -53,36 +66,57 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [tool.hatch]
 metadata.allow-direct-references = true
-version.path = "src/elisa/__init__.py"
+version.path = "src/elisa/__about__.py"
+build.targets.wheel.packages = ["src/elisa"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.9", "3.10", "3.11"]
 
-
-[tool.black]
-target-version = ["py39"]
+[tool.ruff]
 line-length = 79
-skip-string-normalization = true
+target-version = "py39"
+extend-exclude = ["src/elisa/infer/nested_sampling.py"]
+extend-include = ["*.ipynb"]
+format.quote-style = "single"
+lint.extend-select = ["Q"]
+lint.flake8-quotes.inline-quotes = "single"
+lint.ignore = [
+    "B028",  # allow warnings without stacklevel
+    "C901",  # allow functions with a high complexity
+    "E731",  # allow lambda functions
+]
+lint.ignore-init-module-imports = true
+lint.isort.known-first-party = ["elisa"]
+lint.isort.combine-as-imports = true
+lint.select = [
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # pyflakes
+    "I",  # isort
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+    "UP",  # pyupgrade
+]
+#lint.pydocstyle.convention = "numpy"
+
+[tool.coverage.run]
+branch = true
+parallel = true
+source = ["src/"]
+omit = [
+    "docs/*",
+    "src/elisa/infer/nested_sampling.py",
+    "src/elisa/models/tables/*",
+    "tests/*",
+    "*__init__*"
+]
 
+[tool.coverage.paths]
+source = ["src/", "*/site-packages"]
 
-[tool.ruff]
-target-version = "py39"
-line-length = 79
-select = ["F", "I", "E", "W", "YTT", "B", "Q", "PLE", "PLR", "PLW", "UP"]
-ignore = [
-    "E741",     # Allow ambiguous variable names
-    "PLR0911",  # Allow many return statements
-    "PLR0913",  # Allow many arguments to functions
-    "PLR0915",  # Allow many statements
-    "PLR2004",  # Allow magic numbers in comparisons
-]
-unfixable = [
-    "F401",  # Don't touch unused imports
-]
-exclude = []
-isort.known-first-party = ["elisa"]
-isort.combine-as-imports = true
+[tool.coverage.report]
+show_missing = true
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

