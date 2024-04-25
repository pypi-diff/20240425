# Comparing `tmp/barmuscomp-0.1.2.tar.gz` & `tmp/barmuscomp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\amarmore\Desktop\Projects\PhD main projects\Releases\barmuscomp\pip version (sans notebook)\dist\.tmp-jzv5ria_\barmusc", last modified: Tue Jan 17 18:36:36 2023, max compression
+gzip compressed data, was "barmuscomp-0.1.3.tar", last modified: Thu Apr 25 15:14:22 2024, max compression
```

## Comparing `barmuscomp-0.1.2.tar` & `barmuscomp-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 18:36:36.000000 barmuscomp-0.1.2/
--rw-rw-rw-   0        0        0       88 2022-09-21 14:47:09.000000 barmuscomp-0.1.2/AUTHORS
--rw-rw-rw-   0        0        0     1516 2022-09-21 14:48:42.000000 barmuscomp-0.1.2/LICENSE.md
--rw-rw-rw-   0        0        0     3768 2023-01-17 18:36:36.000000 barmuscomp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3031 2023-01-17 18:34:19.000000 barmuscomp-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp/
--rw-rw-rw-   0        0        0      318 2022-12-23 14:40:15.000000 barmuscomp-0.1.2/barmuscomp/__init__.py
--rw-rw-rw-   0        0        0    37466 2022-12-23 21:20:01.000000 barmuscomp-0.1.2/barmuscomp/ae.py
--rw-rw-rw-   0        0        0    20097 2022-12-23 14:42:03.000000 barmuscomp-0.1.2/barmuscomp/ae_ntd.py
--rw-rw-rw-   0        0        0    13949 2022-12-23 14:42:36.000000 barmuscomp-0.1.2/barmuscomp/ae_utils.py
--rw-rw-rw-   0        0        0    13860 2022-12-23 20:40:11.000000 barmuscomp-0.1.2/barmuscomp/lra.py
-drwxrwxrwx   0        0        0        0 2023-01-17 18:36:36.000000 barmuscomp-0.1.2/barmuscomp/model/
--rw-rw-rw-   0        0        0        0 2022-12-23 14:40:38.000000 barmuscomp-0.1.2/barmuscomp/model/__init__.py
--rw-rw-rw-   0        0        0     7506 2022-12-23 22:59:00.000000 barmuscomp-0.1.2/barmuscomp/model/current_plot.py
--rw-rw-rw-   0        0        0     3039 2021-09-22 13:36:36.000000 barmuscomp-0.1.2/barmuscomp/model/early_stopping.py
--rw-rw-rw-   0        0        0      212 2022-12-22 14:43:38.000000 barmuscomp-0.1.2/barmuscomp/model/errors.py
--rw-rw-rw-   0        0        0     4535 2022-12-23 14:43:43.000000 barmuscomp-0.1.2/barmuscomp/model/features.py
--rw-rw-rw-   0        0        0    20432 2022-12-23 14:43:47.000000 barmuscomp-0.1.2/barmuscomp/model/pattern_study.py
--rw-rw-rw-   0        0        0     5004 2022-12-23 14:44:04.000000 barmuscomp-0.1.2/barmuscomp/model/plot_comparison_ae_ntd.py
-drwxrwxrwx   0        0        0        0 2023-01-17 18:36:36.000000 barmuscomp-0.1.2/barmuscomp/scripts/
--rw-rw-rw-   0        0        0        0 2021-09-20 17:43:10.000000 barmuscomp-0.1.2/barmuscomp/scripts/__init__.py
--rw-rw-rw-   0        0        0     1814 2022-12-22 14:54:01.000000 barmuscomp-0.1.2/barmuscomp/scripts/default_path.py
--rw-rw-rw-   0        0        0     7607 2022-12-23 14:45:12.000000 barmuscomp-0.1.2/barmuscomp/scripts/overall_scripts.py
-drwxrwxrwx   0        0        0        0 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/
--rw-rw-rw-   0        0        0     3768 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-17 18:36:35.000000 barmuscomp-0.1.2/barmuscomp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-17 18:36:36.000000 barmuscomp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1315 2023-01-17 18:36:08.000000 barmuscomp-0.1.2/setup.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       88 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/AUTHORS
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1503 2024-01-10 11:57:04.000000 barmuscomp-0.1.3/LICENSE.md
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3711 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     2985 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/README.md
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      305 2024-01-10 11:57:01.000000 barmuscomp-0.1.3/barmuscomp/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    36646 2024-01-10 11:57:01.000000 barmuscomp-0.1.3/barmuscomp/ae.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19648 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/ae_ntd.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13589 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/ae_utils.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13546 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/lra.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/model/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/model/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7339 2024-01-31 09:55:24.000000 barmuscomp-0.1.3/barmuscomp/model/current_plot.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3039 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/model/early_stopping.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      201 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/errors.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4388 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/features.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19983 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/pattern_study.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4910 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/plot_comparison_ae_ntd.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/scripts/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/scripts/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1790 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/scripts/default_path.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7444 2024-01-10 11:57:04.000000 barmuscomp-0.1.3/barmuscomp/scripts/overall_scripts.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp.egg-info/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3711 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      642 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/SOURCES.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/dependency_links.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      172 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/requires.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       11 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/top_level.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/setup.cfg
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1329 2024-04-25 15:14:06.000000 barmuscomp-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `barmuscomp-0.1.2/LICENSE.md` & `barmuscomp-0.1.3/LICENSE.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright (c) 2022 Marmoret Axel
-
-BSD 3-Clause "New" or "Revised" License
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2022 Marmoret Axel
+
+BSD 3-Clause "New" or "Revised" License
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `barmuscomp-0.1.2/PKG-INFO` & `barmuscomp-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-Metadata-Version: 2.1
-Name: barmuscomp
-Version: 0.1.2
-Summary: Package for barwise compression applied on musical segmentation.
-Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
-Author: Marmoret Axel
-Author-email: axel.marmoret@irisa.fr
-License: BSD
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8.*
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: AUTHORS
-
-# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
-
-Hello, and welcome on this repository!
-
-This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
-
-This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
-
-This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
-
-It can be installed with pip using `pip install barmuscomp`.
-
-This is a first release, and may contain bug. Comments are welcomed!
-
-## Software version ##
-
-This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
-
-## Tutorial Notebook ##
-
-3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
-
-They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
-
-## How to cite ##
-
-You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
-
-Here are two styles of citations:
-
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
-
-In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
-
-## Credits ##
-
-Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
-
-The technique in itself was also developed by FrÃ©dÃ©ric Bimbot (<bimbot@irisa.fr>).
-
-## References ##
-[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, UniversitÃ© de Rennes 1, 2022.
-(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
-
-[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
-
-[3] A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices", 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+Metadata-Version: 2.1
+Name: barmuscomp
+Version: 0.1.3
+Summary: Package for barwise compression applied on musical segmentation.
+Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
+Author: Marmoret Axel
+Author-email: axel.marmoret@irisa.fr
+License: BSD
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS
+
+# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
+
+Hello, and welcome on this repository!
+
+This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
+
+This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
+
+This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
+
+It can be installed with pip using `pip install barmuscomp`.
+
+This is a first release, and may contain bug. Comments are welcomed!
+
+## Software version ##
+
+This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
+
+## Tutorial Notebook ##
+
+3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
+
+They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
+
+## How to cite ##
+
+You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
+
+Here are two styles of citations:
+
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+
+In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
+
+## Credits ##
+
+Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
+
+The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
+
+## References ##
+[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, Université de Rennes 1, 2022.
+(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
+
+[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
+
+[3] A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices", 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+
```

### Comparing `barmuscomp-0.1.2/README.md` & `barmuscomp-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
-
-Hello, and welcome on this repository!
-
-This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
-
-This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
-
-This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
-
-It can be installed with pip using `pip install barmuscomp`.
-
-This is a first release, and may contain bug. Comments are welcomed!
-
-## Software version ##
-
-This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
-
-## Tutorial Notebook ##
-
-3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
-
-They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
-
-## How to cite ##
-
-You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
-
-Here are two styles of citations:
-
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
-
-In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
-
-## Credits ##
-
-Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
-
-The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
-
-## References ##
-[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, Université de Rennes 1, 2022.
-(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
-
-[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
-
+# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
+
+Hello, and welcome on this repository!
+
+This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
+
+This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
+
+This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
+
+It can be installed with pip using `pip install barmuscomp`.
+
+This is a first release, and may contain bug. Comments are welcomed!
+
+## Software version ##
+
+This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
+
+## Tutorial Notebook ##
+
+3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
+
+They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
+
+## How to cite ##
+
+You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
+
+Here are two styles of citations:
+
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+
+In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
+
+## Credits ##
+
+Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
+
+The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
+
+## References ##
+[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, Université de Rennes 1, 2022.
+(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
+
+[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
+
 [3] A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices", 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
```

### Comparing `barmuscomp-0.1.2/barmuscomp/ae.py` & `barmuscomp-0.1.3/barmuscomp/ae.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,820 +1,820 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 14 18:46:42 2021
-
-@author: amarmore
-
-Single-song autoencoding paradigm.
-
-See [1 - Chapter 5.4] or [2] for more information.
-
-References
-----------
-[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
-PhD Thesis Marmoret Axel 
-(not uploaded yet but will be soon!)
-(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
-
-[2] Marmoret, A., Cohen, J.E, and Bimbot, F., "Barwise Compression Schemes 
-for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, 
-SMC 2022, Sound and music Computing network, 2022.
-"""
-
-import as_seg.barwise_input as bi
-import barmuscomp.ae_utils as ae_utils
-from barmuscomp.model.early_stopping import EarlyStopping
-import barmuscomp.model.current_plot as current_plot
-import barmuscomp.model.errors as err
-
-import numpy as np
-import random
-import warnings
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-class GenericAutoencoder(nn.Module):
-    """
-    General autoencoder, acting as a parent class, specifying the functions shared between models.
-    
-    This autoencoder does not define an encoder or a decoder, they must be specified in children classes.
-    """
-    def __init__(self, dim_latent_space = 16, beta = 2, latent_nonlinearity = None, seed = None):
-        """
-        Constructor of the autoencoder.
-
-        Parameters
-        ----------
-        dim_latent_space : positive int, optional
-            Dimension of the latent space. 
-            The default is 16.
-        beta : float, optional
-            The beta value in the beta-divergence, 
-            specifying the loss function between the input and the output. 
-            The default is 2 (i.e. Euclidean Loss).
-            See [1,2] for details on the beta-divergence.
-        latent_nonlinearity : string, optional
-            A value specfiying the choice for a nonlinear activation function
-            constraining the values of the latent representation.
-            The default is None, meaning no nonlinear activation function.
-        seed : float, optional
-            A seed to fix pseudo-randomness.
-            The default is None, meaning no seed.
-
-        Raises
-        ------
-        InvalidArgumentValueException
-            Raised if the specified nonlinear activation function is unknown.
-        
-        References
-        ----------
-        [1] Basu, A., Harris, I.R., Hjort, L.N., and Jones, M.C., "Robust and Efficient
-        Estimation by Minimising a Density Power Divergence", in: Biometrika 85.3 (1998),
-        pp. 549–559, issn: 00063444.
-        
-        [2] Marmoret, A., Voorwinden, F., Leplat, V., Cohen, J.E., and Bimbot, F.,
-        "Nonnegative Tucker Decomposition with Beta-divergence for Music Structure 
-        Analysis of audio signals", in: GRETSI (2022).
-
-        """
-        super(GenericAutoencoder, self).__init__()
-        self.device = "cuda" if torch.cuda.is_available() else "cpu"
-        
-        self.dim_latent_space = dim_latent_space
-        self.beta = beta
-        self.seed = seed
-        
-        if latent_nonlinearity is None:
-            self.latent_nonlinearity = None
-        elif latent_nonlinearity == "sigmoid":
-            self.latent_nonlinearity = nn.Sigmoid()
-        # elif latent_nonlinearity == "hardshrink":
-        #     self.latent_nonlinearity = nn.Hardshrink(lambd = 0.5)
-        elif latent_nonlinearity == "softmax":
-            self.latent_nonlinearity = nn.Softmax(dim=1)
-        elif latent_nonlinearity == "tanh":
-            self.latent_nonlinearity = nn.Tanh()
-        else:
-            raise err.InvalidArgumentValueException(f"Activation function not understood for the latent space: {latent_nonlinearity}") from None
-
-    def forward(self, x):
-        """
-        Forward pass.
-        x_hat is the reconstructed input, z is the latent projection.
-        """        
-        # Encoding
-        z = self.encoder(x)
-            
-        # Decoding
-        x_hat = self.decoder(z)
-
-        return x_hat, z
-    
-    def encoder(self, x):
-        """
-        Encoder default value, raising an error.
-        It must be implemented in chlidren classes.
-        """
-        raise NotImplementedError("To be redefined in children classes")
-    
-    def decoder(self, z):
-        """
-        Decoder default value, raising an error.
-        It must be implemented in chlidren classes.
-        """
-        raise NotImplementedError("To be redefined in children classes")
-    
-    def my_optim_method(self, n_epochs, data_loader, lr = 1e-3, early_stop_patience = 100, verbose = False, labels = None):
-        """
-        Default optimization method.
-        
-        This method is to be called in order to optimize the network.
-
-        Parameters
-        ----------
-        n_epochs : int
-            Number of epochs to perform.
-        data_loader : torch.DataLoader
-            The DataLoader to optimize on.
-        lr : float, optional
-            Learning rate of the Network. 
-            The default is 1e-3.
-        early_stop_patience : int, optional
-            Patience for the number of consecutive epochs.
-            If the loss doesn't decrease during early_stop_patience epochs, the optimization stops. 
-            The default is 100.
-        verbose : boolean, optional
-            Argument to print the evolution of the optimization.
-            Prints the current loss and plots a view of the autosimilarity of 
-            latent variables and a PCA of the latent space.
-            The default is False.
-        labels : None or array, optional
-            Only used if verbose is set to True.
-            If labels are set, they will be used to color the output of PCA projection.
-            If they are set to None, no label is used. The default is None.
-
-        Returns
-        -------
-        GenericAutoencoder
-            The instance of the network, optimized.
-            NB: it is not required to return the network, this is rather implemented 
-            in order to avoid some "unintenional" optimization 
-            (as it forces a human user to notice that something is returned,
-             and hence that some code was run).
-        losses : list of positive floats
-            The loss values at each iteration.
-
-        """
-        self = self.to(self.device)
-        #print(f"Using {self.device}")
-        es = EarlyStopping(patience=early_stop_patience)
-        
-        nb_bars = 0
-        for iter_dl in data_loader:
-            nb_bars += iter_dl.shape[0]
-
-        if self.beta == 2:
-            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
-        else:
-            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
-            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
-        losses = []
-            
-        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
-        
-        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
-        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
-        
-        if self.seed is not None:
-            self.apply(lambda layer: ae_utils.seeded_weights_init_kaiming(layer, seed=self.seed))
-        else:
-            self.apply(ae_utils.random_weights_init_kaiming) # Random initialization of the network
-            
-        for epoch in range(1, n_epochs+1):
-            total_loss_epoch = 0.0
-            for spec in data_loader:
-                spec = spec.float().to(self.device)
-                optimizer.zero_grad()
-                spec_recons, z = self.forward(spec) # Forward pass
-                loss = recons_loss(spec_recons, spec) # Loss
-                loss.backward() # Backward pass
-                optimizer.step() # Optimizes the net with grads
-                
-                total_loss_epoch += loss.item() * spec.size(0)
-            total_loss_epoch = total_loss_epoch/nb_bars
-            losses.append(total_loss_epoch)
-            scheduler.step(total_loss_epoch) # scheduler for the decrease of lr on a plateau
-                
-            if verbose:
-                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
-                if epoch%50 == 0:
-                    projection = self.get_latent_projection(data_loader)
-                    current_plot.plot_latent_space(projection, labels = labels)
-                    
-            if es.step(total_loss_epoch): # Checks if loss has decreased, to stop the optimization if performances don't increase for early_stop_patience epochs.
-                if verbose:
-                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
-                break 
-        return self, losses
-    
-    def get_latent_projection(self, data_loader):
-        """
-        Returns the latent representation on a given network.
-        
-        Used after optimization to access to the latent representations.
-        
-        Parameters
-        ----------
-        data_loader : torch.DataLoader
-            The DataLoader to project (intended to be the same that the one used for optimization).
-
-        Returns
-        -------
-        all_data : numpy array
-            The latent representation for each data in the dataset.
-
-        """
-        all_data = []
-        for spec in data_loader:
-            spec = spec.float().to(self.device)
-            spec_recons, z = self.forward(spec)
-            for elt in z:
-                all_data.append(elt.cpu().detach().numpy())
-        return all_data
-       
-# %% Fully-connected
-def get_fc_ssae_projection(spectrogram, compression_dimension, bars, 
-                           n_epochs = 1000, lr = 1e-3, beta = 2, latent_nonlinearity = None, seed = None, 
-                           subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
-    """
-    Return the projection of the barwise content with a Fully-Connected AutoEncoder (SSAE).
-
-    Parameters
-    ----------
-    spectrogram : numpy array
-        The spectrogram to analyze, barwise.
-    compression_dimension : positive integer
-        Dimension of compression (size of the latent space).
-    bars : list of tuples
-        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
-    n_epochs : int
-        Number of epochs to perform.
-    lr : float, optional
-        Learning rate of the Network. 
-        The default is 1e-3.
-    beta, latent_nonlinearity, seed:
-        See GenericAutoencoder.
-    subdivision_bars : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    hop_length : integer, optional
-        The hop_length used for the computation of the spectrogram.
-        It is expressed in terms of number of samples, which are defined by the sampling rate.
-        The default is 32.
-    sampling_rate : float, optional
-        Sampling rate used when computing the spectrogram (typically 44100Hz).
-        The default is 44100.
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix (latent representations), of size (bars, compression_dimension).
-        
-    """
-    ae_model = FullyConnectedAutoencoder(input_size_x = subdivision_bars, input_size_y = spectrogram.shape[0], dim_latent_space = compression_dimension, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-    tensor_barwise_BFT = bi.tensorize_barwise_BFT(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
-    data_loader = ae_utils.generate_flatten_dataloader(tensor_barwise_BFT)
-    ae_model, losses = ae_model.my_optim_method(n_epochs=n_epochs, data_loader=data_loader, lr=lr, verbose = False, labels = None)
-    return ae_model.get_latent_projection(data_loader)
-
-class FullyConnectedAutoencoder(GenericAutoencoder):
-    """
-    AutoEncoder with fully-connected layers as encoder and decoder.
-    """
-    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None):#, batch_norm = True):
-        """
-        Constructor of the Fully-connected autoencoder.
-
-        Parameters
-        ----------
-        input_size_x : integer
-            Size of the x axis dimension of the input.
-        input_size_y : integer
-            Size of the y axis dimension of the input.
-        dim_latent_space, beta, latent_nonlinearity, seed:
-            See GenericAutoencoder.
-
-        """
-        super().__init__(dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-        self.fc = nn.Linear(in_features=input_size_x * input_size_y, out_features=128)
-        self.fc_2 = nn.Linear(in_features=128, out_features=dim_latent_space)
-        self.i_fc = nn.Linear(in_features=dim_latent_space, out_features=128)
-        self.i_fc_2 = nn.Linear(in_features=128, out_features=input_size_x * input_size_y)
-        
-        # self.batch_norm = batch_norm # DEPRECATED: it should always be designed with batch norm layers.
-        # if self.batch_norm:
-        self.bn_1 = nn.BatchNorm1d(128)
-        self.bn_2 = nn.BatchNorm1d(dim_latent_space)
-        self.i_bn_1 = nn.BatchNorm1d(128)
-       
-    def encoder(self, x):    
-        """
-        Encoder of the Fully-Connected network.
-        Two dense layers, each followed by a batch normalization layer.
-        The last layer (the 2nd one) may contain a nonnlinear activation function.
-        In that case, the activation function replace the batch normalization layer.
-        """
-        x = F.relu(self.fc(x))
-        x = self.bn_1(x)
-        x = self.fc_2(x)
-        if self.latent_nonlinearity is None:
-            return self.bn_2(x)
-        else:
-            return self.latent_nonlinearity(x)
-
-        
-    # def encoder(self, x):
-    #     """
-    #     Encoder definition.
-    #     Switch between an encoder with and without batch normalization layer.
-    #     """
-    #     if self.batch_norm:
-    #         z = self.bn_encoder(x)
-    #     else:
-    #         z = self.no_bn_encoder(x)
-
-    #     if self.latent_nonlinearity is not None:
-    #         z = self.latent_nonlinearity(z)
-    #     return z
-    
-    # def no_bn_encoder(self, x):
-    #     """
-    #     Encoder without batch normlization layers.
-    #     """
-    #     x = F.relu(self.fc(x))
-    #     return self.fc_2(x)
-        
-
-    def decoder(self, z):
-        """
-        Decoder of the Fully-Connected network.
-        Two dense layers. The first one is followed by a batch normalization layer.
-        """
-        x = F.relu(self.i_fc(z))
-        x = self.i_bn_1(x)
-        x_hat = self.i_fc_2(x)
-        
-        # To compute the beta-divergence, needing nonnegative outputs
-        x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
-        # TODO: Experiences should account for this bias, i.e. be redone.
-        return x_hat
-    
-    # def decoder(self, z):
-    #     """
-    #     Decoder definition.
-    #     Switch between a decoder with and without batch normalization layer.
-    #     """
-    #     if self.batch_norm:
-    #         return self.bn_decoder(z)
-    #     else:
-    #         return self.no_bn_decoder(z)
-        
-    
-    # def no_bn_decoder(self, z):
-    #     """
-    #     Decoder without batch normlization layers.
-    #     """
-    #     x = F.relu(self.i_fc(z))
-    #     x_hat = self.i_fc_2(x)
-        
-    #     # To compute the beta-divergence, needing nonnegative outputs
-    #     x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
-    #     return x_hat
-    
-# %% Convolutional
-def get_conv_ssae_projection(spectrogram, compression_dimension, bars, 
-                             n_epochs = 1000, lr = 1e-3, beta = 2, latent_nonlinearity = None, seed = None, 
-                             subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
-    """
-    Return the projection of the barwise content with a convolutional AutoEncoder (SSAE).
-
-    Parameters
-    ----------
-    spectrogram : list of list of floats or numpy array
-        The spectrogram to analyze, barwise.
-    compression_dimension : positive integer
-        Dimension of compression (size of the latent space).
-    bars : list of tuples
-        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
-    n_epochs : int
-        Number of epochs to perform.
-    lr : float, optional
-        Learning rate of the Network. 
-        The default is 1e-3.
-    beta, latent_nonlinearity, seed:
-        See GenericAutoencoder.
-    subdivision_bars : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    hop_length : integer, optional
-        The hop_length used for the computation of the spectrogram.
-        It is expressed in terms of number of samples, which are defined by the sampling rate.
-        The default is 32.
-    sampling_rate : float, optional
-        Sampling rate used when computing the spectrogram (typically 44100Hz).
-        The default is 44100.
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix (latent representations), of size (bars, compression_dimension).
-        
-    """
-    ae_model = ConvolutionalAutoencoder(input_size_x = subdivision_bars, input_size_y = spectrogram.shape[0], dim_latent_space = compression_dimension, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-    tensor_barwise_BFT = bi.tensorize_barwise_BFT(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
-    data_loader = ae_utils.generate_dataloader(tensor_barwise_BFT)
-    ae_model, losses = ae_model.my_optim_method(n_epochs=n_epochs, data_loader=data_loader, lr=lr, verbose = False, labels = None)
-    return ae_model.get_latent_projection(data_loader)
-
-class ConvolutionalAutoencoder(GenericAutoencoder):
-    """
-    Autoencoder with Convolutional layers as encoder and decoder.
-    """
-    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None):
-        """
-        Constructor of the Convolutional autoencoder.
-
-        Parameters
-        ----------
-        input_size_x : integer
-            Size of the x axis dimension of the input.
-        input_size_y : integer
-            Size of the y axis dimension of the input.
-        dim_latent_space, beta, latent_nonlinearity, seed:
-            See GenericAutoencoder.
-            
-        """
-        super().__init__(dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-        self.input_size_pool_y = int(input_size_y/4) # input_size / pool ## NOTE: Doesn't work for odd input sizes (in reconstruction), so TODO.
-        self.input_size_pool_x = int(input_size_x/4) # input_size / pool
-        
-        # Encoder
-        ## Convolutional layers
-        self.conv1 = nn.Conv2d(1, 4, 3, padding=1)  
-        self.conv2 = nn.Conv2d(4,16, 3, padding=1)
-        self.pool = nn.MaxPool2d(2, 2)
-        self.flatten = nn.Flatten()
-
-        ## Fully-connected controling latent space size.
-        in_features = 16 * self.input_size_pool_x * self.input_size_pool_y # nb_kernels_last_conv * (input_size / pool)
-        self.fc = nn.Linear(in_features=in_features, out_features=dim_latent_space)
-        
-        # Decoder
-        ## Inverse of previous FC
-        self.i_fc = nn.Linear(in_features=dim_latent_space, out_features=in_features)
-
-        # Transposed conv layers
-        self.t_conv1 = nn.ConvTranspose2d(16, 4, 3, stride=2, padding=1, output_padding=1)
-        self.t_conv2 = nn.ConvTranspose2d(4, 1, 3, stride=2, padding=1, output_padding=1)
-        
-        self.bn_1 = nn.BatchNorm2d(4)
-        self.bn_2 = nn.BatchNorm2d(16)
-        self.bn_fc = nn.BatchNorm1d(dim_latent_space)
-        
-        self.i_bn_fc = nn.BatchNorm1d(16 * self.input_size_pool_y * self.input_size_pool_x)
-        self.i_bn_1 = nn.BatchNorm2d(4)
-       
-           
-    def encoder(self, x):
-        """
-        Encoder of the Covolutional Autoencoder.
-        It is implemented with two convolutional layers, 
-        each followed by a ReLU, a pooling layer, and a batch normalization layer.
-        After these convolutional blocks, a fully-connected layer is implemented,
-        leading to the latent representations.
-        A batch normalization layer is implemented after the dense layer,
-        but it can be replaced by a nonlinear activation function if specified.
-        """
-        x = F.relu(self.conv1(x))
-        x = self.pool(x)
-        x = self.bn_1(x)
-        x = F.relu(self.conv2(x))
-        x = self.pool(x)
-        x = self.bn_2(x)
-        
-        x = self.flatten(x)
-        x = self.fc(x)
-        if self.latent_nonlinearity is None:
-            return self.bn_fc(x)
-        else:
-            return self.latent_nonlinearity(x)
-        
-    def decoder(self, z):
-        """
-        Decoder of the Convolutioanl autoencoder.
-        It is implemented as the inverse of the encoder, with a dense layer
-        followed by two transposed convolution layers.
-        The two first layers implement a batch normalization layer, but not the last one
-        (i.e. no batch normalization before the reconstruction).
-        """
-        x = self.i_fc(z)
-        x = self.i_bn_fc(x)
-        x = x.view((x.shape[0], 16, self.input_size_pool_y, self.input_size_pool_x))
-        x = F.relu(self.t_conv1(x))
-        x = self.i_bn_1(x)
-        x_hat = self.t_conv2(x)
-        
-        # To compute the beta-divergence, needing nonnegative outputs
-        x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
-        # TODO: Experiences should account for this bias, i.e. make new experiments.
-        return x_hat
-
-    
-class ConvolutionalAutoencoderTriplet(ConvolutionalAutoencoder):
-    """
-    Class defining AutoEncoders used to compress barwise representation of a song, with an added Triplet loss to regularize the latent space.
-    This triplet loss is designed to favor the bars which are very similar in the initial representation, 
-    and to scatter bars which are very dissimilar.
-    The positive (similar) and negative (dissimilar) examples are chosen by thresholding the autosimilarity matrix,
-    and taking either the most or least similar examples (hence, two thresolds parameters are to be defined, see my_optim_method()).
-    
-    For more information, refer to [1 - Chapter 5.4.5]
-    
-    References
-    ----------
-    [1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
-    PhD Thesis Marmoret Axel 
-    (not uploaded yet but will be soon!)
-    (You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
-    """
-    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None, triplet_lambda = 1, triplet_type = "simple", triplet_margins = [1]):
-        """
-        Constructor of the triplet-loss regularized convolutional autoencoder.
-        
-        input_size_x, input_size_y, dim_latent_space, beta, latent_nonlinearity, seed,
-            See parent class (ConvolutionalAutoencoder)
-        triplet_lambda : float, optional
-            Ponderation for the triplet loss in the mixed loss. The default is 1.
-        triplet_type : string, optional
-            Type of triplet loss, either simple or double.
-             - "simple" refer to the standard triplet loss,
-             - "double" refer to the triplet loss with a positive and a negative margin.
-             Both triplet losses are introduced in [2], respectively as triplet loss 1 and triplet loss 3.
-            The default is "simple".
-        triplet_margins : array of ints, optional
-            Margins for both triplet losses.
-            "simple" triplet loss uses one argument in the array, and "double" uses two, in the order [positive_margin, negative_margin].
-            The default is "[1]".
-        
-        References
-        ----------
-        [2] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
-        Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
-        In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
-
-        """
-
-        super().__init__(input_size_x, input_size_y, dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-        self.triplet_lambda = triplet_lambda
-        if triplet_type == "simple":
-            self.triplet_function = ae_utils.TripletLoss(margin = triplet_margins[0])
-        elif triplet_type == "double":
-            self.triplet_function = ae_utils.TripletLossDoubleMargin(pos_margin = triplet_margins[0], neg_margin = triplet_margins[1])
-        else:
-            raise err.InvalidArgumentValueException(f"Triplet loss type not understood: {triplet_type}")
-
-    def forward(self, anchor, positive, negative):
-        """
-        Forward pass: pass all examples based on the parent class (anchor, positive and negative).
-        """
-        x_hat_a, z_a = super().forward(anchor)
-        x_hat_p, z_p = super().forward(positive)
-        x_hat_n, z_n = super().forward(negative)
-        return x_hat_a, z_a, x_hat_p, z_p, x_hat_n, z_n
-    
-    def my_optim_method(self, n_epochs, data_loader, lr=1e-2, verbose = False, labels = None, early_stop_patience = 100, regenerate_data_loader = True, tensor_barwise = None, thresholds_data_loader = [0.1, 0.5]):
-        """
-        Default optimization method.
-        
-        This method is to be called in order to optimize the network.
-
-        Parameters
-        ----------
-        n_epochs, data_loader, lr, verbose, labels, early_stop_patience
-            See grand-parent Class (GenericAutoencoder)
-        regenerate_data_loader : boolean, optional
-            Boolean specifying whether the positive and negative examples needs to be recomputed at each epoch.
-            The default is True (i.e. regenrating positive and negative example at each epoch).
-            This is made to counter the small numbers of exceprts in our original formulation
-            (~100 examples per epoch, each of dimension ~10000, hence largely higher.)
-        tensor_barwise : None or numpy.array, optional
-            Only used if regenerate_data_loader is set to True.
-            Original tensor_barwise, on which is computed the optimization, to regenrate positive and negative examples. 
-            The default is None. Should not be set to None if regenerate_data_loader is set to True.
-        thresholds_data_loader : list of floats, each 0 \leq float \leq 1, optional
-            The thresholds for sampling positive and negative examples, based on the initial similarity between pairs of bars
-            (repsectively for positive and negative examples).
-            The default is [0.1, 0.5], 
-            i.e. positive examples are taken from the 10% most similar bars, and negative from the 50% least similar bars.
-
-        Returns
-        -------
-        See grand-parent Class (GenericAutoencoder)
-
-        """
-        self = self.to(self.device)
-        #print(f"Using {self.device}")
-        es = EarlyStopping(patience=early_stop_patience)
-        
-        nb_bars = 0
-        for iter_dl, _, _ in data_loader:
-            nb_bars += iter_dl.shape[0]
-
-        if self.beta == 2:
-            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
-        else:
-            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
-            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
-        losses = []
-            
-        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
-        
-        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
-        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
-        
-        if self.seed is not None:
-            self.apply(lambda layer: ae_utils.seeded_weights_init_kaiming(layer, seed=self.seed))
-        else:
-            self.apply(ae_utils.random_weights_init_kaiming) # Random initialization of the network
-
-        triplet_loss_function = torch.jit.script(self.triplet_function)
-
-        for epoch in range(1, n_epochs+1):
-            total_loss_epoch = 0.0
-            if regenerate_data_loader:
-                data_loader, _ = ae_utils.generate_triplet_dataloader(tensor_barwise, top_partition = thresholds_data_loader[0], medium_partition = thresholds_data_loader[1])
-            for anchor, positive, negative in data_loader:
-                anchor = torch.reshape(anchor, (anchor.shape[0],1, anchor.shape[1],anchor.shape[2]))
-                anchor = anchor.float().to(self.device)
-                positive = torch.reshape(positive, (positive.shape[0],1, positive.shape[1],positive.shape[2]))
-                positive = positive.float().to(self.device)
-                negative = torch.reshape(negative, (negative.shape[0],1, negative.shape[1],negative.shape[2]))
-                negative = negative.float().to(self.device)
-                
-                optimizer.zero_grad()
-                
-                x_hat_a, z_a, x_hat_p, z_p, x_hat_n, z_n = self.forward(anchor, positive, negative) # Forward
-        
-                # Recon losses
-                recons_loss_a = recons_loss(x_hat_a, anchor)
-                recons_loss_p = recons_loss(x_hat_p, positive)
-                recons_loss_n = recons_loss(x_hat_n, negative)
-                # Triplet loss
-                triplet_loss_val = triplet_loss_function(z_a, z_p, z_n)
-                # Mixed loss
-                loss = recons_loss_a + recons_loss_p + recons_loss_n + self.triplet_lambda * triplet_loss_val
-                loss.backward() # Backward
-                optimizer.step()
-                total_loss_epoch += loss.item() * anchor.size(0)
-            total_loss_epoch = total_loss_epoch/nb_bars
-            losses.append(total_loss_epoch)
-            scheduler.step(total_loss_epoch)
-            
-            if verbose:
-                total_loss_epoch = total_loss_epoch
-                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch,total_loss_epoch))
-                
-                if epoch%50 == 0:
-                    projection = self.get_latent_projection(data_loader)
-                    current_plot.plot_latent_space(projection, labels = labels)
-                    
-            if es.step(total_loss_epoch):
-                if verbose:
-                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
-                break 
-        return self, losses
-    
-    def get_latent_projection(self, data_loader):
-        """
-        Returns the latent representation on a given network, redefined for handling the triplets.
-        
-        Used after optimization to access to the latent representations.
-        """
-        all_data = []
-        for spec, _, _ in data_loader:
-            spec = spec.float().to(self.device)
-            spec = torch.reshape(spec, (spec.shape[0], 1, spec.shape[1], spec.shape[2]))
-            spec_recons, z = super().forward(spec)
-            for elt in z:
-                all_data.append(elt.cpu().detach().numpy())
-        return all_data
-
-
-####################################### Sparse networks, deprecated !!!
-class ConvolutionalAutoencoderSparse(ConvolutionalAutoencoder):
-    """
-    Class defining the Sparse Convolutional Neural Network (SAE) used to compress barwise representation of a song.
-    
-    This SAE is the same CNN than the previously defined (``ConvolutionalAutoencoder'') but adds a saprsity constraint on the latent representation.
-    The goal of this sparsity is to disentangle the different dimensions of the latent space.
-    """
-    def __init__(self, input_size_x, input_size_y, dim_latent_space, sparsity_lambda, norm_tensor, beta = 2):
-        """
-        Constructor of the network.
-
-        Parameters
-        ----------
-        input_size_x : int
-            The x-axis size of the input matrix.
-        input_size_y : int
-            The y-axis size of the input matrix.
-        dim_latent_space : int, optional
-            Dimension of the latent space. The default is 16.
-        sparsity_lambda : float
-            Ponderation parameter for the sparsity constraint (on z).
-        norm_tensor : float
-            Norm of the tensor on which to optimize, used as a normalization for the sparsity parameter.
-
-        Raises
-        ------
-        err.OutdatedBehaviorException.
-            Raised if ``nonnegative'' argument is set to True.
-
-        Returns
-        -------
-        None.
-
-        """
-        if nonnegative:
-            raise err.OutdatedBehaviorException("So-called ``nonnegative networks'' are not supported anymore, as they weren't succesful.") from None
-        
-        super().__init__(input_size_x, input_size_y, dim_latent_space, beta = beta)
-        self.sparsity_lambda_normed = sparsity_lambda #round(sparsity_lambda/norm_tensor, 8) ## Normalized sparsity parameter
-
-    def my_optim_method(self, n_epochs, data_loader, lr=1e-2, verbose = False, labels = None, early_stop_patience = 100):
-        """
-        Optimization method. Defined directly in the class, in order to be called from the object.
-
-        Parameters
-        ----------
-        n_epochs : int
-            Number of epochs to perform.
-        data_loader : torch.DataLoader
-            The DataLoader to optimize on.
-        lr : float, optional
-            Learning rate of the Network. The default is 1e-3.
-        early_stop_patience : int, optional
-            Patience for the number of consecutive epochs.
-            If the loss doesn't improve during early_stop_patience epochs, the optimization stops. The default is 100.
-        verbose : boolean, optional
-            Argument to print the evolution of the optimization.
-            Prints the current loss and plot a view of the autosimilarity of latent variables and a PCA of the latent space.
-            The default is False.
-        labels : None or array, optional
-            Only used if verbose is set to True.
-            If labels are set, they will be used to color the output of PCA projection.
-            If they are set to None, no label is used. The default is None.
-
-        Returns
-        -------
-        ConvolutionalAutoencoderSparse
-            Returns the Network.
-            Note: not mandatory (as the object needs to be instanciated to call this method), but returned as a good practice.
-
-        """
-        es = EarlyStopping(patience=early_stop_patience)
-        
-        recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
-        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
-        
-        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
-        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5) 
-        self.apply(ae_utils.seeded_weights_init_kaiming) # Seeded initialization of the network
-
-        for epoch in range(1, n_epochs+1):
-            total_loss_epoch = 0.0
-            for spec in data_loader:
-                spec = spec.float()
-        
-                optimizer.zero_grad()
-                x_hat, z = self.forward(spec) # Forward
-                recons_loss_spec = recons_loss(x_hat, spec) # Reconstruction loss
-                l1_regularization = torch.abs(z).mean() # L1 reg
-                loss = recons_loss_spec + self.sparsity_lambda_normed * l1_regularization # Mixed loss
-                loss.backward() # Backward
-                optimizer.step()
-                total_loss_epoch += loss.item()
-            scheduler.step(total_loss_epoch)
-            
-            if verbose:
-                total_loss_epoch = total_loss_epoch
-                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
-                if epoch%50 == 0:
-                    projection = self.get_latent_projection(data_loader)
-                    current_plot.plot_latent_space(projection, labels = labels)
-                    
-            if es.step(total_loss_epoch):
-                if verbose:
-                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
-                break 
-        return self    
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Apr 14 18:46:42 2021
+
+@author: amarmore
+
+Single-song autoencoding paradigm.
+
+See [1 - Chapter 5.4] or [2] for more information.
+
+References
+----------
+[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
+PhD Thesis Marmoret Axel 
+(not uploaded yet but will be soon!)
+(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
+
+[2] Marmoret, A., Cohen, J.E, and Bimbot, F., "Barwise Compression Schemes 
+for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, 
+SMC 2022, Sound and music Computing network, 2022.
+"""
+
+import as_seg.barwise_input as bi
+import barmuscomp.ae_utils as ae_utils
+from barmuscomp.model.early_stopping import EarlyStopping
+import barmuscomp.model.current_plot as current_plot
+import barmuscomp.model.errors as err
+
+import numpy as np
+import random
+import warnings
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+class GenericAutoencoder(nn.Module):
+    """
+    General autoencoder, acting as a parent class, specifying the functions shared between models.
+    
+    This autoencoder does not define an encoder or a decoder, they must be specified in children classes.
+    """
+    def __init__(self, dim_latent_space = 16, beta = 2, latent_nonlinearity = None, seed = None):
+        """
+        Constructor of the autoencoder.
+
+        Parameters
+        ----------
+        dim_latent_space : positive int, optional
+            Dimension of the latent space. 
+            The default is 16.
+        beta : float, optional
+            The beta value in the beta-divergence, 
+            specifying the loss function between the input and the output. 
+            The default is 2 (i.e. Euclidean Loss).
+            See [1,2] for details on the beta-divergence.
+        latent_nonlinearity : string, optional
+            A value specfiying the choice for a nonlinear activation function
+            constraining the values of the latent representation.
+            The default is None, meaning no nonlinear activation function.
+        seed : float, optional
+            A seed to fix pseudo-randomness.
+            The default is None, meaning no seed.
+
+        Raises
+        ------
+        InvalidArgumentValueException
+            Raised if the specified nonlinear activation function is unknown.
+        
+        References
+        ----------
+        [1] Basu, A., Harris, I.R., Hjort, L.N., and Jones, M.C., "Robust and Efficient
+        Estimation by Minimising a Density Power Divergence", in: Biometrika 85.3 (1998),
+        pp. 549–559, issn: 00063444.
+        
+        [2] Marmoret, A., Voorwinden, F., Leplat, V., Cohen, J.E., and Bimbot, F.,
+        "Nonnegative Tucker Decomposition with Beta-divergence for Music Structure 
+        Analysis of audio signals", in: GRETSI (2022).
+
+        """
+        super(GenericAutoencoder, self).__init__()
+        self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        
+        self.dim_latent_space = dim_latent_space
+        self.beta = beta
+        self.seed = seed
+        
+        if latent_nonlinearity is None:
+            self.latent_nonlinearity = None
+        elif latent_nonlinearity == "sigmoid":
+            self.latent_nonlinearity = nn.Sigmoid()
+        # elif latent_nonlinearity == "hardshrink":
+        #     self.latent_nonlinearity = nn.Hardshrink(lambd = 0.5)
+        elif latent_nonlinearity == "softmax":
+            self.latent_nonlinearity = nn.Softmax(dim=1)
+        elif latent_nonlinearity == "tanh":
+            self.latent_nonlinearity = nn.Tanh()
+        else:
+            raise err.InvalidArgumentValueException(f"Activation function not understood for the latent space: {latent_nonlinearity}") from None
+
+    def forward(self, x):
+        """
+        Forward pass.
+        x_hat is the reconstructed input, z is the latent projection.
+        """        
+        # Encoding
+        z = self.encoder(x)
+            
+        # Decoding
+        x_hat = self.decoder(z)
+
+        return x_hat, z
+    
+    def encoder(self, x):
+        """
+        Encoder default value, raising an error.
+        It must be implemented in chlidren classes.
+        """
+        raise NotImplementedError("To be redefined in children classes")
+    
+    def decoder(self, z):
+        """
+        Decoder default value, raising an error.
+        It must be implemented in chlidren classes.
+        """
+        raise NotImplementedError("To be redefined in children classes")
+    
+    def my_optim_method(self, n_epochs, data_loader, lr = 1e-3, early_stop_patience = 100, verbose = False, labels = None):
+        """
+        Default optimization method.
+        
+        This method is to be called in order to optimize the network.
+
+        Parameters
+        ----------
+        n_epochs : int
+            Number of epochs to perform.
+        data_loader : torch.DataLoader
+            The DataLoader to optimize on.
+        lr : float, optional
+            Learning rate of the Network. 
+            The default is 1e-3.
+        early_stop_patience : int, optional
+            Patience for the number of consecutive epochs.
+            If the loss doesn't decrease during early_stop_patience epochs, the optimization stops. 
+            The default is 100.
+        verbose : boolean, optional
+            Argument to print the evolution of the optimization.
+            Prints the current loss and plots a view of the autosimilarity of 
+            latent variables and a PCA of the latent space.
+            The default is False.
+        labels : None or array, optional
+            Only used if verbose is set to True.
+            If labels are set, they will be used to color the output of PCA projection.
+            If they are set to None, no label is used. The default is None.
+
+        Returns
+        -------
+        GenericAutoencoder
+            The instance of the network, optimized.
+            NB: it is not required to return the network, this is rather implemented 
+            in order to avoid some "unintenional" optimization 
+            (as it forces a human user to notice that something is returned,
+             and hence that some code was run).
+        losses : list of positive floats
+            The loss values at each iteration.
+
+        """
+        self = self.to(self.device)
+        #print(f"Using {self.device}")
+        es = EarlyStopping(patience=early_stop_patience)
+        
+        nb_bars = 0
+        for iter_dl in data_loader:
+            nb_bars += iter_dl.shape[0]
+
+        if self.beta == 2:
+            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
+        else:
+            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
+            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
+        losses = []
+            
+        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
+        
+        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
+        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
+        
+        if self.seed is not None:
+            self.apply(lambda layer: ae_utils.seeded_weights_init_kaiming(layer, seed=self.seed))
+        else:
+            self.apply(ae_utils.random_weights_init_kaiming) # Random initialization of the network
+            
+        for epoch in range(1, n_epochs+1):
+            total_loss_epoch = 0.0
+            for spec in data_loader:
+                spec = spec.float().to(self.device)
+                optimizer.zero_grad()
+                spec_recons, z = self.forward(spec) # Forward pass
+                loss = recons_loss(spec_recons, spec) # Loss
+                loss.backward() # Backward pass
+                optimizer.step() # Optimizes the net with grads
+                
+                total_loss_epoch += loss.item() * spec.size(0)
+            total_loss_epoch = total_loss_epoch/nb_bars
+            losses.append(total_loss_epoch)
+            scheduler.step(total_loss_epoch) # scheduler for the decrease of lr on a plateau
+                
+            if verbose:
+                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
+                if epoch%50 == 0:
+                    projection = self.get_latent_projection(data_loader)
+                    current_plot.plot_latent_space(projection, labels = labels)
+                    
+            if es.step(total_loss_epoch): # Checks if loss has decreased, to stop the optimization if performances don't increase for early_stop_patience epochs.
+                if verbose:
+                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
+                break 
+        return self, losses
+    
+    def get_latent_projection(self, data_loader):
+        """
+        Returns the latent representation on a given network.
+        
+        Used after optimization to access to the latent representations.
+        
+        Parameters
+        ----------
+        data_loader : torch.DataLoader
+            The DataLoader to project (intended to be the same that the one used for optimization).
+
+        Returns
+        -------
+        all_data : numpy array
+            The latent representation for each data in the dataset.
+
+        """
+        all_data = []
+        for spec in data_loader:
+            spec = spec.float().to(self.device)
+            spec_recons, z = self.forward(spec)
+            for elt in z:
+                all_data.append(elt.cpu().detach().numpy())
+        return all_data
+       
+# %% Fully-connected
+def get_fc_ssae_projection(spectrogram, compression_dimension, bars, 
+                           n_epochs = 1000, lr = 1e-3, beta = 2, latent_nonlinearity = None, seed = None, 
+                           subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
+    """
+    Return the projection of the barwise content with a Fully-Connected AutoEncoder (SSAE).
+
+    Parameters
+    ----------
+    spectrogram : numpy array
+        The spectrogram to analyze, barwise.
+    compression_dimension : positive integer
+        Dimension of compression (size of the latent space).
+    bars : list of tuples
+        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
+    n_epochs : int
+        Number of epochs to perform.
+    lr : float, optional
+        Learning rate of the Network. 
+        The default is 1e-3.
+    beta, latent_nonlinearity, seed:
+        See GenericAutoencoder.
+    subdivision_bars : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    hop_length : integer, optional
+        The hop_length used for the computation of the spectrogram.
+        It is expressed in terms of number of samples, which are defined by the sampling rate.
+        The default is 32.
+    sampling_rate : float, optional
+        Sampling rate used when computing the spectrogram (typically 44100Hz).
+        The default is 44100.
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix (latent representations), of size (bars, compression_dimension).
+        
+    """
+    ae_model = FullyConnectedAutoencoder(input_size_x = subdivision_bars, input_size_y = spectrogram.shape[0], dim_latent_space = compression_dimension, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+    tensor_barwise_BFT = bi.tensorize_barwise_BFT(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
+    data_loader = ae_utils.generate_flatten_dataloader(tensor_barwise_BFT)
+    ae_model, losses = ae_model.my_optim_method(n_epochs=n_epochs, data_loader=data_loader, lr=lr, verbose = False, labels = None)
+    return ae_model.get_latent_projection(data_loader)
+
+class FullyConnectedAutoencoder(GenericAutoencoder):
+    """
+    AutoEncoder with fully-connected layers as encoder and decoder.
+    """
+    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None):#, batch_norm = True):
+        """
+        Constructor of the Fully-connected autoencoder.
+
+        Parameters
+        ----------
+        input_size_x : integer
+            Size of the x axis dimension of the input.
+        input_size_y : integer
+            Size of the y axis dimension of the input.
+        dim_latent_space, beta, latent_nonlinearity, seed:
+            See GenericAutoencoder.
+
+        """
+        super().__init__(dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+        self.fc = nn.Linear(in_features=input_size_x * input_size_y, out_features=128)
+        self.fc_2 = nn.Linear(in_features=128, out_features=dim_latent_space)
+        self.i_fc = nn.Linear(in_features=dim_latent_space, out_features=128)
+        self.i_fc_2 = nn.Linear(in_features=128, out_features=input_size_x * input_size_y)
+        
+        # self.batch_norm = batch_norm # DEPRECATED: it should always be designed with batch norm layers.
+        # if self.batch_norm:
+        self.bn_1 = nn.BatchNorm1d(128)
+        self.bn_2 = nn.BatchNorm1d(dim_latent_space)
+        self.i_bn_1 = nn.BatchNorm1d(128)
+       
+    def encoder(self, x):    
+        """
+        Encoder of the Fully-Connected network.
+        Two dense layers, each followed by a batch normalization layer.
+        The last layer (the 2nd one) may contain a nonnlinear activation function.
+        In that case, the activation function replace the batch normalization layer.
+        """
+        x = F.relu(self.fc(x))
+        x = self.bn_1(x)
+        x = self.fc_2(x)
+        if self.latent_nonlinearity is None:
+            return self.bn_2(x)
+        else:
+            return self.latent_nonlinearity(x)
+
+        
+    # def encoder(self, x):
+    #     """
+    #     Encoder definition.
+    #     Switch between an encoder with and without batch normalization layer.
+    #     """
+    #     if self.batch_norm:
+    #         z = self.bn_encoder(x)
+    #     else:
+    #         z = self.no_bn_encoder(x)
+
+    #     if self.latent_nonlinearity is not None:
+    #         z = self.latent_nonlinearity(z)
+    #     return z
+    
+    # def no_bn_encoder(self, x):
+    #     """
+    #     Encoder without batch normlization layers.
+    #     """
+    #     x = F.relu(self.fc(x))
+    #     return self.fc_2(x)
+        
+
+    def decoder(self, z):
+        """
+        Decoder of the Fully-Connected network.
+        Two dense layers. The first one is followed by a batch normalization layer.
+        """
+        x = F.relu(self.i_fc(z))
+        x = self.i_bn_1(x)
+        x_hat = self.i_fc_2(x)
+        
+        # To compute the beta-divergence, needing nonnegative outputs
+        x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
+        # TODO: Experiences should account for this bias, i.e. be redone.
+        return x_hat
+    
+    # def decoder(self, z):
+    #     """
+    #     Decoder definition.
+    #     Switch between a decoder with and without batch normalization layer.
+    #     """
+    #     if self.batch_norm:
+    #         return self.bn_decoder(z)
+    #     else:
+    #         return self.no_bn_decoder(z)
+        
+    
+    # def no_bn_decoder(self, z):
+    #     """
+    #     Decoder without batch normlization layers.
+    #     """
+    #     x = F.relu(self.i_fc(z))
+    #     x_hat = self.i_fc_2(x)
+        
+    #     # To compute the beta-divergence, needing nonnegative outputs
+    #     x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
+    #     return x_hat
+    
+# %% Convolutional
+def get_conv_ssae_projection(spectrogram, compression_dimension, bars, 
+                             n_epochs = 1000, lr = 1e-3, beta = 2, latent_nonlinearity = None, seed = None, 
+                             subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
+    """
+    Return the projection of the barwise content with a convolutional AutoEncoder (SSAE).
+
+    Parameters
+    ----------
+    spectrogram : list of list of floats or numpy array
+        The spectrogram to analyze, barwise.
+    compression_dimension : positive integer
+        Dimension of compression (size of the latent space).
+    bars : list of tuples
+        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
+    n_epochs : int
+        Number of epochs to perform.
+    lr : float, optional
+        Learning rate of the Network. 
+        The default is 1e-3.
+    beta, latent_nonlinearity, seed:
+        See GenericAutoencoder.
+    subdivision_bars : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    hop_length : integer, optional
+        The hop_length used for the computation of the spectrogram.
+        It is expressed in terms of number of samples, which are defined by the sampling rate.
+        The default is 32.
+    sampling_rate : float, optional
+        Sampling rate used when computing the spectrogram (typically 44100Hz).
+        The default is 44100.
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix (latent representations), of size (bars, compression_dimension).
+        
+    """
+    ae_model = ConvolutionalAutoencoder(input_size_x = subdivision_bars, input_size_y = spectrogram.shape[0], dim_latent_space = compression_dimension, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+    tensor_barwise_BFT = bi.tensorize_barwise_BFT(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
+    data_loader = ae_utils.generate_dataloader(tensor_barwise_BFT)
+    ae_model, losses = ae_model.my_optim_method(n_epochs=n_epochs, data_loader=data_loader, lr=lr, verbose = False, labels = None)
+    return ae_model.get_latent_projection(data_loader)
+
+class ConvolutionalAutoencoder(GenericAutoencoder):
+    """
+    Autoencoder with Convolutional layers as encoder and decoder.
+    """
+    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None):
+        """
+        Constructor of the Convolutional autoencoder.
+
+        Parameters
+        ----------
+        input_size_x : integer
+            Size of the x axis dimension of the input.
+        input_size_y : integer
+            Size of the y axis dimension of the input.
+        dim_latent_space, beta, latent_nonlinearity, seed:
+            See GenericAutoencoder.
+            
+        """
+        super().__init__(dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+        self.input_size_pool_y = int(input_size_y/4) # input_size / pool ## NOTE: Doesn't work for odd input sizes (in reconstruction), so TODO.
+        self.input_size_pool_x = int(input_size_x/4) # input_size / pool
+        
+        # Encoder
+        ## Convolutional layers
+        self.conv1 = nn.Conv2d(1, 4, 3, padding=1)  
+        self.conv2 = nn.Conv2d(4,16, 3, padding=1)
+        self.pool = nn.MaxPool2d(2, 2)
+        self.flatten = nn.Flatten()
+
+        ## Fully-connected controling latent space size.
+        in_features = 16 * self.input_size_pool_x * self.input_size_pool_y # nb_kernels_last_conv * (input_size / pool)
+        self.fc = nn.Linear(in_features=in_features, out_features=dim_latent_space)
+        
+        # Decoder
+        ## Inverse of previous FC
+        self.i_fc = nn.Linear(in_features=dim_latent_space, out_features=in_features)
+
+        # Transposed conv layers
+        self.t_conv1 = nn.ConvTranspose2d(16, 4, 3, stride=2, padding=1, output_padding=1)
+        self.t_conv2 = nn.ConvTranspose2d(4, 1, 3, stride=2, padding=1, output_padding=1)
+        
+        self.bn_1 = nn.BatchNorm2d(4)
+        self.bn_2 = nn.BatchNorm2d(16)
+        self.bn_fc = nn.BatchNorm1d(dim_latent_space)
+        
+        self.i_bn_fc = nn.BatchNorm1d(16 * self.input_size_pool_y * self.input_size_pool_x)
+        self.i_bn_1 = nn.BatchNorm2d(4)
+       
+           
+    def encoder(self, x):
+        """
+        Encoder of the Covolutional Autoencoder.
+        It is implemented with two convolutional layers, 
+        each followed by a ReLU, a pooling layer, and a batch normalization layer.
+        After these convolutional blocks, a fully-connected layer is implemented,
+        leading to the latent representations.
+        A batch normalization layer is implemented after the dense layer,
+        but it can be replaced by a nonlinear activation function if specified.
+        """
+        x = F.relu(self.conv1(x))
+        x = self.pool(x)
+        x = self.bn_1(x)
+        x = F.relu(self.conv2(x))
+        x = self.pool(x)
+        x = self.bn_2(x)
+        
+        x = self.flatten(x)
+        x = self.fc(x)
+        if self.latent_nonlinearity is None:
+            return self.bn_fc(x)
+        else:
+            return self.latent_nonlinearity(x)
+        
+    def decoder(self, z):
+        """
+        Decoder of the Convolutioanl autoencoder.
+        It is implemented as the inverse of the encoder, with a dense layer
+        followed by two transposed convolution layers.
+        The two first layers implement a batch normalization layer, but not the last one
+        (i.e. no batch normalization before the reconstruction).
+        """
+        x = self.i_fc(z)
+        x = self.i_bn_fc(x)
+        x = x.view((x.shape[0], 16, self.input_size_pool_y, self.input_size_pool_x))
+        x = F.relu(self.t_conv1(x))
+        x = self.i_bn_1(x)
+        x_hat = self.t_conv2(x)
+        
+        # To compute the beta-divergence, needing nonnegative outputs
+        x_hat = F.relu(x_hat) # !!! Introduces a hugh bias when the feature is negative ! (Log MEl, MFCC)
+        # TODO: Experiences should account for this bias, i.e. make new experiments.
+        return x_hat
+
+    
+class ConvolutionalAutoencoderTriplet(ConvolutionalAutoencoder):
+    """
+    Class defining AutoEncoders used to compress barwise representation of a song, with an added Triplet loss to regularize the latent space.
+    This triplet loss is designed to favor the bars which are very similar in the initial representation, 
+    and to scatter bars which are very dissimilar.
+    The positive (similar) and negative (dissimilar) examples are chosen by thresholding the autosimilarity matrix,
+    and taking either the most or least similar examples (hence, two thresolds parameters are to be defined, see my_optim_method()).
+    
+    For more information, refer to [1 - Chapter 5.4.5]
+    
+    References
+    ----------
+    [1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
+    PhD Thesis Marmoret Axel 
+    (not uploaded yet but will be soon!)
+    (You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
+    """
+    def __init__(self, input_size_x, input_size_y, dim_latent_space, beta = 2, latent_nonlinearity = None, seed = None, triplet_lambda = 1, triplet_type = "simple", triplet_margins = [1]):
+        """
+        Constructor of the triplet-loss regularized convolutional autoencoder.
+        
+        input_size_x, input_size_y, dim_latent_space, beta, latent_nonlinearity, seed,
+            See parent class (ConvolutionalAutoencoder)
+        triplet_lambda : float, optional
+            Ponderation for the triplet loss in the mixed loss. The default is 1.
+        triplet_type : string, optional
+            Type of triplet loss, either simple or double.
+             - "simple" refer to the standard triplet loss,
+             - "double" refer to the triplet loss with a positive and a negative margin.
+             Both triplet losses are introduced in [2], respectively as triplet loss 1 and triplet loss 3.
+            The default is "simple".
+        triplet_margins : array of ints, optional
+            Margins for both triplet losses.
+            "simple" triplet loss uses one argument in the array, and "double" uses two, in the order [positive_margin, negative_margin].
+            The default is "[1]".
+        
+        References
+        ----------
+        [2] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
+        Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
+        In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
+
+        """
+
+        super().__init__(input_size_x, input_size_y, dim_latent_space, beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+        self.triplet_lambda = triplet_lambda
+        if triplet_type == "simple":
+            self.triplet_function = ae_utils.TripletLoss(margin = triplet_margins[0])
+        elif triplet_type == "double":
+            self.triplet_function = ae_utils.TripletLossDoubleMargin(pos_margin = triplet_margins[0], neg_margin = triplet_margins[1])
+        else:
+            raise err.InvalidArgumentValueException(f"Triplet loss type not understood: {triplet_type}")
+
+    def forward(self, anchor, positive, negative):
+        """
+        Forward pass: pass all examples based on the parent class (anchor, positive and negative).
+        """
+        x_hat_a, z_a = super().forward(anchor)
+        x_hat_p, z_p = super().forward(positive)
+        x_hat_n, z_n = super().forward(negative)
+        return x_hat_a, z_a, x_hat_p, z_p, x_hat_n, z_n
+    
+    def my_optim_method(self, n_epochs, data_loader, lr=1e-2, verbose = False, labels = None, early_stop_patience = 100, regenerate_data_loader = True, tensor_barwise = None, thresholds_data_loader = [0.1, 0.5]):
+        """
+        Default optimization method.
+        
+        This method is to be called in order to optimize the network.
+
+        Parameters
+        ----------
+        n_epochs, data_loader, lr, verbose, labels, early_stop_patience
+            See grand-parent Class (GenericAutoencoder)
+        regenerate_data_loader : boolean, optional
+            Boolean specifying whether the positive and negative examples needs to be recomputed at each epoch.
+            The default is True (i.e. regenrating positive and negative example at each epoch).
+            This is made to counter the small numbers of exceprts in our original formulation
+            (~100 examples per epoch, each of dimension ~10000, hence largely higher.)
+        tensor_barwise : None or numpy.array, optional
+            Only used if regenerate_data_loader is set to True.
+            Original tensor_barwise, on which is computed the optimization, to regenrate positive and negative examples. 
+            The default is None. Should not be set to None if regenerate_data_loader is set to True.
+        thresholds_data_loader : list of floats, each 0 \leq float \leq 1, optional
+            The thresholds for sampling positive and negative examples, based on the initial similarity between pairs of bars
+            (repsectively for positive and negative examples).
+            The default is [0.1, 0.5], 
+            i.e. positive examples are taken from the 10% most similar bars, and negative from the 50% least similar bars.
+
+        Returns
+        -------
+        See grand-parent Class (GenericAutoencoder)
+
+        """
+        self = self.to(self.device)
+        #print(f"Using {self.device}")
+        es = EarlyStopping(patience=early_stop_patience)
+        
+        nb_bars = 0
+        for iter_dl, _, _ in data_loader:
+            nb_bars += iter_dl.shape[0]
+
+        if self.beta == 2:
+            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
+        else:
+            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
+            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
+        losses = []
+            
+        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
+        
+        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
+        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
+        
+        if self.seed is not None:
+            self.apply(lambda layer: ae_utils.seeded_weights_init_kaiming(layer, seed=self.seed))
+        else:
+            self.apply(ae_utils.random_weights_init_kaiming) # Random initialization of the network
+
+        triplet_loss_function = torch.jit.script(self.triplet_function)
+
+        for epoch in range(1, n_epochs+1):
+            total_loss_epoch = 0.0
+            if regenerate_data_loader:
+                data_loader, _ = ae_utils.generate_triplet_dataloader(tensor_barwise, top_partition = thresholds_data_loader[0], medium_partition = thresholds_data_loader[1])
+            for anchor, positive, negative in data_loader:
+                anchor = torch.reshape(anchor, (anchor.shape[0],1, anchor.shape[1],anchor.shape[2]))
+                anchor = anchor.float().to(self.device)
+                positive = torch.reshape(positive, (positive.shape[0],1, positive.shape[1],positive.shape[2]))
+                positive = positive.float().to(self.device)
+                negative = torch.reshape(negative, (negative.shape[0],1, negative.shape[1],negative.shape[2]))
+                negative = negative.float().to(self.device)
+                
+                optimizer.zero_grad()
+                
+                x_hat_a, z_a, x_hat_p, z_p, x_hat_n, z_n = self.forward(anchor, positive, negative) # Forward
+        
+                # Recon losses
+                recons_loss_a = recons_loss(x_hat_a, anchor)
+                recons_loss_p = recons_loss(x_hat_p, positive)
+                recons_loss_n = recons_loss(x_hat_n, negative)
+                # Triplet loss
+                triplet_loss_val = triplet_loss_function(z_a, z_p, z_n)
+                # Mixed loss
+                loss = recons_loss_a + recons_loss_p + recons_loss_n + self.triplet_lambda * triplet_loss_val
+                loss.backward() # Backward
+                optimizer.step()
+                total_loss_epoch += loss.item() * anchor.size(0)
+            total_loss_epoch = total_loss_epoch/nb_bars
+            losses.append(total_loss_epoch)
+            scheduler.step(total_loss_epoch)
+            
+            if verbose:
+                total_loss_epoch = total_loss_epoch
+                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch,total_loss_epoch))
+                
+                if epoch%50 == 0:
+                    projection = self.get_latent_projection(data_loader)
+                    current_plot.plot_latent_space(projection, labels = labels)
+                    
+            if es.step(total_loss_epoch):
+                if verbose:
+                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
+                break 
+        return self, losses
+    
+    def get_latent_projection(self, data_loader):
+        """
+        Returns the latent representation on a given network, redefined for handling the triplets.
+        
+        Used after optimization to access to the latent representations.
+        """
+        all_data = []
+        for spec, _, _ in data_loader:
+            spec = spec.float().to(self.device)
+            spec = torch.reshape(spec, (spec.shape[0], 1, spec.shape[1], spec.shape[2]))
+            spec_recons, z = super().forward(spec)
+            for elt in z:
+                all_data.append(elt.cpu().detach().numpy())
+        return all_data
+
+
+####################################### Sparse networks, deprecated !!!
+class ConvolutionalAutoencoderSparse(ConvolutionalAutoencoder):
+    """
+    Class defining the Sparse Convolutional Neural Network (SAE) used to compress barwise representation of a song.
+    
+    This SAE is the same CNN than the previously defined (``ConvolutionalAutoencoder'') but adds a saprsity constraint on the latent representation.
+    The goal of this sparsity is to disentangle the different dimensions of the latent space.
+    """
+    def __init__(self, input_size_x, input_size_y, dim_latent_space, sparsity_lambda, norm_tensor, beta = 2):
+        """
+        Constructor of the network.
+
+        Parameters
+        ----------
+        input_size_x : int
+            The x-axis size of the input matrix.
+        input_size_y : int
+            The y-axis size of the input matrix.
+        dim_latent_space : int, optional
+            Dimension of the latent space. The default is 16.
+        sparsity_lambda : float
+            Ponderation parameter for the sparsity constraint (on z).
+        norm_tensor : float
+            Norm of the tensor on which to optimize, used as a normalization for the sparsity parameter.
+
+        Raises
+        ------
+        err.OutdatedBehaviorException.
+            Raised if ``nonnegative'' argument is set to True.
+
+        Returns
+        -------
+        None.
+
+        """
+        if nonnegative:
+            raise err.OutdatedBehaviorException("So-called ``nonnegative networks'' are not supported anymore, as they weren't succesful.") from None
+        
+        super().__init__(input_size_x, input_size_y, dim_latent_space, beta = beta)
+        self.sparsity_lambda_normed = sparsity_lambda #round(sparsity_lambda/norm_tensor, 8) ## Normalized sparsity parameter
+
+    def my_optim_method(self, n_epochs, data_loader, lr=1e-2, verbose = False, labels = None, early_stop_patience = 100):
+        """
+        Optimization method. Defined directly in the class, in order to be called from the object.
+
+        Parameters
+        ----------
+        n_epochs : int
+            Number of epochs to perform.
+        data_loader : torch.DataLoader
+            The DataLoader to optimize on.
+        lr : float, optional
+            Learning rate of the Network. The default is 1e-3.
+        early_stop_patience : int, optional
+            Patience for the number of consecutive epochs.
+            If the loss doesn't improve during early_stop_patience epochs, the optimization stops. The default is 100.
+        verbose : boolean, optional
+            Argument to print the evolution of the optimization.
+            Prints the current loss and plot a view of the autosimilarity of latent variables and a PCA of the latent space.
+            The default is False.
+        labels : None or array, optional
+            Only used if verbose is set to True.
+            If labels are set, they will be used to color the output of PCA projection.
+            If they are set to None, no label is used. The default is None.
+
+        Returns
+        -------
+        ConvolutionalAutoencoderSparse
+            Returns the Network.
+            Note: not mandatory (as the object needs to be instanciated to call this method), but returned as a good practice.
+
+        """
+        es = EarlyStopping(patience=early_stop_patience)
+        
+        recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
+        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
+        
+        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
+        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5) 
+        self.apply(ae_utils.seeded_weights_init_kaiming) # Seeded initialization of the network
+
+        for epoch in range(1, n_epochs+1):
+            total_loss_epoch = 0.0
+            for spec in data_loader:
+                spec = spec.float()
+        
+                optimizer.zero_grad()
+                x_hat, z = self.forward(spec) # Forward
+                recons_loss_spec = recons_loss(x_hat, spec) # Reconstruction loss
+                l1_regularization = torch.abs(z).mean() # L1 reg
+                loss = recons_loss_spec + self.sparsity_lambda_normed * l1_regularization # Mixed loss
+                loss.backward() # Backward
+                optimizer.step()
+                total_loss_epoch += loss.item()
+            scheduler.step(total_loss_epoch)
+            
+            if verbose:
+                total_loss_epoch = total_loss_epoch
+                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
+                if epoch%50 == 0:
+                    projection = self.get_latent_projection(data_loader)
+                    current_plot.plot_latent_space(projection, labels = labels)
+                    
+            if es.step(total_loss_epoch):
+                if verbose:
+                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
+                break 
+        return self
```

### Comparing `barmuscomp-0.1.2/barmuscomp/ae_ntd.py` & `barmuscomp-0.1.3/barmuscomp/ae_ntd.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,449 +1,449 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 14 18:46:42 2021
-
-@author: amarmore
-
-Mixing the Nonnegative Tucker Decomposition (NTD) with Autoencoders (Single-Song AutoEncoders).
-
-In short, the idea is to implement an NTD structure in the decoder. See [1 - Chapter 6] for details.
-
-References
-----------
-[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
-PhD Thesis Marmoret Axel 
-(not uploaded yet but will be soon!)
-(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
-"""
-
-import barmuscomp.ae_utils as ae_utils
-from barmuscomp.model.early_stopping import EarlyStopping
-import barmuscomp.model.current_plot as current_plot
-import barmuscomp.model.errors as err
-
-import numpy as np
-import random
-import warnings
-import tensorly as tl
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-class GenericAutoencoderNTD(nn.Module):
-    """
-    Generic Autoencoder, with NTD decoder.
-    
-    Hence, the decoder is structured with matrices W, H and the core tensor G.
-    """
-    def __init__(self,  input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
-        """
-        Constructor of the AE-NTD.
-
-        Parameters
-        ----------
-        input_size_x : positive int
-            Dimension of the x axis (time at barscale). 
-        input_size_y : positive int
-            Dimension of the y axis (frequency scale). .
-        ntd_dimensions : list of integers.
-            Dimensions of the factors for NTD 
-            (i.e. number of columns of each matrix factor, 
-             or , equivalently, dimensions of the core tensor).
-        unfolded_G : numpy array
-            Initialization for the core tensor G.
-            The tensor must be unfolded on the barwise mode.
-        W : numpy array
-            Initialization for the factor matrix W (frequency mode).
-        H : numpy array
-            Initialization for the factor matrix H (rhythmic factors).
-        bn_latent_init_stds : list of float, optional
-            Initialization of the batch normalization layer on the latent space,
-            here, the standard deviation.
-            If set, they must be computed as the std of the dimensions of the Q matrix.
-            The default is None.
-        bn_latent_init_avgs :list of float, optional
-            Initialization of the batch normalization layer on the latent space,
-            here, the averages.
-            If set, they must be computed as the averages of the dimensions of the Q matrix.
-            The default is None.
-        beta : float, optional
-            The beta value in the beta-divergence, 
-            specifying the loss function between the input and the output. 
-            The default is 2 (i.e. Euclidean Loss).
-        latent_nonlinearity : string, optional
-            A value specfiying the choice for a nonlinear activation function
-            constraining the values of the latent representation.
-            The default is None, meaning no nonlinear activation function.
-        seed : float, optional
-            A seed to fix pseudo-randomness.
-            The default is None, meaning no seed.
-
-        Raises
-        ------
-        InvalidArgumentValueException
-            Raised if arguments are not accurately set.
-
-        """
-        if W is None and input_size_y == None:
-            raise err.InvalidArgumentValueException("You must specify either W or its size. Here, both args 'W' and 'input_size_y' are set to None.")
-        if H is None and input_size_x == None:
-            raise err.InvalidArgumentValueException("You must specify either H or its size. Here, both args 'H' and 'input_size_x' are set to None.")
-        super(GenericAutoencoderNTD, self).__init__()
-        self.device = "cuda" if torch.cuda.is_available() else "cpu"
-        
-        self.input_size_x = input_size_x
-        self.input_size_y = input_size_y
-        
-        self.beta = beta
-        self.ntd_dimensions = ntd_dimensions
-        
-        if seed is not None:
-            torch.manual_seed(seed)
-        
-        if W is None:
-            self.W_torch = nn.Parameter(torch.empty(input_size_y, ntd_dimensions[0]), requires_grad = True)
-            nn.init.kaiming_uniform_(self.W_torch, mode='fan_out', nonlinearity='relu')
-        else:
-            self.W_torch = nn.Parameter(torch.tensor(W).float().contiguous(), requires_grad = True)
-
-        if H is None:
-            self.H_torch = nn.Parameter(torch.empty(input_size_x, ntd_dimensions[1]), requires_grad = True)
-            nn.init.kaiming_uniform_(self.H_torch, mode='fan_out', nonlinearity='relu')
-        else:
-            self.H_torch = nn.Parameter(torch.tensor(H).float().contiguous(), requires_grad = True)
-
-        if unfolded_G is None:
-            self.unfolded_G_torch = nn.Parameter(torch.empty(ntd_dimensions[2], ntd_dimensions[0]*ntd_dimensions[1]), requires_grad = True)        
-            nn.init.kaiming_uniform_(self.unfolded_G_torch, mode='fan_out', nonlinearity='relu')
-        else:
-            self.unfolded_G_torch = nn.Parameter(torch.tensor(unfolded_G).float().contiguous(), requires_grad = True)
-            
-        if latent_nonlinearity is None:
-            self.latent_nonlinearity = None
-
-            self.bn_latent = nn.BatchNorm1d(ntd_dimensions[2])
-            if bn_latent_init_stds != None:
-                self.bn_latent.weight.data = torch.tensor(bn_latent_init_stds).float() if not torch.is_tensor(bn_latent_init_stds) else bn_latent_init_stds.clone().detach()
-            if bn_latent_init_avgs != None:
-                self.bn_latent.bias.data = torch.tensor(bn_latent_init_avgs).float() if not torch.is_tensor(bn_latent_init_avgs) else bn_latent_init_avgs.clone().detach()
-
-        elif latent_nonlinearity == "sigmoid":
-            self.latent_nonlinearity = nn.Sigmoid()
-        # elif latent_nonlinearity == "hardshrink":
-        #     self.latent_nonlinearity = nn.Hardshrink(lambd = 0.5)
-        elif latent_nonlinearity == "softmax":
-            self.latent_nonlinearity = nn.Softmax(dim=1)
-        elif latent_nonlinearity == "tanh":
-            self.latent_nonlinearity = nn.Tanh()
-        else:
-            raise err.InvalidArgumentValueException(f"Activation function not understood for the latent space: {latent_nonlinearity}") from None
-
-    def forward(self, x):
-        """
-        Forward pass.
-        x_hat is the reconstructed input, z is the latent projection.
-        """        
-        # Encoding
-        z = self.encoder(x)
-            
-        # Decoding
-        x_hat = self.decoder(z)
-
-        return x_hat, z
-    
-    def encoder(self, x):
-        """
-        Generic encoder, not defined in the parent class, must be redefined in children classes.
-        """
-        raise NotImplementedError("To be redefined in children classes")
-    
-    def decoder(self, z):
-        """
-        NTD based decoder.
-        
-        It consists of two fully-connected layers, with two relu functions:
-            - The first with the structure of the core tensor G,
-            - The second with the structure of the Kronecker product between W and H.
-        Hence, the decoder fully mimics an NTD, and these matrices may be initialized from the results of an NTD.
-        """
-        x = F.relu(torch.matmul(z, self.unfolded_G_torch))
-        
-        w_kron_h = torch.kron(self.W_torch.T, self.H_torch.T)
-        mat_mul = torch.matmul(x, w_kron_h)
-        x_hat = F.relu(mat_mul)
-        
-        return x_hat
-    
-    def my_optim_method(self, n_epochs, data_loader, lr = 1e-3, early_stop_patience = 100, verbose = False, labels = None):
-        """
-        Default optimization method.
-        
-        This method is to be called in order to optimize the network.
-
-        Parameters
-        ----------
-        n_epochs : int
-            Number of epochs to perform.
-        data_loader : torch.DataLoader
-            The DataLoader to optimize on.
-        lr : float, optional
-            Learning rate of the Network. 
-            The default is 1e-3.
-        early_stop_patience : int, optional
-            Patience for the number of consecutive epochs.
-            If the loss doesn't decrease during early_stop_patience epochs, the optimization stops. 
-            The default is 100.
-        verbose : boolean, optional
-            Argument to print the evolution of the optimization.
-            Prints the current loss and plots a view of the autosimilarity of 
-            latent variables and a PCA of the latent space.
-            The default is False.
-        labels : None or array, optional
-            Only used if verbose is set to True.
-            If labels are set, they will be used to color the output of PCA projection.
-            If they are set to None, no label is used. The default is None.
-
-        Returns
-        -------
-        GenericAutoencoder
-            The instance of the network, optimized.
-            NB: it is not required to return the network, this is rather implemented 
-            in order to avoid some "unintenional" optimization 
-            (as it forces a human user to notice that something is returned,
-             and hence that some code was run).
-        losses : list of positive floats
-            The loss values at each iteration.
-
-        """
-        self = self.to(self.device)
-        #print(f"Using {self.device}")
-        es = EarlyStopping(patience=early_stop_patience)
-        
-        nb_bars = 0
-        for iter_dl in data_loader:
-            nb_bars += iter_dl.shape[0]
-
-        if self.beta == 2:
-            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
-        else:
-            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
-            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
-        losses = []
-            
-        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
-        
-        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
-        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
-            
-        for epoch in range(1, n_epochs+1):
-            total_loss_epoch = 0.0
-            for spec in data_loader:
-                spec = spec.float().to(self.device)
-                optimizer.zero_grad()
-                spec_recons, z = self.forward(spec) # Forward pass
-                loss = recons_loss(spec_recons, spec) # Loss
-                loss.backward() # Backward pass
-                optimizer.step() # Optimizes the net with grads
-                
-                total_loss_epoch += loss.item() * spec.size(0)
-            total_loss_epoch = total_loss_epoch/nb_bars
-            losses.append(total_loss_epoch)
-            scheduler.step(total_loss_epoch) # scheduler for the decrease of lr on a plateau
-                
-            if verbose:
-                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
-                if epoch%50 == 0:
-                    projection = self.get_latent_projection(data_loader)
-                    current_plot.plot_latent_space(projection, labels = labels)
-                    
-            if es.step(total_loss_epoch): # Checks if loss has decreased, to stop the optimization if performances don't increase for early_stop_patience epochs.
-                if verbose:
-                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
-                break 
-        return self, losses
-    
-    def get_latent_projection(self, data_loader):
-        """
-        Returns the latent representation on a given network.
-        
-        Used after optimization to access to the latent representations.
-        
-        Parameters
-        ----------
-        data_loader : torch.DataLoader
-            The DataLoader to project (intended to be the same that the one used for optimization).
-
-        Returns
-        -------
-        all_data : numpy array
-            The latent representation for each data in the dataset.
-
-        """
-        all_data = []
-        for spec in data_loader:
-            spec = spec.float().to(self.device)
-            spec_recons, z = self.forward(spec)
-            for elt in z:
-                all_data.append(elt.cpu().detach().numpy())
-        return all_data
-    
-    def get_W(self):
-        """
-        Method returning the nonnegative part of W, used for reconstructing patterns and studying the decoder.
-        """
-        return F.relu(self.W_torch).cpu().detach().numpy()
-    
-    def get_H(self):
-        """
-        Method returning the nonnegative part of H, used for reconstructing patterns and studying the decoder.
-        """
-        return F.relu(self.H_torch).cpu().detach().numpy()
-    
-    def get_G(self):
-        """
-        Method returning the nonnegative part of the G core tensor (refolded into a tensor), used for reconstructing patterns and studying the decoder.
-        """
-        return tl.fold(F.relu(self.unfolded_G_torch).cpu().detach().numpy(), mode = 2, shape = (self.ntd_dimensions[0], self.ntd_dimensions[1], self.ntd_dimensions[2]))
-    
-    def get_pattern_list(self):
-        """
-        Method computing all patterns and returning them.
-        """
-        nn_g = F.relu(self.unfolded_G_torch)
-        kron_T = torch.kron(self.W_torch.T, self.H_torch.T)
-        pat_torch = F.relu(torch.matmul(nn_g, kron_T)).cpu().detach().numpy()
-        return np.reshape(pat_torch,(self.ntd_dimensions[2], self.input_size_y, self.input_size_x))
-       
-# %% Fully-connected
-class FullyConnectedAutoencoderNTD(GenericAutoencoderNTD):
-    """
-    AE-NTD with a fully-connected (2 layers) encoder.
-    """
-    def __init__(self, input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
-        """
-        Constructor.
-        
-        See parent class for parameters.
-        """
-        super().__init__(input_size_x = input_size_x, input_size_y = input_size_y, ntd_dimensions = ntd_dimensions, unfolded_G = unfolded_G, W = W, H = H, bn_latent_init_stds = bn_latent_init_stds, bn_latent_init_avgs = bn_latent_init_avgs, 
-                         beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-
-        # Encoder
-        self.enc1 = nn.Linear(in_features=input_size_x * input_size_y, out_features=ntd_dimensions[0]*ntd_dimensions[1])
-        self.enc2 = nn.Linear(in_features=ntd_dimensions[0]*ntd_dimensions[1], out_features=ntd_dimensions[2])
-
-        self.bn1 = nn.BatchNorm1d(ntd_dimensions[0]*ntd_dimensions[1])
-
-        # if seed is not None: # Should aready be set in parent class
-        #     torch.manual_seed(seed)
-
-        nn.init.kaiming_uniform_(self.enc1.weight, mode='fan_out', nonlinearity='relu')
-        nn.init.zeros_(self.enc1.bias)
-        # nn.init.kaiming_uniform_(self.enc2.weight, a=-1e-5, mode='fan_out', nonlinearity='leaky_relu')
-        nn.init.kaiming_uniform_(self.enc2.weight, mode='fan_out', nonlinearity='relu')
-        nn.init.zeros_(self.enc2.bias)
-
-    def encoder(self, x):
-        """
-        Encoder of the Fully-Connected network.
-        Two dense layers, each followed by a batch normalization layer.
-        The last layer (the 2nd one) may contain a nonnlinear activation function.
-        In that case, the activation function replace the batch normalization layer.
-        """
-        x = F.relu(self.enc1(x))
-        x = self.bn1(x)
-
-        x = self.enc2(x)
-        
-        if self.latent_nonlinearity is not None:
-            z = self.latent_nonlinearity(x)
-        else:
-            x = self.bn_latent(x)
-            #z = F.leaky_relu(x, negative_slope = -1e-5)
-            z = torch.add(F.relu(x), 1e-10)
-
-        return z
-    
-# %% Convolutional
-class ConvolutionalAutoencoderNTD(GenericAutoencoderNTD):
-    """
-    AE-NTD with a convolutional (3 layers) encoder.
-    """
-    def __init__(self, input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
-        """
-        Constructor.
-        
-        See parent class for parameters.
-        """
-        super().__init__(input_size_x = input_size_x, input_size_y = input_size_y, ntd_dimensions = ntd_dimensions, unfolded_G = unfolded_G, W = W, H = H, bn_latent_init_stds = bn_latent_init_stds, bn_latent_init_avgs = bn_latent_init_avgs, 
-                         beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
-        
-        self.input_size_pool_y = int(input_size_y/4) # input_size / pool ## NOTE: Doesn't work for odd input sizes (in reconstruction), so TODO.
-        self.input_size_pool_x = int(input_size_x/4) # input_size / pool
-        
-        self.input_size_x = input_size_x
-        self.input_size_y = input_size_y
-        
-        # if seed is not None: # Should aready be set in parent class
-        #     torch.manual_seed(seed)
-        
-        # Encoder
-        ## Convolutional layers
-        self.conv1 = nn.Conv2d(1, 4, 3, padding=1)  
-        self.conv2 = nn.Conv2d(4,16, 3, padding=1)
-        nn.init.kaiming_uniform_(self.conv1.weight, mode='fan_out', nonlinearity='relu')
-        nn.init.zeros_(self.conv1.bias)
-        nn.init.kaiming_uniform_(self.conv2.weight, mode='fan_out', nonlinearity='relu')
-        nn.init.zeros_(self.conv2.bias)
-        
-        self.bn_1 = nn.BatchNorm2d(4)
-        self.bn_2 = nn.BatchNorm2d(16)
-        
-        self.pool = nn.MaxPool2d(2, 2)
-        self.flatten = nn.Flatten()
-
-        ## Fully-connected controling latent space size.
-        in_features = 16 * self.input_size_pool_x * self.input_size_pool_y # nb_kernels_last_conv * (input_size / pool)
-        self.fc = nn.Linear(in_features=in_features, out_features=ntd_dimensions[2])
-        
-        # nn.init.kaiming_uniform_(self.fc.weight, a=-1e-5, mode='fan_out', nonlinearity='leaky_relu')
-        nn.init.kaiming_uniform_(self.fc.weight, mode='fan_out', nonlinearity='relu')
-        nn.init.zeros_(self.fc.bias)
-        
-    def encoder(self, x):
-        """
-        Encoder of the Covolutional Autoencoder.
-        It is implemented with two convolutional layers, 
-        each followed by a ReLU, a pooling layer, and a batch normalization layer.
-        After these convolutional blocks, a fully-connected layer is implemented,
-        leading to the latent representations.
-        A batch normalization layer is implemented after the dense layer,
-        but it can be replaced by a nonlinear activation function if specified.
-        """
-        self.batch_size = x.shape[0]
-        
-        x = F.relu(self.conv1(x))
-        x = self.pool(x)
-        x = self.bn_1(x)
-        x = F.relu(self.conv2(x))
-        x = self.pool(x)
-        x = self.bn_2(x)
-        
-        x = self.flatten(x)
-        x = self.fc(x)
-        
-        if self.latent_nonlinearity is not None:
-            z = self.latent_nonlinearity(x)
-        else:
-            x = self.bn_latent(x)
-            z = torch.add(F.relu(x), 1e-10)
-        return z
-    
-    def forward(self, x):
-        """
-        Redefinition of the forward method, in order to account for the matrix shape of the input (conv network).
-        """
-        batch_size = x.shape[0]
-        x_hat, z = super().forward(x)
-        x_hat = x_hat.reshape((batch_size, 1, self.input_size_y, self.input_size_x))
-        return x_hat, z
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Apr 14 18:46:42 2021
+
+@author: amarmore
+
+Mixing the Nonnegative Tucker Decomposition (NTD) with Autoencoders (Single-Song AutoEncoders).
+
+In short, the idea is to implement an NTD structure in the decoder. See [1 - Chapter 6] for details.
+
+References
+----------
+[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
+PhD Thesis Marmoret Axel 
+(not uploaded yet but will be soon!)
+(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
+"""
+
+import barmuscomp.ae_utils as ae_utils
+from barmuscomp.model.early_stopping import EarlyStopping
+import barmuscomp.model.current_plot as current_plot
+import barmuscomp.model.errors as err
+
+import numpy as np
+import random
+import warnings
+import tensorly as tl
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+class GenericAutoencoderNTD(nn.Module):
+    """
+    Generic Autoencoder, with NTD decoder.
+    
+    Hence, the decoder is structured with matrices W, H and the core tensor G.
+    """
+    def __init__(self,  input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
+        """
+        Constructor of the AE-NTD.
+
+        Parameters
+        ----------
+        input_size_x : positive int
+            Dimension of the x axis (time at barscale). 
+        input_size_y : positive int
+            Dimension of the y axis (frequency scale). .
+        ntd_dimensions : list of integers.
+            Dimensions of the factors for NTD 
+            (i.e. number of columns of each matrix factor, 
+             or , equivalently, dimensions of the core tensor).
+        unfolded_G : numpy array
+            Initialization for the core tensor G.
+            The tensor must be unfolded on the barwise mode.
+        W : numpy array
+            Initialization for the factor matrix W (frequency mode).
+        H : numpy array
+            Initialization for the factor matrix H (rhythmic factors).
+        bn_latent_init_stds : list of float, optional
+            Initialization of the batch normalization layer on the latent space,
+            here, the standard deviation.
+            If set, they must be computed as the std of the dimensions of the Q matrix.
+            The default is None.
+        bn_latent_init_avgs :list of float, optional
+            Initialization of the batch normalization layer on the latent space,
+            here, the averages.
+            If set, they must be computed as the averages of the dimensions of the Q matrix.
+            The default is None.
+        beta : float, optional
+            The beta value in the beta-divergence, 
+            specifying the loss function between the input and the output. 
+            The default is 2 (i.e. Euclidean Loss).
+        latent_nonlinearity : string, optional
+            A value specfiying the choice for a nonlinear activation function
+            constraining the values of the latent representation.
+            The default is None, meaning no nonlinear activation function.
+        seed : float, optional
+            A seed to fix pseudo-randomness.
+            The default is None, meaning no seed.
+
+        Raises
+        ------
+        InvalidArgumentValueException
+            Raised if arguments are not accurately set.
+
+        """
+        if W is None and input_size_y == None:
+            raise err.InvalidArgumentValueException("You must specify either W or its size. Here, both args 'W' and 'input_size_y' are set to None.")
+        if H is None and input_size_x == None:
+            raise err.InvalidArgumentValueException("You must specify either H or its size. Here, both args 'H' and 'input_size_x' are set to None.")
+        super(GenericAutoencoderNTD, self).__init__()
+        self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        
+        self.input_size_x = input_size_x
+        self.input_size_y = input_size_y
+        
+        self.beta = beta
+        self.ntd_dimensions = ntd_dimensions
+        
+        if seed is not None:
+            torch.manual_seed(seed)
+        
+        if W is None:
+            self.W_torch = nn.Parameter(torch.empty(input_size_y, ntd_dimensions[0]), requires_grad = True)
+            nn.init.kaiming_uniform_(self.W_torch, mode='fan_out', nonlinearity='relu')
+        else:
+            self.W_torch = nn.Parameter(torch.tensor(W).float().contiguous(), requires_grad = True)
+
+        if H is None:
+            self.H_torch = nn.Parameter(torch.empty(input_size_x, ntd_dimensions[1]), requires_grad = True)
+            nn.init.kaiming_uniform_(self.H_torch, mode='fan_out', nonlinearity='relu')
+        else:
+            self.H_torch = nn.Parameter(torch.tensor(H).float().contiguous(), requires_grad = True)
+
+        if unfolded_G is None:
+            self.unfolded_G_torch = nn.Parameter(torch.empty(ntd_dimensions[2], ntd_dimensions[0]*ntd_dimensions[1]), requires_grad = True)        
+            nn.init.kaiming_uniform_(self.unfolded_G_torch, mode='fan_out', nonlinearity='relu')
+        else:
+            self.unfolded_G_torch = nn.Parameter(torch.tensor(unfolded_G).float().contiguous(), requires_grad = True)
+            
+        if latent_nonlinearity is None:
+            self.latent_nonlinearity = None
+
+            self.bn_latent = nn.BatchNorm1d(ntd_dimensions[2])
+            if bn_latent_init_stds != None:
+                self.bn_latent.weight.data = torch.tensor(bn_latent_init_stds).float() if not torch.is_tensor(bn_latent_init_stds) else bn_latent_init_stds.clone().detach()
+            if bn_latent_init_avgs != None:
+                self.bn_latent.bias.data = torch.tensor(bn_latent_init_avgs).float() if not torch.is_tensor(bn_latent_init_avgs) else bn_latent_init_avgs.clone().detach()
+
+        elif latent_nonlinearity == "sigmoid":
+            self.latent_nonlinearity = nn.Sigmoid()
+        # elif latent_nonlinearity == "hardshrink":
+        #     self.latent_nonlinearity = nn.Hardshrink(lambd = 0.5)
+        elif latent_nonlinearity == "softmax":
+            self.latent_nonlinearity = nn.Softmax(dim=1)
+        elif latent_nonlinearity == "tanh":
+            self.latent_nonlinearity = nn.Tanh()
+        else:
+            raise err.InvalidArgumentValueException(f"Activation function not understood for the latent space: {latent_nonlinearity}") from None
+
+    def forward(self, x):
+        """
+        Forward pass.
+        x_hat is the reconstructed input, z is the latent projection.
+        """        
+        # Encoding
+        z = self.encoder(x)
+            
+        # Decoding
+        x_hat = self.decoder(z)
+
+        return x_hat, z
+    
+    def encoder(self, x):
+        """
+        Generic encoder, not defined in the parent class, must be redefined in children classes.
+        """
+        raise NotImplementedError("To be redefined in children classes")
+    
+    def decoder(self, z):
+        """
+        NTD based decoder.
+        
+        It consists of two fully-connected layers, with two relu functions:
+            - The first with the structure of the core tensor G,
+            - The second with the structure of the Kronecker product between W and H.
+        Hence, the decoder fully mimics an NTD, and these matrices may be initialized from the results of an NTD.
+        """
+        x = F.relu(torch.matmul(z, self.unfolded_G_torch))
+        
+        w_kron_h = torch.kron(self.W_torch.T, self.H_torch.T)
+        mat_mul = torch.matmul(x, w_kron_h)
+        x_hat = F.relu(mat_mul)
+        
+        return x_hat
+    
+    def my_optim_method(self, n_epochs, data_loader, lr = 1e-3, early_stop_patience = 100, verbose = False, labels = None):
+        """
+        Default optimization method.
+        
+        This method is to be called in order to optimize the network.
+
+        Parameters
+        ----------
+        n_epochs : int
+            Number of epochs to perform.
+        data_loader : torch.DataLoader
+            The DataLoader to optimize on.
+        lr : float, optional
+            Learning rate of the Network. 
+            The default is 1e-3.
+        early_stop_patience : int, optional
+            Patience for the number of consecutive epochs.
+            If the loss doesn't decrease during early_stop_patience epochs, the optimization stops. 
+            The default is 100.
+        verbose : boolean, optional
+            Argument to print the evolution of the optimization.
+            Prints the current loss and plots a view of the autosimilarity of 
+            latent variables and a PCA of the latent space.
+            The default is False.
+        labels : None or array, optional
+            Only used if verbose is set to True.
+            If labels are set, they will be used to color the output of PCA projection.
+            If they are set to None, no label is used. The default is None.
+
+        Returns
+        -------
+        GenericAutoencoder
+            The instance of the network, optimized.
+            NB: it is not required to return the network, this is rather implemented 
+            in order to avoid some "unintenional" optimization 
+            (as it forces a human user to notice that something is returned,
+             and hence that some code was run).
+        losses : list of positive floats
+            The loss values at each iteration.
+
+        """
+        self = self.to(self.device)
+        #print(f"Using {self.device}")
+        es = EarlyStopping(patience=early_stop_patience)
+        
+        nb_bars = 0
+        for iter_dl in data_loader:
+            nb_bars += iter_dl.shape[0]
+
+        if self.beta == 2:
+            recons_loss = nn.MSELoss() # Mean Squared Euclidian loss
+        else:
+            recons_loss = ae_utils.BetaDivergenceLoss(beta = self.beta)
+            # recons_loss = torch.jit.script(ae_utils.BetaDivergenceLoss(beta = self.beta))
+        losses = []
+            
+        optimizer = torch.optim.Adam(self.parameters(), lr=lr)
+        
+        # Scheduler to decrease the learning rate when optimization reaches a plateau (20 iterations)
+        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=20, verbose=verbose,min_lr=1e-5)
+            
+        for epoch in range(1, n_epochs+1):
+            total_loss_epoch = 0.0
+            for spec in data_loader:
+                spec = spec.float().to(self.device)
+                optimizer.zero_grad()
+                spec_recons, z = self.forward(spec) # Forward pass
+                loss = recons_loss(spec_recons, spec) # Loss
+                loss.backward() # Backward pass
+                optimizer.step() # Optimizes the net with grads
+                
+                total_loss_epoch += loss.item() * spec.size(0)
+            total_loss_epoch = total_loss_epoch/nb_bars
+            losses.append(total_loss_epoch)
+            scheduler.step(total_loss_epoch) # scheduler for the decrease of lr on a plateau
+                
+            if verbose:
+                print('Epoch: {} \tCumulated reconstruction loss: {:.6f}'.format(epoch, total_loss_epoch))
+                if epoch%50 == 0:
+                    projection = self.get_latent_projection(data_loader)
+                    current_plot.plot_latent_space(projection, labels = labels)
+                    
+            if es.step(total_loss_epoch): # Checks if loss has decreased, to stop the optimization if performances don't increase for early_stop_patience epochs.
+                if verbose:
+                    print(f"Early stopping criterion has been met in {epoch}, computation is stopped.")
+                break 
+        return self, losses
+    
+    def get_latent_projection(self, data_loader):
+        """
+        Returns the latent representation on a given network.
+        
+        Used after optimization to access to the latent representations.
+        
+        Parameters
+        ----------
+        data_loader : torch.DataLoader
+            The DataLoader to project (intended to be the same that the one used for optimization).
+
+        Returns
+        -------
+        all_data : numpy array
+            The latent representation for each data in the dataset.
+
+        """
+        all_data = []
+        for spec in data_loader:
+            spec = spec.float().to(self.device)
+            spec_recons, z = self.forward(spec)
+            for elt in z:
+                all_data.append(elt.cpu().detach().numpy())
+        return all_data
+    
+    def get_W(self):
+        """
+        Method returning the nonnegative part of W, used for reconstructing patterns and studying the decoder.
+        """
+        return F.relu(self.W_torch).cpu().detach().numpy()
+    
+    def get_H(self):
+        """
+        Method returning the nonnegative part of H, used for reconstructing patterns and studying the decoder.
+        """
+        return F.relu(self.H_torch).cpu().detach().numpy()
+    
+    def get_G(self):
+        """
+        Method returning the nonnegative part of the G core tensor (refolded into a tensor), used for reconstructing patterns and studying the decoder.
+        """
+        return tl.fold(F.relu(self.unfolded_G_torch).cpu().detach().numpy(), mode = 2, shape = (self.ntd_dimensions[0], self.ntd_dimensions[1], self.ntd_dimensions[2]))
+    
+    def get_pattern_list(self):
+        """
+        Method computing all patterns and returning them.
+        """
+        nn_g = F.relu(self.unfolded_G_torch)
+        kron_T = torch.kron(self.W_torch.T, self.H_torch.T)
+        pat_torch = F.relu(torch.matmul(nn_g, kron_T)).cpu().detach().numpy()
+        return np.reshape(pat_torch,(self.ntd_dimensions[2], self.input_size_y, self.input_size_x))
+       
+# %% Fully-connected
+class FullyConnectedAutoencoderNTD(GenericAutoencoderNTD):
+    """
+    AE-NTD with a fully-connected (2 layers) encoder.
+    """
+    def __init__(self, input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
+        """
+        Constructor.
+        
+        See parent class for parameters.
+        """
+        super().__init__(input_size_x = input_size_x, input_size_y = input_size_y, ntd_dimensions = ntd_dimensions, unfolded_G = unfolded_G, W = W, H = H, bn_latent_init_stds = bn_latent_init_stds, bn_latent_init_avgs = bn_latent_init_avgs, 
+                         beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+
+        # Encoder
+        self.enc1 = nn.Linear(in_features=input_size_x * input_size_y, out_features=ntd_dimensions[0]*ntd_dimensions[1])
+        self.enc2 = nn.Linear(in_features=ntd_dimensions[0]*ntd_dimensions[1], out_features=ntd_dimensions[2])
+
+        self.bn1 = nn.BatchNorm1d(ntd_dimensions[0]*ntd_dimensions[1])
+
+        # if seed is not None: # Should aready be set in parent class
+        #     torch.manual_seed(seed)
+
+        nn.init.kaiming_uniform_(self.enc1.weight, mode='fan_out', nonlinearity='relu')
+        nn.init.zeros_(self.enc1.bias)
+        # nn.init.kaiming_uniform_(self.enc2.weight, a=-1e-5, mode='fan_out', nonlinearity='leaky_relu')
+        nn.init.kaiming_uniform_(self.enc2.weight, mode='fan_out', nonlinearity='relu')
+        nn.init.zeros_(self.enc2.bias)
+
+    def encoder(self, x):
+        """
+        Encoder of the Fully-Connected network.
+        Two dense layers, each followed by a batch normalization layer.
+        The last layer (the 2nd one) may contain a nonnlinear activation function.
+        In that case, the activation function replace the batch normalization layer.
+        """
+        x = F.relu(self.enc1(x))
+        x = self.bn1(x)
+
+        x = self.enc2(x)
+        
+        if self.latent_nonlinearity is not None:
+            z = self.latent_nonlinearity(x)
+        else:
+            x = self.bn_latent(x)
+            #z = F.leaky_relu(x, negative_slope = -1e-5)
+            z = torch.add(F.relu(x), 1e-10)
+
+        return z
+    
+# %% Convolutional
+class ConvolutionalAutoencoderNTD(GenericAutoencoderNTD):
+    """
+    AE-NTD with a convolutional (3 layers) encoder.
+    """
+    def __init__(self, input_size_x, input_size_y, ntd_dimensions, unfolded_G, W, H, bn_latent_init_stds = None, bn_latent_init_avgs = None, beta = 2, latent_nonlinearity = None, seed = None):
+        """
+        Constructor.
+        
+        See parent class for parameters.
+        """
+        super().__init__(input_size_x = input_size_x, input_size_y = input_size_y, ntd_dimensions = ntd_dimensions, unfolded_G = unfolded_G, W = W, H = H, bn_latent_init_stds = bn_latent_init_stds, bn_latent_init_avgs = bn_latent_init_avgs, 
+                         beta = beta, latent_nonlinearity = latent_nonlinearity, seed = seed)
+        
+        self.input_size_pool_y = int(input_size_y/4) # input_size / pool ## NOTE: Doesn't work for odd input sizes (in reconstruction), so TODO.
+        self.input_size_pool_x = int(input_size_x/4) # input_size / pool
+        
+        self.input_size_x = input_size_x
+        self.input_size_y = input_size_y
+        
+        # if seed is not None: # Should aready be set in parent class
+        #     torch.manual_seed(seed)
+        
+        # Encoder
+        ## Convolutional layers
+        self.conv1 = nn.Conv2d(1, 4, 3, padding=1)  
+        self.conv2 = nn.Conv2d(4,16, 3, padding=1)
+        nn.init.kaiming_uniform_(self.conv1.weight, mode='fan_out', nonlinearity='relu')
+        nn.init.zeros_(self.conv1.bias)
+        nn.init.kaiming_uniform_(self.conv2.weight, mode='fan_out', nonlinearity='relu')
+        nn.init.zeros_(self.conv2.bias)
+        
+        self.bn_1 = nn.BatchNorm2d(4)
+        self.bn_2 = nn.BatchNorm2d(16)
+        
+        self.pool = nn.MaxPool2d(2, 2)
+        self.flatten = nn.Flatten()
+
+        ## Fully-connected controling latent space size.
+        in_features = 16 * self.input_size_pool_x * self.input_size_pool_y # nb_kernels_last_conv * (input_size / pool)
+        self.fc = nn.Linear(in_features=in_features, out_features=ntd_dimensions[2])
+        
+        # nn.init.kaiming_uniform_(self.fc.weight, a=-1e-5, mode='fan_out', nonlinearity='leaky_relu')
+        nn.init.kaiming_uniform_(self.fc.weight, mode='fan_out', nonlinearity='relu')
+        nn.init.zeros_(self.fc.bias)
+        
+    def encoder(self, x):
+        """
+        Encoder of the Covolutional Autoencoder.
+        It is implemented with two convolutional layers, 
+        each followed by a ReLU, a pooling layer, and a batch normalization layer.
+        After these convolutional blocks, a fully-connected layer is implemented,
+        leading to the latent representations.
+        A batch normalization layer is implemented after the dense layer,
+        but it can be replaced by a nonlinear activation function if specified.
+        """
+        self.batch_size = x.shape[0]
+        
+        x = F.relu(self.conv1(x))
+        x = self.pool(x)
+        x = self.bn_1(x)
+        x = F.relu(self.conv2(x))
+        x = self.pool(x)
+        x = self.bn_2(x)
+        
+        x = self.flatten(x)
+        x = self.fc(x)
+        
+        if self.latent_nonlinearity is not None:
+            z = self.latent_nonlinearity(x)
+        else:
+            x = self.bn_latent(x)
+            z = torch.add(F.relu(x), 1e-10)
+        return z
+    
+    def forward(self, x):
+        """
+        Redefinition of the forward method, in order to account for the matrix shape of the input (conv network).
+        """
+        batch_size = x.shape[0]
+        x_hat, z = super().forward(x)
+        x_hat = x_hat.reshape((batch_size, 1, self.input_size_y, self.input_size_x))
+        return x_hat, z
```

### Comparing `barmuscomp-0.1.2/barmuscomp/ae_utils.py` & `barmuscomp-0.1.3/barmuscomp/ae_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,361 +1,361 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 14 18:34:29 2021
-
-@author: amarmore
-
-Useful functions for handling single-song compression paradigms.
-"""
-
-import as_seg.data_manipulation as dm
-import as_seg.autosimilarity_computation as as_comp
-import barmuscomp.model.errors as err
-
-import copy
-import random
-import numpy as np
-import tensorly as tl
-import torch
-import torch.nn as nn
-import matplotlib.pyplot as plt
-import matplotlib.cm as cm
-
-# %% Dataloaders generation
-def generate_dataloader(tensor_barwise, batch_size = None):
-    """
-    Generates a torch.DataLoader from the tensor spectrogram.
-    
-    Each barwise spectrogram is a matrix (frequency, time at barscale).
-
-    Parameters
-    ----------
-    tensor_barwise : np.array tensor
-        The tensor-spectrogram as a np.array.
-
-    Returns
-    -------
-    data_loader : torch.DataLoader
-        torch.DataLoader for this song and this tensor-spectrogram.
-    """
-    if batch_size == None:
-        batch_size = tensor_barwise.shape[0]
-    num_workers = 0
-    nb_bars = tensor_barwise.shape[0]
-    freq_len, subdivision_bars = tensor_barwise.shape[1], tensor_barwise.shape[2]
-
-    barwise_spec = copy.deepcopy(tensor_barwise)
-    
-    barwise_spec = barwise_spec.reshape((nb_bars, 1, freq_len, subdivision_bars))
-    data_loader = torch.utils.data.DataLoader(barwise_spec, batch_size=batch_size, num_workers=num_workers)
-    
-    return data_loader
-    
-def generate_flatten_dataloader(tensor_barwise, batch_size = None):
-    """
-    Generates a torch.DataLoader from the tensor spectrogram.
-    
-    Each barwise spectrogram is a vector (frequency x time at barscale).
-
-    Parameters
-    ----------
-    tensor_barwise : np.array tensor
-        The tensor-spectrogram as a np.array.
-
-    Returns
-    -------
-    data_loader : torch.DataLoader
-        torch.DataLoader for this song and this tensor-spectrogram.
-    """
-    if batch_size == None:
-        batch_size = tensor_barwise.shape[0]
-    num_workers = 0
-    nb_bars = tensor_barwise.shape[0]
-    freq_len, subdivision_bars = tensor_barwise.shape[1], tensor_barwise.shape[2]
-
-    barwise_spec = copy.deepcopy(tensor_barwise)
-    
-    flatten_barwise_spec = barwise_spec.reshape((nb_bars, freq_len*subdivision_bars), order="C")
-    flatten_simplet_data_loader = torch.utils.data.DataLoader(flatten_barwise_spec, batch_size=batch_size, num_workers=num_workers)
-    
-    return flatten_simplet_data_loader
-    
-# %% Deterministic initializations for networks
-def seeded_weights_init_kaiming(m, seed = 42): 
-    """ 
-    Determinstic initialization of weights with Kaiming uniform distribution.
-
-    Parameters
-    ----------
-    m : torch.nn
-        A layer of the network.
-    seed : float, optional
-        The seed to fix the pseudo-randomness. The default is 42.
-
-    """
-    torch.manual_seed(seed)
-    #torch.use_deterministic_algorithms(True)
-    # if isinstance(m, nn.BatchNorm1d):
-    #     nn.init.zeros_(m.bias)
-    #     nn.init.ones_(m.weight)
-    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
-        #nn.init.kaiming_uniform_(m.weight, mode='fan_in', nonlinearity='relu')
-        nn.init.kaiming_uniform_(m.weight, mode='fan_out', nonlinearity='relu')
-        if m.bias is not None:
-            nn.init.zeros_(m.bias)
-     
-def random_weights_init_kaiming(m): 
-    """
-    Random initialization of weights with Kaiming uniform distribution.
-
-    Parameters
-    ----------
-    m : torch.nn
-        A layer of the network.
-    """
-    #torch.use_deterministic_algorithms(False)
-    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
-        #nn.init.kaiming_uniform_(m.weight, mode='fan_in', nonlinearity='relu')
-        nn.init.kaiming_uniform_(m.weight, mode='fan_out', nonlinearity='relu')
-        if m.bias is not None:
-            nn.init.zeros_(m.bias)
-
-def seeded_weights_init_xavier(m):
-    """
-    Determinstic initialization of weights with Xavier uniform distribution.
-
-    Parameters
-    ----------
-    m : torch.nn
-        A layer of the network.
-    """    
-    torch.manual_seed(42)
-    torch.use_deterministic_algorithms(True)
-    # if isinstance(m, nn.BatchNorm1d):
-    #     nn.init.zeros_(m.bias)
-    #     nn.init.ones_(m.weight)
-    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
-        nn.init.xavier_uniform_(m.weight)
-        if m.bias is not None:
-            nn.init.zeros_(m.bias)
-        
-def weights_init_sparse(m):
-    """
-    Determinstic initialization of weights with sparse initialization.
-
-    Parameters
-    ----------
-    m : torch.nn
-        A layer of the network.
-    """   
-    if isinstance(m, nn.Conv1d) or isinstance(m, nn.Linear) or isinstance(m, nn.ConvTranspose1d):
-        torch.nn.init.sparse_(m.weight, sparsity = 0.1)
-        
-def weights_ones(m):
-    """
-    Determinstic initialization of weights with layers full of ones.
-
-    Parameters
-    ----------
-    m : torch.nn
-        A layer of the network.
-    """   
-    if isinstance(m, nn.Linear):# or isinstance(m, nn.ConvTranspose2d):
-        nn.init.ones_(m.weight) 
-        
-# %% Triplet losees
-class TripletLoss(nn.Module):
-    """
-    Triplet Loss class, following the Triplet Loss paradigm. See [1] for details.
-        
-    Comes from: https://www.kaggle.com/hirotaka0122/triplet-loss-with-pytorch
-    
-    References
-    ----------
-    [1] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
-    Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
-    In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
-    """
-    
-    def __init__(self, margin=1.0):
-        """
-        Constructor of the loss.
-
-        Parameters
-        ----------
-        margin : float, optional
-            Margin for the triplet loss. The default is 1.0.
-
-        """
-        super(TripletLoss, self).__init__()
-        self.margin = margin
-        
-    def calc_euclidean(self, x1, x2):
-        """
-        Euclidean distance between x1 and x2.
-        """
-        return (x1 - x2).pow(2).sum(1)
-    
-    def forward(self, anchor, positive, negative):
-        """
-        Computes the triplet loss, based on the euclidean distances between samples.
-        """
-        distance_positive = self.calc_euclidean(anchor, positive)
-        distance_negative = self.calc_euclidean(anchor, negative)
-        losses = torch.relu(distance_positive - distance_negative + self.margin)
-        return losses.mean()
-    
-class TripletLossDoubleMargin(nn.Module):
-    """
-    Triplet Loss with positive and negative margins, following the work of [1]
-    
-    References
-    ----------
-    [1] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
-    Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
-    In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
-    """
-    def __init__(self, pos_margin=1.0, neg_margin = 3.0):
-        """
-        Constructor of the loss.
-
-        Parameters
-        ----------
-        pos_margin : float, optional
-            Margin for positive examples. The default is 1.0.
-        neg_margin : float, optional
-            Margin for negative examples. The default is 3.0.
-
-        """
-        super(TripletLossDoubleMargin, self).__init__()
-        self.pos_margin = pos_margin
-        self.neg_margin = neg_margin
-        
-    def calc_euclidean(self, x1, x2):
-        """
-        Euclidean distance between x1 and x2.
-        """
-        return (x1 - x2).pow(2).sum(1)
-    
-    def forward(self, anchor, positive, negative):
-        """
-        Computes the triplet loss, based on the euclidean distances between samples.
-        """
-        distance_positive = self.calc_euclidean(anchor, positive)
-        distance_negative = self.calc_euclidean(anchor, negative)
-        losses = torch.relu(self.neg_margin - distance_negative) + torch.relu(distance_positive - self.pos_margin)
-        return losses.mean()
-    
-def generate_triplet_dataloader(tensor_barwise, top_partition = 0.1, medium_partition = 0.5, batch_size = None):
-    """
-    Generates torch.DataLoaders for TripletLoss, with a positive and a negative example for each bar.
-    Positive and negative examples are randomly selected from most similar and less similar bars.
-    The similarity is the feature_wise similarity.
-    Both arguments ``top_partition'' and ``medium_partition'' are dedicated to thresholding most and less similar for random selection.
-
-    Parameters
-    ----------
-    tensor_barwise : np.array tensor
-        The tensor-spectrogram as a np.array.
-    top_partition : float \in [0,1], optional
-        Percentage of most similar bars (in feature-wise similarity) on which select a positive example.
-        The default is 0.1, corresponding to 10% most similar bars.
-    medium_partition : float \in [0,1], optional
-        Percentage of less similar bars (in feature-wise similarity) on which select a positive example.
-        The default is 0.5, selecting from the 50% least similar bars.
-
-    Returns
-    -------
-    triplet_data_loader : torch.DataLoader
-        torch.DataLoader for this song and this tensor-spectrogram.
-        Each barwise spectrogram is kept as a matrix, for convolutional networks.
-    flatten_triplet_data_loader : torch.DataLoader
-        torch.DataLoader for this song and this tensor-spectrogram.
-        On this DataLoader, each barwise spectrogram is flattened, for networks which needs vectors as inputs.
-
-    """
-    if batch_size == None:
-        batch_size = tensor_barwise.shape[0]
-    num_workers = 0
-    signal_autosimilarity = as_comp.get_cosine_autosimilarity(tl.unfold(tensor_barwise,0))
-    nb_bars = tensor_barwise.shape[0]
-    vectorized_spec_dim = tensor_barwise.shape[1]*tensor_barwise.shape[2]
-    
-    barwise_spec = copy.deepcopy(tensor_barwise)
-    triplet_data = []
-    flatten_triplet_data = []
-    
-    # threshed_mat = np.ones((nb_bars, nb_bars))
-
-    high_thresh = int(top_partition * nb_bars) + 1
-    medium_thresh = int(medium_partition * nb_bars)
-
-    for index, bar in enumerate(barwise_spec):
-        this_bar_similarities = signal_autosimilarity[index]
-        highest_indexes = np.argpartition(this_bar_similarities, -high_thresh)[-high_thresh:]
-        # threshed_mat[index,highest_indexes] = 2
-        # threshed_mat[highest_indexes,index] = 2
-        selected_high = random.choice(highest_indexes)
-        while selected_high == index:
-            selected_high = random.choice(highest_indexes)
-        positive_bar = barwise_spec[selected_high]
-
-        lowest_indexes = np.argpartition(this_bar_similarities, medium_thresh)[:medium_thresh]
-        # threshed_mat[index,lowest_indexes] = 0
-        # threshed_mat[lowest_indexes,index] = 0
-        selected_low = random.choice(lowest_indexes)
-        negative_bar = barwise_spec[selected_low]
-        
-        triplet_data.append((bar, positive_bar, negative_bar))
-        flatten_triplet_data.append((bar.reshape((vectorized_spec_dim), order="F"), positive_bar.reshape((vectorized_spec_dim), order="F"), negative_bar.reshape((vectorized_spec_dim), order="F")))
-    # plot_me_this_spectrogram(threshed_mat)
-
-    triplet_data_loader = torch.utils.data.DataLoader(triplet_data, batch_size=batch_size, num_workers=num_workers)
-    flatten_triplet_data_loader = torch.utils.data.DataLoader(flatten_triplet_data, batch_size=batch_size, num_workers=num_workers)
-    return triplet_data_loader, flatten_triplet_data_loader
-    
-# %% Beta-divergence loss
-class BetaDivergenceLoss(nn.Module):
-    """
-    Class defining the Beta divergence loss.
-    
-    Some inspiration was taken from https://github.com/yoyololicon/pytorch-NMF/blob/master/torchnmf/metrics.py
-    """
-
-    def __init__(self, beta = 1, eps = 1e-12):
-        """
-        Constructor. "eps" is a small contant to avoid dividing by zero.
-        """
-        super(BetaDivergenceLoss, self).__init__()
-        self.beta = beta
-        self.eps = eps
-        
-    def calc_beta_div(self, x1, x2):
-        """
-        Definition of the beta-divergence.
-        """
-        if self.beta == 1:
-            log_prod = torch.mul(x1, (x1.add(self.eps).log() - x2.add(self.eps).log()))
-            return (torch.add(torch.sub(log_prod, x1), x2)).mean()
-        elif self.beta == 0:
-            x1_div_x2 = torch.div(x1, x2.add(self.eps)).add(self.eps)
-            return torch.sub(x1_div_x2, x1_div_x2.log()).sub(1).mean()
-        else:
-            if self.beta < 0:
-                x1 = x1.add(self.eps)
-                x2 = x2.add(self.eps)
-            elif self.beta < 1:
-                x2 = x2.add(self.eps)
-            num =  torch.sub(torch.add(x1.pow(self.beta), x2.pow(self.beta).mul(self.beta - 1)), torch.mul(x1, x2.pow(self.beta-1)).mul(self.beta)).mean()
-            return num / (self.beta * (self.beta - 1))
-
-    def forward(self, x, y):
-        """
-        Computation.
-        """
-        if (x < 0).any():
-            raise err.NegativeValuesNotAccepted("Negative values in the input of the network, can't perform beta divergence.")
-        if (y < 0).any():
-            raise err.NegativeValuesNotAccepted("Negative values in the output of the network, can't perform beta divergence.")
-        losses = self.calc_beta_div(x, y)
-        return losses.mean()
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Apr 14 18:34:29 2021
+
+@author: amarmore
+
+Useful functions for handling single-song compression paradigms.
+"""
+
+import as_seg.data_manipulation as dm
+import as_seg.autosimilarity_computation as as_comp
+import barmuscomp.model.errors as err
+
+import copy
+import random
+import numpy as np
+import tensorly as tl
+import torch
+import torch.nn as nn
+import matplotlib.pyplot as plt
+import matplotlib.cm as cm
+
+# %% Dataloaders generation
+def generate_dataloader(tensor_barwise, batch_size = None):
+    """
+    Generates a torch.DataLoader from the tensor spectrogram.
+    
+    Each barwise spectrogram is a matrix (frequency, time at barscale).
+
+    Parameters
+    ----------
+    tensor_barwise : np.array tensor
+        The tensor-spectrogram as a np.array.
+
+    Returns
+    -------
+    data_loader : torch.DataLoader
+        torch.DataLoader for this song and this tensor-spectrogram.
+    """
+    if batch_size == None:
+        batch_size = tensor_barwise.shape[0]
+    num_workers = 0
+    nb_bars = tensor_barwise.shape[0]
+    freq_len, subdivision_bars = tensor_barwise.shape[1], tensor_barwise.shape[2]
+
+    barwise_spec = copy.deepcopy(tensor_barwise)
+    
+    barwise_spec = barwise_spec.reshape((nb_bars, 1, freq_len, subdivision_bars))
+    data_loader = torch.utils.data.DataLoader(barwise_spec, batch_size=batch_size, num_workers=num_workers)
+    
+    return data_loader
+    
+def generate_flatten_dataloader(tensor_barwise, batch_size = None):
+    """
+    Generates a torch.DataLoader from the tensor spectrogram.
+    
+    Each barwise spectrogram is a vector (frequency x time at barscale).
+
+    Parameters
+    ----------
+    tensor_barwise : np.array tensor
+        The tensor-spectrogram as a np.array.
+
+    Returns
+    -------
+    data_loader : torch.DataLoader
+        torch.DataLoader for this song and this tensor-spectrogram.
+    """
+    if batch_size == None:
+        batch_size = tensor_barwise.shape[0]
+    num_workers = 0
+    nb_bars = tensor_barwise.shape[0]
+    freq_len, subdivision_bars = tensor_barwise.shape[1], tensor_barwise.shape[2]
+
+    barwise_spec = copy.deepcopy(tensor_barwise)
+    
+    flatten_barwise_spec = barwise_spec.reshape((nb_bars, freq_len*subdivision_bars), order="C")
+    flatten_simplet_data_loader = torch.utils.data.DataLoader(flatten_barwise_spec, batch_size=batch_size, num_workers=num_workers)
+    
+    return flatten_simplet_data_loader
+    
+# %% Deterministic initializations for networks
+def seeded_weights_init_kaiming(m, seed = 42): 
+    """ 
+    Determinstic initialization of weights with Kaiming uniform distribution.
+
+    Parameters
+    ----------
+    m : torch.nn
+        A layer of the network.
+    seed : float, optional
+        The seed to fix the pseudo-randomness. The default is 42.
+
+    """
+    torch.manual_seed(seed)
+    #torch.use_deterministic_algorithms(True)
+    # if isinstance(m, nn.BatchNorm1d):
+    #     nn.init.zeros_(m.bias)
+    #     nn.init.ones_(m.weight)
+    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
+        #nn.init.kaiming_uniform_(m.weight, mode='fan_in', nonlinearity='relu')
+        nn.init.kaiming_uniform_(m.weight, mode='fan_out', nonlinearity='relu')
+        if m.bias is not None:
+            nn.init.zeros_(m.bias)
+     
+def random_weights_init_kaiming(m): 
+    """
+    Random initialization of weights with Kaiming uniform distribution.
+
+    Parameters
+    ----------
+    m : torch.nn
+        A layer of the network.
+    """
+    #torch.use_deterministic_algorithms(False)
+    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
+        #nn.init.kaiming_uniform_(m.weight, mode='fan_in', nonlinearity='relu')
+        nn.init.kaiming_uniform_(m.weight, mode='fan_out', nonlinearity='relu')
+        if m.bias is not None:
+            nn.init.zeros_(m.bias)
+
+def seeded_weights_init_xavier(m):
+    """
+    Determinstic initialization of weights with Xavier uniform distribution.
+
+    Parameters
+    ----------
+    m : torch.nn
+        A layer of the network.
+    """    
+    torch.manual_seed(42)
+    torch.use_deterministic_algorithms(True)
+    # if isinstance(m, nn.BatchNorm1d):
+    #     nn.init.zeros_(m.bias)
+    #     nn.init.ones_(m.weight)
+    if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Conv2d) or isinstance(m, nn.ConvTranspose2d):
+        nn.init.xavier_uniform_(m.weight)
+        if m.bias is not None:
+            nn.init.zeros_(m.bias)
+        
+def weights_init_sparse(m):
+    """
+    Determinstic initialization of weights with sparse initialization.
+
+    Parameters
+    ----------
+    m : torch.nn
+        A layer of the network.
+    """   
+    if isinstance(m, nn.Conv1d) or isinstance(m, nn.Linear) or isinstance(m, nn.ConvTranspose1d):
+        torch.nn.init.sparse_(m.weight, sparsity = 0.1)
+        
+def weights_ones(m):
+    """
+    Determinstic initialization of weights with layers full of ones.
+
+    Parameters
+    ----------
+    m : torch.nn
+        A layer of the network.
+    """   
+    if isinstance(m, nn.Linear):# or isinstance(m, nn.ConvTranspose2d):
+        nn.init.ones_(m.weight) 
+        
+# %% Triplet losees
+class TripletLoss(nn.Module):
+    """
+    Triplet Loss class, following the Triplet Loss paradigm. See [1] for details.
+        
+    Comes from: https://www.kaggle.com/hirotaka0122/triplet-loss-with-pytorch
+    
+    References
+    ----------
+    [1] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
+    Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
+    In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
+    """
+    
+    def __init__(self, margin=1.0):
+        """
+        Constructor of the loss.
+
+        Parameters
+        ----------
+        margin : float, optional
+            Margin for the triplet loss. The default is 1.0.
+
+        """
+        super(TripletLoss, self).__init__()
+        self.margin = margin
+        
+    def calc_euclidean(self, x1, x2):
+        """
+        Euclidean distance between x1 and x2.
+        """
+        return (x1 - x2).pow(2).sum(1)
+    
+    def forward(self, anchor, positive, negative):
+        """
+        Computes the triplet loss, based on the euclidean distances between samples.
+        """
+        distance_positive = self.calc_euclidean(anchor, positive)
+        distance_negative = self.calc_euclidean(anchor, negative)
+        losses = torch.relu(distance_positive - distance_negative + self.margin)
+        return losses.mean()
+    
+class TripletLossDoubleMargin(nn.Module):
+    """
+    Triplet Loss with positive and negative margins, following the work of [1]
+    
+    References
+    ----------
+    [1] Ho, K., Keuper, J., Pfreundt, F. J., & Keuper, M. (2021, January). 
+    Learning embeddings for image clustering: An empirical study of triplet loss approaches. 
+    In 2020 25th International Conference on Pattern Recognition (ICPR) (pp. 87-94). IEEE.
+    """
+    def __init__(self, pos_margin=1.0, neg_margin = 3.0):
+        """
+        Constructor of the loss.
+
+        Parameters
+        ----------
+        pos_margin : float, optional
+            Margin for positive examples. The default is 1.0.
+        neg_margin : float, optional
+            Margin for negative examples. The default is 3.0.
+
+        """
+        super(TripletLossDoubleMargin, self).__init__()
+        self.pos_margin = pos_margin
+        self.neg_margin = neg_margin
+        
+    def calc_euclidean(self, x1, x2):
+        """
+        Euclidean distance between x1 and x2.
+        """
+        return (x1 - x2).pow(2).sum(1)
+    
+    def forward(self, anchor, positive, negative):
+        """
+        Computes the triplet loss, based on the euclidean distances between samples.
+        """
+        distance_positive = self.calc_euclidean(anchor, positive)
+        distance_negative = self.calc_euclidean(anchor, negative)
+        losses = torch.relu(self.neg_margin - distance_negative) + torch.relu(distance_positive - self.pos_margin)
+        return losses.mean()
+    
+def generate_triplet_dataloader(tensor_barwise, top_partition = 0.1, medium_partition = 0.5, batch_size = None):
+    """
+    Generates torch.DataLoaders for TripletLoss, with a positive and a negative example for each bar.
+    Positive and negative examples are randomly selected from most similar and less similar bars.
+    The similarity is the feature_wise similarity.
+    Both arguments ``top_partition'' and ``medium_partition'' are dedicated to thresholding most and less similar for random selection.
+
+    Parameters
+    ----------
+    tensor_barwise : np.array tensor
+        The tensor-spectrogram as a np.array.
+    top_partition : float \in [0,1], optional
+        Percentage of most similar bars (in feature-wise similarity) on which select a positive example.
+        The default is 0.1, corresponding to 10% most similar bars.
+    medium_partition : float \in [0,1], optional
+        Percentage of less similar bars (in feature-wise similarity) on which select a positive example.
+        The default is 0.5, selecting from the 50% least similar bars.
+
+    Returns
+    -------
+    triplet_data_loader : torch.DataLoader
+        torch.DataLoader for this song and this tensor-spectrogram.
+        Each barwise spectrogram is kept as a matrix, for convolutional networks.
+    flatten_triplet_data_loader : torch.DataLoader
+        torch.DataLoader for this song and this tensor-spectrogram.
+        On this DataLoader, each barwise spectrogram is flattened, for networks which needs vectors as inputs.
+
+    """
+    if batch_size == None:
+        batch_size = tensor_barwise.shape[0]
+    num_workers = 0
+    signal_autosimilarity = as_comp.get_cosine_autosimilarity(tl.unfold(tensor_barwise,0))
+    nb_bars = tensor_barwise.shape[0]
+    vectorized_spec_dim = tensor_barwise.shape[1]*tensor_barwise.shape[2]
+    
+    barwise_spec = copy.deepcopy(tensor_barwise)
+    triplet_data = []
+    flatten_triplet_data = []
+    
+    # threshed_mat = np.ones((nb_bars, nb_bars))
+
+    high_thresh = int(top_partition * nb_bars) + 1
+    medium_thresh = int(medium_partition * nb_bars)
+
+    for index, bar in enumerate(barwise_spec):
+        this_bar_similarities = signal_autosimilarity[index]
+        highest_indexes = np.argpartition(this_bar_similarities, -high_thresh)[-high_thresh:]
+        # threshed_mat[index,highest_indexes] = 2
+        # threshed_mat[highest_indexes,index] = 2
+        selected_high = random.choice(highest_indexes)
+        while selected_high == index:
+            selected_high = random.choice(highest_indexes)
+        positive_bar = barwise_spec[selected_high]
+
+        lowest_indexes = np.argpartition(this_bar_similarities, medium_thresh)[:medium_thresh]
+        # threshed_mat[index,lowest_indexes] = 0
+        # threshed_mat[lowest_indexes,index] = 0
+        selected_low = random.choice(lowest_indexes)
+        negative_bar = barwise_spec[selected_low]
+        
+        triplet_data.append((bar, positive_bar, negative_bar))
+        flatten_triplet_data.append((bar.reshape((vectorized_spec_dim), order="F"), positive_bar.reshape((vectorized_spec_dim), order="F"), negative_bar.reshape((vectorized_spec_dim), order="F")))
+    # plot_me_this_spectrogram(threshed_mat)
+
+    triplet_data_loader = torch.utils.data.DataLoader(triplet_data, batch_size=batch_size, num_workers=num_workers)
+    flatten_triplet_data_loader = torch.utils.data.DataLoader(flatten_triplet_data, batch_size=batch_size, num_workers=num_workers)
+    return triplet_data_loader, flatten_triplet_data_loader
+    
+# %% Beta-divergence loss
+class BetaDivergenceLoss(nn.Module):
+    """
+    Class defining the Beta divergence loss.
+    
+    Some inspiration was taken from https://github.com/yoyololicon/pytorch-NMF/blob/master/torchnmf/metrics.py
+    """
+
+    def __init__(self, beta = 1, eps = 1e-12):
+        """
+        Constructor. "eps" is a small contant to avoid dividing by zero.
+        """
+        super(BetaDivergenceLoss, self).__init__()
+        self.beta = beta
+        self.eps = eps
+        
+    def calc_beta_div(self, x1, x2):
+        """
+        Definition of the beta-divergence.
+        """
+        if self.beta == 1:
+            log_prod = torch.mul(x1, (x1.add(self.eps).log() - x2.add(self.eps).log()))
+            return (torch.add(torch.sub(log_prod, x1), x2)).mean()
+        elif self.beta == 0:
+            x1_div_x2 = torch.div(x1, x2.add(self.eps)).add(self.eps)
+            return torch.sub(x1_div_x2, x1_div_x2.log()).sub(1).mean()
+        else:
+            if self.beta < 0:
+                x1 = x1.add(self.eps)
+                x2 = x2.add(self.eps)
+            elif self.beta < 1:
+                x2 = x2.add(self.eps)
+            num =  torch.sub(torch.add(x1.pow(self.beta), x2.pow(self.beta).mul(self.beta - 1)), torch.mul(x1, x2.pow(self.beta-1)).mul(self.beta)).mean()
+            return num / (self.beta * (self.beta - 1))
+
+    def forward(self, x, y):
+        """
+        Computation.
+        """
+        if (x < 0).any():
+            raise err.NegativeValuesNotAccepted("Negative values in the input of the network, can't perform beta divergence.")
+        if (y < 0).any():
+            raise err.NegativeValuesNotAccepted("Negative values in the output of the network, can't perform beta divergence.")
+        losses = self.calc_beta_div(x, y)
+        return losses.mean()
```

### Comparing `barmuscomp-0.1.2/barmuscomp/lra.py` & `barmuscomp-0.1.3/barmuscomp/lra.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Feb  4 18:47:32 2022
-
-@author: amarmore
-
-Multilinear (NTD) and Linear (PCA and NMF) barwise compression schemes.
-
-All fused under the term "low-rank approximations".
-
-See [1 - Chapter 4] or [2] for details on NTD, and [1, Chap 5.3] or [3] for details about PCA and NMF.
-
-References
-----------
-[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
-PhD Thesis Marmoret Axel 
-(not uploaded yet but will be soon!)
-(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
-
-[2] Marmoret, A., Cohen, J., Bertin, N., & Bimbot, F. (2020, October). 
-Uncovering Audio Patterns in Music with Nonnegative Tucker Decomposition for Structural Segmentation. 
-In ISMIR 2020-21st International Society for Music Information Retrieval (pp. 1-7).
-
-[3] Marmoret, A., Cohen, J.E, and Bimbot, F., "Barwise Compression Schemes 
-for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, 
-SMC 2022, Sound and music Computing network, 2022.
-"""
-
-import as_seg.barwise_input as bi
-
-import nn_fac.nmf as NMF
-import nn_fac.ntd as NTD
-
-from sklearn.decomposition import PCA
-from sklearn.decomposition import KernelPCA
-import numpy as np
-
-# %% NTD
-def get_ntd_projection(spectrogram, core_dimensions, bars, 
-                       beta = 2, init = "tucker", 
-                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
-    """
-    Return the Q matrix of NTD (barwise projection).
-
-    Parameters
-    ----------
-    spectrogram : list of list of floats or numpy array
-        The spectrogram to analyze, barwise.
-    core_dimensions : list of integers
-        The dimensions for each mode of the core tensor (number of columns for each factor).
-    bars : list of tuples
-        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
-    beta: float
-        The beta parameter for the beta-divergence.
-        Particular cases:
-            2 - Euclidean norm
-            1 - Kullback-Leibler divergence
-            0 - Itakura-Saito divergence
-        Default: 2
-    init: "random" | "tucker" | "chromas" |
-        - If set to random:
-            Initializes with random factors of the correct size.
-            The randomization is the uniform distribution in [0,1),
-            which is the default from numpy random.
-        - If set to tucker:
-            Resolve a tucker decomposition of the tensor T (by HOSVD) and
-            initializes the factors and the core as this resolution, clipped to be nonnegative.
-            The tucker decomposition is performed with tensorly [3].
-        - If set to "chromas":
-            Resolve a tucker decomposition of the tensor T (by HOSVD) and
-            initializes the factors and the core as this resolution, clipped to be nonnegative.
-            The tucker decomposition is performed with tensorly [3].
-            Contrary to "tucker" init, the first factor will then be set to the 12-size identity matrix,
-            because it's a decomposition model specific for modeling music expressed in chromas.
-        Default: tucker
-    subdivision_bars : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    hop_length : integer, optional
-        The hop_length used for the computation of the spectrogram.
-        It is expressed in terms of number of samples, which are defined by the sampling rate.
-        The default is 32.
-    sampling_rate : float, optional
-        Sampling rate used when computing the spectrogram (typically 44100Hz).
-        The default is 44100.
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix, of size (bars, compression_dimension).
-
-    """
-    tensor_spectrogram = bi.tensorize_barwise_FTB(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
-    _, factors = ntd_computation(tensor_spectrogram, core_dimensions, beta, init)
-    return factors[2]
-
-def ntd_computation(tensor_spectrogram, core_dimensions, beta = 2, init = "tucker"):
-    """
-    Computed the NTD on the given tensor_spectrogram.
-
-    Parameters
-    ----------
-    tensor_spectrogram : tensorly tensor
-        The tensor-spectrogram on which should be performed NTD.
-    core_dimensions : list of integers
-        The dimensions for each mode of the core tensor (number of columns for each factor).
-    beta: float
-        The beta parameter for the beta-divergence.
-        Particular cases:
-            2 - Euclidean norm
-            1 - Kullback-Leibler divergence
-            0 - Itakura-Saito divergence
-        Default: 2
-    init: "random" | "tucker" | "chromas" |
-        - If set to random:
-            Initializes with random factors of the correct size.
-            The randomization is the uniform distribution in [0,1),
-            which is the default from numpy random.
-        - If set to tucker:
-            Resolve a tucker decomposition of the tensor T (by HOSVD) and
-            initializes the factors and the core as this resolution, clipped to be nonnegative.
-            The tucker decomposition is performed with tensorly [3].
-        - If set to "chromas":
-            Resolve a tucker decomposition of the tensor T (by HOSVD) and
-            initializes the factors and the core as this resolution, clipped to be nonnegative.
-            The tucker decomposition is performed with tensorly [3].
-            Contrary to "tucker" init, the first factor will then be set to the 12-size identity matrix,
-            because it's a decomposition model specific for modeling music expressed in chromas.
-        Default: tucker
-
-    Returns
-    -------
-    core: tensorly tensor
-        The core tensor linking the factors of the decomposition
-    factors: numpy
-        An array containing all the factors computed with the NTD
-
-    """
-    if beta == 2:
-        core, factors = NTD.ntd(tensor_spectrogram, ranks = core_dimensions, init = init, verbose = False,
-                            sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
-                            deterministic = True)
-    else:
-        core, factors = NTD.ntd_mu(tensor_spectrogram, ranks = core_dimensions, init = init, verbose = False, beta = beta, n_iter_max=1000,
-                            sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
-                            deterministic = True)
-    return core, factors
-
-# %% PCA
-def get_pca_projection(spectrogram, compression_dimension, bars, 
-                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
-    """
-    Returns the PCA projection of this spectrogram.
-
-    Parameters
-    ----------
-    spectrogram : list of list of floats or numpy array
-        The spectrogram to analyze, barwise.
-    compression_dimension : positive integer
-        Dimension of compression (number of principal components to keep).
-    bars : list of tuples
-        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
-    subdivision_bars : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    hop_length : integer, optional
-        The hop_length used for the computation of the spectrogram.
-        It is expressed in terms of number of samples, which are defined by the sampling rate.
-        The default is 32.
-    sampling_rate : float, optional
-        Sampling rate used when computing the spectrogram (typically 44100Hz).
-        The default is 44100.
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix, of size (bars, compression_dimension).
-
-    """
-    barwise_tf_matrix = bi.barwise_TF_matrix(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
-    return pca_projection(barwise_tf_matrix, compression_dimension)
-    
-def pca_projection(barwise_tf_matrix, compression_dimension):
-    """
-    Computes the PCA projection of a Barwise TF matrix 
-    (matrix where one mode is the different bars in the song, 
-     and the other is the vectorization of both the frequency and the time at barscale).
-    
-    The idea is to compress each bar with PCA, summing up the content.
-
-    Parameters
-    ----------
-    barwise_tf_matrix : numpy array
-        Barwise TF matrix.
-    compression_dimension : positive integer
-        Dimension of compression (number of principal components to keep).
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix, of size (bars, compression_dimension).
-
-    """
-    if compression_dimension > barwise_tf_matrix.shape[0]:
-        return pca_projection(barwise_tf_matrix, barwise_tf_matrix.shape[0])
-    pca = PCA(n_components=compression_dimension)
-    pca_spec = pca.fit(barwise_tf_matrix)
-    return pca_spec.transform(barwise_tf_matrix)
-
-def kernel_pca_projection(barwise_tf_matrix, compression_dimension, gamma, kernel='rbf'):
-    """
-    Projection with Kernel PCA instead of PCA (see scikit_learn() documentation).
-    """
-    k_pca = KernelPCA(eigen_solver = 'arpack', n_components=compression_dimension, kernel=kernel, gamma = gamma)
-    return k_pca.fit_transform(barwise_tf_matrix)
-
-# %% NMF
-def get_nmf_projection(spectrogram, compression_dimension, bars, 
-                       beta = 2, init = "nndsvd", 
-                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
-    """
-    Returns the NMF projection of this spectrogram.
-
-    Parameters
-    ----------
-    spectrogram : list of list of floats or numpy array
-        The spectrogram to analyze, barwise.
-    compression_dimension : positive integer
-        Dimension of compression (number of principal components to keep).
-    bars : list of tuples
-        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
-    beta: float
-        The beta parameter for the beta-divergence.
-        Particular cases:
-            2 - Euclidean norm
-            1 - Kullback-Leibler divergence
-            0 - Itakura-Saito divergence
-        Default: 2
-    init: "random" | "nndsvd" |
-        - If set to random:
-            Initialize with random factors of the correct size.
-            The randomization is the uniform distribution in [0,1),
-            which is the default from numpy random.
-        - If set to nnsvd:
-            Corresponds to a Nonnegative Double Singular Value Decomposition
-            (NNDSVD) initialization, which is a data based initialization,
-            designed for NMF. See [2] for details.
-            This NNDSVD if performed via the nimfa toolbox [3].
-        Default: nndsvd
-    subdivision_bars : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    hop_length : integer, optional
-        The hop_length used for the computation of the spectrogram.
-        It is expressed in terms of number of samples, which are defined by the sampling rate.
-        The default is 32.
-    sampling_rate : float, optional
-        Sampling rate used when computing the spectrogram (typically 44100Hz).
-        The default is 44100.
-
-    Returns
-    -------
-    numpy array
-        Compressed matrix, of size (bars, compression_dimension).
-
-    """
-    barwise_tf_matrix = bi.barwise_TF_matrix(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
-    return nmf_computation(barwise_tf_matrix, compression_dimension, beta = beta, init = init)[0]
-
-def nmf_computation(barwise_tf_matrix, compression_dimension, beta = 2, init = "nndsvd"):
-    """
-    Computes the Barwise NMF, on the Barwise TF matrix. Returns only the compressed representations.
-    
-    The idea is to compress each bar with NMF, summing up the content.
-    
-    See nn_fac.nmf() for details.
-
-    Parameters
-    ----------
-    barwise_tf_matrix : numpy array
-        Barwise TF matrix.
-    compression_dimension : positive integer
-        Dimension of compression (number of principal components to keep).
-    beta: float
-        The beta parameter for the beta-divergence.
-        Particular cases:
-            2 - Euclidean norm
-            1 - Kullback-Leibler divergence
-            0 - Itakura-Saito divergence
-        Default: 2
-    init: "random" | "nndsvd" | "custom" |
-        - If set to random:
-            Initialize with random factors of the correct size.
-            The randomization is the uniform distribution in [0,1),
-            which is the default from numpy random.
-        - If set to nnsvd:
-            Corresponds to a Nonnegative Double Singular Value Decomposition
-            (NNDSVD) initialization, which is a data based initialization,
-            designed for NMF. See [2] for details.
-            This NNDSVD if performed via the nimfa toolbox [3].
-        - If set to custom:
-            U_0 and V_0 (see below) will be used for the initialization
-        Default: random
-
-    Returns
-    -------
-    W_nmf : numpy array
-        The barwise compressed representaiton with NMF.
-
-    """
-    if beta == 2:
-        W_nmf, H_nmf = NMF.nmf(barwise_tf_matrix, compression_dimension, update_rule = "hals", beta = 2, init = init, return_costs = False, deterministic = True)
-    else:
-        W_nmf, H_nmf = NMF.nmf(barwise_tf_matrix, compression_dimension, update_rule = "mu", beta = beta, init = init, return_costs = False, deterministic = True)
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Feb  4 18:47:32 2022
+
+@author: amarmore
+
+Multilinear (NTD) and Linear (PCA and NMF) barwise compression schemes.
+
+All fused under the term "low-rank approximations".
+
+See [1 - Chapter 4] or [2] for details on NTD, and [1, Chap 5.3] or [3] for details about PCA and NMF.
+
+References
+----------
+[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
+PhD Thesis Marmoret Axel 
+(not uploaded yet but will be soon!)
+(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
+
+[2] Marmoret, A., Cohen, J., Bertin, N., & Bimbot, F. (2020, October). 
+Uncovering Audio Patterns in Music with Nonnegative Tucker Decomposition for Structural Segmentation. 
+In ISMIR 2020-21st International Society for Music Information Retrieval (pp. 1-7).
+
+[3] Marmoret, A., Cohen, J.E, and Bimbot, F., "Barwise Compression Schemes 
+for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, 
+SMC 2022, Sound and music Computing network, 2022.
+"""
+
+import as_seg.barwise_input as bi
+
+import nn_fac.nmf as NMF
+import nn_fac.ntd as NTD
+
+from sklearn.decomposition import PCA
+from sklearn.decomposition import KernelPCA
+import numpy as np
+
+# %% NTD
+def get_ntd_projection(spectrogram, core_dimensions, bars, 
+                       beta = 2, init = "tucker", 
+                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
+    """
+    Return the Q matrix of NTD (barwise projection).
+
+    Parameters
+    ----------
+    spectrogram : list of list of floats or numpy array
+        The spectrogram to analyze, barwise.
+    core_dimensions : list of integers
+        The dimensions for each mode of the core tensor (number of columns for each factor).
+    bars : list of tuples
+        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
+    beta: float
+        The beta parameter for the beta-divergence.
+        Particular cases:
+            2 - Euclidean norm
+            1 - Kullback-Leibler divergence
+            0 - Itakura-Saito divergence
+        Default: 2
+    init: "random" | "tucker" | "chromas" |
+        - If set to random:
+            Initializes with random factors of the correct size.
+            The randomization is the uniform distribution in [0,1),
+            which is the default from numpy random.
+        - If set to tucker:
+            Resolve a tucker decomposition of the tensor T (by HOSVD) and
+            initializes the factors and the core as this resolution, clipped to be nonnegative.
+            The tucker decomposition is performed with tensorly [3].
+        - If set to "chromas":
+            Resolve a tucker decomposition of the tensor T (by HOSVD) and
+            initializes the factors and the core as this resolution, clipped to be nonnegative.
+            The tucker decomposition is performed with tensorly [3].
+            Contrary to "tucker" init, the first factor will then be set to the 12-size identity matrix,
+            because it's a decomposition model specific for modeling music expressed in chromas.
+        Default: tucker
+    subdivision_bars : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    hop_length : integer, optional
+        The hop_length used for the computation of the spectrogram.
+        It is expressed in terms of number of samples, which are defined by the sampling rate.
+        The default is 32.
+    sampling_rate : float, optional
+        Sampling rate used when computing the spectrogram (typically 44100Hz).
+        The default is 44100.
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix, of size (bars, compression_dimension).
+
+    """
+    tensor_spectrogram = bi.tensorize_barwise_FTB(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
+    _, factors = ntd_computation(tensor_spectrogram, core_dimensions, beta, init)
+    return factors[2]
+
+def ntd_computation(tensor_spectrogram, core_dimensions, beta = 2, init = "tucker"):
+    """
+    Computed the NTD on the given tensor_spectrogram.
+
+    Parameters
+    ----------
+    tensor_spectrogram : tensorly tensor
+        The tensor-spectrogram on which should be performed NTD.
+    core_dimensions : list of integers
+        The dimensions for each mode of the core tensor (number of columns for each factor).
+    beta: float
+        The beta parameter for the beta-divergence.
+        Particular cases:
+            2 - Euclidean norm
+            1 - Kullback-Leibler divergence
+            0 - Itakura-Saito divergence
+        Default: 2
+    init: "random" | "tucker" | "chromas" |
+        - If set to random:
+            Initializes with random factors of the correct size.
+            The randomization is the uniform distribution in [0,1),
+            which is the default from numpy random.
+        - If set to tucker:
+            Resolve a tucker decomposition of the tensor T (by HOSVD) and
+            initializes the factors and the core as this resolution, clipped to be nonnegative.
+            The tucker decomposition is performed with tensorly [3].
+        - If set to "chromas":
+            Resolve a tucker decomposition of the tensor T (by HOSVD) and
+            initializes the factors and the core as this resolution, clipped to be nonnegative.
+            The tucker decomposition is performed with tensorly [3].
+            Contrary to "tucker" init, the first factor will then be set to the 12-size identity matrix,
+            because it's a decomposition model specific for modeling music expressed in chromas.
+        Default: tucker
+
+    Returns
+    -------
+    core: tensorly tensor
+        The core tensor linking the factors of the decomposition
+    factors: numpy
+        An array containing all the factors computed with the NTD
+
+    """
+    if beta == 2:
+        core, factors = NTD.ntd(tensor_spectrogram, ranks = core_dimensions, init = init, verbose = False,
+                            sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
+                            deterministic = True)
+    else:
+        core, factors = NTD.ntd_mu(tensor_spectrogram, ranks = core_dimensions, init = init, verbose = False, beta = beta, n_iter_max=1000,
+                            sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
+                            deterministic = True)
+    return core, factors
+
+# %% PCA
+def get_pca_projection(spectrogram, compression_dimension, bars, 
+                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
+    """
+    Returns the PCA projection of this spectrogram.
+
+    Parameters
+    ----------
+    spectrogram : list of list of floats or numpy array
+        The spectrogram to analyze, barwise.
+    compression_dimension : positive integer
+        Dimension of compression (number of principal components to keep).
+    bars : list of tuples
+        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
+    subdivision_bars : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    hop_length : integer, optional
+        The hop_length used for the computation of the spectrogram.
+        It is expressed in terms of number of samples, which are defined by the sampling rate.
+        The default is 32.
+    sampling_rate : float, optional
+        Sampling rate used when computing the spectrogram (typically 44100Hz).
+        The default is 44100.
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix, of size (bars, compression_dimension).
+
+    """
+    barwise_tf_matrix = bi.barwise_TF_matrix(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
+    return pca_projection(barwise_tf_matrix, compression_dimension)
+    
+def pca_projection(barwise_tf_matrix, compression_dimension):
+    """
+    Computes the PCA projection of a Barwise TF matrix 
+    (matrix where one mode is the different bars in the song, 
+     and the other is the vectorization of both the frequency and the time at barscale).
+    
+    The idea is to compress each bar with PCA, summing up the content.
+
+    Parameters
+    ----------
+    barwise_tf_matrix : numpy array
+        Barwise TF matrix.
+    compression_dimension : positive integer
+        Dimension of compression (number of principal components to keep).
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix, of size (bars, compression_dimension).
+
+    """
+    if compression_dimension > barwise_tf_matrix.shape[0]:
+        return pca_projection(barwise_tf_matrix, barwise_tf_matrix.shape[0])
+    pca = PCA(n_components=compression_dimension)
+    pca_spec = pca.fit(barwise_tf_matrix)
+    return pca_spec.transform(barwise_tf_matrix)
+
+def kernel_pca_projection(barwise_tf_matrix, compression_dimension, gamma, kernel='rbf'):
+    """
+    Projection with Kernel PCA instead of PCA (see scikit_learn() documentation).
+    """
+    k_pca = KernelPCA(eigen_solver = 'arpack', n_components=compression_dimension, kernel=kernel, gamma = gamma)
+    return k_pca.fit_transform(barwise_tf_matrix)
+
+# %% NMF
+def get_nmf_projection(spectrogram, compression_dimension, bars, 
+                       beta = 2, init = "nndsvd", 
+                       subdivision_bars = 96, hop_length = 32, sampling_rate = 44100):
+    """
+    Returns the NMF projection of this spectrogram.
+
+    Parameters
+    ----------
+    spectrogram : list of list of floats or numpy array
+        The spectrogram to analyze, barwise.
+    compression_dimension : positive integer
+        Dimension of compression (number of principal components to keep).
+    bars : list of tuples
+        List of the bars (start, end), in seconds, to cut the spectrogram at bar delimitation.
+    beta: float
+        The beta parameter for the beta-divergence.
+        Particular cases:
+            2 - Euclidean norm
+            1 - Kullback-Leibler divergence
+            0 - Itakura-Saito divergence
+        Default: 2
+    init: "random" | "nndsvd" |
+        - If set to random:
+            Initialize with random factors of the correct size.
+            The randomization is the uniform distribution in [0,1),
+            which is the default from numpy random.
+        - If set to nnsvd:
+            Corresponds to a Nonnegative Double Singular Value Decomposition
+            (NNDSVD) initialization, which is a data based initialization,
+            designed for NMF. See [2] for details.
+            This NNDSVD if performed via the nimfa toolbox [3].
+        Default: nndsvd
+    subdivision_bars : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    hop_length : integer, optional
+        The hop_length used for the computation of the spectrogram.
+        It is expressed in terms of number of samples, which are defined by the sampling rate.
+        The default is 32.
+    sampling_rate : float, optional
+        Sampling rate used when computing the spectrogram (typically 44100Hz).
+        The default is 44100.
+
+    Returns
+    -------
+    numpy array
+        Compressed matrix, of size (bars, compression_dimension).
+
+    """
+    barwise_tf_matrix = bi.barwise_TF_matrix(spectrogram, bars, hop_length/sampling_rate, subdivision_bars)
+    return nmf_computation(barwise_tf_matrix, compression_dimension, beta = beta, init = init)[0]
+
+def nmf_computation(barwise_tf_matrix, compression_dimension, beta = 2, init = "nndsvd"):
+    """
+    Computes the Barwise NMF, on the Barwise TF matrix. Returns only the compressed representations.
+    
+    The idea is to compress each bar with NMF, summing up the content.
+    
+    See nn_fac.nmf() for details.
+
+    Parameters
+    ----------
+    barwise_tf_matrix : numpy array
+        Barwise TF matrix.
+    compression_dimension : positive integer
+        Dimension of compression (number of principal components to keep).
+    beta: float
+        The beta parameter for the beta-divergence.
+        Particular cases:
+            2 - Euclidean norm
+            1 - Kullback-Leibler divergence
+            0 - Itakura-Saito divergence
+        Default: 2
+    init: "random" | "nndsvd" | "custom" |
+        - If set to random:
+            Initialize with random factors of the correct size.
+            The randomization is the uniform distribution in [0,1),
+            which is the default from numpy random.
+        - If set to nnsvd:
+            Corresponds to a Nonnegative Double Singular Value Decomposition
+            (NNDSVD) initialization, which is a data based initialization,
+            designed for NMF. See [2] for details.
+            This NNDSVD if performed via the nimfa toolbox [3].
+        - If set to custom:
+            U_0 and V_0 (see below) will be used for the initialization
+        Default: random
+
+    Returns
+    -------
+    W_nmf : numpy array
+        The barwise compressed representaiton with NMF.
+
+    """
+    if beta == 2:
+        W_nmf, H_nmf = NMF.nmf(barwise_tf_matrix, compression_dimension, update_rule = "hals", beta = 2, init = init, return_costs = False, deterministic = True)
+    else:
+        W_nmf, H_nmf = NMF.nmf(barwise_tf_matrix, compression_dimension, update_rule = "mu", beta = beta, init = init, return_costs = False, deterministic = True)
     return W_nmf, H_nmf
```

### Comparing `barmuscomp-0.1.2/barmuscomp/model/current_plot.py` & `barmuscomp-0.1.3/barmuscomp/model/current_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Feb 22 16:29:17 2019
-
-@author: amarmore
-
-Defining common plotting functions.
-
-NB: This module's name actually comes from an incorrect translation
-from the french "courant" into "current", instead of "common".
-Please excuse me for this translation.
-"""
-
-import as_seg.autosimilarity_computation as as_comp
-
-from sklearn.decomposition import PCA
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.cm as cm
-import pandas as pd
-import IPython.display as ipd
-
-# %% Load everything from as_seg
-from as_seg.model.current_plot import *
-
-# %% NTD specific
-def plot_me_this_tucker(factors, core, cmap = cm.Greys):
-    """
-    Plot all factors, and each slice of the core (as musical pattern) from the NTD.
-    """
-    plot_me_this_spectrogram(factors[0], title = "Midi factor", x_axis = "Atoms", y_axis = "Midi value", invert_y_axis = False, cmap = cmap)
-    plot_me_this_spectrogram(factors[1].T, title = "Rythmic patterns factor", x_axis = "Position in bar", y_axis = "Atoms", cmap = cmap)
-    plot_me_this_spectrogram(factors[2].T, title = "Structural patterns factor", x_axis = "Bar index", y_axis = "Atoms", cmap = cmap)
-    print("Core:")
-    for i in range(len(core[0,0,:])):
-        plot_me_this_spectrogram(core[:,:,i], title = "Core, slice " + str(i), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cmap)
-
-def permutate_factor(factor):
-    """
-    Computes the permutation of columns of the factors for them to be visually more comprehensible.
-    """
-    permutations = []
-    for i in factor:
-        idx_max = np.argmax(i)
-        if idx_max not in permutations:
-            permutations.append(idx_max)
-    for i in range(factor.shape[1]):
-        if i not in permutations:
-            permutations.append(i)
-    return permutations
-
-def plot_permuted_factor(factor, title = None,x_axis = None, y_axis = None, cmap = cm.Greys):
-    """
-    Plots this factor, but permuted to be easier to understand visually.
-    """
-    permut = permutate_factor(factor)
-    plot_me_this_spectrogram(factor.T[permut], title = title,x_axis = x_axis, y_axis = y_axis,
-                             figsize=(factor.shape[0]/10,factor.shape[1]/10), cmap = cmap)
-
-def plot_permuted_tucker(factors, core, cmap = cm.Greys, plot_core = True):
-    """
-    Plots every factor and slice of the core from the NTD, but permuted to be easier to understand visually.
-    """
-    plot_me_this_spectrogram(factors[0], title = "W matrix (muscial content)",
-                         x_axis = "Atoms", y_axis = "Pitch-class Index", cmap = cmap)
-    h_permut = permutate_factor(factors[1])
-    plot_me_this_spectrogram(factors[1].T[h_permut], title = "H matrix: time at barscale (rythmic content)",
-                             x_axis = "Position in the bar\n(in frame indexes)", y_axis = "Atoms\n(permuted for\nvisualization purpose)", 
-                             figsize=(factors[1].shape[0]/10,factors[1].shape[1]/10), cmap = cmap)
-    q_permut = permutate_factor(factors[2])
-    plot_me_this_spectrogram(factors[2].T[q_permut], title = "Q matrix: Bar content feature",
-                             x_axis = "Index of the bar", y_axis = "Musical pattern index\n(permuted for\nvisualization purpose)", 
-                             figsize=(factors[2].shape[0]/10,factors[2].shape[1]/10), cmap = cmap)
-    if plot_core:
-        for i, idx in enumerate(q_permut):
-            plot_me_this_spectrogram(core[:,h_permut,idx], title = "Core, slice {} (slice {} in original decomposition order)".format(i, idx), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cm.Greys)
-  
-
-# %% Plotting audio files, in order to listen to them
-def plot_audio_list_in_dataframe(audios_list):
-    """
-    Print this list of audio signals in a list.
-    """
-    #Never tested, tocheck
-    df = pd.DataFrame(np.array(audios_list), columns = ["All patterns"]).T
-    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-# %% Single-Song AutoEncoders specific
-def plot_latent_space(latent_vectors, labels = None):
-    """
-    Visualization of the latent projection, as the matrix of representation, and as both autosimilarity and PCA of latent vectors.
-
-    Parameters
-    ----------
-    latent_vectors : array
-        Concatenation of the latent vectors, or matrix of latent representations. 
-        (same mathematical meaning but can be of different computation types.)
-    labels : None or array, optional
-        If labels are set, they will be used to color the output of PCA projection.
-        If they are set to None, no label is used. The default is None.
-
-    Returns
-    -------
-    None, but plots latent visualizations.
-
-    """
-    np_lv = np.array(latent_vectors)
-    plot_me_this_spectrogram(np_lv.T, figsize=(np_lv.shape[0]/5,np_lv.shape[1]/5), title = "z matrix", x_axis = "Bar index", y_axis = "Latent space")
-    
-    fig, axs = plt.subplots(1, 2, figsize=(15,7))
-
-    autosimil = as_comp.switch_autosimilarity(latent_vectors, similarity_type = "cosine", normalise = True)
-    padded_autosimil = pad_factor(autosimil)
-    axs[0].pcolormesh(np.arange(padded_autosimil.shape[1]), np.arange(padded_autosimil.shape[0]), padded_autosimil, cmap = cm.Greys)
-    axs[0].set_title('Autosimilarity of the z (projection in latent space)')
-    axs[0].invert_yaxis()
-    axs[0].set_xlabel("Bar index")
-    axs[0].set_ylabel("Bar index")
-    
-    if np_lv.shape[1] == 2:
-        if not isinstance(labels,np.ndarray) and labels == None:
-            axs[1].scatter(np_lv[:,0],np_lv[:,1])
-        else:
-            axs[1].scatter(np_lv[:,0],np_lv[:,1], c=labels)
-    else:
-        pca = PCA(n_components=2)
-        principalComponents = pca.fit_transform(np_lv)
-        if not isinstance(labels,np.ndarray) and labels == None:
-            axs[1].scatter(principalComponents[:,0],principalComponents[:,1])
-        else:
-            axs[1].scatter(principalComponents[:,0],principalComponents[:,1], c=labels)
-
-    axs[1].set_title('PCA of the z (projection in the latent space)')
-    plt.show()
-
-# %% AE-NTD
-def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
-    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-    import pandas as pd
-import IPython.display as ipd
-
-def plot_audio_diff_beta_in_dataframe(signal_beta2, signal_beta1, signal_beta0):
-    """
-    Plots the different reconstruction with different beta values in a dataframe.
-    Hardcoded for Beta = 2, 1 and 0.
-    """
-    df = pd.DataFrame(np.array([signal_beta2, signal_beta1, signal_beta0]), index = ["beta = 2", "beta = 1", "beta = 0"])
-    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Feb 22 16:29:17 2019
+
+@author: amarmore
+
+Defining common plotting functions.
+
+NB: This module's name actually comes from an incorrect translation
+from the french "courant" into "current", instead of "common".
+Please excuse me for this translation.
+"""
+
+import as_seg.autosimilarity_computation as as_comp
+
+from sklearn.decomposition import PCA
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib.cm as cm
+import pandas as pd
+import IPython.display as ipd
+
+# %% Load everything from as_seg
+from as_seg.model.current_plot import *
+
+# %% NTD specific
+def plot_me_this_tucker(factors, core, cmap = cm.Greys):
+    """
+    Plot all factors, and each slice of the core (as musical pattern) from the NTD.
+    """
+    plot_me_this_spectrogram(factors[0], title = "Midi factor", x_axis = "Atoms", y_axis = "Midi value", invert_y_axis = False, cmap = cmap)
+    plot_me_this_spectrogram(factors[1].T, title = "Rythmic patterns factor", x_axis = "Position in bar", y_axis = "Atoms", cmap = cmap)
+    plot_me_this_spectrogram(factors[2].T, title = "Structural patterns factor", x_axis = "Bar index", y_axis = "Atoms", cmap = cmap)
+    print("Core:")
+    for i in range(len(core[0,0,:])):
+        plot_me_this_spectrogram(core[:,:,i], title = "Core, slice " + str(i), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cmap)
+
+def permutate_factor(factor):
+    """
+    Computes the permutation of columns of the factors for them to be visually more comprehensible.
+    """
+    permutations = []
+    for i in factor:
+        idx_max = np.argmax(i)
+        if idx_max not in permutations:
+            permutations.append(idx_max)
+    for i in range(factor.shape[1]):
+        if i not in permutations:
+            permutations.append(i)
+    return permutations
+
+def plot_permuted_factor(factor, title = None,x_axis = None, y_axis = None, cmap = cm.Greys):
+    """
+    Plots this factor, but permuted to be easier to understand visually.
+    """
+    permut = permutate_factor(factor)
+    plot_me_this_spectrogram(factor.T[permut], title = title,x_axis = x_axis, y_axis = y_axis,
+                             figsize=(factor.shape[0]/10,factor.shape[1]/10), cmap = cmap)
+
+def plot_permuted_tucker(factors, core, cmap = cm.Greys, plot_core = True):
+    """
+    Plots every factor and slice of the core from the NTD, but permuted to be easier to understand visually.
+    """
+    plot_me_this_spectrogram(factors[0], title = "W matrix (muscial content)",
+                         x_axis = "Atoms", y_axis = "Pitch-class Index", cmap = cmap)
+    h_permut = permutate_factor(factors[1])
+    plot_me_this_spectrogram(factors[1].T[h_permut], title = "H matrix: time at barscale (rythmic content)",
+                             x_axis = "Position in the bar\n(in frame indexes)", y_axis = "Atoms\n(permuted for\nvisualization purpose)", 
+                             figsize=(factors[1].shape[0]/10,factors[1].shape[1]/10), cmap = cmap)
+    q_permut = permutate_factor(factors[2])
+    plot_me_this_spectrogram(factors[2].T[q_permut], title = "Q matrix: Bar content feature",
+                             x_axis = "Index of the bar", y_axis = "Musical pattern index\n(permuted for\nvisualization purpose)", 
+                             figsize=(factors[2].shape[0]/10,factors[2].shape[1]/10), cmap = cmap)
+    if plot_core:
+        for i, idx in enumerate(q_permut):
+            plot_me_this_spectrogram(core[:,h_permut,idx], title = "Core, slice {} (slice {} in original decomposition order)".format(i, idx), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cm.Greys)
+  
+
+# %% Plotting audio files, in order to listen to them
+def plot_audio_list_in_dataframe(audios_list):
+    """
+    Print this list of audio signals in a list.
+    """
+    #Never tested, tocheck
+    df = pd.DataFrame(np.array(audios_list), columns = ["All patterns"]).T
+    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+# %% Single-Song AutoEncoders specific
+def plot_latent_space(latent_vectors, labels = None):
+    """
+    Visualization of the latent projection, as the matrix of representation, and as both autosimilarity and PCA of latent vectors.
+
+    Parameters
+    ----------
+    latent_vectors : array
+        Concatenation of the latent vectors, or matrix of latent representations. 
+        (same mathematical meaning but can be of different computation types.)
+    labels : None or array, optional
+        If labels are set, they will be used to color the output of PCA projection.
+        If they are set to None, no label is used. The default is None.
+
+    Returns
+    -------
+    None, but plots latent visualizations.
+
+    """
+    np_lv = np.array(latent_vectors)
+    plot_me_this_spectrogram(np_lv.T, figsize=(np_lv.shape[0]/5,np_lv.shape[1]/5), title = "z matrix", x_axis = "Bar index", y_axis = "Latent space")
+    
+    fig, axs = plt.subplots(1, 2, figsize=(15,7))
+
+    autosimil = as_comp.switch_autosimilarity(latent_vectors, similarity_type = "cosine", normalise = True)
+    padded_autosimil = pad_factor(autosimil)
+    axs[0].pcolormesh(np.arange(padded_autosimil.shape[1]), np.arange(padded_autosimil.shape[0]), padded_autosimil, cmap = cm.Greys)
+    axs[0].set_title('Autosimilarity of the z (projection in latent space)')
+    axs[0].invert_yaxis()
+    axs[0].set_xlabel("Bar index")
+    axs[0].set_ylabel("Bar index")
+    
+    if np_lv.shape[1] == 2:
+        if not isinstance(labels,np.ndarray) and labels == None:
+            axs[1].scatter(np_lv[:,0],np_lv[:,1])
+        else:
+            axs[1].scatter(np_lv[:,0],np_lv[:,1], c=labels)
+    else:
+        pca = PCA(n_components=2)
+        principalComponents = pca.fit_transform(np_lv)
+        if not isinstance(labels,np.ndarray) and labels == None:
+            axs[1].scatter(principalComponents[:,0],principalComponents[:,1])
+        else:
+            axs[1].scatter(principalComponents[:,0],principalComponents[:,1], c=labels)
+
+    axs[1].set_title('PCA of the z (projection in the latent space)')
+    plt.show()
+
+# %% AE-NTD
+def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
+    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+import pandas as pd
+import IPython.display as ipd
+
+def plot_audio_diff_beta_in_dataframe(signal_beta2, signal_beta1, signal_beta0):
+    """
+    Plots the different reconstruction with different beta values in a dataframe.
+    Hardcoded for Beta = 2, 1 and 0.
+    """
+    df = pd.DataFrame(np.array([signal_beta2, signal_beta1, signal_beta0]), index = ["beta = 2", "beta = 1", "beta = 0"])
+    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+
+
```

### Comparing `barmuscomp-0.1.2/barmuscomp/model/early_stopping.py` & `barmuscomp-0.1.3/barmuscomp/model/early_stopping.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.2/barmuscomp/model/features.py` & `barmuscomp-0.1.3/barmuscomp/model/features.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 25 16:54:59 2020
-
-@author: amarmore
-"""
-
-import barmuscomp.model.errors as err
-
-# %% Load everything from as_seg
-from as_seg.model.features import *
-# See details in as_seg
-
-# %% HCQT
-def get_hcqt_params():
-    """
-    Credit to & al. [1] (comes directly from https://github.com/rabitt/ismir2017-deepsalience)
-    
-    Fixing parameters for the HCQT computation.
-
-    Returns
-    -------
-    bins_per_octave : TYPE
-        DESCRIPTION.
-    n_octaves : TYPE
-        DESCRIPTION.
-    harmonics : TYPE
-        DESCRIPTION.
-    sr : TYPE
-        DESCRIPTION.
-    fmin : TYPE
-        DESCRIPTION.
-    hop_length : TYPE
-        DESCRIPTION.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-
-    """
-    bins_per_octave = 60
-    n_octaves = 6
-    harmonics = [0.5, 1, 2, 3, 4, 5]
-    sr = 22050
-    fmin = 32.7
-    hop_length = 256
-    return bins_per_octave, n_octaves, harmonics, sr, fmin, hop_length
-
-
-def compute_hcqt_bittner(signal, sr):
-    """
-    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
-    
-    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
-
-    Parameters
-    ----------
-    signal : numpy array
-        Signal of the song.
-    sr : int
-        the sampling_rate
-
-    Returns
-    -------
-    log_hcqt : np array
-        The tensor of logarithm HCQT.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-    """
-    (bins_per_octave, n_octaves, harmonics,
-     sr, f_min, hop_length) = get_hcqt_params()
-    #y, fs = librosa.load(audio_fpath, sr=sr)
-
-    cqt_list = []
-    shapes = []
-    for h in harmonics:
-        cqt = librosa.cqt(
-            signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
-            n_bins=bins_per_octave*n_octaves,
-            bins_per_octave=bins_per_octave
-        )
-        cqt_list.append(cqt)
-        shapes.append(cqt.shape)
-
-    shapes_equal = [s == shapes[0] for s in shapes]
-    if not all(shapes_equal):
-        min_time = np.min([s[1] for s in shapes])
-        new_cqt_list = []
-        for i in range(len(cqt_list)):
-            new_cqt_list.append(cqt_list[i][:, :min_time])
-        cqt_list = new_cqt_list
-
-    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(
-        np.abs(np.array(cqt_list)), ref=np.max)) + 1.0
-
-    return log_hcqt
-
-def my_compute_hcqt(signal, sr):
-    """
-    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
-    
-    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
-    The order of the mode is changed though, so tht first two modes correspond to frequency and time respectively,
-    and that the third corresponds to harmonic content.
-
-    Parameters
-    ----------
-    signal : numpy array
-        Signal of the song.
-    sr : int
-        the sampling_rate
-
-    Returns
-    -------
-    log_hcqt : np array
-        The tensor of logarithm HCQT.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-    """
-    (bins_per_octave, n_octaves, harmonics, sr, f_min, hop_length) = get_hcqt_params()
-
-    freq_mode_len = bins_per_octave*n_octaves
-
-    first_cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(harmonics[0]),
-                            n_bins=freq_mode_len, bins_per_octave=bins_per_octave)
-
-    time_mode_len = first_cqt.shape[1]
-    
-    h_cqt = np.array(first_cqt).reshape(freq_mode_len, time_mode_len, 1)
-    
-    for h in harmonics[1:]:
-        cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
-            n_bins=bins_per_octave*n_octaves,bins_per_octave=bins_per_octave)
-        current_cqt = cqt.reshape(freq_mode_len, time_mode_len, 1)
-        h_cqt = np.append(h_cqt, current_cqt, axis = 2)
-
-    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(np.abs(h_cqt), ref=np.max)) + 1.0
-
-    return log_hcqt
-
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Mar 25 16:54:59 2020
+
+@author: amarmore
+"""
+
+import barmuscomp.model.errors as err
+
+# %% Load everything from as_seg
+from as_seg.model.features import *
+# See details in as_seg
+
+# %% HCQT
+def get_hcqt_params():
+    """
+    Credit to & al. [1] (comes directly from https://github.com/rabitt/ismir2017-deepsalience)
+    
+    Fixing parameters for the HCQT computation.
+
+    Returns
+    -------
+    bins_per_octave : TYPE
+        DESCRIPTION.
+    n_octaves : TYPE
+        DESCRIPTION.
+    harmonics : TYPE
+        DESCRIPTION.
+    sr : TYPE
+        DESCRIPTION.
+    fmin : TYPE
+        DESCRIPTION.
+    hop_length : TYPE
+        DESCRIPTION.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+
+    """
+    bins_per_octave = 60
+    n_octaves = 6
+    harmonics = [0.5, 1, 2, 3, 4, 5]
+    sr = 22050
+    fmin = 32.7
+    hop_length = 256
+    return bins_per_octave, n_octaves, harmonics, sr, fmin, hop_length
+
+
+def compute_hcqt_bittner(signal, sr):
+    """
+    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
+    
+    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
+
+    Parameters
+    ----------
+    signal : numpy array
+        Signal of the song.
+    sr : int
+        the sampling_rate
+
+    Returns
+    -------
+    log_hcqt : np array
+        The tensor of logarithm HCQT.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+    """
+    (bins_per_octave, n_octaves, harmonics,
+     sr, f_min, hop_length) = get_hcqt_params()
+    #y, fs = librosa.load(audio_fpath, sr=sr)
+
+    cqt_list = []
+    shapes = []
+    for h in harmonics:
+        cqt = librosa.cqt(
+            signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
+            n_bins=bins_per_octave*n_octaves,
+            bins_per_octave=bins_per_octave
+        )
+        cqt_list.append(cqt)
+        shapes.append(cqt.shape)
+
+    shapes_equal = [s == shapes[0] for s in shapes]
+    if not all(shapes_equal):
+        min_time = np.min([s[1] for s in shapes])
+        new_cqt_list = []
+        for i in range(len(cqt_list)):
+            new_cqt_list.append(cqt_list[i][:, :min_time])
+        cqt_list = new_cqt_list
+
+    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(
+        np.abs(np.array(cqt_list)), ref=np.max)) + 1.0
+
+    return log_hcqt
+
+def my_compute_hcqt(signal, sr):
+    """
+    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
+    
+    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
+    The order of the mode is changed though, so tht first two modes correspond to frequency and time respectively,
+    and that the third corresponds to harmonic content.
+
+    Parameters
+    ----------
+    signal : numpy array
+        Signal of the song.
+    sr : int
+        the sampling_rate
+
+    Returns
+    -------
+    log_hcqt : np array
+        The tensor of logarithm HCQT.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+    """
+    (bins_per_octave, n_octaves, harmonics, sr, f_min, hop_length) = get_hcqt_params()
+
+    freq_mode_len = bins_per_octave*n_octaves
+
+    first_cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(harmonics[0]),
+                            n_bins=freq_mode_len, bins_per_octave=bins_per_octave)
+
+    time_mode_len = first_cqt.shape[1]
+    
+    h_cqt = np.array(first_cqt).reshape(freq_mode_len, time_mode_len, 1)
+    
+    for h in harmonics[1:]:
+        cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
+            n_bins=bins_per_octave*n_octaves,bins_per_octave=bins_per_octave)
+        current_cqt = cqt.reshape(freq_mode_len, time_mode_len, 1)
+        h_cqt = np.append(h_cqt, current_cqt, axis = 2)
+
+    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(np.abs(h_cqt), ref=np.max)) + 1.0
+
+    return log_hcqt
+
```

### Comparing `barmuscomp-0.1.2/barmuscomp/model/pattern_study.py` & `barmuscomp-0.1.3/barmuscomp/model/pattern_study.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,450 +1,450 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Jul 26 15:38:26 2022
-
-@author: amarmore
-
-Set of functions dedicated to the qualitative study of patterns in a song.
-
-In a nutshell, the idea is to:
-     - Compute patterns as WG_[::i]H (a musical pattern)
-     - Reconstruct them in audio signals
-     - Listening to these signals and estimating the assocated quality with SDR
-
-Details can be found in [1, Chapter 4.5.2 and 6.4.4], 
-and applications at https://ax-le.github.io/resources/examples/ListeningNTD.html.
-
-IDEAS:
-    - Initialize Griffin-Lim with the original phase.
-
-References
-----------
-[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
-PhD Thesis Marmoret Axel 
-(not uploaded yet but will be soon!)
-(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
-"""
-
-import barmuscomp.model.errors as err
-
-import librosa
-import mir_eval
-import numpy as np
-import IPython.display as ipd
-import warnings
-import tensorly as tl
-
-def get_median_hop(bars, subdivision = 96, sampling_rate = 44100):
-    """
-    Returns the median hop length in the song, used for audio reconstruction.
-    The rationale is that all bars are sampled with 'subdivision' number of frames, 
-    but they can be of different lengths in absolute time.
-    Hence, the time gap between two consecutive frames (the hop length) can differ between bars.
-    For reconstruction, we use the median hop length among all bars.
-
-    Parameters
-    ----------
-    bars : list of tuples of float
-        The bars, as (start time, end time) tuples.
-    subdivision : integer, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-        The default is 96.
-    sampling_rate : integer, optional
-        The sampling rate of the signal, in Hz.
-        The default is 44100.
-
-    Returns
-    -------
-    integer
-        The median hop length in these bars.
-
-    """
-    hops = []
-    for bar_idx in range(1, len(bars)):
-        len_sig = bars[bar_idx][1] - bars[bar_idx][0]
-        hop = int(len_sig/subdivision * sampling_rate)
-        hops.append(hop)
-    return int(np.median(hops)) #For audio reconstruction
-
-def encapsulate_sdr_computation(audio_ref, audio_estimate):
-    """
-    Function encapsulating the SDR computation in mir_eval.
-    SDR is computed between 'audio_ref' and 'audio_estimate'.
-    """
-    if (audio_estimate == 0).all():
-        return -np.inf
-    return mir_eval.separation.bss_eval_sources(np.array([audio_ref]), np.array([audio_estimate]))[0][0]
-
-def compute_patterns(core, W, H):
-    """
-    Compute the list of musical patterns, given factors G (core tensor), W and H.
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    W : numpy array
-        W matrix factor.
-    H : numpy array
-        H matrix factor..
-
-    Returns
-    -------
-    pattern_list : list of 2D numpy arrays
-        The list of patterns.
-
-    """
-    pattern_list = []
-    for pat_idx in range(core.shape[2]):
-        pattern_list.append(W@core[:,:,pat_idx]@H.T) 
-    return pattern_list
-    # pat_computed = tl.tenalg.multi_mode_dot(core, [W, H], modes=[0,1], skip=None, transpose=False)
-    # reordered = np.moveaxis(pat_computed, -1, 0)
-    # return reordered
-
-def sdr_songscale_patternscale_encpasulation(core, factors, hop_length, tensor_mag_original, tensor_phase_original,
-                                             pattern_list = None, phase_retrieval_song = "original_phase", phase_retrieval_patterns = "original_phase", sampling_rate = 44100):
-    """
-    Computes the SDR for the entire song and for all patterns, 
-    as defined in [1, Chapter 4.5.2] (see References, top of this file).   
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    factors : list of numpy arrays
-        The matrix factors of NTD.
-    hop_length : integer
-        Number of samples between two consecutive time frames.
-    tensor_mag_original : 3D numpy array
-        Magnitude of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    tensor_phase_original : 3D numpy array
-        Phase of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    pattern_list : list of 2D numpy arrays, optional
-        The list of patterns, if already computed
-        (avoid to recompute them again, for time saving).
-    phase_retrieval_song : string, optional
-        Specifies the type of phase retrieval which should be used for 
-        reconstructing the signal of at the songscale.
-        Possible types are:
-            - "original_phase", which uses the original phase of the tensor as phase information,
-            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
-        The default is "string".
-    phase_retrieval_patterns : string, optional
-        Specifies the type of phase retrieval which should be used for 
-        reconstructing the signal of each pattern.
-        Possible types are:
-            - "original_phase", which uses the original phase of the tensor as phase information,
-            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
-            - "softmasking", which uses Weiner filtering-like operation, detailed in [1].
-        The default is "original_phase".
-    sampling_rate : integer, optional
-        The sampling rate of the signal, in Hz.
-        The default is 44100.
-
-    Returns
-    -------
-    song_sdr : float
-        The SDR at the song scale.
-    patterns_sdr : list of float
-        The SDR for each pattern.
-    audio_songscale : IPython.display audio
-        The audio signal of the song, reconstructed from NTD
-        (the one the SDR was computed on).
-    audio_patterns : list of IPython.display
-        The audio signal of all patterns, reconstructed from NTD
-        (the one the SDRs were computed on).
-    """
-    if pattern_list is None:
-        pattern_list = compute_patterns(core, factors[0], factors[1])
-    
-    audio_songscale, song_sdr = songscale_audio_sdr(core, factors, hop_length, 
-                                                    tensor_mag_original = tensor_mag_original,
-                                                    tensor_phase_original = tensor_phase_original, 
-                                                    pattern_list = pattern_list, 
-                                                    phase_retrieval = phase_retrieval_song, 
-                                                    sampling_rate = sampling_rate)
-    
-    audio_patterns, patterns_sdr = patternscale_audio_sdr(core, factors[2], 
-                                                          pattern_list, hop_length = hop_length, 
-                                                          tensor_mag_original = tensor_mag_original,
-                                                          tensor_phase_original = tensor_phase_original,
-                                                          phase_retrieval = phase_retrieval_patterns,
-                                                          sampling_rate = sampling_rate)
-    
-    return song_sdr, patterns_sdr, audio_songscale, audio_patterns
-
-def songscale_audio_sdr(core, factors, hop_length, tensor_mag_original, tensor_phase_original, pattern_list = None, phase_retrieval = "original_phase", sampling_rate = 44100):
-    """
-    Computes the SDR for the entire song, 
-    as defined in [1, Chapter 4.5.2] (see References, top of this file).   
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    factors : list of numpy arrays
-        The matrix factors of NTD.
-    hop_length : integer
-        Number of samples between two consecutive time frames.
-    tensor_mag_original : 3D numpy array
-        Magnitude of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    tensor_phase_original : 3D numpy array
-        Phase of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    pattern_list : list of 2D numpy arrays, optional
-        The list of patterns, if already computed
-        (avoid to recompute them again, for time saving).
-    phase_retrieval : string, optional
-        Specifies the type of phase retrieval which should be used for 
-        reconstructing the signal of at the songscale.
-        Possible types are:
-            - "original_phase", which uses the original phase of the tensor as phase information,
-            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
-        The default is "string".
-    sampling_rate : integer, optional
-        The sampling rate of the signal, in Hz.
-        The default is 44100.
-
-    Returns
-    -------
-    audio_reconstructed : IPython.display
-        The audio signal of the song, reconstructed from NTD
-        (the one the SDR was computed on).
-    song_sdr : float
-        The SDR at the song scale.
-    """
-    if pattern_list is None:
-        pattern_list = compute_patterns(core, factors[0], factors[1])
-    
-    signal_reconstructed = reconstruct_song_from_factors(core, factors, hop_length, nb_bars = None, pattern_list = pattern_list, phase_retrieval = phase_retrieval, tensor_phase_original = tensor_phase_original)    
-    original_song_signal_istft = librosa.istft(np.reshape((tensor_mag_original*tensor_phase_original), (tensor_mag_original.shape[0], tensor_mag_original.shape[1] * tensor_mag_original.shape[2]), order = 'F'), hop_length = hop_length)
-    song_sdr = encapsulate_sdr_computation(original_song_signal_istft, signal_reconstructed)
-    
-    audio_reconstructed = ipd.Audio(signal_reconstructed, rate=sampling_rate)
-    
-    return audio_reconstructed, song_sdr
-
-def reconstruct_song_from_factors(core, factors, hop_length, nb_bars = None, pattern_list = None, phase_retrieval = "griffin_lim", tensor_phase_original = None):
-    """
-    Reconstructing the entire song as an audio signal.
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    factors : list of numpy arrays
-        The matrix factors of NTD.
-    hop_length : integer
-        Number of samples between two consecutive time frames.
-    nb_bars : positive integer, optional
-        Number of bars for reconstructing the song. 
-        The default is None, i.e. all bars in the song.
-        (May be useful for large songs or fewer computational complexity)
-    pattern_list : list of 2D numpy arrays, optional
-        The list of patterns, if already computed
-        (avoid to recompute them again, for time saving).
-    phase_retrieval : string, optional
-        Specifies the type of phase retrieval which should be used for 
-        reconstructing the signal of at the songscale.
-        Possible types are:
-            - "original_phase", which uses the original phase of the tensor as phase information,
-            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
-        The default is "string".
-    tensor_phase_original : 3D numpy array, optional
-        Phase of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-        Necesary for original_phase only (not used for Griffin-Lim).
-        Can be set to None if not not necessary.
-
-    Raises
-    ------
-    err.InvalidArgumentValueException
-        If the phase retrieval method is unknown.
-
-    Returns
-    -------
-    audio signal (numpy array)
-        The audio signal (as an array).
-
-    """
-    if pattern_list is None:
-        pattern_list = compute_patterns(core, factors[0], factors[1])
-    spectrogram_list_contribs = contribution_song_each_pattern(core, factors[2], pattern_list, nb_bars)
-    spectrogram_content = np.sum(spectrogram_list_contribs, axis = 0)
-    if phase_retrieval == "griffin_lim":
-        return librosa.griffinlim(spectrogram_content, hop_length = hop_length, random_state = 0)
-    elif phase_retrieval == "original_phase":
-        assert tensor_phase_original is not None
-        spectrogram_to_inverse = spectrogram_content * np.reshape(tensor_phase_original[:,:,:nb_bars], spectrogram_content.shape, order = 'F')
-        return librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
-    else:
-        raise err.InvalidArgumentValueException("Phase retrieval method not understood.")
-        
-def contribution_song_each_pattern(core, Q, pattern_list, nb_bars = None):
-    """
-    Computes the contribution to the song of each pattern, as spectrograms
-    (i.e. the exact spectrogram stemming from each pattern, 
-     weighted by its contribution in Q matrix).
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    Q : numpy array
-        The Q matrix factor.
-    pattern_list : list of 2D numpy arrays
-        The list of patterns.
-    nb_bars : positive integer, optional
-        Number of bars for reconstructing the song. 
-        The default is None, i.e. all bars in the song.
-        (May be useful for large songs or fewer computational complexity)
-
-    Returns
-    -------
-    list_contribs : list of 2D numpy arrays
-        The list of spectrogram for each pattern.
-
-    """
-    if nb_bars == None:
-        nb_bars = Q.shape[0]
-    list_contribs = []
-    for pat_idx in range(Q.shape[1]):
-        spectrogram_content = None
-        for bar_idx in range(nb_bars):
-            bar_content = Q[bar_idx, pat_idx] * pattern_list[pat_idx]
-            bar_content = np.where(bar_content > 1e-8, bar_content, 0)
-            spectrogram_content = np.concatenate((spectrogram_content, bar_content), axis=1) if spectrogram_content is not None else bar_content
-        list_contribs.append(spectrogram_content)
-    return list_contribs
-        
-def patternscale_audio_sdr(core, Q, pattern_list, hop_length, tensor_mag_original, tensor_phase_original, phase_retrieval = "griffin_lim", sampling_rate = 44100):
-    """
-    Studies all patterns, as SDR and as audio signals, to listen to them.
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    Q : numpy array
-        The Q matrix factor.
-    pattern_list : list of 2D numpy arrays
-        The list of patterns.
-    hop_length : integer
-        Number of samples between two consecutive time frames.
-    tensor_mag_original : 3D numpy array
-        Magnitude of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    tensor_phase_original : 3D numpy array
-        Phase of the barwise spectrograms (3D).
-        The order is BFT (Indexes of bars, Frequency, Time at barscale).
-    phase_retrieval : string, optional
-        Specifies the type of phase retrieval which should be used for 
-        reconstructing the signal of each pattern.
-        Possible types are:
-            - "original_phase", which uses the original phase of the tensor as phase information,
-            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
-            - "softmasking", which uses Weiner filtering-like operation, detailed in [1].
-        The default is "original_phase".
-    sampling_rate : integer, optional
-        The sampling rate of the signal, in Hz.
-        The default is 44100.
-
-    Raises
-    ------
-    err
-        Wrong argument or abnormal behavior.
-
-    Returns
-    -------
-    list of IPython.display
-        The audio signal of the each pattern, reconstructed from NTD
-        (the ones SDR are computed on).
-    list of floats
-        The SDR of all patterns.
-        
-    """
-    best_choice_bar = [] # Local variable, to know which bar is to be considered for this particular pattern
-    audios_list = [] # To be returned
-    signal_list = [] # To be returned
-    sdr_list = [] # To be returned
-        
-    for current_pattern_idx in range(Q.shape[1]):
-        bar_original = select_associated_bar(core, Q, pattern_list, current_pattern_idx)
-        signal_baseline_bar = librosa.istft(np.reshape((tensor_mag_original*tensor_phase_original)[:,:,bar_original], (tensor_mag_original.shape[0], tensor_mag_original.shape[1]), order = 'F'), hop_length = hop_length)
-        
-        if phase_retrieval == "griffin_lim":
-            signal_audio = librosa.griffinlim(pattern_list[current_pattern_idx], hop_length = hop_length, random_state = 0)
-           
-        elif phase_retrieval == "original_phase":
-            spectrogram_to_inverse = tensor_phase_original[:,:,bar_original] * pattern_list[current_pattern_idx]
-            signal_audio = librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
-            
-        elif phase_retrieval in ["masking", "softmasking"]:
-            if phase_retrieval == "masking":
-                warnings.warn("'masking' is deprecated, you should use 'softmasking' instead.")
-            assert tensor_mag_original is not None
-            assert tensor_phase_original is not None
-            if Q[bar_original, current_pattern_idx] != 0:
-                pattern = Q[bar_original, current_pattern_idx] * pattern_list[current_pattern_idx]  # Numerator of masking
-                pattern = 1e6 * np.where(pattern > 1e-8, pattern, 0) # Very low values lead to undeterminism in the divide.
-
-                bar_content_patternwise = np.zeros(pattern.shape)
-                for pat_idx_loop in range(Q.shape[1]):
-                    bar_content_patternwise += Q[bar_original, pat_idx_loop] * pattern_list[pat_idx_loop] # Denominator of masking
-                bar_content_patternwise = 1e6 * np.where(bar_content_patternwise > 1e-8, bar_content_patternwise, 0) # Very low values lead to undeterminism in the divide.
-
-                mask = np.divide(pattern, bar_content_patternwise, where=bar_content_patternwise != 0)  # if bar_content_patternwise == 0, pattern also equals 0.
-                    
-                spectrogram_to_inverse = tensor_phase_original[:,:,bar_original] * tensor_mag_original[:,:,bar_original] * mask # Masked content                  
-                signal_audio = librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
-                if np.mean(mask) > 0.99: # Mask too close to original
-                    warnings.warn(f"The current masked spectrogram is too close to the ogirinal spectrogram, the SDR would be disinformative.")
-                    continue
-
-            else:
-                warnings.warn(f"The {current_pattern_idx}-th pattern is never used in the $Q$ matrix.")
-                continue
-        else:
-            raise err.InvalidArgumentValueException("Phase retrieval method not understood.")
-        signal_list.append(signal_audio)
-        audios_list.append(ipd.Audio(signal_audio, rate=sampling_rate))
-        sdr_list.append(encapsulate_sdr_computation(signal_baseline_bar, signal_audio))
-    
-    if signal_list == []:
-        raise err.AbnormalBehaviorException("No signal was computed, which should be considered a problem.")
-
-    return audios_list, np.ma.masked_invalid(sdr_list)
-
-def select_associated_bar(core, Q, pattern_list, pat_idx):
-    """
-    Method selecting the associated bar (the most similar) for a particular pattern.
-    For now, only a simple strategy is computed (the bar which has the maximal value in Q),
-    but additional strategies can be found in [2].
-
-    Parameters
-    ----------
-    core : numpy array
-        The core tensor.
-    Q : numpy array
-        The Q matrix factor.
-    pattern_list : list of 2D numpy arrays
-        The list of patterns.
-    pat_idx : integer
-        The index of the current pattern.
-
-    Returns
-    -------
-    integer
-        Index of the associated bar in the song.
-        
-    References
-    ----------
-    [2] Smith, J. B., Kawasaki, Y., & Goto, M. (2019). Unmixer: An Interface for 
-    Extracting and Remixing Loops. In ISMIR (pp. 824-831).
-
-    """
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Jul 26 15:38:26 2022
+
+@author: amarmore
+
+Set of functions dedicated to the qualitative study of patterns in a song.
+
+In a nutshell, the idea is to:
+     - Compute patterns as WG_[::i]H (a musical pattern)
+     - Reconstruct them in audio signals
+     - Listening to these signals and estimating the assocated quality with SDR
+
+Details can be found in [1, Chapter 4.5.2 and 6.4.4], 
+and applications at https://ax-le.github.io/resources/examples/ListeningNTD.html.
+
+IDEAS:
+    - Initialize Griffin-Lim with the original phase.
+
+References
+----------
+[1] Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure, 
+PhD Thesis Marmoret Axel 
+(not uploaded yet but will be soon!)
+(You should check the website hal.archives-ouvertes.fr/ in case this docstring is not updated with the reference.)
+"""
+
+import barmuscomp.model.errors as err
+
+import librosa
+import mir_eval
+import numpy as np
+import IPython.display as ipd
+import warnings
+import tensorly as tl
+
+def get_median_hop(bars, subdivision = 96, sampling_rate = 44100):
+    """
+    Returns the median hop length in the song, used for audio reconstruction.
+    The rationale is that all bars are sampled with 'subdivision' number of frames, 
+    but they can be of different lengths in absolute time.
+    Hence, the time gap between two consecutive frames (the hop length) can differ between bars.
+    For reconstruction, we use the median hop length among all bars.
+
+    Parameters
+    ----------
+    bars : list of tuples of float
+        The bars, as (start time, end time) tuples.
+    subdivision : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    sampling_rate : integer, optional
+        The sampling rate of the signal, in Hz.
+        The default is 44100.
+
+    Returns
+    -------
+    integer
+        The median hop length in these bars.
+
+    """
+    hops = []
+    for bar_idx in range(1, len(bars)):
+        len_sig = bars[bar_idx][1] - bars[bar_idx][0]
+        hop = int(len_sig/subdivision * sampling_rate)
+        hops.append(hop)
+    return int(np.median(hops)) #For audio reconstruction
+
+def encapsulate_sdr_computation(audio_ref, audio_estimate):
+    """
+    Function encapsulating the SDR computation in mir_eval.
+    SDR is computed between 'audio_ref' and 'audio_estimate'.
+    """
+    if (audio_estimate == 0).all():
+        return -np.inf
+    return mir_eval.separation.bss_eval_sources(np.array([audio_ref]), np.array([audio_estimate]))[0][0]
+
+def compute_patterns(core, W, H):
+    """
+    Compute the list of musical patterns, given factors G (core tensor), W and H.
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    W : numpy array
+        W matrix factor.
+    H : numpy array
+        H matrix factor..
+
+    Returns
+    -------
+    pattern_list : list of 2D numpy arrays
+        The list of patterns.
+
+    """
+    pattern_list = []
+    for pat_idx in range(core.shape[2]):
+        pattern_list.append(W@core[:,:,pat_idx]@H.T) 
+    return pattern_list
+    # pat_computed = tl.tenalg.multi_mode_dot(core, [W, H], modes=[0,1], skip=None, transpose=False)
+    # reordered = np.moveaxis(pat_computed, -1, 0)
+    # return reordered
+
+def sdr_songscale_patternscale_encpasulation(core, factors, hop_length, tensor_mag_original, tensor_phase_original,
+                                             pattern_list = None, phase_retrieval_song = "original_phase", phase_retrieval_patterns = "original_phase", sampling_rate = 44100):
+    """
+    Computes the SDR for the entire song and for all patterns, 
+    as defined in [1, Chapter 4.5.2] (see References, top of this file).   
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    factors : list of numpy arrays
+        The matrix factors of NTD.
+    hop_length : integer
+        Number of samples between two consecutive time frames.
+    tensor_mag_original : 3D numpy array
+        Magnitude of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    tensor_phase_original : 3D numpy array
+        Phase of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    pattern_list : list of 2D numpy arrays, optional
+        The list of patterns, if already computed
+        (avoid to recompute them again, for time saving).
+    phase_retrieval_song : string, optional
+        Specifies the type of phase retrieval which should be used for 
+        reconstructing the signal of at the songscale.
+        Possible types are:
+            - "original_phase", which uses the original phase of the tensor as phase information,
+            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
+        The default is "string".
+    phase_retrieval_patterns : string, optional
+        Specifies the type of phase retrieval which should be used for 
+        reconstructing the signal of each pattern.
+        Possible types are:
+            - "original_phase", which uses the original phase of the tensor as phase information,
+            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
+            - "softmasking", which uses Weiner filtering-like operation, detailed in [1].
+        The default is "original_phase".
+    sampling_rate : integer, optional
+        The sampling rate of the signal, in Hz.
+        The default is 44100.
+
+    Returns
+    -------
+    song_sdr : float
+        The SDR at the song scale.
+    patterns_sdr : list of float
+        The SDR for each pattern.
+    audio_songscale : IPython.display audio
+        The audio signal of the song, reconstructed from NTD
+        (the one the SDR was computed on).
+    audio_patterns : list of IPython.display
+        The audio signal of all patterns, reconstructed from NTD
+        (the one the SDRs were computed on).
+    """
+    if pattern_list is None:
+        pattern_list = compute_patterns(core, factors[0], factors[1])
+    
+    audio_songscale, song_sdr = songscale_audio_sdr(core, factors, hop_length, 
+                                                    tensor_mag_original = tensor_mag_original,
+                                                    tensor_phase_original = tensor_phase_original, 
+                                                    pattern_list = pattern_list, 
+                                                    phase_retrieval = phase_retrieval_song, 
+                                                    sampling_rate = sampling_rate)
+    
+    audio_patterns, patterns_sdr = patternscale_audio_sdr(core, factors[2], 
+                                                          pattern_list, hop_length = hop_length, 
+                                                          tensor_mag_original = tensor_mag_original,
+                                                          tensor_phase_original = tensor_phase_original,
+                                                          phase_retrieval = phase_retrieval_patterns,
+                                                          sampling_rate = sampling_rate)
+    
+    return song_sdr, patterns_sdr, audio_songscale, audio_patterns
+
+def songscale_audio_sdr(core, factors, hop_length, tensor_mag_original, tensor_phase_original, pattern_list = None, phase_retrieval = "original_phase", sampling_rate = 44100):
+    """
+    Computes the SDR for the entire song, 
+    as defined in [1, Chapter 4.5.2] (see References, top of this file).   
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    factors : list of numpy arrays
+        The matrix factors of NTD.
+    hop_length : integer
+        Number of samples between two consecutive time frames.
+    tensor_mag_original : 3D numpy array
+        Magnitude of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    tensor_phase_original : 3D numpy array
+        Phase of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    pattern_list : list of 2D numpy arrays, optional
+        The list of patterns, if already computed
+        (avoid to recompute them again, for time saving).
+    phase_retrieval : string, optional
+        Specifies the type of phase retrieval which should be used for 
+        reconstructing the signal of at the songscale.
+        Possible types are:
+            - "original_phase", which uses the original phase of the tensor as phase information,
+            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
+        The default is "string".
+    sampling_rate : integer, optional
+        The sampling rate of the signal, in Hz.
+        The default is 44100.
+
+    Returns
+    -------
+    audio_reconstructed : IPython.display
+        The audio signal of the song, reconstructed from NTD
+        (the one the SDR was computed on).
+    song_sdr : float
+        The SDR at the song scale.
+    """
+    if pattern_list is None:
+        pattern_list = compute_patterns(core, factors[0], factors[1])
+    
+    signal_reconstructed = reconstruct_song_from_factors(core, factors, hop_length, nb_bars = None, pattern_list = pattern_list, phase_retrieval = phase_retrieval, tensor_phase_original = tensor_phase_original)    
+    original_song_signal_istft = librosa.istft(np.reshape((tensor_mag_original*tensor_phase_original), (tensor_mag_original.shape[0], tensor_mag_original.shape[1] * tensor_mag_original.shape[2]), order = 'F'), hop_length = hop_length)
+    song_sdr = encapsulate_sdr_computation(original_song_signal_istft, signal_reconstructed)
+    
+    audio_reconstructed = ipd.Audio(signal_reconstructed, rate=sampling_rate)
+    
+    return audio_reconstructed, song_sdr
+
+def reconstruct_song_from_factors(core, factors, hop_length, nb_bars = None, pattern_list = None, phase_retrieval = "griffin_lim", tensor_phase_original = None):
+    """
+    Reconstructing the entire song as an audio signal.
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    factors : list of numpy arrays
+        The matrix factors of NTD.
+    hop_length : integer
+        Number of samples between two consecutive time frames.
+    nb_bars : positive integer, optional
+        Number of bars for reconstructing the song. 
+        The default is None, i.e. all bars in the song.
+        (May be useful for large songs or fewer computational complexity)
+    pattern_list : list of 2D numpy arrays, optional
+        The list of patterns, if already computed
+        (avoid to recompute them again, for time saving).
+    phase_retrieval : string, optional
+        Specifies the type of phase retrieval which should be used for 
+        reconstructing the signal of at the songscale.
+        Possible types are:
+            - "original_phase", which uses the original phase of the tensor as phase information,
+            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
+        The default is "string".
+    tensor_phase_original : 3D numpy array, optional
+        Phase of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+        Necesary for original_phase only (not used for Griffin-Lim).
+        Can be set to None if not not necessary.
+
+    Raises
+    ------
+    err.InvalidArgumentValueException
+        If the phase retrieval method is unknown.
+
+    Returns
+    -------
+    audio signal (numpy array)
+        The audio signal (as an array).
+
+    """
+    if pattern_list is None:
+        pattern_list = compute_patterns(core, factors[0], factors[1])
+    spectrogram_list_contribs = contribution_song_each_pattern(core, factors[2], pattern_list, nb_bars)
+    spectrogram_content = np.sum(spectrogram_list_contribs, axis = 0)
+    if phase_retrieval == "griffin_lim":
+        return librosa.griffinlim(spectrogram_content, hop_length = hop_length, random_state = 0)
+    elif phase_retrieval == "original_phase":
+        assert tensor_phase_original is not None
+        spectrogram_to_inverse = spectrogram_content * np.reshape(tensor_phase_original[:,:,:nb_bars], spectrogram_content.shape, order = 'F')
+        return librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
+    else:
+        raise err.InvalidArgumentValueException("Phase retrieval method not understood.")
+        
+def contribution_song_each_pattern(core, Q, pattern_list, nb_bars = None):
+    """
+    Computes the contribution to the song of each pattern, as spectrograms
+    (i.e. the exact spectrogram stemming from each pattern, 
+     weighted by its contribution in Q matrix).
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    Q : numpy array
+        The Q matrix factor.
+    pattern_list : list of 2D numpy arrays
+        The list of patterns.
+    nb_bars : positive integer, optional
+        Number of bars for reconstructing the song. 
+        The default is None, i.e. all bars in the song.
+        (May be useful for large songs or fewer computational complexity)
+
+    Returns
+    -------
+    list_contribs : list of 2D numpy arrays
+        The list of spectrogram for each pattern.
+
+    """
+    if nb_bars == None:
+        nb_bars = Q.shape[0]
+    list_contribs = []
+    for pat_idx in range(Q.shape[1]):
+        spectrogram_content = None
+        for bar_idx in range(nb_bars):
+            bar_content = Q[bar_idx, pat_idx] * pattern_list[pat_idx]
+            bar_content = np.where(bar_content > 1e-8, bar_content, 0)
+            spectrogram_content = np.concatenate((spectrogram_content, bar_content), axis=1) if spectrogram_content is not None else bar_content
+        list_contribs.append(spectrogram_content)
+    return list_contribs
+        
+def patternscale_audio_sdr(core, Q, pattern_list, hop_length, tensor_mag_original, tensor_phase_original, phase_retrieval = "griffin_lim", sampling_rate = 44100):
+    """
+    Studies all patterns, as SDR and as audio signals, to listen to them.
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    Q : numpy array
+        The Q matrix factor.
+    pattern_list : list of 2D numpy arrays
+        The list of patterns.
+    hop_length : integer
+        Number of samples between two consecutive time frames.
+    tensor_mag_original : 3D numpy array
+        Magnitude of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    tensor_phase_original : 3D numpy array
+        Phase of the barwise spectrograms (3D).
+        The order is BFT (Indexes of bars, Frequency, Time at barscale).
+    phase_retrieval : string, optional
+        Specifies the type of phase retrieval which should be used for 
+        reconstructing the signal of each pattern.
+        Possible types are:
+            - "original_phase", which uses the original phase of the tensor as phase information,
+            - "griffin_lim", which uses the Griffin-Lim algortihm for estimating the phase information,
+            - "softmasking", which uses Weiner filtering-like operation, detailed in [1].
+        The default is "original_phase".
+    sampling_rate : integer, optional
+        The sampling rate of the signal, in Hz.
+        The default is 44100.
+
+    Raises
+    ------
+    err
+        Wrong argument or abnormal behavior.
+
+    Returns
+    -------
+    list of IPython.display
+        The audio signal of the each pattern, reconstructed from NTD
+        (the ones SDR are computed on).
+    list of floats
+        The SDR of all patterns.
+        
+    """
+    best_choice_bar = [] # Local variable, to know which bar is to be considered for this particular pattern
+    audios_list = [] # To be returned
+    signal_list = [] # To be returned
+    sdr_list = [] # To be returned
+        
+    for current_pattern_idx in range(Q.shape[1]):
+        bar_original = select_associated_bar(core, Q, pattern_list, current_pattern_idx)
+        signal_baseline_bar = librosa.istft(np.reshape((tensor_mag_original*tensor_phase_original)[:,:,bar_original], (tensor_mag_original.shape[0], tensor_mag_original.shape[1]), order = 'F'), hop_length = hop_length)
+        
+        if phase_retrieval == "griffin_lim":
+            signal_audio = librosa.griffinlim(pattern_list[current_pattern_idx], hop_length = hop_length, random_state = 0)
+           
+        elif phase_retrieval == "original_phase":
+            spectrogram_to_inverse = tensor_phase_original[:,:,bar_original] * pattern_list[current_pattern_idx]
+            signal_audio = librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
+            
+        elif phase_retrieval in ["masking", "softmasking"]:
+            if phase_retrieval == "masking":
+                warnings.warn("'masking' is deprecated, you should use 'softmasking' instead.")
+            assert tensor_mag_original is not None
+            assert tensor_phase_original is not None
+            if Q[bar_original, current_pattern_idx] != 0:
+                pattern = Q[bar_original, current_pattern_idx] * pattern_list[current_pattern_idx]  # Numerator of masking
+                pattern = 1e6 * np.where(pattern > 1e-8, pattern, 0) # Very low values lead to undeterminism in the divide.
+
+                bar_content_patternwise = np.zeros(pattern.shape)
+                for pat_idx_loop in range(Q.shape[1]):
+                    bar_content_patternwise += Q[bar_original, pat_idx_loop] * pattern_list[pat_idx_loop] # Denominator of masking
+                bar_content_patternwise = 1e6 * np.where(bar_content_patternwise > 1e-8, bar_content_patternwise, 0) # Very low values lead to undeterminism in the divide.
+
+                mask = np.divide(pattern, bar_content_patternwise, where=bar_content_patternwise != 0)  # if bar_content_patternwise == 0, pattern also equals 0.
+                    
+                spectrogram_to_inverse = tensor_phase_original[:,:,bar_original] * tensor_mag_original[:,:,bar_original] * mask # Masked content                  
+                signal_audio = librosa.istft(spectrogram_to_inverse, hop_length = hop_length)
+                if np.mean(mask) > 0.99: # Mask too close to original
+                    warnings.warn(f"The current masked spectrogram is too close to the ogirinal spectrogram, the SDR would be disinformative.")
+                    continue
+
+            else:
+                warnings.warn(f"The {current_pattern_idx}-th pattern is never used in the $Q$ matrix.")
+                continue
+        else:
+            raise err.InvalidArgumentValueException("Phase retrieval method not understood.")
+        signal_list.append(signal_audio)
+        audios_list.append(ipd.Audio(signal_audio, rate=sampling_rate))
+        sdr_list.append(encapsulate_sdr_computation(signal_baseline_bar, signal_audio))
+    
+    if signal_list == []:
+        raise err.AbnormalBehaviorException("No signal was computed, which should be considered a problem.")
+
+    return audios_list, np.ma.masked_invalid(sdr_list)
+
+def select_associated_bar(core, Q, pattern_list, pat_idx):
+    """
+    Method selecting the associated bar (the most similar) for a particular pattern.
+    For now, only a simple strategy is computed (the bar which has the maximal value in Q),
+    but additional strategies can be found in [2].
+
+    Parameters
+    ----------
+    core : numpy array
+        The core tensor.
+    Q : numpy array
+        The Q matrix factor.
+    pattern_list : list of 2D numpy arrays
+        The list of patterns.
+    pat_idx : integer
+        The index of the current pattern.
+
+    Returns
+    -------
+    integer
+        Index of the associated bar in the song.
+        
+    References
+    ----------
+    [2] Smith, J. B., Kawasaki, Y., & Goto, M. (2019). Unmixer: An Interface for 
+    Extracting and Remixing Loops. In ISMIR (pp. 824-831).
+
+    """
     return np.argmax(Q[:,pat_idx])
```

### Comparing `barmuscomp-0.1.2/barmuscomp/model/plot_comparison_ae_ntd.py` & `barmuscomp-0.1.3/barmuscomp/model/plot_comparison_ae_ntd.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Jul 26 15:37:15 2022
-
-@author: amarmore
-
-Plotting functions used for comparing NTD and AE-NTD outputs.
-Ugly code.
-"""
-import as_seg.autosimilarity_computation as as_comp
-from barmuscomp.model.current_plot import *
-import barmuscomp.model.pattern_study as ps
-
-import numpy as np
-import pandas as pd
-
-def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
-    """
-    Listening to both audio examples (comparing NTD and AE-NTD).
-    """
-    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-def plot_spec_ntd_ae(spec_1, spec_2, title, to_permute = True, plot_diff = False):
-    """
-    Plotting both NTD and AE-NTD Q matrix.
-    """
-    if spec_1.shape[0] == spec_1.shape[1]:
-        fig, axs = plt.subplots(1, 2, figsize=(14,7))
-    else:
-        fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
-    if to_permute:
-        permut_1 = permutate_factor(spec_1.T) 
-        spec_1 = spec_1[permut_1]
-        permut_2 = permutate_factor(spec_2.T)
-        spec_2 = spec_2[permut_2]
-    diff = spec_2 - spec_1
-    axs[0].pcolormesh(np.arange(spec_1.shape[1]), np.arange(spec_1.shape[0]), spec_1, cmap=cm.Greys, shading='auto')
-    axs[0].set_title(f"{title} of NTD")
-    axs[1].pcolormesh(np.arange(spec_2.shape[1]), np.arange(spec_2.shape[0]), spec_2, cmap=cm.Greys, shading='auto')
-    axs[1].set_title(f"{title} of AE")
-    axs[0].invert_yaxis()
-    axs[1].invert_yaxis()
-    plt.show()
-    if plot_diff:
-        if spec_1.shape[0] == spec_1.shape[1]:
-            fig, axs = plt.subplots(1, 2, figsize=(14,7))
-        else:
-            fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
-        axs[0].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, shading='auto')
-        axs[0].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre min et max)\n Diff maximale: {np.amax(np.abs(diff))}")
-        the_max = max(np.amax(spec_1), np.amax(spec_2))
-        axs[1].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, vmin=0, vmax=the_max, shading='auto')
-        axs[1].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre 0 et max des 2 spectrogrammes)\n Valeur max des 2 specs{the_max}")
-        axs[0].invert_yaxis()
-        axs[1].invert_yaxis()
-        plt.show()
-
-def plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, core_ae, factors_ae, signal_patterns_ae, nb_patterns_to_show):
-    """
-    Compares the patterns of both NTD and AE-NTD.
-    """
-    for i in range(nb_patterns_to_show):
-        pattern = factors_ae[0]@core_ae[:,:,i]@factors_ae[1].T
-        plot_spec_ntd_ae(spec_patterns_ntd[i], pattern, title = f"{i}-th pattern in the decoder", to_permute = False)
-        plot_audio_diff_ntd_ae_in_dataframe(signal_patterns_ntd[i], signal_patterns_ae[i])
-        
-def plot_comparison_this_ae_ntd(ssae, projection, hop_length, factors_ntd, tensor_mag_original, tensor_phase_original, nb_bars, phase_retrieval_song, phase_retrieval_patterns,
-                                autosimilarity_type = "Cosine", plot_patterns = False, nb_patterns_to_show = 4, subdivision = 96, spec_patterns_ntd = None, signal_patterns_ntd = None):
-    """
-    Compares the overall outputs of both NTD and AE-NTD.
-    """    
-    autosimil = as_comp.switch_autosimilarity(projection, similarity_type = autosimilarity_type, normalise = True)
-    autosimil_ntd = as_comp.switch_autosimilarity(factors_ntd[2], similarity_type = autosimilarity_type, normalise = True)
-    plot_spec_ntd_ae(autosimil_ntd, autosimil, "Autosimilarity", to_permute = False)
-
-    W = ssae.get_W()
-    H = ssae.get_H()
-    G = ssae.get_G()
-    proj_np = np.array(projection)
-
-    plot_spec_ntd_ae(factors_ntd[0], W, title = "W matrix")
-    plot_spec_ntd_ae(factors_ntd[1].T, H.T, title = "H matrix")
-    plot_spec_ntd_ae(factors_ntd[2].T, proj_np.T, title = "Latent representations")
-    song_sdr, patterns_sdr, audio_patterns = ps.sdr_songscale_patternscale_encpasulation(G, [W, H, proj_np], hop_length, tensor_mag_original, tensor_phase_original,
-                                                                 nb_bars, phase_retrieval_song, phase_retrieval_patterns, subdivision = subdivision)
-    
-    print(f"SDR at the song scale: {song_sdr}")
-    print(f"SDR at the pattern scale: average = {np.mean(patterns_sdr)}, std = {np.std(patterns_sdr)}")
-
-    if plot_patterns:
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Jul 26 15:37:15 2022
+
+@author: amarmore
+
+Plotting functions used for comparing NTD and AE-NTD outputs.
+Ugly code.
+"""
+import as_seg.autosimilarity_computation as as_comp
+from barmuscomp.model.current_plot import *
+import barmuscomp.model.pattern_study as ps
+
+import numpy as np
+import pandas as pd
+
+def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
+    """
+    Listening to both audio examples (comparing NTD and AE-NTD).
+    """
+    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+def plot_spec_ntd_ae(spec_1, spec_2, title, to_permute = True, plot_diff = False):
+    """
+    Plotting both NTD and AE-NTD Q matrix.
+    """
+    if spec_1.shape[0] == spec_1.shape[1]:
+        fig, axs = plt.subplots(1, 2, figsize=(14,7))
+    else:
+        fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
+    if to_permute:
+        permut_1 = permutate_factor(spec_1.T) 
+        spec_1 = spec_1[permut_1]
+        permut_2 = permutate_factor(spec_2.T)
+        spec_2 = spec_2[permut_2]
+    diff = spec_2 - spec_1
+    axs[0].pcolormesh(np.arange(spec_1.shape[1]), np.arange(spec_1.shape[0]), spec_1, cmap=cm.Greys, shading='auto')
+    axs[0].set_title(f"{title} of NTD")
+    axs[1].pcolormesh(np.arange(spec_2.shape[1]), np.arange(spec_2.shape[0]), spec_2, cmap=cm.Greys, shading='auto')
+    axs[1].set_title(f"{title} of AE")
+    axs[0].invert_yaxis()
+    axs[1].invert_yaxis()
+    plt.show()
+    if plot_diff:
+        if spec_1.shape[0] == spec_1.shape[1]:
+            fig, axs = plt.subplots(1, 2, figsize=(14,7))
+        else:
+            fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
+        axs[0].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, shading='auto')
+        axs[0].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre min et max)\n Diff maximale: {np.amax(np.abs(diff))}")
+        the_max = max(np.amax(spec_1), np.amax(spec_2))
+        axs[1].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, vmin=0, vmax=the_max, shading='auto')
+        axs[1].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre 0 et max des 2 spectrogrammes)\n Valeur max des 2 specs{the_max}")
+        axs[0].invert_yaxis()
+        axs[1].invert_yaxis()
+        plt.show()
+
+def plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, core_ae, factors_ae, signal_patterns_ae, nb_patterns_to_show):
+    """
+    Compares the patterns of both NTD and AE-NTD.
+    """
+    for i in range(nb_patterns_to_show):
+        pattern = factors_ae[0]@core_ae[:,:,i]@factors_ae[1].T
+        plot_spec_ntd_ae(spec_patterns_ntd[i], pattern, title = f"{i}-th pattern in the decoder", to_permute = False)
+        plot_audio_diff_ntd_ae_in_dataframe(signal_patterns_ntd[i], signal_patterns_ae[i])
+        
+def plot_comparison_this_ae_ntd(ssae, projection, hop_length, factors_ntd, tensor_mag_original, tensor_phase_original, nb_bars, phase_retrieval_song, phase_retrieval_patterns,
+                                autosimilarity_type = "Cosine", plot_patterns = False, nb_patterns_to_show = 4, subdivision = 96, spec_patterns_ntd = None, signal_patterns_ntd = None):
+    """
+    Compares the overall outputs of both NTD and AE-NTD.
+    """    
+    autosimil = as_comp.switch_autosimilarity(projection, similarity_type = autosimilarity_type, normalise = True)
+    autosimil_ntd = as_comp.switch_autosimilarity(factors_ntd[2], similarity_type = autosimilarity_type, normalise = True)
+    plot_spec_ntd_ae(autosimil_ntd, autosimil, "Autosimilarity", to_permute = False)
+
+    W = ssae.get_W()
+    H = ssae.get_H()
+    G = ssae.get_G()
+    proj_np = np.array(projection)
+
+    plot_spec_ntd_ae(factors_ntd[0], W, title = "W matrix")
+    plot_spec_ntd_ae(factors_ntd[1].T, H.T, title = "H matrix")
+    plot_spec_ntd_ae(factors_ntd[2].T, proj_np.T, title = "Latent representations")
+    song_sdr, patterns_sdr, audio_patterns = ps.sdr_songscale_patternscale_encpasulation(G, [W, H, proj_np], hop_length, tensor_mag_original, tensor_phase_original,
+                                                                 nb_bars, phase_retrieval_song, phase_retrieval_patterns, subdivision = subdivision)
+    
+    print(f"SDR at the song scale: {song_sdr}")
+    print(f"SDR at the pattern scale: average = {np.mean(patterns_sdr)}, std = {np.std(patterns_sdr)}")
+
+    if plot_patterns:
         plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, G, [W, H, proj_np], signal_patterns_ae = audio_patterns, nb_patterns_to_show = nb_patterns_to_show)
```

### Comparing `barmuscomp-0.1.2/barmuscomp/scripts/default_path.py` & `barmuscomp-0.1.3/barmuscomp/scripts/default_path.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Sep 22 17:22:59 2021
-
-Default paths for the different folders.
-Should be changed prior to any computation.
-
-@author: amarmore
-"""
-# RWC
-path_data_persisted_rwc = "C:/Users/amarmore/Desktop/data_persisted" ## Path where pre-computed data on RWC Pop should be stored (spectrograms, NTD, neural networks, etc)
-path_annotation_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/annotations" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
-path_entire_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Entire RWC" ## Path where are stored wav files of RWC
-path_even_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Even songs" ## Path containing only the wav files of songs of odd numbers
-path_odd_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Odd songs" ## Path containing only the wav files of songs of even numbers
-path_debug_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/debug" ## Debug path, containing only two songs, to fix functions quickly
-path_mirdata_rwc = "C:/Users/amarmore/Desktop/Audio samples/mirdata/RWC Pop/" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
-
-# SALAMI
-path_data_persisted_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami/data_persisted" ## Path where pre-computed data on the SALAMI dataset should be stored (spectrograms, NTD, neural networks, etc)
-path_entire_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami" ## Path where are stored wav files of SALAMI (path where it is downloaded by mirdata also)
-
-# Come Together
-come_together = "C:/Users/amarmore/this_folder/The Beatles - Come Together"
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Sep 22 17:22:59 2021
+
+Default paths for the different folders.
+Should be changed prior to any computation.
+
+@author: amarmore
+"""
+# RWC
+path_data_persisted_rwc = "C:/Users/amarmore/Desktop/data_persisted" ## Path where pre-computed data on RWC Pop should be stored (spectrograms, NTD, neural networks, etc)
+path_annotation_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/annotations" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
+path_entire_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Entire RWC" ## Path where are stored wav files of RWC
+path_even_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Even songs" ## Path containing only the wav files of songs of odd numbers
+path_odd_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Odd songs" ## Path containing only the wav files of songs of even numbers
+path_debug_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/debug" ## Debug path, containing only two songs, to fix functions quickly
+path_mirdata_rwc = "C:/Users/amarmore/Desktop/Audio samples/mirdata/RWC Pop/" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
+
+# SALAMI
+path_data_persisted_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami/data_persisted" ## Path where pre-computed data on the SALAMI dataset should be stored (spectrograms, NTD, neural networks, etc)
+path_entire_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami" ## Path where are stored wav files of SALAMI (path where it is downloaded by mirdata also)
+
+# Come Together
+come_together = "C:/Users/amarmore/this_folder/The Beatles - Come Together"
 path_data_persisted_come_together = "C:/Users/amarmore/Desktop/data_persisted"
```

### Comparing `barmuscomp-0.1.2/barmuscomp/scripts/overall_scripts.py` & `barmuscomp-0.1.3/barmuscomp/scripts/overall_scripts.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar  4 17:34:39 2020
-
-@author: amarmore
-
-"""
-
-import as_seg.data_manipulation as dm
-import barmuscomp.ae as ae
-import barmuscomp.model.errors as err
-import barmuscomp.scripts.default_path as paths
-import nn_fac.ntd as NTD
-
-import os
-import numpy as np
-
-# %% Load everything from as_seg
-from as_seg.scripts.overall_scripts import *
-
-# %% NTD specific
-def NTD_decomp_as_script(persisted_path, persisted_arguments, tensor_spectrogram, ranks, init = "tucker", update_rule = "hals", beta = None, compute_if_not_persisted = True): 
-    """
-    Computes the NTD from the tensor_spectrogram and with specified ranks.
-    On the first hand, if the NTD is persisted, it will load and return its results.
-    If it's not, it will compute the NTD, store it, and return it.
-
-    Parameters
-    ----------
-    persisted_path : String
-        Path of the persisted decompositions and bars.
-    persisted_arguments : String
-        Identifier of the specific NTD to load/save.
-    tensor_spectrogram : tensorly tensor
-        The tensor to decompose.
-    ranks : list of integers
-        Ranks of the decomposition.
-    init : String, optional
-        The type of initialization of the NTD.
-        See the NTD module to have more information regarding initialization.
-        The default is "chromas",
-        meaning that the first factor will be set to the 12-size identity matrix,
-        and the other factors will be initialized by HOSVD.
-
-    Raises
-    ------
-    NotImplementedError
-        Errors in the arguments.
-
-    Returns
-    -------
-    core : tensorly tensor
-        The core of the decomposition.
-    factors : numpy array
-        The factors of the decomposition.
-
-    """
-    if update_rule == "hals":
-        path_for_ntd = "{}/ntd/{}_{}_{}".format(persisted_path, ranks[0], ranks[1], ranks[2])
-    elif update_rule == "mu":
-        path_for_ntd = "{}/ntd_mu/{}_{}_{}".format(persisted_path, ranks[0], ranks[1], ranks[2])
-    else:
-        raise NotImplementedError(f"Update rule type not understood: {update_rule}")
-    
-    if update_rule == "mu" and beta == None:
-        raise NotImplementedError("Inconsistent arguments. Beta should be set if the update_rule is the MU.")
-        
-    try:
-        a_core_path = "{}/core{}.npy".format(path_for_ntd, persisted_arguments)
-        a_core = np.load(a_core_path)
-        a_factor_path = "{}/factors{}.npy".format(path_for_ntd, persisted_arguments)
-        a_factor = np.load(a_factor_path, allow_pickle=True)
-        return a_core, a_factor
-    except FileNotFoundError:
-        assert compute_if_not_persisted
-        if update_rule == "hals":
-            core, factors = NTD.ntd(tensor_spectrogram, ranks = ranks, init = init, verbose = False,
-                                sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
-                                deterministic = True)
-        elif update_rule == "mu":
-            core, factors = NTD.ntd_mu(tensor_spectrogram, ranks = ranks, init = init, verbose = False, beta = beta, n_iter_max=1000,
-                                sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
-                                deterministic = True)
-        
-        pathlib.Path(path_for_ntd).mkdir(parents=True, exist_ok=True)
-    
-        core_path = "{}/core{}".format(path_for_ntd, persisted_arguments)
-        np.save(core_path, core)
-        factors_path = "{}/factors{}".format(path_for_ntd, persisted_arguments)
-        np.save(factors_path, factors)
-        return core, factors
-    
-# %% SSAE specific 
-def load_or_save_convolutional_projection(persisted_path, song_name, data_loader, dim_latent_space, lr = 1e-3, n_epochs = 1000, feature = "pcp", hop_length = 32, subdivision_bars = 96, freq_len = 12, compute_if_not_persisted = True):
-    """
-    Loads the neural network projection for this song, which was persisted after its computation.
-
-    Parameters
-    ----------
-    persisted_path : string
-        Path of the folder where the projections should be found.
-    song_name : int or string
-        Identifier of the song.
-    data_loader : torch.DataLoader
-        The DataLoader associated with the barwise tensor of this song.
-    dim_latent_space : int
-        Dimension of the latent space.
-    sparsity_lambda : None or float
-        The sparisty ponderation parameter.
-        If set to None, no sparsity is enforced.
-    nn : boolean, optional
-        DEPRECATED. Whether the latent vectors should be nonnegative or not. 
-        Accepted behavior nowadays is not enforcing nonnegativity. The default is False.
-    lr : float, optional
-        Learning rate of the network. The default is 1e-3.
-    n_epochs : int, optional
-        Number of epochs to perform. The default is 1000.
-    norm_tensor : float, optional
-        Norm of the barwise tensor. Used to noramlize the sparsity parameter, so useless when sparsity lambda is set to None.
-        The default is None.
-    feature : string, optional
-        The feature used to represent the song. See model.feature.py for details. The default is "pcp".
-    hop_length : int, optional
-        Hop_length used to compute the original spectrogram. The default is 32.
-    subdivision_bars : int, optional
-        The number of subdivision of the bar to be contained in each slice of the tensor.
-    freq_len : int, optional
-        Dimension of the frequency mode (frequency-related representation of music). The default is 12.
-    compute_if_not_persisted : boolean, optional
-        Indicating hether the network should be computed if it's not found in persisted networks.
-        Should be set to True if networks are computed for the first time, and to False to speed up computation in tests where they have already been computed.
-        The default is True.
-
-    Raises
-    ------
-    FileNotFoundError
-        If the network asn't found and if ``FileNotFoundError'' is set to False.
-
-    Returns
-    -------
-    projection : numpy array
-        Latent projection of each bar through this network.
-
-    """
-    persisted_params = "song{}_feature{}_hop{}_subdivbars{}_initkaiming_lr{}_nepochs{}".format(song_name, feature, hop_length, subdivision_bars, lr, n_epochs)
-    
-    conv_save_name = "{}/neural_nets/conv_4_16_k3_transk3_latentfc{}_{}".format(persisted_path, dim_latent_space, persisted_params)
-    conv_load_name = "{}/neural_nets/transfered/conv_4_16_k3_transk3_latentfc{}_{}".format(persisted_path, dim_latent_space, persisted_params)
-    
-    try:
-        projection = np.load("{}.npy".format(conv_load_name), allow_pickle = True)
-    except FileNotFoundError:
-        try:
-            projection = np.load("{}.npy".format(conv_save_name), allow_pickle = True)
-        except FileNotFoundError:
-            if compute_if_not_persisted:
-                conv_model = ae.ConvolutionalAutoencoder(input_size_x = subdivision_bars, input_size_y = freq_len, dim_latent_space = dim_latent_spaces)
-                conv_model = conv_model.my_optim_method(n_epochs, data_loader, lr=lr, verbose = False, labels = None)
-                projection = conv_model.get_latent_projection(data_loader)
-                np.save(conv_save_name, projection)
-            else:
-                raise FileNotFoundError(f"Neural network projection not found, check the name: {conv_save_name}") from None
-
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Mar  4 17:34:39 2020
+
+@author: amarmore
+
+"""
+
+import as_seg.data_manipulation as dm
+import barmuscomp.ae as ae
+import barmuscomp.model.errors as err
+import barmuscomp.scripts.default_path as paths
+import nn_fac.ntd as NTD
+
+import os
+import numpy as np
+
+# %% Load everything from as_seg
+from as_seg.scripts.overall_scripts import *
+
+# %% NTD specific
+def NTD_decomp_as_script(persisted_path, persisted_arguments, tensor_spectrogram, ranks, init = "tucker", update_rule = "hals", beta = None, compute_if_not_persisted = True): 
+    """
+    Computes the NTD from the tensor_spectrogram and with specified ranks.
+    On the first hand, if the NTD is persisted, it will load and return its results.
+    If it's not, it will compute the NTD, store it, and return it.
+
+    Parameters
+    ----------
+    persisted_path : String
+        Path of the persisted decompositions and bars.
+    persisted_arguments : String
+        Identifier of the specific NTD to load/save.
+    tensor_spectrogram : tensorly tensor
+        The tensor to decompose.
+    ranks : list of integers
+        Ranks of the decomposition.
+    init : String, optional
+        The type of initialization of the NTD.
+        See the NTD module to have more information regarding initialization.
+        The default is "chromas",
+        meaning that the first factor will be set to the 12-size identity matrix,
+        and the other factors will be initialized by HOSVD.
+
+    Raises
+    ------
+    NotImplementedError
+        Errors in the arguments.
+
+    Returns
+    -------
+    core : tensorly tensor
+        The core of the decomposition.
+    factors : numpy array
+        The factors of the decomposition.
+
+    """
+    if update_rule == "hals":
+        path_for_ntd = "{}/ntd/{}_{}_{}".format(persisted_path, ranks[0], ranks[1], ranks[2])
+    elif update_rule == "mu":
+        path_for_ntd = "{}/ntd_mu/{}_{}_{}".format(persisted_path, ranks[0], ranks[1], ranks[2])
+    else:
+        raise NotImplementedError(f"Update rule type not understood: {update_rule}")
+    
+    if update_rule == "mu" and beta == None:
+        raise NotImplementedError("Inconsistent arguments. Beta should be set if the update_rule is the MU.")
+        
+    try:
+        a_core_path = "{}/core{}.npy".format(path_for_ntd, persisted_arguments)
+        a_core = np.load(a_core_path)
+        a_factor_path = "{}/factors{}.npy".format(path_for_ntd, persisted_arguments)
+        a_factor = np.load(a_factor_path, allow_pickle=True)
+        return a_core, a_factor
+    except FileNotFoundError:
+        assert compute_if_not_persisted
+        if update_rule == "hals":
+            core, factors = NTD.ntd(tensor_spectrogram, ranks = ranks, init = init, verbose = False,
+                                sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
+                                deterministic = True)
+        elif update_rule == "mu":
+            core, factors = NTD.ntd_mu(tensor_spectrogram, ranks = ranks, init = init, verbose = False, beta = beta, n_iter_max=1000,
+                                sparsity_coefficients = [None, None, None, None], normalize = [True, True, False, True], mode_core_norm = 2,
+                                deterministic = True)
+        
+        pathlib.Path(path_for_ntd).mkdir(parents=True, exist_ok=True)
+    
+        core_path = "{}/core{}".format(path_for_ntd, persisted_arguments)
+        np.save(core_path, core)
+        factors_path = "{}/factors{}".format(path_for_ntd, persisted_arguments)
+        np.save(factors_path, factors)
+        return core, factors
+    
+# %% SSAE specific 
+def load_or_save_convolutional_projection(persisted_path, song_name, data_loader, dim_latent_space, lr = 1e-3, n_epochs = 1000, feature = "pcp", hop_length = 32, subdivision_bars = 96, freq_len = 12, compute_if_not_persisted = True):
+    """
+    Loads the neural network projection for this song, which was persisted after its computation.
+
+    Parameters
+    ----------
+    persisted_path : string
+        Path of the folder where the projections should be found.
+    song_name : int or string
+        Identifier of the song.
+    data_loader : torch.DataLoader
+        The DataLoader associated with the barwise tensor of this song.
+    dim_latent_space : int
+        Dimension of the latent space.
+    sparsity_lambda : None or float
+        The sparisty ponderation parameter.
+        If set to None, no sparsity is enforced.
+    nn : boolean, optional
+        DEPRECATED. Whether the latent vectors should be nonnegative or not. 
+        Accepted behavior nowadays is not enforcing nonnegativity. The default is False.
+    lr : float, optional
+        Learning rate of the network. The default is 1e-3.
+    n_epochs : int, optional
+        Number of epochs to perform. The default is 1000.
+    norm_tensor : float, optional
+        Norm of the barwise tensor. Used to noramlize the sparsity parameter, so useless when sparsity lambda is set to None.
+        The default is None.
+    feature : string, optional
+        The feature used to represent the song. See model.feature.py for details. The default is "pcp".
+    hop_length : int, optional
+        Hop_length used to compute the original spectrogram. The default is 32.
+    subdivision_bars : int, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+    freq_len : int, optional
+        Dimension of the frequency mode (frequency-related representation of music). The default is 12.
+    compute_if_not_persisted : boolean, optional
+        Indicating hether the network should be computed if it's not found in persisted networks.
+        Should be set to True if networks are computed for the first time, and to False to speed up computation in tests where they have already been computed.
+        The default is True.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the network asn't found and if ``FileNotFoundError'' is set to False.
+
+    Returns
+    -------
+    projection : numpy array
+        Latent projection of each bar through this network.
+
+    """
+    persisted_params = "song{}_feature{}_hop{}_subdivbars{}_initkaiming_lr{}_nepochs{}".format(song_name, feature, hop_length, subdivision_bars, lr, n_epochs)
+    
+    conv_save_name = "{}/neural_nets/conv_4_16_k3_transk3_latentfc{}_{}".format(persisted_path, dim_latent_space, persisted_params)
+    conv_load_name = "{}/neural_nets/transfered/conv_4_16_k3_transk3_latentfc{}_{}".format(persisted_path, dim_latent_space, persisted_params)
+    
+    try:
+        projection = np.load("{}.npy".format(conv_load_name), allow_pickle = True)
+    except FileNotFoundError:
+        try:
+            projection = np.load("{}.npy".format(conv_save_name), allow_pickle = True)
+        except FileNotFoundError:
+            if compute_if_not_persisted:
+                conv_model = ae.ConvolutionalAutoencoder(input_size_x = subdivision_bars, input_size_y = freq_len, dim_latent_space = dim_latent_spaces)
+                conv_model = conv_model.my_optim_method(n_epochs, data_loader, lr=lr, verbose = False, labels = None)
+                projection = conv_model.get_latent_projection(data_loader)
+                np.save(conv_save_name, projection)
+            else:
+                raise FileNotFoundError(f"Neural network projection not found, check the name: {conv_save_name}") from None
+
     return projection
```

### Comparing `barmuscomp-0.1.2/barmuscomp.egg-info/PKG-INFO` & `barmuscomp-0.1.3/barmuscomp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-Metadata-Version: 2.1
-Name: barmuscomp
-Version: 0.1.2
-Summary: Package for barwise compression applied on musical segmentation.
-Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
-Author: Marmoret Axel
-Author-email: axel.marmoret@irisa.fr
-License: BSD
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8.*
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: AUTHORS
-
-# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
-
-Hello, and welcome on this repository!
-
-This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
-
-This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
-
-This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
-
-It can be installed with pip using `pip install barmuscomp`.
-
-This is a first release, and may contain bug. Comments are welcomed!
-
-## Software version ##
-
-This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
-
-## Tutorial Notebook ##
-
-3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
-
-They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
-
-## How to cite ##
-
-You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
-
-Here are two styles of citations:
-
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
-
-In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
-
-## Credits ##
-
-Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
-
-The technique in itself was also developed by FrÃ©dÃ©ric Bimbot (<bimbot@irisa.fr>).
-
-## References ##
-[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, UniversitÃ© de Rennes 1, 2022.
-(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
-
-[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
-
-[3] A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices", 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+Metadata-Version: 2.1
+Name: barmuscomp
+Version: 0.1.3
+Summary: Package for barwise compression applied on musical segmentation.
+Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
+Author: Marmoret Axel
+Author-email: axel.marmoret@irisa.fr
+License: BSD
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS
+
+# BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
+
+Hello, and welcome on this repository!
+
+This project aims at compressing all bars in a song, and studies the compressed representations of every bar to infer its structure. It is related to my PhD thesis [1].
+
+This repository contains code for the NTD, PCA, NMF, and Autoencoders (developed in PyTorch), as presented in [2].
+
+This project is an extension of the toolbox as_seg [3], which computes the segmentation of an autosimilarity matrix.
+
+It can be installed with pip using `pip install barmuscomp`.
+
+This is a first release, and may contain bug. Comments are welcomed!
+
+## Software version ##
+
+This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
+
+## Tutorial Notebook ##
+
+3 tutorial notebooks are available in the folder "Notebooks", and present the different compression methods on the song 'Come Together'.
+
+They are only present if you downloaded the project from git (e.g. https://gitlab.inria.fr/amarmore/barmuscomp), and are not available in the pip version (which is in general not accessible easily in the file tree).
+
+## How to cite ##
+
+You should cite the package `BarMusComp`, available on HAL (https://hal.archives-ouvertes.fr/hal-03782914).
+
+Here are two styles of citations:
+
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022barmuscomp, title={BarMusComp: module for computing barwise compressed representations of music}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/barmuscomp}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+
+In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, BarMusComp: module for computing barwise compressed representations of music, 2022, url: https://gitlab.inria.fr/amarmore/barmuscomp.
+
+## Credits ##
+
+Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
+
+The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
+
+## References ##
+[1] A. Marmoret, "Unsupervised Machine Learning Paradigms for the Representation of Music Similarity and Structure", Ph.D. dissertation, Université de Rennes 1, 2022.
+(not uploaded yet but will be soon! You should check the website hal.archives-ouvertes.fr/ in case this README is not updated with the reference.)
+
+[2] A. Marmoret, J.E. Cohen, and F. Bimbot, "Barwise Compression Schemes for Audio-Based Music Structure Analysis"", in: 19th Sound and Music Computing Conference, SMC 2022, Sound and music Computing network, 2022.
+
+[3] A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices", 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+
```

### Comparing `barmuscomp-0.1.2/barmuscomp.egg-info/SOURCES.txt` & `barmuscomp-0.1.3/barmuscomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.2/setup.py` & `barmuscomp-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="barmuscomp",
-    version="0.1.2",
-    author="Marmoret Axel",
-    author_email="axel.marmoret@irisa.fr",
-    description="Package for barwise compression applied on musical segmentation.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://gitlab.inria.fr/amarmore/barmuscomp",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python",
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "Topic :: Multimedia :: Sound/Audio :: Analysis",
-        "Programming Language :: Python :: 3.8"
-    ],
-    license='BSD',
-    install_requires=[
-        'as_seg',
-        'librosa >= 0.8.0',
-        'madmom >= 0.16.1',
-        'matplotlib',
-        'mir_eval >= 0.6',
-        'mirdata >= 0.3.3',
-        'nn-fac >= 0.2.0',
-        'numpy >= 1.18.2',
-        'pandas',
-        'scipy >= 1.4.1',
-        'sklearn',
-        'soundfile',
-        'tensorly >= 0.5.1',
-        'torch >= 1.8.0'
-    ],
-    python_requires='>=3.8.*',
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="barmuscomp",
+    version="0.1.3",
+    author="Marmoret Axel",
+    author_email="axel.marmoret@irisa.fr",
+    description="Package for barwise compression applied on musical segmentation.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://gitlab.inria.fr/amarmore/barmuscomp",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Topic :: Multimedia :: Sound/Audio :: Analysis",
+        "Programming Language :: Python :: 3.8"
+    ],
+    license='BSD',
+    install_requires=[
+        'as_seg',
+        'librosa >= 0.8.0',
+        #'madmom @ git+https://github.com/CPJKU/madmom',
+        'madmom >= 0.16.1' ,
+        'matplotlib',
+        'mir_eval >= 0.6',
+        'mirdata >= 0.3.3',
+        'nn-fac >= 0.2.0',
+        'numpy >= 1.18.2',
+        'pandas',
+        'scipy >= 1.4.1',
+        'sklearn',
+        'soundfile',
+        'tensorly >= 0.5.1',
+        'torch >= 1.8.0'
+    ],
+    python_requires='>3.7',
+)
```

