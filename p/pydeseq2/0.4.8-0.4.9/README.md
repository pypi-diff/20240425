# Comparing `tmp/pydeseq2-0.4.8.tar.gz` & `tmp/pydeseq2-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeseq2-0.4.8.tar", last modified: Tue Mar 26 15:54:30 2024, max compression
+gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-je9a9da7/pydeseq2-0.4.9.tar", last modified: Thu Apr 25 09:53:50 2024, max compression
```

## Comparing `pydeseq2-0.4.8.tar` & `pydeseq2-0.4.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-03-26 15:54:30.965615 pydeseq2-0.4.8/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.4.8/LICENSE
--rw-r--r--   0 bmuzellec   (501) staff       (20)     7001 2024-03-26 15:54:30.963070 pydeseq2-0.4.8/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6228 2024-03-25 10:26:40.000000 pydeseq2-0.4.8/README.md
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-03-26 15:54:30.935263 pydeseq2-0.4.8/pydeseq2/
--rw-r--r--   0 bmuzellec   (501) staff       (20)       45 2023-10-26 15:26:46.000000 pydeseq2-0.4.8/pydeseq2/__init__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2024-03-26 15:46:43.000000 pydeseq2-0.4.8/pydeseq2/__version__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    46958 2024-03-26 15:45:37.000000 pydeseq2-0.4.8/pydeseq2/dds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     9181 2024-03-21 15:57:54.000000 pydeseq2-0.4.8/pydeseq2/default_inference.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    28487 2024-03-01 17:49:12.000000 pydeseq2-0.4.8/pydeseq2/ds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     8479 2023-10-26 15:26:46.000000 pydeseq2-0.4.8/pydeseq2/grid_search.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    10352 2024-02-19 14:22:07.000000 pydeseq2-0.4.8/pydeseq2/inference.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     3486 2023-11-24 10:14:50.000000 pydeseq2-0.4.8/pydeseq2/preprocessing.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    49534 2024-02-28 08:24:25.000000 pydeseq2-0.4.8/pydeseq2/utils.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-03-26 15:54:30.955429 pydeseq2-0.4.8/pydeseq2.egg-info/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     7001 2024-03-26 15:54:30.000000 pydeseq2-0.4.8/pydeseq2.egg-info/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)      464 2024-03-26 15:54:30.000000 pydeseq2-0.4.8/pydeseq2.egg-info/SOURCES.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2024-03-26 15:54:30.000000 pydeseq2-0.4.8/pydeseq2.egg-info/dependency_links.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      171 2024-03-26 15:54:30.000000 pydeseq2-0.4.8/pydeseq2.egg-info/requires.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2024-03-26 15:54:30.000000 pydeseq2-0.4.8/pydeseq2.egg-info/top_level.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1381 2024-02-19 14:22:07.000000 pydeseq2-0.4.8/pyproject.toml
--rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2024-03-26 15:54:30.966281 pydeseq2-0.4.8/setup.cfg
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1318 2024-02-26 15:09:30.000000 pydeseq2-0.4.8/setup.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-03-26 15:54:30.952484 pydeseq2-0.4.8/tests/
--rw-r--r--   0 bmuzellec   (501) staff       (20)    16069 2024-02-23 08:50:56.000000 pydeseq2-0.4.8/tests/test_edge_cases.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    21985 2024-03-25 13:49:14.000000 pydeseq2-0.4.8/tests/test_pydeseq2.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2024-02-19 14:04:01.000000 pydeseq2-0.4.8/tests/test_utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.4.9/LICENSE
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6561 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6228 2024-04-05 07:58:10.000000 pydeseq2-0.4.9/README.md
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       45 2024-04-05 07:58:10.000000 pydeseq2-0.4.9/pydeseq2/__init__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2024-04-25 08:53:06.000000 pydeseq2-0.4.9/pydeseq2/__version__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    47206 2024-04-25 08:51:55.000000 pydeseq2-0.4.9/pydeseq2/dds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     9181 2024-04-05 07:58:10.000000 pydeseq2-0.4.9/pydeseq2/default_inference.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    28726 2024-04-25 08:51:55.000000 pydeseq2-0.4.9/pydeseq2/ds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     8472 2024-04-09 12:39:43.000000 pydeseq2-0.4.9/pydeseq2/grid_search.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    10352 2024-04-05 07:58:10.000000 pydeseq2-0.4.9/pydeseq2/inference.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     3486 2024-04-05 07:58:10.000000 pydeseq2-0.4.9/pydeseq2/preprocessing.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    49482 2024-04-09 12:39:43.000000 pydeseq2-0.4.9/pydeseq2/utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6561 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      464 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/SOURCES.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/dependency_links.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      171 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/requires.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/pydeseq2.egg-info/top_level.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1381 2024-04-09 12:39:43.000000 pydeseq2-0.4.9/pyproject.toml
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/setup.cfg
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1318 2024-04-09 12:39:43.000000 pydeseq2-0.4.9/setup.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2024-04-25 09:53:50.000000 pydeseq2-0.4.9/tests/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    16069 2024-04-09 12:39:43.000000 pydeseq2-0.4.9/tests/test_edge_cases.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    23546 2024-04-25 08:51:55.000000 pydeseq2-0.4.9/tests/test_pydeseq2.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2024-02-19 14:04:01.000000 pydeseq2-0.4.9/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pydeseq2-0.4.8/LICENSE` & `pydeseq2-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/PKG-INFO` & `pydeseq2-0.4.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: anndata>=0.8.0
-Requires-Dist: numpy>=1.23.0
-Requires-Dist: pandas>=1.4.0
-Requires-Dist: scikit-learn>=1.1.0
-Requires-Dist: scipy>=1.11.0
-Requires-Dist: matplotlib>=3.6.2
 Provides-Extra: dev
-Requires-Dist: pytest>=6.2.4; extra == "dev"
-Requires-Dist: pre-commit>=2.13.0; extra == "dev"
-Requires-Dist: numpydoc; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pandas-stubs; extra == "dev"
+License-File: LICENSE
 
 <img src="docs/source/_static/pydeseq2_logo_green.png" width="600">
 
 #
 [![pypi version](https://img.shields.io/pypi/v/pydeseq2)](https://pypi.org/project/pydeseq2)
 [![pypiDownloads](https://static.pepy.tech/badge/pydeseq2)](https://pepy.tech/project/pydeseq2)
 [![condaDownloads](https://img.shields.io/conda/dn/bioconda/pydeseq2?logo=Anaconda)](https://anaconda.org/bioconda/pydeseq2)
```

### Comparing `pydeseq2-0.4.8/README.md` & `pydeseq2-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/pydeseq2/dds.py` & `pydeseq2-0.4.9/pydeseq2/dds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1092,14 +1092,20 @@
 
         # Estimate log-fold changes (in natural log scale)
         sub_dds.fit_LFC()
 
         # Replace values in main object
         self.varm["_normed_means"][self.varm["refitted"]] = sub_dds.varm["_normed_means"]
         self.varm["LFC"][self.varm["refitted"]] = sub_dds.varm["LFC"]
+        self.varm["genewise_dispersions"][self.varm["refitted"]] = sub_dds.varm[
+            "genewise_dispersions"
+        ]
+        self.varm["fitted_dispersions"][self.varm["refitted"]] = sub_dds.varm[
+            "fitted_dispersions"
+        ]
         self.varm["dispersions"][self.varm["refitted"]] = sub_dds.varm["dispersions"]
 
         replace_cooks = pd.DataFrame(self.layers["cooks"].copy())
         replace_cooks.loc[self.obsm["replaceable"], self.varm["refitted"]] = 0.0
 
         self.layers["replace_cooks"] = replace_cooks
```

### Comparing `pydeseq2-0.4.8/pydeseq2/default_inference.py` & `pydeseq2-0.4.9/pydeseq2/default_inference.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/pydeseq2/ds.py` & `pydeseq2-0.4.9/pydeseq2/ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                 f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}"
             )
         print(self.results_df)
 
     def run_wald_test(self) -> None:
         """Perform a Wald test.
 
-        Get gene-wise p-values for gene over/under-expression.`
+        Get gene-wise p-values for gene over/under-expression.
         """
         num_vars = self.design_matrix.shape[1]
 
         # Raise a warning if LFCs are shrunk.
         if self.shrunk_LFCs:
             if not self.quiet:
                 print(
@@ -326,27 +326,30 @@
 
         # Account for possible all_zeroes due to outlier refitting in DESeqDataSet
         if self.dds.refit_cooks and self.dds.varm["replaced"].sum() > 0:
             self.SE.loc[self.dds.new_all_zeroes_genes] = 0.0
             self.statistics.loc[self.dds.new_all_zeroes_genes] = 0.0
             self.p_values.loc[self.dds.new_all_zeroes_genes] = 1.0
 
-    def lfc_shrink(self, coeff: Optional[str] = None) -> None:
+    def lfc_shrink(self, coeff: Optional[str] = None, adapt: bool = True) -> None:
         """LFC shrinkage with an apeGLM prior :cite:p:`DeseqStats-zhu2019heavy`.
 
         Shrinks LFCs using a heavy-tailed Cauchy prior, leaving p-values unchanged.
 
         Parameters
         ----------
         coeff : str or None
             The LFC coefficient to shrink. If set to ``None``, the method will try to
             shrink the coefficient corresponding to the ``contrast`` attribute.
             If the desired coefficient is not available, it may be set from the
             :class:`pydeseq2.dds.DeseqDataSet` argument ``ref_level``.
             (default: ``None``).
+        adapt: bool
+            Whether to use the MLE estimates of LFC to adapt the prior. If False, the
+            prior scale is set to 1. (``default=True``)
         """
         if self.contrast[1] == self.contrast[2] == "":
             # The factor being tested is continuous
             contrast_level = self.contrast[0]
         else:
             # The factor being tested is categorical
             contrast_level = (
@@ -386,16 +389,18 @@
         coeff_idx = self.LFC.columns.get_loc(coeff)
 
         size = 1.0 / self.dds.varm["dispersions"]
         offset = np.log(self.dds.obsm["size_factors"])
 
         # Set priors
         prior_no_shrink_scale = 15
-        prior_var = self._fit_prior_var(coeff_idx=coeff_idx)
-        prior_scale = np.minimum(np.sqrt(prior_var), 1)
+        prior_scale = 1
+        if adapt:
+            prior_var = self._fit_prior_var(coeff_idx=coeff_idx)
+            prior_scale = np.minimum(np.sqrt(prior_var), 1)
 
         design_matrix = self.design_matrix.values
 
         if not self.quiet:
             print("Fitting MAP LFCs...", file=sys.stderr)
         start = time.time()
         lfcs, inv_hessians, l_bfgs_b_converged_ = self.inference.lfc_shrink_nbinom_glm(
@@ -464,15 +469,15 @@
 
     def plot_MA(self, log: bool = True, save_path: Optional[str] = None, **kwargs):
         """
         Create an log ratio (M)-average (A) plot using matplotlib.
 
         Useful for looking at log fold-change versus mean expression
         between two groups/samples/etc.
-        Uses matplotlib to emulate make_MA() function in DESeq2 in R.
+        Uses matplotlib to emulate the ``make_MA()`` function in DESeq2 in R.
 
         Parameters
         ----------
         log : bool
             Whether or not to log scale x and y axes (``default=True``).
 
         save_path : str or None
```

### Comparing `pydeseq2-0.4.8/pydeseq2/grid_search.py` & `pydeseq2-0.4.9/pydeseq2/grid_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,21 @@
         Observations.
 
     mu : ndarray
         Mean of the distribution.
 
     alpha : ndarray
         Dispersion of the distribution, s.t. the variance is
-        :math:`\\mu + \\alpha * \\mu^2`.
+        :math:`\mu + \alpha \mu^2`.
 
     Returns
     -------
     ndarray
         Negative log likelihood of the observations counts following
-        :math:`NB(\\mu, \\alpha)`.
+        :math:`NB(\mu, \alpha)`.
     """
     n = len(counts)
     alpha_neg1 = 1 / alpha
     logbinom = (
         gammaln(counts[:, None] + alpha_neg1)
         - gammaln(counts + 1)[:, None]
         - gammaln(alpha_neg1)
```

### Comparing `pydeseq2-0.4.8/pydeseq2/inference.py` & `pydeseq2-0.4.9/pydeseq2/inference.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/pydeseq2/preprocessing.py` & `pydeseq2-0.4.9/pydeseq2/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/pydeseq2/utils.py` & `pydeseq2-0.4.9/pydeseq2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,16 +285,16 @@
             design_matrix[factor] = pd.to_numeric(metadata[factor])
     return design_matrix
 
 
 def replace_underscores(factors: List[str]):
     """Replace all underscores from strings in a list by hyphens.
 
-    To be used on design factors to avoid bugs due to the reliance on `str.split("_")`
-    in parts of the code.
+    To be used on design factors to avoid bugs due to the reliance on
+    ``str.split("_")`` in parts of the code.
 
     Parameters
     ----------
     factors : list
         A list of strings which may contain underscores.
 
     Returns
@@ -335,55 +335,55 @@
 def nb_nll(
     counts: np.ndarray, mu: np.ndarray, alpha: Union[float, np.ndarray]
 ) -> Union[float, np.ndarray]:
     r"""Neg log-likelihood of a negative binomial of parameters ``mu`` and ``alpha``.
 
     Mathematically, if ``counts`` is a vector of counting entries :math:`y_i`
     then the likelihood of each entry :math:`y_i` to be drawn from a negative
-    binomial :math:`NB(\\mu, \\alpha)` is [1]
+    binomial :math:`NB(\mu, \alpha)` is [1]
 
     .. math::
-        p(y_i | \\mu, \\alpha) = \\frac{\\Gamma(y_i + \\alpha^{-1})}{
-            \\Gamma(y_i + 1)\\Gamma(\\alpha^{-1})
+        p(y_i | \mu, \alpha) = \frac{\Gamma(y_i + \alpha^{-1})}{
+            \Gamma(y_i + 1)\Gamma(\alpha^{-1})
         }
-        \\left(\\frac{1}{1 + \\alpha \\mu} \\right)^{1/\\alpha}
-        \\left(\\frac{\\mu}{\\alpha^{-1} + \\mu} \\right)^{y_i}
+        \left(\frac{1}{1 + \alpha \mu} \right)^{1/\alpha}
+        \left(\frac{\mu}{\alpha^{-1} + \mu} \right)^{y_i}
 
     As a consequence, assuming there are :math:`n` entries,
     the total negative log-likelihood for ``counts`` is
 
     .. math::
-        \\ell(\\mu, \\alpha) = \\frac{n}{\\alpha} \\log(\\alpha) +
-            \\sum_i \\left \\lbrace
-            - \\log \\left( \\frac{\\Gamma(y_i + \\alpha^{-1})}{
-            \\Gamma(y_i + 1)\\Gamma(\\alpha^{-1})
-        } \\right)
-        + (\\alpha^{-1} + y_i) \\log (\\alpha^{-1} + y_i)
-        - y_i \\log \\mu
-            \\right \\rbrace
+        \ell(\mu, \alpha) = \frac{n}{\alpha} \log(\alpha) +
+            \sum_i \left \lbrace
+            - \log \left( \frac{\Gamma(y_i + \alpha^{-1})}{
+            \Gamma(y_i + 1)\Gamma(\alpha^{-1})
+        } \right)
+        + (\alpha^{-1} + y_i) \log (\alpha^{-1} + \mu)
+        - y_i \log \mu
+            \right \rbrace
 
     This is implemented in this function.
 
     Parameters
     ----------
     counts : ndarray
         Observations.
 
     mu : ndarray
-        Mean of the distribution :math:`\\mu`.
+        Mean of the distribution :math:`\mu`.
 
     alpha : float or ndarray
-        Dispersion of the distribution :math:`\\alpha`,
-        s.t. the variance is :math:`\\mu + \\alpha \\mu^2`.
+        Dispersion of the distribution :math:`\alpha`,
+        s.t. the variance is :math:`\mu + \alpha \mu^2`.
 
     Returns
     -------
     float or ndarray
         Negative log likelihood of the observations counts
-        following :math:`NB(\\mu, \\alpha)`.
+        following :math:`NB(\mu, \alpha)`.
 
     Notes
     -----
     [1] https://en.wikipedia.org/wiki/Negative_binomial_distribution
     """
     n = len(counts)
     alpha_neg1 = 1 / alpha
@@ -417,20 +417,20 @@
         Observations.
 
     mu : float
         Mean of the distribution.
 
     alpha : float
         Dispersion of the distribution,
-        s.t. the variance is :math:`\\mu + \\alpha * \\mu^2`.
+        s.t. the variance is :math:`\mu + \alpha\mu^2`.
 
     Returns
     -------
     float
-        Derivative of negative log likelihood of NB w.r.t. :math:`\\alpha`.
+        Derivative of negative log likelihood of NB w.r.t. :math:`\alpha`.
     """
     alpha_neg1 = 1 / alpha
     ll_part = (
         alpha_neg1**2
         * (
             polygamma(0, alpha_neg1)
             - polygamma(0, counts + alpha_neg1)
@@ -1464,15 +1464,15 @@
     **kwargs,
 ) -> None:
     """
     Create an log ratio (M)-average (A) plot using matplotlib.
 
     Useful for looking at log fold-change versus mean expression
     between two groups/samples/etc.
-    Uses matplotlib to emulate make_MA() function in DESeq2 in R.
+    Uses matplotlib to emulate the ``make_MA()`` function in DESeq2 in R.
 
     Parameters
     ----------
     results_df : pd.DataFrame
         Resultant dataframe after running DeseqStats() and .summary().
 
     padj_thresh : float
```

### Comparing `pydeseq2-0.4.8/pydeseq2.egg-info/PKG-INFO` & `pydeseq2-0.4.9/pydeseq2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: anndata>=0.8.0
-Requires-Dist: numpy>=1.23.0
-Requires-Dist: pandas>=1.4.0
-Requires-Dist: scikit-learn>=1.1.0
-Requires-Dist: scipy>=1.11.0
-Requires-Dist: matplotlib>=3.6.2
 Provides-Extra: dev
-Requires-Dist: pytest>=6.2.4; extra == "dev"
-Requires-Dist: pre-commit>=2.13.0; extra == "dev"
-Requires-Dist: numpydoc; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pandas-stubs; extra == "dev"
+License-File: LICENSE
 
 <img src="docs/source/_static/pydeseq2_logo_green.png" width="600">
 
 #
 [![pypi version](https://img.shields.io/pypi/v/pydeseq2)](https://pypi.org/project/pydeseq2)
 [![pypiDownloads](https://static.pepy.tech/badge/pydeseq2)](https://pepy.tech/project/pydeseq2)
 [![condaDownloads](https://img.shields.io/conda/dn/bioconda/pydeseq2?logo=Anaconda)](https://anaconda.org/bioconda/pydeseq2)
```

### Comparing `pydeseq2-0.4.8/pyproject.toml` & `pydeseq2-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/setup.py` & `pydeseq2-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/tests/test_edge_cases.py` & `pydeseq2-0.4.9/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.4.8/tests/test_pydeseq2.py` & `pydeseq2-0.4.9/tests/test_pydeseq2.py`

 * *Files 5% similar despite different names*

```diff
@@ -238,14 +238,59 @@
     # Check that the same LFC are found (up to tol)
     assert (
         abs(r_shrunk_res.log2FoldChange - shrunk_res.log2FoldChange)
         / abs(r_shrunk_res.log2FoldChange)
     ).max() < tol
 
 
+def test_lfc_shrinkage_no_apeAdapt(counts_df, metadata, tol=0.02):
+    """Test that the outputs of the lfc_shrink function match those of the original
+    R package (starting from the same inputs), up to a tolerance in relative error.
+    """
+
+    test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
+    r_res = pd.read_csv(
+        os.path.join(test_path, "data/single_factor/r_test_res.csv"), index_col=0
+    )
+    r_shrunk_res = pd.read_csv(
+        os.path.join(
+            test_path, "data/single_factor/r_test_lfc_shrink_no_apeAdapt_res.csv"
+        ),
+        index_col=0,
+    )
+
+    r_size_factors = pd.read_csv(
+        os.path.join(test_path, "data/single_factor/r_test_size_factors.csv"),
+        index_col=0,
+    ).squeeze()
+
+    r_dispersions = pd.read_csv(
+        os.path.join(test_path, "data/single_factor/r_test_dispersions.csv"),
+        index_col=0,
+    ).squeeze()
+
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
+    dds.deseq2()
+    dds.obsm["size_factors"] = r_size_factors.values
+    dds.varm["dispersions"] = r_dispersions.values
+    dds.varm["LFC"].iloc[:, 1] = r_res.log2FoldChange.values * np.log(2)
+
+    res = DeseqStats(dds)
+    res.summary()
+    res.SE = r_res.lfcSE * np.log(2)
+    res.lfc_shrink(coeff="condition_B_vs_A", adapt=False)
+    shrunk_res = res.results_df
+
+    # Check that the same LFC are found (up to tol)
+    assert (
+        abs(r_shrunk_res.log2FoldChange - shrunk_res.log2FoldChange)
+        / abs(r_shrunk_res.log2FoldChange)
+    ).max() < tol
+
+
 def test_iterative_size_factors(counts_df, metadata, tol=0.02):
     """Test that the outputs of the iterative size factor method match those of the
     original R package (starting from the same inputs), up to a tolerance in relative
     error.
     """
 
     test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
```

### Comparing `pydeseq2-0.4.8/tests/test_utils.py` & `pydeseq2-0.4.9/tests/test_utils.py`

 * *Files identical despite different names*

