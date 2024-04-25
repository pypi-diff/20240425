# Comparing `tmp/tajimas_d-2.0.1.tar.gz` & `tmp/tajimas_d-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tajimas_d-2.0.1.tar", last modified: Tue Mar 12 10:25:10 2024, max compression
+gzip compressed data, was "tajimas_d-2.0.2.tar", last modified: Thu Apr 25 08:25:53 2024, max compression
```

## Comparing `tajimas_d-2.0.1.tar` & `tajimas_d-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 10:25:10.718708 tajimas_d-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-12 10:25:10.718708 tajimas_d-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-12 10:25:10.718708 tajimas_d-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 10:25:10.714708 tajimas_d-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 10:25:10.714708 tajimas_d-2.0.1/src/tajimas_d/
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/src/tajimas_d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6741 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/src/tajimas_d/_tajimas_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 10:25:10.714708 tajimas_d-2.0.1/src/tajimas_d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 10:25:10.000000 tajimas_d-2.0.1/src/tajimas_d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 10:25:10.714708 tajimas_d-2.0.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1445 2024-03-12 10:25:03.000000 tajimas_d-2.0.1/tests/test_tajimasd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:25:53.734514 tajimas_d-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-25 08:25:53.734514 tajimas_d-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-25 08:25:53.734514 tajimas_d-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:25:53.730514 tajimas_d-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:25:53.730514 tajimas_d-2.0.2/src/tajimas_d/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/src/tajimas_d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/src/tajimas_d/_tajimas_d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:25:53.730514 tajimas_d-2.0.2/src/tajimas_d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 08:25:53.000000 tajimas_d-2.0.2/src/tajimas_d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:25:53.730514 tajimas_d-2.0.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1445 2024-04-25 08:25:46.000000 tajimas_d-2.0.2/tests/test_tajimasd.py
```

### Comparing `tajimas_d-2.0.1/LICENSE` & `tajimas_d-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tajimas_d-2.0.1/PKG-INFO` & `tajimas_d-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajimas_d
-Version: 2.0.1
+Version: 2.0.2
 Summary: Computes Tajimas D, the Pi- or Watterson-Estimator for multiple sequences.
 Home-page: https://github.com/not-a-feature/tajimas_d/
 Author: Jules Kreuer / not_a_feature
 License: gpl-3.0
 Keywords: Tajima,Tajimas D,Pi,Watterson,Estimator,Population,Bioinformatics,Genetics
 Platform: unix
 Platform: linux
@@ -17,45 +17,46 @@
 License-File: LICENSE
 Provides-Extra: testing
 Requires-Dist: pytest>=6.0; extra == "testing"
 Requires-Dist: pytest-cov>=2.0; extra == "testing"
 Requires-Dist: tox>=3.20; extra == "testing"
 Requires-Dist: miniFasta>=2.2; extra == "testing"
 
-![tajimas-d](https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png)
+<img src="https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png" width=300px alt="tajimas_d logo"></img>
 
 Compute the Tajima's-D, Pi-Estimator or Watterson-Estimator for multiple sequences.
 
+This module is now part of the bfx suite. See https://py-bfx.readthedocs.io for more information.
+
 ![Test Badge](https://github.com/not-a-feature/tajimas_d/actions/workflows/tests.yml/badge.svg)
 ![Python Version Badge](https://img.shields.io/pypi/pyversions/tajimas_d)
 ![Download Badge](https://img.shields.io/pypi/dm/tajimas_d.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Tajima's D is a population genetic test statistic that computes the difference between the mean number of pairwise differences and the number of segregating sites. It is used to determine whether a population is expanding or shrinking.
 
 ## Tajima's D
 Tajima's D is defined as follows:
+$\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}}$
 
-![Tajima](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}})
-
-If ![expanding](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<0), there are many rare variants, indicating an **expanding** population.
+If $\theta_\text{Tajima}<0$, there are many rare variants, indicating an **expanding** population.
 
-Whereas ![declining](https://render.githubusercontent.com/render/math?math=0<\theta_\text{Tajima}), indicates an **declining** population as there are many intermediate variants.
+Whereas $0<\theta_\text{Tajima}$, indicates an **declining** population as there are many intermediate variants.
 
-A result is consideres significant if  ![declining-sig](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<-2) or ![expanding-sig](https://render.githubusercontent.com/render/math?math=2<\theta_\text{Tajima}).
+A result is consideres significant if $\theta_\text{Tajima}<-2$ or $2<\theta_\text{Tajima}$.
 
 ## Pi-Estimator
 The π estimator is the average number of pairwise differences between any two sequences:
 
-![Pi](https://render.githubusercontent.com/render/math?math=\theta_{\pi}=\frac{\text{Nr.%20of%20pairwise%20differences}}{\binom{n}{2}})
+$\theta_{\pi}=\frac{\text{Nr. of pairwise differences}}{\binom{n}{2}}$
 
 ## Watterson-Estimator
 The Watterson estimator is the expected number of segregating sites.
 
-![Watterson](https://render.githubusercontent.com/render/math?math=\theta_{\W}=\frac{\text{Nr.%20of%20segregating%20sites}}{\sum^{n-1}_{i=1}\frac{1}{i}})
+$\theta_{W}=\frac{\text{Nr. of segregating sites}}{\Sigma_{i=1}^{n-1}\frac{1}{i}}$
 
 ## Installation
 Using pip  / pip3:
 ```bash
 pip install tajimas_d
 ```
```

### Comparing `tajimas_d-2.0.1/README.md` & `tajimas_d-2.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-![tajimas-d](https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png)
+<img src="https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png" width=300px alt="tajimas_d logo"></img>
 
 Compute the Tajima's-D, Pi-Estimator or Watterson-Estimator for multiple sequences.
 
+This module is now part of the bfx suite. See https://py-bfx.readthedocs.io for more information.
+
 ![Test Badge](https://github.com/not-a-feature/tajimas_d/actions/workflows/tests.yml/badge.svg)
 ![Python Version Badge](https://img.shields.io/pypi/pyversions/tajimas_d)
 ![Download Badge](https://img.shields.io/pypi/dm/tajimas_d.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Tajima's D is a population genetic test statistic that computes the difference between the mean number of pairwise differences and the number of segregating sites. It is used to determine whether a population is expanding or shrinking.
 
 ## Tajima's D
 Tajima's D is defined as follows:
+$\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}}$
 
-![Tajima](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}})
-
-If ![expanding](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<0), there are many rare variants, indicating an **expanding** population.
+If $\theta_\text{Tajima}<0$, there are many rare variants, indicating an **expanding** population.
 
-Whereas ![declining](https://render.githubusercontent.com/render/math?math=0<\theta_\text{Tajima}), indicates an **declining** population as there are many intermediate variants.
+Whereas $0<\theta_\text{Tajima}$, indicates an **declining** population as there are many intermediate variants.
 
-A result is consideres significant if  ![declining-sig](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<-2) or ![expanding-sig](https://render.githubusercontent.com/render/math?math=2<\theta_\text{Tajima}).
+A result is consideres significant if $\theta_\text{Tajima}<-2$ or $2<\theta_\text{Tajima}$.
 
 ## Pi-Estimator
 The π estimator is the average number of pairwise differences between any two sequences:
 
-![Pi](https://render.githubusercontent.com/render/math?math=\theta_{\pi}=\frac{\text{Nr.%20of%20pairwise%20differences}}{\binom{n}{2}})
+$\theta_{\pi}=\frac{\text{Nr. of pairwise differences}}{\binom{n}{2}}$
 
 ## Watterson-Estimator
 The Watterson estimator is the expected number of segregating sites.
 
-![Watterson](https://render.githubusercontent.com/render/math?math=\theta_{\W}=\frac{\text{Nr.%20of%20segregating%20sites}}{\sum^{n-1}_{i=1}\frac{1}{i}})
+$\theta_{W}=\frac{\text{Nr. of segregating sites}}{\Sigma_{i=1}^{n-1}\frac{1}{i}}$
 
 ## Installation
 Using pip  / pip3:
 ```bash
 pip install tajimas_d
 ```
```

### Comparing `tajimas_d-2.0.1/setup.cfg` & `tajimas_d-2.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tajimas_d
-version = 2.0.1
+version = 2.0.2
 description = Computes Tajimas D, the Pi- or Watterson-Estimator for multiple sequences.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Tajima, Tajimas D, Pi, Watterson, Estimator, Population, Bioinformatics, Genetics
 home-page = https://github.com/not-a-feature/tajimas_d/
 author = Jules Kreuer / not_a_feature
 license = gpl-3.0
```

### Comparing `tajimas_d-2.0.1/src/tajimas_d/_tajimas_d.py` & `tajimas_d-2.0.2/src/tajimas_d/_tajimas_d.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,45 +6,61 @@
 @author: Jules Kreuer / not_a_feature
 License: GPL-3.0
 """
 
 from itertools import combinations
 from typing import List
 import argparse
-import miniFasta
+
+try:
+    from miniFasta import fasta_object, read
+except ModuleNotFoundError:
+    # Import as submodule of the bfx suite.
+    from ....miniFasta.src.miniFasta import fasta_object, read  # type: ignore
+
 from sys import argv
 
 
 def __check(sequences: List[str]) -> None:
     """
     Check for valid sequence proportions (1 < n, samle length).
 
-    Input:
-        sequences: list of str, list of sequences.
-    Returns:
-        Raises ValueError
+    Parameters
+    ----------
+        sequences: List[str]
+            List of sequences.
+
+    Raises
+    -------
+        ValueError: If less than two sequences are provided.
     """
     if len(sequences) < 2:
         raise ValueError("At leat 2 sequences required")
 
     ref_len = len(sequences[0])
     if not all([len(s) == ref_len for s in sequences]):
         raise ValueError("Sequences are required to have the same length.")
 
 
 def pi_estimator(sequences: List[str], safe=True) -> float:
     """
     Computes Θ_π, the Pi estimator.
     Θ_π = Number of pairwise differences / binomial(n, 2)
 
-    Input:
-        sequences: list of str, list of sequences.
-        safe: bool, check if sequences have the same length.
-    Returns:
-        Θ_π: float: Pi estimator.
+    Parameters
+    ----------
+        sequences: List[str]
+            List of sequences.
+        safe: bool, default: True
+            Check if sequences have the same length.
+
+    Returns
+    -------
+        Θ_π: float
+            Pi estimator value.
     """
     # Check for valid sequence proportions.
     if safe:
         __check(sequences)
 
     pairwise = combinations(sequences, 2)
     # Pairwise differences
@@ -55,18 +71,21 @@
     return sum(cs) / binomial
 
 
 def __segregating(sequences: List[str]) -> int:
     """
     Counts the number of segregating sites.
 
-    Input:
-        sequences: list of str, list of sequences.
+    Parameters
+    ----------
+        sequences: List[str]
+            List of sequences.
     Returns:
-        seg_sites: int, number of segregating sites.
+        seg_sites: int
+            Number of segregating sites.
     """
     seg_sites = 0
     # For each position in sequence
     for i in range(0, len(sequences[0])):
         s = sequences[0][i]  # Take the char of first sequence as reference
         for seq in sequences:  # For each other sequence
             if not seq[i] == s:
@@ -74,31 +93,43 @@
                 break  # And stop comparing this position
     return seg_sites
 
 
 def __harmonic(n: int) -> float:
     """
     Computes the n-1th harmonic number.
-    Input:
+
+    Parameters
+    ----------
         n: int
-    Returns:
-        h: float, n-1th harmonic number
+
+    Returns
+    -------
+        h: float
+            N-th harmonic number
     """
     return sum([1 / i for i in range(1, n)])
 
 
 def watterson_estimator(sequences: List[str], safe=True) -> float:
     """
     Computes Θ_W, the Watterson estimator.
     Θ_W = Number of segregating sites / (n th harmonic number)
-    Input:
-        sequences: list of str, list of sequences.
-        safe: bool, check for valid sequence proportions.
-    Returns:
-        Θ_W: float: Watterson estimator.
+
+    Parameters
+    ----------
+        sequences: List[str]
+            List of sequences.
+        safe: bool, default: True
+            Check for valid sequence proportions.
+
+    Returns
+    -------
+        Θ_W: float
+            Watterson estimator value.
     """
     # Check for valid sequence proportions.
     if safe:
         __check(sequences)
 
     seg_sites = __segregating(sequences)
     harmonic = __harmonic(len(sequences))
@@ -107,20 +138,23 @@
 
 
 def tajimas_d(sequences: List[str]) -> float:
     """
     Computes Tajima's D for a list of sequences.
     See: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1203831/
     and https://ocw.mit.edu/courses/health-sciences-and-technology/hst-508-quantitative-
-        genomics-fall-2005/study-materials/tajimad1.pdf
+    genomics-fall-2005/study-materials/tajimad1.pdf
 
-    Input:
-        sequences: list of str, list of sequences.
+    Parameters
+    ----------
+        sequences: List[str]
+            List of sequences.
     Returns:
-        Θ_D: float: Tajima's D.
+        Θ_D: float
+            Tajima's D value.
     """
     # Check for valid sequence proportions.
     __check(sequences)
 
     seg_sites = __segregating(sequences)  # Number of segregatig sites
 
     # Prevent devision by 0
@@ -148,20 +182,23 @@
     tD = delta_Theta / (((e1 * seg_sites) + (e2 * seg_sites * (seg_sites - 1))) ** 0.5)  # Ref 27
     return float(tD)
 
 
 def parse_args(args):
     """Parse command line parameters.
 
-    Args:
+    Args
+    ----
       args (List[str]): command line parameters as list of strings
           (for example  ``["--help"]``).
 
-    Returns:
-      :obj:`argparse.Namespace`: command line parameters namespace
+    Returns
+    -------
+      args: obj:`argparse.Namespace`
+        Command line parameters namespace
     """
     # Parse arguments
     parser = argparse.ArgumentParser(
         description="""tajimas_d: Compute Tajima's D, the Pi- or Watterson-Estimator for multiple sequences."""
     )
 
     parser.add_argument(
@@ -202,15 +239,15 @@
 
     return parser.parse_args()
 
 
 def _main_cli(args):
     args = parse_args(args)
     # Load sequences
-    sequences = [mf.body for mf in miniFasta.read(args.path)]
+    sequences = [mf.body for mf in read(args.path)]
 
     # Compute
     if args.tajima or not (args.pi or args.watterson):
         print(f"Tajima's D score:\t\t{tajimas_d(sequences)}")
 
     if args.pi:
         print(f"Pi-Estimator score:\t\t{pi_estimator(sequences)}")
```

### Comparing `tajimas_d-2.0.1/src/tajimas_d.egg-info/PKG-INFO` & `tajimas_d-2.0.2/src/tajimas_d.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajimas_d
-Version: 2.0.1
+Version: 2.0.2
 Summary: Computes Tajimas D, the Pi- or Watterson-Estimator for multiple sequences.
 Home-page: https://github.com/not-a-feature/tajimas_d/
 Author: Jules Kreuer / not_a_feature
 License: gpl-3.0
 Keywords: Tajima,Tajimas D,Pi,Watterson,Estimator,Population,Bioinformatics,Genetics
 Platform: unix
 Platform: linux
@@ -17,45 +17,46 @@
 License-File: LICENSE
 Provides-Extra: testing
 Requires-Dist: pytest>=6.0; extra == "testing"
 Requires-Dist: pytest-cov>=2.0; extra == "testing"
 Requires-Dist: tox>=3.20; extra == "testing"
 Requires-Dist: miniFasta>=2.2; extra == "testing"
 
-![tajimas-d](https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png)
+<img src="https://github.com/not-a-feature/tajimas_d/raw/main/tajimas-d.png" width=300px alt="tajimas_d logo"></img>
 
 Compute the Tajima's-D, Pi-Estimator or Watterson-Estimator for multiple sequences.
 
+This module is now part of the bfx suite. See https://py-bfx.readthedocs.io for more information.
+
 ![Test Badge](https://github.com/not-a-feature/tajimas_d/actions/workflows/tests.yml/badge.svg)
 ![Python Version Badge](https://img.shields.io/pypi/pyversions/tajimas_d)
 ![Download Badge](https://img.shields.io/pypi/dm/tajimas_d.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Tajima's D is a population genetic test statistic that computes the difference between the mean number of pairwise differences and the number of segregating sites. It is used to determine whether a population is expanding or shrinking.
 
 ## Tajima's D
 Tajima's D is defined as follows:
+$\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}}$
 
-![Tajima](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}=\frac{\theta_{\pi}%20-%20\theta_{W}}{\sqrt{\text{Var}(\theta_{\pi}-\theta_{W})}})
-
-If ![expanding](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<0), there are many rare variants, indicating an **expanding** population.
+If $\theta_\text{Tajima}<0$, there are many rare variants, indicating an **expanding** population.
 
-Whereas ![declining](https://render.githubusercontent.com/render/math?math=0<\theta_\text{Tajima}), indicates an **declining** population as there are many intermediate variants.
+Whereas $0<\theta_\text{Tajima}$, indicates an **declining** population as there are many intermediate variants.
 
-A result is consideres significant if  ![declining-sig](https://render.githubusercontent.com/render/math?math=\theta_\text{Tajima}<-2) or ![expanding-sig](https://render.githubusercontent.com/render/math?math=2<\theta_\text{Tajima}).
+A result is consideres significant if $\theta_\text{Tajima}<-2$ or $2<\theta_\text{Tajima}$.
 
 ## Pi-Estimator
 The π estimator is the average number of pairwise differences between any two sequences:
 
-![Pi](https://render.githubusercontent.com/render/math?math=\theta_{\pi}=\frac{\text{Nr.%20of%20pairwise%20differences}}{\binom{n}{2}})
+$\theta_{\pi}=\frac{\text{Nr. of pairwise differences}}{\binom{n}{2}}$
 
 ## Watterson-Estimator
 The Watterson estimator is the expected number of segregating sites.
 
-![Watterson](https://render.githubusercontent.com/render/math?math=\theta_{\W}=\frac{\text{Nr.%20of%20segregating%20sites}}{\sum^{n-1}_{i=1}\frac{1}{i}})
+$\theta_{W}=\frac{\text{Nr. of segregating sites}}{\Sigma_{i=1}^{n-1}\frac{1}{i}}$
 
 ## Installation
 Using pip  / pip3:
 ```bash
 pip install tajimas_d
 ```
```

### Comparing `tajimas_d-2.0.1/tests/test_tajimasd.py` & `tajimas_d-2.0.2/tests/test_tajimasd.py`

 * *Files identical despite different names*

