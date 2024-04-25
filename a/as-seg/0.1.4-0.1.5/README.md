# Comparing `tmp/as_seg-0.1.4.tar.gz` & `tmp/as_seg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as_seg-0.1.4.tar", last modified: Wed Nov 15 12:10:00 2023, max compression
+gzip compressed data, was "as_seg-0.1.5.tar", last modified: Thu Apr 25 15:34:36 2024, max compression
```

## Comparing `as_seg-0.1.4.tar` & `as_seg-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 12:10:00.941298 as_seg-0.1.4/
--rw-rw-rw-   0        0        0       90 2023-11-15 10:18:55.000000 as_seg-0.1.4/AUTHORS
--rw-rw-rw-   0        0        0     1516 2023-11-15 10:18:55.000000 as_seg-0.1.4/LICENSE.md
--rw-rw-rw-   0        0        0     4015 2023-11-15 12:10:00.937308 as_seg-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3207 2023-11-15 10:18:55.000000 as_seg-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-15 12:10:00.910602 as_seg-0.1.4/as_seg/
--rw-rw-rw-   0        0        0    24645 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/CBM_algorithm.py
--rw-rw-rw-   0        0        0      254 2023-11-15 10:31:54.000000 as_seg-0.1.4/as_seg/__init__.py
--rw-rw-rw-   0        0        0     9650 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/autosimilarity_computation.py
--rw-rw-rw-   0        0        0     7553 2023-11-15 10:28:45.000000 as_seg-0.1.4/as_seg/barwise_input.py
--rw-rw-rw-   0        0        0    23674 2023-11-15 10:41:51.000000 as_seg-0.1.4/as_seg/data_manipulation.py
--rw-rw-rw-   0        0        0    13720 2023-11-15 10:33:54.000000 as_seg-0.1.4/as_seg/foote_novelty.py
-drwxrwxrwx   0        0        0        0 2023-11-15 12:10:00.929327 as_seg-0.1.4/as_seg/model/
--rw-rw-rw-   0        0        0       78 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/model/__init__.py
--rw-rw-rw-   0        0        0     6046 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/model/current_plot.py
--rw-rw-rw-   0        0        0      568 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/model/errors.py
--rw-rw-rw-   0        0        0    17519 2023-11-15 11:53:20.000000 as_seg-0.1.4/as_seg/model/features.py
-drwxrwxrwx   0        0        0        0 2023-11-15 12:10:00.935314 as_seg-0.1.4/as_seg/scripts/
--rw-rw-rw-   0        0        0        0 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/scripts/__init__.py
--rw-rw-rw-   0        0        0     1814 2023-11-15 10:18:55.000000 as_seg-0.1.4/as_seg/scripts/default_path.py
--rw-rw-rw-   0        0        0     6765 2023-11-15 11:49:38.000000 as_seg-0.1.4/as_seg/scripts/example.py
--rw-rw-rw-   0        0        0    19193 2023-11-15 10:43:05.000000 as_seg-0.1.4/as_seg/scripts/overall_scripts.py
-drwxrwxrwx   0        0        0        0 2023-11-15 12:10:00.919505 as_seg-0.1.4/as_seg.egg-info/
--rw-rw-rw-   0        0        0     4015 2023-11-15 12:10:00.000000 as_seg-0.1.4/as_seg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-11-15 12:10:00.000000 as_seg-0.1.4/as_seg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 12:10:00.000000 as_seg-0.1.4/as_seg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-11-15 12:10:00.000000 as_seg-0.1.4/as_seg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-15 12:10:00.000000 as_seg-0.1.4/as_seg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-15 12:10:00.942295 as_seg-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-11-15 12:08:54.000000 as_seg-0.1.4/setup.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       90 2023-11-15 10:18:55.000000 as_seg-0.1.5/AUTHORS
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1516 2023-11-15 10:18:55.000000 as_seg-0.1.5/LICENSE.md
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-04-25 15:34:36.736010 as_seg-0.1.5/PKG-INFO
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     3440 2023-12-18 15:34:55.000000 as_seg-0.1.5/README.md
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    24645 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/CBM_algorithm.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      289 2023-11-16 18:06:00.000000 as_seg-0.1.5/as_seg/__init__.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     9650 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/autosimilarity_computation.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     7606 2023-12-20 10:11:43.000000 as_seg-0.1.5/as_seg/barwise_input.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    26568 2023-12-20 14:33:07.000000 as_seg-0.1.5/as_seg/data_manipulation.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6765 2023-11-15 11:49:38.000000 as_seg-0.1.5/as_seg/example.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    15361 2023-11-20 15:28:34.000000 as_seg-0.1.5/as_seg/foote_novelty.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/model/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       78 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/__init__.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6046 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/current_plot.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1773 2023-11-17 10:45:00.000000 as_seg-0.1.5/as_seg/model/display_results.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      568 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/errors.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    17519 2023-11-15 11:53:20.000000 as_seg-0.1.5/as_seg/model/features.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/scripts/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)        0 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/scripts/__init__.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1965 2024-01-10 12:12:43.000000 as_seg-0.1.5/as_seg/scripts/default_path.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    30588 2023-11-16 19:04:30.000000 as_seg-0.1.5/as_seg/scripts/overall_scripts.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg.egg-info/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      586 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/SOURCES.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/dependency_links.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      147 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/requires.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        7 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/top_level.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-04-25 15:34:36.736010 as_seg-0.1.5/setup.cfg
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1359 2024-04-25 15:31:49.000000 as_seg-0.1.5/setup.py
```

### Comparing `as_seg-0.1.4/LICENSE.md` & `as_seg-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/PKG-INFO` & `as_seg-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-Metadata-Version: 2.1
-Name: as_seg
-Version: 0.1.4
-Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
-Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
-Author: Marmoret Axel
-Author-email: axel.marmoret@imt-atlantique.fr
-License: BSD
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: AUTHORS
-
-# as_seg: module for computing and segmenting autosimilarity matrices. #
-
-Hello, and welcome on this repository!
-
-This project aims at computing autosimilarity matrices, and segmenting them, which consists of the task of structural segmentation.
-
-The current version contains the CBM algorithm [1], along with a (low-effort) implementation of Foote's novelty algorithm [2].
-
-It can be installed using pip as `pip install as-seg`.
-
-This is a first release, and may contain bug. Comments are welcomed!
-
-## Tutorial notebook ##
-
-A tutorial notebook presenting the most important components of this toolbox is available in the folder "Notebooks".
-
-## Experimental notebook ##
-
-Experimental notebooks are available in the folder "Notebooks". They present the code used to compute the main experiments of the paper, in order to improve the reproducibility. Please tell me if any problem would appear when trying to launch them.
-
-## Data ##
-
-Some data is available with the code, in the folder "data". This includes the bar estimates, obtained with the madmom toolbox [3], the Barwise TF matrices, which are the barwise pre-processed versions of the spectrograms we use to estimate boundaries, and the estimated boundaries obtained with the CBM algorithm in the different conditions.
-
-## Software version ##
-
-This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
-
-## How to cite ##
-
-You should cite the package `as_seg`, available on HAL (https://hal.archives-ouvertes.fr/hal-03797507).
-
-Here are two styles of citations:
-
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/autosimilarity_segmentation}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
-
-In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices," 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
-
-## Credits ##
-
-Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
-
-The technique in itself was also developed by FrÃ©dÃ©ric Bimbot (<bimbot@irisa.fr>).
-
-## References ##
-[1] A. Marmoret, J.E. Cohen, and F. Bimbot, "Convolutive Block-Matching Segmentation Algorithm with Application to Music Structure Analysis", 2023, to be published at WASPAA 2023.
-
-[2] J. Foote, "Automatic audio segmentation using a measure of audio novelty," in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000, pp. 452â€“455.
-
-[3] BÃ¶ck, S., Korzeniowski, F., SchlÃ¼ter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+Metadata-Version: 2.1
+Name: as_seg
+Version: 0.1.5
+Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
+Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
+Author: Marmoret Axel
+Author-email: axel.marmoret@imt-atlantique.fr
+License: BSD
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS
+
+# as_seg: module for computing and segmenting autosimilarity matrices. #
+
+Hello, and welcome on this repository!
+
+This project aims at computing autosimilarity matrices, and segmenting them, which consists of the task of structural segmentation.
+
+The current version contains the CBM algorithm [1], along with an implementation of Foote's novelty algorithm [2] based on the MSAF toolbox [3].
+
+It can be installed using pip as `pip install as-seg`.
+
+This is a first release, and may contain bug. Comments are welcomed!
+
+## Tutorial notebook ##
+
+A tutorial notebook presenting the most important components of this toolbox is available in the folder "Notebooks".
+
+## Experimental notebook ##
+
+Experimental notebooks are available in the folder "Notebooks". They present the code used to compute the main experiments of the paper, in order to improve the reproducibility. Please tell me if any problem would appear when trying to launch them.
+
+Experimental Notebooks requires some pre-computed data to work, which can be found on zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
+
+## Data ##
+
+Should be obtained from Zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
+
+## Software version ##
+
+This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
+
+## How to cite ##
+
+You should cite the package `as_seg`, available on HAL (https://hal.archives-ouvertes.fr/hal-03797507).
+
+Here are two styles of citations:
+
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+
+In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices," 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+
+## Credits ##
+
+Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
+
+The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
+
+## References ##
+[1] A. Marmoret, J.E. Cohen, F. Bimbot. Barwise Music Structure Analysis with the Correlation Block-Matching Segmentation Algorithm. Transactions of the International Society for Music Information Retrieval (TISMIR), 2023, 6 (1), pp.167-185. ⟨10.5334/tismir.167⟩. ⟨hal-04323556⟩, https://hal.science/hal-04323556.
+
+[2] J. Foote, "Automatic audio segmentation using a measure of audio novelty," in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000, pp. 452–455.
+
+[3] Nieto, O., Bello, J. P., Systematic Exploration Of Computational Music Structure Research. Proc. of the 17th International Society for Music Information Retrieval Conference (ISMIR). New York City, NY, USA, 2016.
+
+[4] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+
+
```

### Comparing `as_seg-0.1.4/README.md` & `as_seg-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 # as_seg: module for computing and segmenting autosimilarity matrices. #
 
 Hello, and welcome on this repository!
 
 This project aims at computing autosimilarity matrices, and segmenting them, which consists of the task of structural segmentation.
 
-The current version contains the CBM algorithm [1], along with a (low-effort) implementation of Foote's novelty algorithm [2].
+The current version contains the CBM algorithm [1], along with an implementation of Foote's novelty algorithm [2] based on the MSAF toolbox [3].
 
 It can be installed using pip as `pip install as-seg`.
 
 This is a first release, and may contain bug. Comments are welcomed!
 
 ## Tutorial notebook ##
 
 A tutorial notebook presenting the most important components of this toolbox is available in the folder "Notebooks".
 
 ## Experimental notebook ##
 
 Experimental notebooks are available in the folder "Notebooks". They present the code used to compute the main experiments of the paper, in order to improve the reproducibility. Please tell me if any problem would appear when trying to launch them.
 
+Experimental Notebooks requires some pre-computed data to work, which can be found on zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
+
 ## Data ##
 
-Some data is available with the code, in the folder "data". This includes the bar estimates, obtained with the madmom toolbox [3], the Barwise TF matrices, which are the barwise pre-processed versions of the spectrograms we use to estimate boundaries, and the estimated boundaries obtained with the CBM algorithm in the different conditions.
+Should be obtained from Zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
 
 ## Software version ##
 
 This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
 
 ## How to cite ##
 
 You should cite the package `as_seg`, available on HAL (https://hal.archives-ouvertes.fr/hal-03797507).
 
 Here are two styles of citations:
 
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/autosimilarity_segmentation}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
 
 In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices," 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
 
 ## Credits ##
 
 Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
 
 The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
 
 ## References ##
-[1] A. Marmoret, J.E. Cohen, and F. Bimbot, "Convolutive Block-Matching Segmentation Algorithm with Application to Music Structure Analysis", 2023, to be published at WASPAA 2023.
+[1] A. Marmoret, J.E. Cohen, F. Bimbot. Barwise Music Structure Analysis with the Correlation Block-Matching Segmentation Algorithm. Transactions of the International Society for Music Information Retrieval (TISMIR), 2023, 6 (1), pp.167-185. ⟨10.5334/tismir.167⟩. ⟨hal-04323556⟩, https://hal.science/hal-04323556.
 
 [2] J. Foote, "Automatic audio segmentation using a measure of audio novelty," in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000, pp. 452–455.
 
-[3] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+[3] Nieto, O., Bello, J. P., Systematic Exploration Of Computational Music Structure Research. Proc. of the 17th International Society for Music Information Retrieval Conference (ISMIR). New York City, NY, USA, 2016.
+
+[4] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
```

### Comparing `as_seg-0.1.4/as_seg/CBM_algorithm.py` & `as_seg-0.1.5/as_seg/CBM_algorithm.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg/autosimilarity_computation.py` & `as_seg-0.1.5/as_seg/autosimilarity_computation.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg/barwise_input.py` & `as_seg-0.1.5/as_seg/barwise_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,7 +174,10 @@
 
     # Assign times (and add last time if padded)
     beatsync_times = np.copy(beat_times)
     if beatsync_times.shape[0] != beatsync_feats.shape[0]:
         beatsync_times = np.concatenate((beatsync_times,
                                          [frame_times[-1]]))
     return beatsync_feats, beatsync_times
+
+if __name__ == "__main__":
+    print("HelloWorld")
```

### Comparing `as_seg-0.1.4/as_seg/data_manipulation.py` & `as_seg-0.1.5/as_seg/data_manipulation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,645 +1,707 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Feb 21 15:09:10 2020
-
-@author: amarmore
-
-A file which contains all code regarding conversion of data, or information extraction from it
-(typically getting the bars, converting segments in frontiers, sonifying segmentation or computing its Hit-Rate score, etc).
-"""
-
-import as_seg.model.errors as err
-
-import numpy as np
-import madmom.features.downbeats as dbt
-import madmom.features.beats as bt
-import mir_eval
-import scipy
-import librosa
-
-# %% Read and treat inputs
-def get_bars_from_audio(song_path):
-    """
-    Returns the bars of a song, directly from its audio signal.
-    Encapsulates the downbeat estimator from the madmom toolbox [1].
-    
-    NB1: Note that the estimation implicitely assumes 3 or 4 beats per bar.
-    
-    NB2: Note also that this function artificially adds bars at the end of the song, so that the estimation spans the entire song length.
-    May/should be debated.
-
-    Parameters
-    ----------
-    song_path : String
-        Path to the desired song.
-
-    Returns
-    -------
-    downbeats_times : list of tuples of float
-        List of the estimated bars, as (start, end) times.
-        
-    References
-    ----------
-    [1] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). 
-    Madmom: A new python audio and music signal processing library. 
-    In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
-
-    """
-    act = dbt.RNNDownBeatProcessor()(song_path)
-    proc = dbt.DBNDownBeatTrackingProcessor(beats_per_bar=[3,4], fps=100)
-    song_beats = proc(act)
-    downbeats_times = []
-    
-    if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
-        downbeats_times.append(0.1)
-    for beat in song_beats:
-        if beat[1] == 1: # If the beat is a downbeat
-            downbeats_times.append(beat[0])
-            
-    # The following block of code artificially adds bars to the end of the song, in order to span the total song length.
-    # It seems like a good idea initially but may be detrimental, and should be debated anyway.
-    average_bar_length = np.mean([downbeats_times[i + 1] - downbeats_times[i] for i in range(len(downbeats_times) - 1)]) # average bar length in the song
-    song_length = act.shape[0]/100 # Total length of the song
-    while downbeats_times[-1] + 1.1*average_bar_length < song_length: # As long as the bar estimation does not cover the entire song
-        downbeats_times.append(round(downbeats_times[-1] + average_bar_length, 2)) # artifically adds bars of the length of the average bar length in the song
-    downbeats_times.append(song_length) # adding the last downbeat
-    
-    return frontiers_to_segments(downbeats_times)
-    
-def get_beats_from_audio_msaf(signal, sr, hop_length):
-    _, audio_percussive = librosa.effects.hpss(signal)
-    
-    # Compute beats
-    _, beat_frames = librosa.beat.beat_track(y=audio_percussive, sr=sr, hop_length=hop_length)
-
-    # To times
-    beat_times = librosa.frames_to_time(beat_frames, sr=sr,hop_length=hop_length)
-
-    # TODO: Is this really necessary?
-    if len(beat_times) > 0 and beat_times[0] == 0:
-        beat_times = beat_times[1:]
-        beat_frames = beat_frames[1:]
-        
-    return beat_times, beat_frames
-    
-# %% Read and treat inputs
-def get_beats_from_audio_madmom(song_path):
-    """
-    TODO
-    """
-    act = bt.TCNBeatProcessor()(song_path)
-    proc = bt.BeatTrackingProcessor(fps=100)
-    song_beats = proc(act)
-    beats_times = []
-    
-    # if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
-        # beats_times.append(0.1)
-    # for beat in song_beats:
-        # if beat[1] == 1: # If the beat is a downbeat
-            # downbeats_times.append(beat[0])
-            
-    return frontiers_to_segments(list(song_beats))
-
-def get_segmentation_from_txt(path, annotations_type):
-    """
-    Reads the segmentation annotations, and returns it in a list of tuples (start, end, index as a number)
-    This function has been developped for AIST and MIREX10 annotations, adapted for these types of annotations.
-    It will not work with another set of annotation.
-
-    Parameters
-    ----------
-    path : String
-        The path to the annotation.
-    annotations_type : "AIST" [1] or "MIREX10" [2]
-        The type of annotations to load (both have a specific behavior and formatting)
-        
-    Raises
-    ------
-    err.InvalidArgumentValueException
-        If the type of annotations is neither AIST or MIREX10
-
-    Returns
-    -------
-    segments : list of tuples (float, float, integer)
-        The segmentation, formatted in a list of tuples, and with labels as numbers (easier to interpret computationnally).
-
-    References
-    ----------
-    [1] Goto, M. (2006, October). AIST Annotation for the RWC Music Database. In ISMIR (pp. 359-360).
-    
-    [2] Bimbot, F., Sargent, G., Deruty, E., Guichaoua, C., & Vincent, E. (2014, January). 
-    Semiotic description of music structure: An introduction to the Quaero/Metiss structural annotations.
-
-    """
-    file_seg = open(path)
-    segments = []
-    labels = []
-    for part in file_seg.readlines():
-        tupl = part.split("\t")
-        if tupl[2] not in labels: # If label wasn't already found in this annotation
-            idx = len(labels)
-            labels.append(tupl[2])
-        else: # If this label was found for another segment
-            idx = labels.index(tupl[2])
-        if annotations_type == "AIST":
-            segments.append(((int(tupl[0]) / 100), (int(tupl[1]) / 100), idx))
-        elif annotations_type == "MIREX10":
-            segments.append((round(float(tupl[0]), 3), round(float(tupl[1]), 3), idx))
-        else:
-            raise err.InvalidArgumentValueException("Annotations type not understood")
-    return segments
-
-def get_annotation_name_from_song(song_number, annotations_type):
-    """
-    Returns the name of the annotation of this song according to the desired annotation type
-    
-    Specificly designed for RWC Pop dataset, shouldn't be used otherwise.
-    For now are available:
-        - AIST annotations [1]
-        - MIREX 10 annotations [2]
-    
-    Parameters
-    ----------
-    song_number : integer or string
-        The number of the song (which is its name).
-    annotations_type : string
-        The desired type of annotation.
-
-    Raises
-    ------
-    InvalidArgumentValueException
-        If the annotatipn type is not implemented.
-
-    Returns
-    -------
-    string
-        The name of the file containing the annotation.
-        
-    References
-    ----------
-    [1] Goto, M. (2006, October). AIST Annotation for the RWC Music Database. In ISMIR (pp. 359-360).
-    
-    [2] Bimbot, F., Sargent, G., Deruty, E., Guichaoua, C., & Vincent, E. (2014, January). 
-    Semiotic description of music structure: An introduction to the Quaero/Metiss structural annotations.
-
-    """
-    if annotations_type == "MIREX10":
-        return "RM-P{:03d}.BLOCKS.lab".format(int(song_number))
-    elif annotations_type == "AIST":
-        return "RM-P{:03d}.CHORUS.TXT".format(int(song_number))
-    else:
-        raise err.InvalidArgumentValueException("Annotations type not understood")
-
-# %% Conversion of data (time/frame/beat and segment/frontiers)
-def frontiers_from_time_to_frame_idx(seq, hop_length_seconds):
-    """
-    Converts a sequence of frontiers in time to their values in frame indexes.
-
-    Parameters
-    ----------
-    seq : list of float/times
-        The list of times to convert.
-    hop_length_seconds : float
-        hop_length (time between two consecutive frames), in seconds.
-
-    Returns
-    -------
-    list of integers
-        The sequence, as a list, in frame indexes.
-    """
-    
-    return [int(round(frontier/hop_length_seconds)) for frontier in seq]
-
-def segments_from_time_to_frame_idx(segments, hop_length_seconds):
-    """
-    Converts a sequence of segments (start, end) in time to their values in frame indexes.
-
-    Parameters
-    ----------
-    segements : list of tuple
-        The list of segments, as tuple (start, end), to convert.
-    hop_length_seconds : float
-        hop_length (time between two consecutive frames), in seconds.
-
-    Returns
-    -------
-    list of integers
-        The sequence, as a list, in frame indexes.
-    """
-    to_return = []
-    for segment in segments:
-        bar_in_frames = [int(round(segment[0]/hop_length_seconds)), int(round(segment[1]/hop_length_seconds))]
-        if bar_in_frames[0] != bar_in_frames[1]:
-            to_return.append(bar_in_frames)
-    return to_return
-    
-def segments_from_time_to_bar(segments, bars):
-    """
-    Converts the segments in time to segments in bar indexes.
-    The selected bar is the one which end is the closest from the frontier.
-
-    Parameters
-    ----------
-    segments : list of tuples
-        The list of segments, in time.
-    bars : list of tuple of floats
-        The bars, as (start time, end time) tuples.
-
-    Returns
-    -------
-    list of tuples of integers
-        List of time instances (start, end) converted in bar indexes.
-
-    """
-    frontiers = segments_to_frontiers(segments)
-    return np.array(frontiers_to_segments(frontiers_from_time_to_bar(frontiers, bars)))
-
-def frontiers_from_time_to_bar(seq, bars):
-    """
-    Converts the frontiers in time to a bar index.
-    The selected bar is the one which end is the closest from the frontier.
-
-    Parameters
-    ----------
-    seq : list of float
-        The list of frontiers, in time.
-    bars : list of tuple of floats
-        The bars, as (start time, end time) tuples.
-
-    Returns
-    -------
-    seq_barwise : list of integers
-        List of times converted in bar indexes.
-
-    """
-    seq_barwise = []
-    for frontier in seq:
-        for idx, bar in enumerate(bars):
-            if frontier >= bar[0] and frontier < bar[1]:
-                if bar[1] - frontier < frontier - bar[0]:
-                    seq_barwise.append(idx)
-                else:
-                    if idx == 0:
-                        seq_barwise.append(idx)
-                        #print("The current frontier {} is labelled in the start silence ({},{}), which is incorrect.".format(frontier, bar[0], bar[1]))
-                    else:
-                        seq_barwise.append(idx - 1)
-                break
-    return seq_barwise
-
-def frontiers_from_bar_to_time(seq, bars):
-    """
-    Converts the frontiers (or a sequence of integers) from bar indexes to absolute times of the bars.
-    The frontier is considered as the end of the bar.
-
-    Parameters
-    ----------
-    seq : list of integers
-        The frontiers, in bar indexes.
-    bars : list of tuple of floats
-        The bars, as (start time, end time) tuples.
-
-    Returns
-    -------
-    to_return : list of float
-        The frontiers, converted in time (from bar indexes).
-
-    """
-    to_return = []
-    for frontier in seq:
-        bar_frontier = bars[frontier][1]
-        if bar_frontier not in to_return:
-            to_return.append(bar_frontier)
-    return to_return
-
-def segments_from_bar_to_time(segments, bars):
-    """
-    Converts segments from bar indexes to time.
-
-    Parameters
-    ----------
-    segments : list of tuple of integers
-        The indexes of the bars defining the segments (start, end).
-    bars : list of tuple of float
-        Bars, as tuples (start, end), in time.
-
-    Returns
-    -------
-    numpy array
-        Segments, in time.
-
-    """
-    to_return = []
-    for start, end in segments:
-        if end >= len(bars):
-            to_return.append([bars[start][1], bars[-1][1]])
-        else:
-            to_return.append([bars[start][1], bars[end][1]])
-    return np.array(to_return)
-    
-def frontiers_to_segments(frontiers):
-    """
-    Computes a list of segments starting from the frontiers between them.
-
-    Parameters
-    ----------
-    frontiers : list of floats
-        The list of frontiers.
-
-    Returns
-    -------
-    to_return : list of tuples of floats
-        The segments, as tuples (start, end).
-
-    """
-    to_return = []
-    while 0 in frontiers:
-        frontiers.remove(0)
-    to_return.append((0,frontiers[0]))
-    for idx in range(len(frontiers) - 1):
-        if frontiers[idx] != frontiers[idx + 1]:
-            to_return.append((frontiers[idx], frontiers[idx + 1]))
-    return to_return
-
-def segments_to_frontiers(segments):
-    """
-    Computes a list of frontiers from the segments.
-
-    Parameters
-    ----------
-    segments : list of tuples of floats
-        The segments, as tuples.
-
-    Returns
-    -------
-    list
-        Frontiers between segments.
-
-    """
-    return [i[1] for i in segments]
-
-def align_segments_on_bars(segments, bars):
-    """
-    Aligns the estimated segments to the closest bars (in time).
-    The idea is that segments generally start and end on downbeats,
-    and that realigning the estimation could improve perfomance for low tolerances scores.
-    Generally used for comparison with techniques which don't align their segmentation on bars.
-
-    Parameters
-    ----------
-    segments : list of tuple of float
-        Time of the estimated segments, as (start, end).
-    bars : list of tuple of float
-        The bars of the signal.
-
-    Returns
-    -------
-    list of tuple of floats
-        Segments, realigned on bars.
-
-    """
-    frontiers = segments_to_frontiers(segments)
-    return frontiers_to_segments(align_frontiers_on_bars(frontiers, bars))
-
-def align_frontiers_on_bars(frontiers, bars):
-    """
-    Aligns the frontiers of segments to the closest bars (in time).
-    The idea is that frontiers generally occurs on downbeats,
-    and that realigning the estimation could improve perfomance for low tolerances scores.
-    Generally used for comparison with techniques which don't align their segmentation on bars.
-
-    Parameters
-    ----------
-    frontiers : list of float
-        Time of the estimated frontiers.
-    bars : list of tuple of float
-        The bars of the signal.
-
-    Returns
-    -------
-    frontiers_on_bars : list of floats
-        Frontiers, realigned on bars.
-
-    """
-    frontiers_on_bars = []
-    i = 1
-    for frontier in frontiers:
-        while i < len(bars) - 1 and bars[i][1] < frontier:
-            i+=1
-        if i == len(bars) - 1:
-            frontiers_on_bars.append(frontier)
-        else:
-            if bars[i][1] - frontier < frontier - bars[i][0]:
-                frontiers_on_bars.append(bars[i][1])
-            else:
-                frontiers_on_bars.append(bars[i][0])
-    return frontiers_on_bars
-            
-# %% Sonification of the segmentation
-def sonify_frontiers_path(audio_file_path, frontiers_in_seconds, output_path):
-    """
-    Takes the path of the song and frontiers, and write a song with the frontiers sonified ("bip" in the song).
-    Function inspired from MSAF.
-
-    Parameters
-    ----------
-    audio_file_path: String
-        The path to the song, (as signal).
-    frontiers_in_seconds: list of floats
-        The frontiers, in time/seconds.
-    output_path: String
-        The path where to write the song with sonified frontiers.
-
-    Returns
-    -------
-    Nothing, but writes a song at output_path
-
-    """
-    the_signal, sampling_rate = librosa.load(audio_file_path, sr=None)
-    sonify_frontiers_song(the_signal, sampling_rate, frontiers_in_seconds, output_path)
-
-def sonify_frontiers_song(song_signal, sampling_rate, frontiers_in_seconds, output_path):
-    """
-    Takes a song as a signal, and add the frontiers to this signal.
-    It then writes it as a file.
-    Function inspired from MSAF.
-
-    Parameters
-    ----------
-    song_signal : numpy array
-        The song as a signal.
-    sampling_rate : integer
-        The sampling rate of the signal, in Hz.
-    frontiers_in_seconds: list of floats
-        The frontiers, in time/seconds.
-    output_path: String
-        The path where to write the song with sonified frontiers.
-
-    Returns
-    -------
-    Nothing, but writes a song at the output_path.
-
-    """
-    frontiers_signal = mir_eval.sonify.clicks(frontiers_in_seconds, sampling_rate)
-    
-    singal_with_frontiers = np.zeros(max(len(song_signal[:,0]), len(frontiers_signal)))
-    
-    singal_with_frontiers[:len(song_signal[:,0])] = song_signal[:,0]
-    singal_with_frontiers[:len(frontiers_signal)] += frontiers_signal
-    
-    scipy.io.wavfile.write(output_path, sampling_rate, singal_with_frontiers)
-    
-# %% Score calculation encapsulation
-def compute_score_from_frontiers_in_bar(reference, frontiers_in_bar, bars, window_length = 0.5):
-    """
-    Computes precision, recall and f measure from estimated frontiers (in bar indexes) and the reference (in seconds).
-    Scores are computed from the mir_eval toolbox.
-
-    Parameters
-    ----------
-    reference : list of tuples
-        The reference annotations, as a list of tuples (start, end), in seconds.
-    frontiers : list of integers
-        The frontiers between segments, in bar indexes.
-    bars : list of tuples
-        The bars of the song.
-    window_length : float, optional
-        The window size for the score (tolerance for the frontier to be validated).
-        The default is 0.5.
-
-    Returns
-    -------
-    precision: float \in [0,1]
-        Precision of these frontiers,
-        ie the proportion of accurately found frontiers among all found frontiers.
-    recall: float \in [0,1]
-        Recall of these frontiers,
-        ie the proportion of accurately found frontiers among all accurate frontiers.
-    f_measure: float \in [0,1]
-        F measure of these frontiers,
-        ie the geometric mean of both precedent scores.
-        
-    """
-    try:
-        np.array(bars).shape[1]
-    except:
-        raise err.OutdatedBehaviorException("Bars is still a list of downbeats, which is an old beavior, and shouldn't happen anymore. To track and to fix.")
-    frontiers_in_time = frontiers_from_bar_to_time(frontiers_in_bar, bars)
-    return compute_score_of_segmentation(reference, frontiers_to_segments(frontiers_in_time), window_length = window_length)
-
-def compute_score_of_segmentation(reference, segments_in_time, window_length = 0.5):
-    """
-    Computes precision, recall and f measure from estimated segments and the reference, both in seconds.    
-    Scores are computed from the mir_eval toolbox.
-
-    Parameters
-    ----------
-    reference : list of tuples
-        The reference annotations, as a list of tuples (start, end), in seconds.
-    segments_in_time : list of tuples
-        The segments, in seconds, as tuples (start, end).
-    window_length : float, optional
-        The window size for the score (tolerance for the frontier to be validated).
-        The default is 0.5.
-
-    Returns
-    -------
-    precision: float \in [0,1]
-        Precision of these frontiers,
-        ie the proportion of accurately found frontiers among all found frontiers.
-    recall: float \in [0,1]
-        Recall of these frontiers,
-        ie the proportion of accurately found frontiers among all accurate frontiers.
-    f_measure: float \in [0,1]
-        F measure of these frontiers,
-        ie the geometric mean of both precedent scores.
-
-    """
-    ref_intervals, useless = mir_eval.util.adjust_intervals(reference,t_min=0)
-    est_intervals, useless = mir_eval.util.adjust_intervals(np.array(segments_in_time), t_min=0, t_max=ref_intervals[-1, 1])
-    try:
-        return mir_eval.segment.detection(ref_intervals, est_intervals, window = window_length, trim = False)
-    except ValueError:
-        cleaned_intervals = []
-        #print("A segment is (probably) composed of the same start and end. Can happen with time -> bar -> time conversion, but should'nt happen for data originally segmented in bars.")
-        for idx in range(len(est_intervals)):
-            if est_intervals[idx][0] != est_intervals[idx][1]:
-                cleaned_intervals.append(est_intervals[idx])
-        return mir_eval.segment.detection(ref_intervals, np.array(cleaned_intervals), window = window_length, trim = False)
-
-def compute_median_deviation_of_segmentation(reference, segments_in_time):
-    """
-    TODO
-
-    Parameters
-    ----------
-    reference : list of tuples
-        The reference annotations, as a list of tuples (start, end), in seconds.
-    segments_in_time : list of tuples
-        The segments, in seconds, as tuples (start, end).
-
-    Returns
-    -------
-    TODO
-    r_to_e then e_to_r
-
-    """
-    ref_intervals, useless = mir_eval.util.adjust_intervals(reference,t_min=0)
-    est_intervals, useless = mir_eval.util.adjust_intervals(np.array(segments_in_time), t_min=0, t_max=ref_intervals[-1, 1])
-    try:
-        return mir_eval.segment.deviation(ref_intervals,est_intervals)
-    except ValueError:
-        cleaned_intervals = []
-        for idx in range(len(est_intervals)):
-            if est_intervals[idx][0] != est_intervals[idx][1]:
-                cleaned_intervals.append(est_intervals[idx])
-        return mir_eval.segment.deviation(ref_intervals,est_intervals)
-
-def compute_rates_of_segmentation(reference, segments_in_time, window_length = 0.5):
-    """
-    Computes True Positives, False Positives and False Negatives from estimated segments and the reference, both in seconds.    
-    Scores are computed from the mir_eval toolbox. (In fact, the code is extracted from mir_eval.segment.detection)
-
-    Parameters
-    ----------
-    reference : list of tuples
-        The reference annotations, as a list of tuples (start, end), in seconds.
-    segments_in_time : list of tuples
-        The segments, in seconds, as tuples (start, end).
-    window_length : float, optional
-        The window size for the score (tolerance for the frontier to be validated).
-        The default is 0.5.
-
-    Returns
-    -------
-    True Positives: Integer
-        The number of True Positives, 
-        ie the number of accurately found frontiers.
-    False Positives: Integer
-        The number of False Positives,
-        ie the number of wrongly found frontiers (estimated frontiers which are incorrect).
-    False Negative : Integer
-        The number of False Negatives,
-        ie the number of frontiers undetected (accurate frontiers which are not found in teh estimation).
-
-    """  
-    reference_intervals, _ = mir_eval.util.adjust_intervals(reference,t_min=0)
-    estimated_intervals, _ = mir_eval.util.adjust_intervals(segments_in_time, t_min=0, t_max=reference_intervals[-1, 1])
-    
-    mir_eval.segment.validate_boundary(reference_intervals, estimated_intervals, False)
-
-    # Convert intervals to boundaries
-    reference_boundaries = mir_eval.util.intervals_to_boundaries(reference_intervals)
-    estimated_boundaries = mir_eval.util.intervals_to_boundaries(estimated_intervals)
-
-    # If we have no boundaries, we get no score.
-    if len(reference_boundaries) == 0 or len(estimated_boundaries) == 0:
-        return 0, 0, 0
-
-    tp = len(mir_eval.util.match_events(reference_boundaries,estimated_boundaries,window_length))
-    fp = len(estimated_boundaries) - tp
-    fn = len(reference_boundaries) - tp
-    
-    return tp, fp, fn
-        
-
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Feb 21 15:09:10 2020
+
+@author: amarmore
+
+A file which contains all code regarding conversion of data, or information extraction from it
+(typically getting the bars, converting segments in frontiers, sonifying segmentation or computing its Hit-Rate score, etc).
+"""
+
+import as_seg.model.errors as err
+
+import numpy as np
+import madmom.features.downbeats as dbt
+import madmom.features.beats as bt
+import mir_eval
+import scipy
+import librosa
+import math
+
+# %% Read and treat inputs
+def get_bars_from_audio(song_path):
+    """
+    Returns the bars of a song, directly from its audio signal.
+    Encapsulates the downbeat estimator from the madmom toolbox [1].
+    
+    NB1: Note that the estimation implicitely assumes 3 or 4 beats per bar.
+    
+    NB2: Note also that this function artificially adds bars at the end of the song, so that the estimation spans the entire song length.
+    May/should be debated.
+
+    Parameters
+    ----------
+    song_path : String
+        Path to the desired song.
+
+    Returns
+    -------
+    downbeats_times : list of tuples of float
+        List of the estimated bars, as (start, end) times.
+        
+    References
+    ----------
+    [1] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). 
+    Madmom: A new python audio and music signal processing library. 
+    In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+
+    """
+    act = dbt.RNNDownBeatProcessor()(song_path)
+    proc = dbt.DBNDownBeatTrackingProcessor(beats_per_bar=[3,4], fps=100)
+    song_beats = proc(act)
+    downbeats_times = []
+    
+    if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
+        downbeats_times.append(0.1)
+    for beat in song_beats:
+        if beat[1] == 1: # If the beat is a downbeat
+            downbeats_times.append(beat[0])
+            
+    # The following block of code artificially adds bars to the end of the song, in order to span the total song length.
+    # It seems like a good idea initially but may be detrimental, and should be debated anyway.
+    average_bar_length = np.mean([downbeats_times[i + 1] - downbeats_times[i] for i in range(len(downbeats_times) - 1)]) # average bar length in the song
+    song_length = act.shape[0]/100 # Total length of the song
+    while downbeats_times[-1] + 1.1*average_bar_length < song_length: # As long as the bar estimation does not cover the entire song
+        downbeats_times.append(round(downbeats_times[-1] + average_bar_length, 2)) # artifically adds bars of the length of the average bar length in the song
+    downbeats_times.append(song_length) # adding the last downbeat
+    
+    return frontiers_to_segments(downbeats_times)
+    
+def get_beats_from_audio_msaf(signal, sr, hop_length):
+    _, audio_percussive = librosa.effects.hpss(signal)
+    
+    # Compute beats
+    _, beat_frames = librosa.beat.beat_track(y=audio_percussive, sr=sr, hop_length=hop_length)
+
+    # To times
+    beat_times = librosa.frames_to_time(beat_frames, sr=sr,hop_length=hop_length)
+
+    # TODO: Is this really necessary?
+    if len(beat_times) > 0 and beat_times[0] == 0:
+        beat_times = beat_times[1:]
+        beat_frames = beat_frames[1:]
+        
+    return beat_times, beat_frames
+    
+# %% Read and treat inputs
+def get_beats_from_audio_madmom(song_path):
+    """
+    TODO
+    """
+    act = bt.TCNBeatProcessor()(song_path)
+    proc = bt.BeatTrackingProcessor(fps=100)
+    song_beats = proc(act)
+    beats_times = []
+    
+    # if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
+        # beats_times.append(0.1)
+    # for beat in song_beats:
+        # if beat[1] == 1: # If the beat is a downbeat
+            # downbeats_times.append(beat[0])
+            
+    return frontiers_to_segments(list(song_beats))
+
+def get_segmentation_from_txt(path, annotations_type):
+    """
+    Reads the segmentation annotations, and returns it in a list of tuples (start, end, index as a number)
+    This function has been developped for AIST and MIREX10 annotations, adapted for these types of annotations.
+    It will not work with another set of annotation.
+
+    Parameters
+    ----------
+    path : String
+        The path to the annotation.
+    annotations_type : "AIST" [1] or "MIREX10" [2]
+        The type of annotations to load (both have a specific behavior and formatting)
+        
+    Raises
+    ------
+    err.InvalidArgumentValueException
+        If the type of annotations is neither AIST or MIREX10
+
+    Returns
+    -------
+    segments : list of tuples (float, float, integer)
+        The segmentation, formatted in a list of tuples, and with labels as numbers (easier to interpret computationnally).
+
+    References
+    ----------
+    [1] Goto, M. (2006, October). AIST Annotation for the RWC Music Database. In ISMIR (pp. 359-360).
+    
+    [2] Bimbot, F., Sargent, G., Deruty, E., Guichaoua, C., & Vincent, E. (2014, January). 
+    Semiotic description of music structure: An introduction to the Quaero/Metiss structural annotations.
+
+    """
+    file_seg = open(path)
+    segments = []
+    labels = []
+    for part in file_seg.readlines():
+        tupl = part.split("\t")
+        if tupl[2] not in labels: # If label wasn't already found in this annotation
+            idx = len(labels)
+            labels.append(tupl[2])
+        else: # If this label was found for another segment
+            idx = labels.index(tupl[2])
+        if annotations_type == "AIST":
+            segments.append(((int(tupl[0]) / 100), (int(tupl[1]) / 100), idx))
+        elif annotations_type == "MIREX10":
+            segments.append((round(float(tupl[0]), 3), round(float(tupl[1]), 3), idx))
+        else:
+            raise err.InvalidArgumentValueException("Annotations type not understood")
+    return segments
+
+def get_annotation_name_from_song(song_number, annotations_type):
+    """
+    Returns the name of the annotation of this song according to the desired annotation type
+    
+    Specificly designed for RWC Pop dataset, shouldn't be used otherwise.
+    For now are available:
+        - AIST annotations [1]
+        - MIREX 10 annotations [2]
+    
+    Parameters
+    ----------
+    song_number : integer or string
+        The number of the song (which is its name).
+    annotations_type : string
+        The desired type of annotation.
+
+    Raises
+    ------
+    InvalidArgumentValueException
+        If the annotatipn type is not implemented.
+
+    Returns
+    -------
+    string
+        The name of the file containing the annotation.
+        
+    References
+    ----------
+    [1] Goto, M. (2006, October). AIST Annotation for the RWC Music Database. In ISMIR (pp. 359-360).
+    
+    [2] Bimbot, F., Sargent, G., Deruty, E., Guichaoua, C., & Vincent, E. (2014, January). 
+    Semiotic description of music structure: An introduction to the Quaero/Metiss structural annotations.
+
+    """
+    if annotations_type == "MIREX10":
+        return "RM-P{:03d}.BLOCKS.lab".format(int(song_number))
+    elif annotations_type == "AIST":
+        return "RM-P{:03d}.CHORUS.TXT".format(int(song_number))
+    else:
+        raise err.InvalidArgumentValueException("Annotations type not understood")
+
+# %% Conversion of data (time/frame/beat and segment/frontiers)
+def frontiers_from_time_to_frame_idx(seq, hop_length_seconds):
+    """
+    Converts a sequence of frontiers in time to their values in frame indexes.
+
+    Parameters
+    ----------
+    seq : list of float/times
+        The list of times to convert.
+    hop_length_seconds : float
+        hop_length (time between two consecutive frames), in seconds.
+
+    Returns
+    -------
+    list of integers
+        The sequence, as a list, in frame indexes.
+    """
+    
+    return [int(round(frontier/hop_length_seconds)) for frontier in seq]
+
+def segments_from_time_to_frame_idx(segments, hop_length_seconds):
+    """
+    Converts a sequence of segments (start, end) in time to their values in frame indexes.
+
+    Parameters
+    ----------
+    segements : list of tuple
+        The list of segments, as tuple (start, end), to convert.
+    hop_length_seconds : float
+        hop_length (time between two consecutive frames), in seconds.
+
+    Returns
+    -------
+    list of integers
+        The sequence, as a list, in frame indexes.
+    """
+    to_return = []
+    for segment in segments:
+        bar_in_frames = [int(round(segment[0]/hop_length_seconds)), int(round(segment[1]/hop_length_seconds))]
+        if bar_in_frames[0] != bar_in_frames[1]:
+            to_return.append(bar_in_frames)
+    return to_return
+    
+def segments_from_time_to_bar(segments, bars):
+    """
+    Converts the segments in time to segments in bar indexes.
+    The selected bar is the one which end is the closest from the frontier.
+
+    Parameters
+    ----------
+    segments : list of tuples
+        The list of segments, in time.
+    bars : list of tuple of floats
+        The bars, as (start time, end time) tuples.
+
+    Returns
+    -------
+    list of tuples of integers
+        List of time instances (start, end) converted in bar indexes.
+
+    """
+    frontiers = segments_to_frontiers(segments)
+    return np.array(frontiers_to_segments(frontiers_from_time_to_bar(frontiers, bars)))
+
+def frontiers_from_time_to_bar(seq, bars):
+    """
+    Converts the frontiers in time to a bar index.
+    The selected bar is the one which end is the closest from the frontier.
+
+    Parameters
+    ----------
+    seq : list of float
+        The list of frontiers, in time.
+    bars : list of tuple of floats
+        The bars, as (start time, end time) tuples.
+
+    Returns
+    -------
+    seq_barwise : list of integers
+        List of times converted in bar indexes.
+
+    """
+    seq_barwise = []
+    for frontier in seq:
+        for idx, bar in enumerate(bars):
+            if frontier >= bar[0] and frontier < bar[1]:
+                if bar[1] - frontier < frontier - bar[0]:
+                    seq_barwise.append(idx)
+                else:
+                    if idx == 0:
+                        seq_barwise.append(idx)
+                        #print("The current frontier {} is labelled in the start silence ({},{}), which is incorrect.".format(frontier, bar[0], bar[1]))
+                    else:
+                        seq_barwise.append(idx - 1)
+                break
+    return seq_barwise
+
+def frontiers_from_bar_to_time(seq, bars):
+    """
+    Converts the frontiers (or a sequence of integers) from bar indexes to absolute times of the bars.
+    The frontier is considered as the end of the bar.
+
+    Parameters
+    ----------
+    seq : list of integers
+        The frontiers, in bar indexes.
+    bars : list of tuple of floats
+        The bars, as (start time, end time) tuples.
+
+    Returns
+    -------
+    to_return : list of float
+        The frontiers, converted in time (from bar indexes).
+
+    """
+    to_return = []
+    for frontier in seq:
+        bar_frontier = bars[frontier][1]
+        if bar_frontier not in to_return:
+            to_return.append(bar_frontier)
+    return to_return
+
+def segments_from_bar_to_time(segments, bars):
+    """
+    Converts segments from bar indexes to time.
+
+    Parameters
+    ----------
+    segments : list of tuple of integers
+        The indexes of the bars defining the segments (start, end).
+    bars : list of tuple of float
+        Bars, as tuples (start, end), in time.
+
+    Returns
+    -------
+    numpy array
+        Segments, in time.
+
+    """
+    to_return = []
+    for start, end in segments:
+        if end >= len(bars):
+            to_return.append([bars[start][1], bars[-1][1]])
+        else:
+            to_return.append([bars[start][1], bars[end][1]])
+    return np.array(to_return)
+    
+def frontiers_to_segments(frontiers):
+    """
+    Computes a list of segments starting from the frontiers between them.
+
+    Parameters
+    ----------
+    frontiers : list of floats
+        The list of frontiers.
+
+    Returns
+    -------
+    to_return : list of tuples of floats
+        The segments, as tuples (start, end).
+
+    """
+    to_return = []
+    while 0 in frontiers:
+        frontiers.remove(0)
+    to_return.append((0,frontiers[0]))
+    for idx in range(len(frontiers) - 1):
+        if frontiers[idx] != frontiers[idx + 1]:
+            to_return.append((frontiers[idx], frontiers[idx + 1]))
+    return to_return
+
+def segments_to_frontiers(segments):
+    """
+    Computes a list of frontiers from the segments.
+
+    Parameters
+    ----------
+    segments : list of tuples of floats
+        The segments, as tuples.
+
+    Returns
+    -------
+    list
+        Frontiers between segments.
+
+    """
+    return [i[1] for i in segments]
+
+def align_segments_on_bars(segments, bars):
+    """
+    Aligns the estimated segments to the closest bars (in time).
+    The idea is that segments generally start and end on downbeats,
+    and that realigning the estimation could improve perfomance for low tolerances scores.
+    Generally used for comparison with techniques which don't align their segmentation on bars.
+
+    Parameters
+    ----------
+    segments : list of tuple of float
+        Time of the estimated segments, as (start, end).
+    bars : list of tuple of float
+        The bars of the signal.
+
+    Returns
+    -------
+    list of tuple of floats
+        Segments, realigned on bars.
+
+    """
+    frontiers = segments_to_frontiers(segments)
+    return frontiers_to_segments(align_frontiers_on_bars(frontiers, bars))
+
+def align_frontiers_on_bars(frontiers, bars):
+    """
+    Aligns the frontiers of segments to the closest bars (in time).
+    The idea is that frontiers generally occurs on downbeats,
+    and that realigning the estimation could improve perfomance for low tolerances scores.
+    Generally used for comparison with techniques which don't align their segmentation on bars.
+
+    Parameters
+    ----------
+    frontiers : list of float
+        Time of the estimated frontiers.
+    bars : list of tuple of float
+        The bars of the signal.
+
+    Returns
+    -------
+    frontiers_on_bars : list of floats
+        Frontiers, realigned on bars.
+
+    """
+    frontiers_on_bars = []
+    i = 1
+    for frontier in frontiers:
+        while i < len(bars) - 1 and bars[i][1] < frontier:
+            i+=1
+        if i == len(bars) - 1:
+            frontiers_on_bars.append(frontier)
+        else:
+            if bars[i][1] - frontier < frontier - bars[i][0]:
+                frontiers_on_bars.append(bars[i][1])
+            else:
+                frontiers_on_bars.append(bars[i][0])
+    return frontiers_on_bars
+            
+# %% Sonification of the segmentation
+def sonify_frontiers_path(audio_file_path, frontiers_in_seconds, output_path):
+    """
+    Takes the path of the song and frontiers, and write a song with the frontiers sonified ("bip" in the song).
+    Function inspired from MSAF.
+
+    Parameters
+    ----------
+    audio_file_path: String
+        The path to the song, (as signal).
+    frontiers_in_seconds: list of floats
+        The frontiers, in time/seconds.
+    output_path: String
+        The path where to write the song with sonified frontiers.
+
+    Returns
+    -------
+    Nothing, but writes a song at output_path
+
+    """
+    the_signal, sampling_rate = librosa.load(audio_file_path, sr=None)
+    sonify_frontiers_song(the_signal, sampling_rate, frontiers_in_seconds, output_path)
+
+def sonify_frontiers_song(song_signal, sampling_rate, frontiers_in_seconds, output_path):
+    """
+    Takes a song as a signal, and add the frontiers to this signal.
+    It then writes it as a file.
+    Function inspired from MSAF.
+
+    Parameters
+    ----------
+    song_signal : numpy array
+        The song as a signal.
+    sampling_rate : integer
+        The sampling rate of the signal, in Hz.
+    frontiers_in_seconds: list of floats
+        The frontiers, in time/seconds.
+    output_path: String
+        The path where to write the song with sonified frontiers.
+
+    Returns
+    -------
+    Nothing, but writes a song at the output_path.
+
+    """
+    frontiers_signal = mir_eval.sonify.clicks(frontiers_in_seconds, sampling_rate)
+    
+    singal_with_frontiers = np.zeros(max(len(song_signal[:,0]), len(frontiers_signal)))
+    
+    singal_with_frontiers[:len(song_signal[:,0])] = song_signal[:,0]
+    singal_with_frontiers[:len(frontiers_signal)] += frontiers_signal
+    
+    scipy.io.wavfile.write(output_path, sampling_rate, singal_with_frontiers)
+    
+# %% Score calculation encapsulation
+def compute_score_from_frontiers_in_bar(reference, frontiers_in_bar, bars, window_length = 0.5):
+    """
+    Computes precision, recall and f measure from estimated frontiers (in bar indexes) and the reference (in seconds).
+    Scores are computed from the mir_eval toolbox.
+
+    Parameters
+    ----------
+    reference : list of tuples
+        The reference annotations, as a list of tuples (start, end), in seconds.
+    frontiers : list of integers
+        The frontiers between segments, in bar indexes.
+    bars : list of tuples
+        The bars of the song.
+    window_length : float, optional
+        The window size for the score (tolerance for the frontier to be validated).
+        The default is 0.5.
+
+    Returns
+    -------
+    precision: float \in [0,1]
+        Precision of these frontiers,
+        ie the proportion of accurately found frontiers among all found frontiers.
+    recall: float \in [0,1]
+        Recall of these frontiers,
+        ie the proportion of accurately found frontiers among all accurate frontiers.
+    f_measure: float \in [0,1]
+        F measure of these frontiers,
+        ie the geometric mean of both precedent scores.
+        
+    """
+    try:
+        np.array(bars).shape[1]
+    except:
+        raise err.OutdatedBehaviorException("Bars is still a list of downbeats, which is an old beavior, and shouldn't happen anymore. To track and to fix.")
+    frontiers_in_time = frontiers_from_bar_to_time(frontiers_in_bar, bars)
+    return compute_score_of_segmentation(reference, frontiers_to_segments(frontiers_in_time), window_length = window_length)
+
+def compute_score_of_segmentation(reference, segments_in_time, window_length = 0.5):
+    """
+    Computes precision, recall and f measure from estimated segments and the reference, both in seconds.    
+    Scores are computed from the mir_eval toolbox.
+
+    Parameters
+    ----------
+    reference : list of tuples
+        The reference annotations, as a list of tuples (start, end), in seconds.
+    segments_in_time : list of tuples
+        The segments, in seconds, as tuples (start, end).
+    window_length : float, optional
+        The window size for the score (tolerance for the frontier to be validated).
+        The default is 0.5.
+
+    Returns
+    -------
+    precision: float \in [0,1]
+        Precision of these frontiers,
+        ie the proportion of accurately found frontiers among all found frontiers.
+    recall: float \in [0,1]
+        Recall of these frontiers,
+        ie the proportion of accurately found frontiers among all accurate frontiers.
+    f_measure: float \in [0,1]
+        F measure of these frontiers,
+        ie the geometric mean of both precedent scores.
+
+    """
+    ref_intervals, useless = mir_eval.util.adjust_intervals(reference,t_min=0)
+    est_intervals, useless = mir_eval.util.adjust_intervals(np.array(segments_in_time), t_min=0, t_max=ref_intervals[-1, 1])
+    try:
+        return mir_eval.segment.detection(ref_intervals, est_intervals, window = window_length, trim = False)
+    except ValueError:
+        cleaned_intervals = []
+        #print("A segment is (probably) composed of the same start and end. Can happen with time -> bar -> time conversion, but should'nt happen for data originally segmented in bars.")
+        for idx in range(len(est_intervals)):
+            if est_intervals[idx][0] != est_intervals[idx][1]:
+                cleaned_intervals.append(est_intervals[idx])
+        return mir_eval.segment.detection(ref_intervals, np.array(cleaned_intervals), window = window_length, trim = False)
+
+def compute_median_deviation_of_segmentation(reference, segments_in_time):
+    """
+    TODO
+
+    Parameters
+    ----------
+    reference : list of tuples
+        The reference annotations, as a list of tuples (start, end), in seconds.
+    segments_in_time : list of tuples
+        The segments, in seconds, as tuples (start, end).
+
+    Returns
+    -------
+    TODO
+    r_to_e then e_to_r
+
+    """
+    ref_intervals, useless = mir_eval.util.adjust_intervals(reference,t_min=0)
+    est_intervals, useless = mir_eval.util.adjust_intervals(np.array(segments_in_time), t_min=0, t_max=ref_intervals[-1, 1])
+    try:
+        return mir_eval.segment.deviation(ref_intervals,est_intervals)
+    except ValueError:
+        cleaned_intervals = []
+        for idx in range(len(est_intervals)):
+            if est_intervals[idx][0] != est_intervals[idx][1]:
+                cleaned_intervals.append(est_intervals[idx])
+        return mir_eval.segment.deviation(ref_intervals,est_intervals)
+
+def compute_rates_of_segmentation(reference, segments_in_time, window_length = 0.5):
+    """
+    Computes True Positives, False Positives and False Negatives from estimated segments and the reference, both in seconds.    
+    Scores are computed from the mir_eval toolbox. (In fact, the code is extracted from mir_eval.segment.detection)
+
+    Parameters
+    ----------
+    reference : list of tuples
+        The reference annotations, as a list of tuples (start, end), in seconds.
+    segments_in_time : list of tuples
+        The segments, in seconds, as tuples (start, end).
+    window_length : float, optional
+        The window size for the score (tolerance for the frontier to be validated).
+        The default is 0.5.
+
+    Returns
+    -------
+    True Positives: Integer
+        The number of True Positives, 
+        ie the number of accurately found frontiers.
+    False Positives: Integer
+        The number of False Positives,
+        ie the number of wrongly found frontiers (estimated frontiers which are incorrect).
+    False Negative : Integer
+        The number of False Negatives,
+        ie the number of frontiers undetected (accurate frontiers which are not found in teh estimation).
+
+    """  
+    reference_intervals, _ = mir_eval.util.adjust_intervals(reference,t_min=0)
+    estimated_intervals, _ = mir_eval.util.adjust_intervals(segments_in_time, t_min=0, t_max=reference_intervals[-1, 1])
+    
+    mir_eval.segment.validate_boundary(reference_intervals, estimated_intervals, False)
+
+    # Convert intervals to boundaries
+    reference_boundaries = mir_eval.util.intervals_to_boundaries(reference_intervals)
+    estimated_boundaries = mir_eval.util.intervals_to_boundaries(estimated_intervals)
+
+    # If we have no boundaries, we get no score.
+    if len(reference_boundaries) == 0 or len(estimated_boundaries) == 0:
+        return 0, 0, 0
+
+    tp = len(mir_eval.util.match_events(reference_boundaries,estimated_boundaries,window_length))
+    fp = len(estimated_boundaries) - tp
+    fn = len(reference_boundaries) - tp
+    
+    return tp, fp, fn
+        
+
+# %% High level encapsulation of the computation of scores, based on segments.
+## Tolerances are MIREX standards in time (0.5s and 3s), or 0 and 1 bar when barwise aligned.
+def get_scores_from_segments_in_time(segments_in_time, ref_tab):
+    if type(ref_tab[0][0]) != np.ndarray: # ref_tab consist in the references, and should be nested in an array (for consistency).
+        ref_tab = [ref_tab]
+
+    res = -math.inf * np.ones((2, 3))
+
+    prec05, rap05, f_mes05 = compute_score_of_segmentation(ref_tab[0], segments_in_time, window_length = 0.5)
+    prec3, rap3, f_mes3 = compute_score_of_segmentation(ref_tab[0], segments_in_time, window_length = 3)
+    res = [[round(prec05,4),round(rap05,4),round(f_mes05,4)], [round(prec3,4),round(rap3,4),round(f_mes3,4)]]
+    
+    if len(ref_tab) > 1:
+        nd_prec05, nd_rap05, nd_f_mes05 = compute_score_of_segmentation(ref_tab[1], segments_in_time, window_length = 0.5)
+        nd_prec3, nd_rap3, nd_f_mes3 = compute_score_of_segmentation(ref_tab[1], segments_in_time, window_length = 3)
+        if nd_f_mes05 + nd_f_mes3 > f_mes05 + f_mes3:
+            res = [[round(nd_prec05,4),round(nd_rap05,4),round(nd_f_mes05,4)], [round(nd_prec3,4),round(nd_rap3,4),round(nd_f_mes3,4)]]
+    
+    return res
+
+def get_scores_in_time_from_barwise_segments(segments, bars, ref_tab):
+    segments_in_time = segments_from_bar_to_time(segments, bars)
+    return get_scores_from_segments_in_time(segments_in_time, ref_tab)
+    
+def get_scores_in_bars_from_barwise_segments(segments, bars, ref_tab):
+    res = -math.inf * np.ones((2, 3))
+
+    if type(ref_tab[0][0]) != np.ndarray: # ref_tab consist in the references, and should be nested in an array (for consistency between double anntoations in SALAMI and single in RWC).
+        ref_tab = [ref_tab]
+
+    ref0_in_bars = np.array(segments_from_time_to_bar(ref_tab[0], bars))
+    
+    prec0bar, rap0bar, f_mes0bar = compute_score_of_segmentation(ref0_in_bars, segments, window_length = 0)
+    prec1bar, rap1bar, f_mes1bar = compute_score_of_segmentation(ref0_in_bars, segments, window_length = 1)
+    res = [[round(prec0bar,4),round(rap0bar,4),round(f_mes0bar,4)], [round(prec1bar,4),round(rap1bar,4),round(f_mes1bar,4)]]
+
+    if len(ref_tab) > 1:
+        ref1_in_bars = np.array(segments_from_time_to_bar(ref_tab[1], bars))
+
+        nd_prec0bar, nd_rap0bar, nd_f_mes0bar = compute_score_of_segmentation(ref1_in_bars, segments, window_length = 0)
+        nd_prec1bar, nd_rap1bar, nd_f_mes1bar = compute_score_of_segmentation(ref1_in_bars, segments, window_length = 1)
+        if nd_f_mes0bar + nd_f_mes1bar > f_mes0bar + f_mes1bar:
+            res = [[round(nd_prec0bar,4),round(nd_rap0bar,4),round(nd_f_mes0bar,4)], [round(nd_prec1bar,4),round(nd_rap1bar,4),round(nd_f_mes1bar,4)]]
+    
+    return res
+                                          
+def get_scores_switch_time_alignment(time_alignment, segments, bars, ref_tab):
+    if type(ref_tab[0][0]) != np.ndarray: # ref_tab consist in the references, and should be nested in an array (for consistency).
+        ref_tab = [ref_tab]
+
+    # Tolerance in absolute time
+    if time_alignment in ["s", "second", "seconds"]:
+        return get_scores_in_time_from_barwise_segments(segments, bars, ref_tab)
+
+    # Tolerance barwise aligned
+    elif time_alignment in ["b", "bars", "bar", "barwise"]:
+        return get_scores_in_bars_from_barwise_segments(segments, bars, ref_tab)
+            
+    else:
+        raise NotImplementedError(f"Time alignment parameter {time_alignment} not understood")
+
```

### Comparing `as_seg-0.1.4/as_seg/foote_novelty.py` & `as_seg-0.1.5/as_seg/foote_novelty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,377 +1,446 @@
-# # -*- coding: utf-8 -*-
-# """
-# Created on Mon Mar 14 16:40:07 2022
-
-# @author: amarmore
-
-# NOTE: EVERYTHING IS COMMENTED FOR AN INSTALLATION IN MSAF. I SHOULD SEE HOW TO PROPERLY HANDLE THIS LATER.
-
-# Novelty cost, adapted from the work of Foote, see [1].
-# The kernel is of binary values : 1 and -1.
-# This code is deprecated, but could be used in comparison tests.
-
-# If interested, one should use the novelty version from the toolbox MSAF [2] instead,
-# whose parameters were tested and optimized.
-
-# References
-# ----------
-# [1] J. Foote, "Automatic audio segmentation using a measure of audio novelty",
-# in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances 
-# in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000,pp. 452–455.
-
-# [2] O. Nieto and J.P. Bello, "Systematic exploration of computational music
-# structure research.", in: ISMIR, 2016, pp. 547–553.
-# """
-# # %% Using implementation from msaf
-# import msaf
-# import numpy as np
-# from scipy import signal
-# from scipy.ndimage import filters
-
-# def process_msaf_own_as(input_spectrogram, M_gaussian = 66, L_peaks = 64):
-#         """Main process.
-#         Returns
-#         -------
-#         est_idxs : np.array(N)
-#             Estimated indeces the segment boundaries in frames.
-#         est_labels : np.array(N-1)
-#             Estimated labels for the segments.
-#         """
-
-#         # Make sure that the M_gaussian is even
-#         if M_gaussian % 2 == 1:
-#             M_gaussian += 1
-
-#         # Self similarity matrix
-#         S = msaf.algorithms.foote.segmenter.compute_ssm(input_spectrogram)
-
-#         # Compute gaussian kernel
-#         G = msaf.algorithms.foote.segmenter.compute_gaussian_krnl(M_gaussian)
-#         #plt.imshow(S, interpolation="nearest", aspect="auto"); plt.show()
-
-#         # Compute the novelty curve
-#         nc = msaf.algorithms.foote.segmenter.compute_nc(S, G)
-
-#         # Find peaks in the novelty curve
-#         est_idxs = pick_peaks(nc, L=L_peaks)
-
-#         # Add first and last frames
-#         est_idxs = np.concatenate(([0], est_idxs, [input_spectrogram.shape[0] - 1]))
-
-#         # Empty labels
-#         est_labels = np.ones(len(est_idxs) - 1) * -1
-
-#         # Post process estimations
-#         est_idxs, est_labels = postprocess_msaf(est_idxs, est_labels)
-
-#         return est_idxs, est_labels
-        
-# def pick_peaks(nc, L=16):
-#     """Obtain peaks from a novelty curve using an adaptive threshold."""
-#     offset = nc.mean() / 20.
-
-#     #nc = filters.gaussian_filter1d(nc, sigma=4)  # Smooth out nc
-
-#     th = filters.median_filter(nc, size=L) + offset
-#     #th = filters.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
-
-#     peaks = []
-#     for i in range(1, nc.shape[0] - 1):
-#         # is it a peak?
-#         if nc[i - 1] < nc[i] and nc[i] > nc[i + 1]:
-#             # is it above the threshold?
-#             if nc[i] > th[i]:
-#                 peaks.append(i)
-#     #plt.plot(nc)
-#     #plt.plot(th)
-#     #for peak in peaks:
-#         #plt.axvline(peak)
-#     #plt.show()
-
-#     return peaks
-        
-# def postprocess_msaf(est_idxs, est_labels):
-#         """Post processes the estimations from the algorithm, removing empty
-#         segments and making sure the lenghts of the boundaries and labels
-#         match."""
-#         # Make sure we are using the previously input bounds, if any
-#         # if self.in_bound_idxs is not None:
-#             # F = self._preprocess()
-#             # est_labels = msaf.utils.synchronize_labels(self.in_bound_idxs, est_idxs,
-#                                               # est_labels, F.shape[0])
-#             # est_idxs = self.in_bound_idxs
-
-#         # Remove empty segments if needed
-#         est_idxs, est_labels = msaf.utils.remove_empty_segments(est_idxs, est_labels)
-
-#         assert len(est_idxs) - 1 == len(est_labels), "Number of boundaries " \
-#             "(%d) and number of labels(%d) don't match" % (len(est_idxs),
-#                                                            len(est_labels))
-
-#         # Make sure the indeces are integers
-#         est_idxs = np.asarray(est_idxs, dtype=int)
-
-#         return est_idxs, est_labels
-
-
-# # %% Novelty computation
-# def novelty_cost(cropped_autosimilarity):
-#     """
-#     Novelty measure on this part of the autosimilarity matrix.
-#     The size of the kernel will be the size of the parameter matrix.
-
-#     Parameters
-#     ----------
-#     cropped_autosimilarity : list of list of floats or numpy array (matrix representation)
-#         The part of the autosimilarity which novelty measure is to compute.
-
-#     Raises
-#     ------
-#     NotImplementedError
-#         If the size of the autosimilarity is odd (novlety kernel can't fit this matrix).
-
-#     Returns
-#     -------
-#     float
-#         The novelty measure.
-
-#     """
-#     # Kernel is of the size of cropped_autosimilarity
-#     if len(cropped_autosimilarity) == 0:
-#         return 0
-    
-#     if len(cropped_autosimilarity) % 2 == 1:
-#         raise NotImplementedError("The novelty computation is not implemented when the kernel is of odd size.") from None
-#         #return (novelty_cost(cropped_autosimilarity[:-1, :-1]) + novelty_cost(cropped_autosimilarity[1:, 1:])) / 2
-    
-#     kernel_size = int(len(cropped_autosimilarity) / 2)
-#     kernel = np.kron(np.array([[1,-1], [-1, 1]]), np.ones((kernel_size, kernel_size)))
-#     return np.mean(kernel*cropped_autosimilarity)
-
-# def novelty_computation(autosimilarity_array, kernel_size):
-#     """
-#     Computes the novelty measure on the entire autosimilarity matrix, with a defined and fixed kernel size.
-
-#     Parameters
-#     ----------
-#     autosimilarity_array : list of list of floats or numpy array (matrix representation)
-#         The autosimilarity matrix.
-
-#     kernel_size : integer
-#         The size of the kernel.
-
-#     Raises
-#     ------
-#     NotImplementedError
-#         If the kernel size is odd, can't compute the novelty measure.
-
-#     Returns
-#     -------
-#     cost : list of float
-#         List of novelty measures, at each bar of the autosimilarity.
-
-#     """
-#     if kernel_size % 2 == 1:
-#         raise NotImplementedError("The novelty computation is not implemented when the kernel is of odd size.") from None
-#     cost = np.zeros(len(autosimilarity_array))
-#     half_kernel = int(kernel_size / 2)
-#     for i in range(half_kernel, len(autosimilarity_array) - half_kernel):
-#         cost[i] = novelty_cost(autosimilarity_array[i - half_kernel:i + half_kernel,i - half_kernel:i + half_kernel])
-#     return cost
-
-# # %% Post-processing of the novelty values
-# ##################### Sandbox ##################
-# def peak_picking(tab, window_size = 1):
-#     """
-#     Returns the indexes of peaks of values in the given list of values.
-#     A value is considered "peak" if it's a local maximum,
-#     and if all values in the window (defined by 'window_size') before and after 
-#     are strictly monotonous.    
-#     Used for peak picking in the novelty measure.
-
-#     Parameters
-#     ----------
-#     tab : list of float
-#         The list of values to study.
-#     window_size : boolean, optional
-#         Size of the window around a possible peak to be considered "peak",
-#         ie number of consecutive values where the values should increase (before) and (decrease) after.
-#         The default is 1.
-
-#     Returns
-#     -------
-#     to_return : list of integers
-#         The indexes where values are peaking.
-
-#     """
-#     to_return = []
-#     for current_idx in range(window_size, len(tab) - window_size):
-#         if is_increasing(tab[current_idx - window_size:current_idx + 1]) and is_increasing(tab[current_idx:current_idx + window_size + 1][::-1]):
-#             to_return.append(current_idx)
-#     return to_return
-
-# def valley_picking(tab, window_size = 1):
-#     """
-#     Returns the indexes of valleys of values in the desired list of values.
-#     A value is considered "valley" if it's a local minimum,
-#     and if all values in the window (defined by 'window_size') before and after 
-#     are strictly monotonous.
-#     Used for peak picking in the novelty measure.
-
-#     Parameters
-#     ----------
-#     tab : list of float
-#         The list of values to study.
-#     window_size : boolean, optional
-#         Size of the window around a possible valley to be considered "valley",
-#         ie number of consecutive values where the values should decrease (before) and increase (after).
-#         The default is 1.
-
-#     Returns
-#     -------
-#     to_return : list of integers
-#         The indexes where values are valleys.
-
-#     """
-#     to_return = []
-#     for current_idx in range(window_size, len(tab) - window_size):
-#         if is_increasing(tab[current_idx - window_size:current_idx + 1][::-1]) and is_increasing(tab[current_idx:current_idx + window_size + 1]):
-#             to_return.append(current_idx)
-#     return to_return
-
-# def is_increasing(tab):
-#     """
-#     Tests if the tab values are increasing.
-#     Used for peak picking in the novelty measure.
-
-#     Parameters
-#     ----------
-#     tab : list of float
-#         The values.
-
-#     Returns
-#     -------
-#     boolean
-#         Whether the values are increasing or not.
-
-#     """
-#     if len(tab) <= 1 or len(np.unique(tab)) == 1:
-#         return False
-#     for idx in range(len(tab) - 1):
-#         if tab[idx] > tab[idx+1]:
-#             return False
-#     return True
-
-# def decreasing_peaks(data):
-#     """
-#     Returns the peaks indexes of a list of values in their decreasing order of values.
-#     Used for peak picking in the novelty measure.
-
-#     Parameters
-#     ----------
-#     data : list of float
-#         The values.
-
-#     Returns
-#     -------
-#     list of integers
-#         The indexes of the peaks, sorted in their decreasing order of values.
-
-#     """
-#     peaks_and_value = []
-#     for idx in peak_picking(data, window_size = 1):
-#         peaks_and_value.append((idx, data[idx]))
-#     return sorted(peaks_and_value, key=lambda x:x[1], reverse = True)
-
-# def select_highest_peaks_thresholded_indexes(data, percentage = 0.33):
-#     """
-#     Returns the peaks higher than a percentage of the maximal peak from a list of values.
-#     Used for peak picking in the novelty measure.
-    
-#     Parameters
-#     ----------
-#     data : list of floats
-#         The values.
-#     percentage : float, optional
-#         The percentage of the maximal value for a peak to be valid.
-#         The default is 0.33.
-
-#     Returns
-#     -------
-#     list of integers
-#         Indexes of the valid peaks.
-
-#     """
-#     peaks = np.array(decreasing_peaks(data))
-#     max_peak = peaks[0,1]
-#     for idx, peak in enumerate(peaks):
-#         if peak[1] < percentage * max_peak:
-#             return [int(i) for i in sorted(peaks[:idx, 0])]
-#     return [int(i) for i in sorted(peaks[:,0])]
-
-# def values_as_slop(value, choice_func = max):
-#     """
-#     Compute peaks of a value (typically novelty measure)
-#     as the difference between absolute peaks and absolute valleys.
-#     Function choice_func determines the way of computing this gap.
-    
-#     Typically, max will compute peaks as the maximum gap between a peaks and its two closest valleys,
-#     whereas min will select the minimal gap.
-    
-#     This returns an array containing zeroes where there is no peak in absoluite value,
-#     and this new value as a gap computation where there was peaks before.
-
-#     Parameters
-#     ----------
-#     value : array of float
-#         The absolute value of the measure.
-#     choice_func : function name, optional
-#         Type of the function selecting the difference between peaks and valleys.
-#         Classical values are "max" for selecting the maximum gap between the peak and both its closest valleys,
-#         "min" for the minimum of both gaps, and "mean" (called as_seg.mean) for the mean of both gaps.
-#         The default is max.
-
-#     Returns
-#     -------
-#     peak_valley_slop : array of floats
-#         The new values of peaks as gaps, and 0 everywhere else.
-
-#     """
-#     peaks = peak_picking(value, window_size = 1)
-#     valleys = valley_picking(value, window_size = 1)
-#     peak_valley_slop = np.zeros(len(value))
-#     for peak in peaks:
-#         i = 0
-#         while i < len(valleys) and valleys[i] < peak:
-#             i+=1
-#         if i == 0:
-#             left_valley = 0
-#             right_valley = valleys[i]
-#         elif i == len(valleys):
-#             left_valley = valleys[i - 1]
-#             right_valley = 0
-#         else:
-#             left_valley = valleys[i - 1]
-#             right_valley = valleys[i]
-#         chosen_valley_value = choice_func(value[left_valley], value[right_valley])
-#         peak_valley_slop[peak] = value[peak] - chosen_valley_value
-#     return peak_valley_slop
-    
-# def mean(val_a, val_b):
-#     """
-#     A function returning the mean of both values.
-#     This function is redeveloped so as to be called as choice_func in the function "values_as_slop()" (see above) in external projects.
-
-#     Parameters
-#     ----------
-#     val_a : float
-#         First value.
-#     val_b : float
-#         Second value.
-
-#     Returns
-#     -------
-#     float: mean of both values.
-
-#     """
-#     return (val_a + val_b) / 2
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Mar 14 16:40:07 2022
+
+@author: amarmore
+
+Novelty cost, adapted from the work of Foote, see [1].
+The kernel is of binary values : 1 and -1.
+This code is deprecated, but could be used in comparison tests.
+
+If interested, one should use the novelty version from the toolbox MSAF [2] instead,
+whose parameters were tested and optimized.
+
+References
+----------
+[1] J. Foote, "Automatic audio segmentation using a measure of audio novelty",
+in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances 
+in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000,pp. 452–455.
+
+[2] O. Nieto and J.P. Bello, "Systematic exploration of computational music
+structure research.", in: ISMIR, 2016, pp. 547–553.
+"""
+# %% Using implementation from msaf
+import msaf
+import numpy as np
+from scipy import signal
+from scipy.ndimage import filters
+
+def compute_foote_ssm(input_spectrogram, pre_filter = 12):
+    spec = input_spectrogram
+    if pre_filter != 0:
+        median_filtering_size = pre_filter
+        spec = median_filter(input_spectrogram, M=median_filtering_size)
+        
+    return msaf.algorithms.foote.segmenter.compute_ssm(spec)
+
+def process_msaf_own_as(input_spectrogram = None, input_ssm = None, M_gaussian = 66, L_peaks = 64, pre_filter = 12, post_filter = 4):
+        """Main process.
+        Returns
+        -------
+        est_idxs : np.array(N)
+            Estimated indeces the segment boundaries in frames.
+        est_labels : np.array(N-1)
+            Estimated labels for the segments.
+        """
+        assert input_ssm is not None or input_spectrogram is not None, "Either input_ssm or input_spectrogram should be provided"
+
+        # Make sure that the M_gaussian is even
+        if M_gaussian % 2 == 1:
+            M_gaussian += 1
+
+        # Self similarity matrix
+        if input_ssm is None:
+            S = compute_foote_ssm(input_spectrogram, pre_filter)
+            input_shape = input_spectrogram.shape
+        else:
+            S = input_ssm
+            input_shape = input_ssm.shape
+
+        # Compute gaussian kernel
+        G = msaf.algorithms.foote.segmenter.compute_gaussian_krnl(M_gaussian)
+        #plt.imshow(S, interpolation="nearest", aspect="auto"); plt.show()
+
+        # Compute the novelty curve
+        nc = msaf.algorithms.foote.segmenter.compute_nc(S, G)
+
+        # Find peaks in the novelty curve
+        sigma = post_filter
+        est_idxs = pick_peaks(nc, sigma = sigma, L=L_peaks)
+
+        # Add first and last frames
+        est_idxs = np.concatenate(([0], est_idxs, [input_shape[0] - 1]))
+
+        # Empty labels
+        est_labels = np.ones(len(est_idxs) - 1) * -1
+
+        # Post process estimations
+        est_idxs, est_labels = postprocess_msaf(est_idxs, est_labels)
+
+        return est_idxs, est_labels
+        
+def median_filter(X, M=8):
+    """Median filter along the first axis of the feature matrix X."""
+    for i in range(X.shape[1]):
+        X[:, i] = filters.median_filter(X[:, i], size=M)
+    return X
+
+def pick_peaks(nc, sigma = 4, L=16):
+    """Obtain peaks from a novelty curve using an adaptive threshold."""
+    offset = nc.mean() / 20.
+
+    if sigma != 0:
+        nc = filters.gaussian_filter1d(nc, sigma=sigma)  # Smooth out nc
+
+    th = filters.median_filter(nc, size=L) + offset
+    #th = filters.gaussian_filter(nc, sigma=L/2., mode="nearest") + offset
+
+    peaks = []
+    for i in range(1, nc.shape[0] - 1):
+        # is it a peak?
+        if nc[i - 1] < nc[i] and nc[i] > nc[i + 1]:
+            # is it above the threshold?
+            if nc[i] > th[i]:
+                peaks.append(i)
+    #plt.plot(nc)
+    #plt.plot(th)
+    #for peak in peaks:
+        #plt.axvline(peak)
+    #plt.show()
+
+    return peaks
+        
+def postprocess_msaf(est_idxs, est_labels):
+        """Post processes the estimations from the algorithm, removing empty
+        segments and making sure the lenghts of the boundaries and labels
+        match."""
+        # Make sure we are using the previously input bounds, if any
+        # if self.in_bound_idxs is not None:
+            # F = self._preprocess()
+            # est_labels = msaf.utils.synchronize_labels(self.in_bound_idxs, est_idxs,
+                                              # est_labels, F.shape[0])
+            # est_idxs = self.in_bound_idxs
+
+        # Remove empty segments if needed
+        est_idxs, est_labels = msaf.utils.remove_empty_segments(est_idxs, est_labels)
+
+        assert len(est_idxs) - 1 == len(est_labels), "Number of boundaries " \
+            "(%d) and number of labels(%d) don't match" % (len(est_idxs),
+                                                           len(est_labels))
+
+        # Make sure the indeces are integers
+        est_idxs = np.asarray(est_idxs, dtype=int)
+
+        return est_idxs, est_labels
+
+def my_process_segmentation_level(est_idxs, est_labels, N, frame_times, dur):
+    """Processes a level of segmentation, and converts it into times.
+
+    Parameters
+    ----------
+    est_idxs: np.array
+        Estimated boundaries in frame indeces.
+    est_labels: np.array
+        Estimated labels.
+    N: int
+        Number of frames in the whole track.
+    frame_times: np.array
+        Time stamp for each frame.
+    dur: float
+        Duration of the audio track.
+
+    Returns
+    -------
+    est_times: np.array
+        Estimated segment boundaries in seconds.
+    est_labels: np.array
+        Estimated labels for each segment.
+    """
+    assert est_idxs[0] == 0 and est_idxs[-1] == N - 1
+    assert len(est_idxs) - 1 == len(est_labels)
+
+    # Add silences, if needed
+    est_times = np.concatenate(([0], frame_times[est_idxs], [dur]))
+    silence_label = np.max(est_labels) + 1
+    est_labels = np.concatenate(([silence_label], est_labels, [silence_label]))
+
+    # Remove empty segments if needed
+    est_times, est_labels = msaf.utils.remove_empty_segments(est_times, est_labels)
+
+    # I've added these lines because bar estimates may be less precise than frame and beats.
+    if est_times[-1] < dur: # Fixing a bug, due to empty segment: [dur, dur]
+        est_times.append(dur)
+    if est_times[-1] > dur: # Fixing a bug, due to inaccuracies (rounding errors mainly)
+        if est_times[-1] - dur < 1:
+            est_times[-1] = dur
+        else:
+            #print(f"Ajout Axel: est_times[-1] = {est_times[-1]}, dur = {dur}, ce qui n'est pas normal. Voir si bug arrive souvent.")
+            est_times[-1] = dur
+    
+    # Make sure that the first and last times are 0 and duration, respectively
+    assert np.allclose([est_times[0]], [0]) and np.allclose([est_times[-1]], [dur])
+
+    return est_times, est_labels
+
+
+# %% Novelty computation
+def novelty_cost(cropped_autosimilarity):
+    """
+    Novelty measure on this part of the autosimilarity matrix.
+    The size of the kernel will be the size of the parameter matrix.
+
+    Parameters
+    ----------
+    cropped_autosimilarity : list of list of floats or numpy array (matrix representation)
+        The part of the autosimilarity which novelty measure is to compute.
+
+    Raises
+    ------
+    NotImplementedError
+        If the size of the autosimilarity is odd (novlety kernel can't fit this matrix).
+
+    Returns
+    -------
+    float
+        The novelty measure.
+
+    """
+    # Kernel is of the size of cropped_autosimilarity
+    if len(cropped_autosimilarity) == 0:
+        return 0
+    
+    if len(cropped_autosimilarity) % 2 == 1:
+        raise NotImplementedError("The novelty computation is not implemented when the kernel is of odd size.") from None
+        #return (novelty_cost(cropped_autosimilarity[:-1, :-1]) + novelty_cost(cropped_autosimilarity[1:, 1:])) / 2
+    
+    kernel_size = int(len(cropped_autosimilarity) / 2)
+    kernel = np.kron(np.array([[1,-1], [-1, 1]]), np.ones((kernel_size, kernel_size)))
+    return np.mean(kernel*cropped_autosimilarity)
+
+def novelty_computation(autosimilarity_array, kernel_size):
+    """
+    Computes the novelty measure on the entire autosimilarity matrix, with a defined and fixed kernel size.
+
+    Parameters
+    ----------
+    autosimilarity_array : list of list of floats or numpy array (matrix representation)
+        The autosimilarity matrix.
+
+    kernel_size : integer
+        The size of the kernel.
+
+    Raises
+    ------
+    NotImplementedError
+        If the kernel size is odd, can't compute the novelty measure.
+
+    Returns
+    -------
+    cost : list of float
+        List of novelty measures, at each bar of the autosimilarity.
+
+    """
+    if kernel_size % 2 == 1:
+        raise NotImplementedError("The novelty computation is not implemented when the kernel is of odd size.") from None
+    cost = np.zeros(len(autosimilarity_array))
+    half_kernel = int(kernel_size / 2)
+    for i in range(half_kernel, len(autosimilarity_array) - half_kernel):
+        cost[i] = novelty_cost(autosimilarity_array[i - half_kernel:i + half_kernel,i - half_kernel:i + half_kernel])
+    return cost
+
+# %% Post-processing of the novelty values
+##################### Sandbox ##################
+def peak_picking(tab, window_size = 1):
+    """
+    Returns the indexes of peaks of values in the given list of values.
+    A value is considered "peak" if it's a local maximum,
+    and if all values in the window (defined by 'window_size') before and after 
+    are strictly monotonous.    
+    Used for peak picking in the novelty measure.
+
+    Parameters
+    ----------
+    tab : list of float
+        The list of values to study.
+    window_size : boolean, optional
+        Size of the window around a possible peak to be considered "peak",
+        ie number of consecutive values where the values should increase (before) and (decrease) after.
+        The default is 1.
+
+    Returns
+    -------
+    to_return : list of integers
+        The indexes where values are peaking.
+
+    """
+    to_return = []
+    for current_idx in range(window_size, len(tab) - window_size):
+        if is_increasing(tab[current_idx - window_size:current_idx + 1]) and is_increasing(tab[current_idx:current_idx + window_size + 1][::-1]):
+            to_return.append(current_idx)
+    return to_return
+
+def valley_picking(tab, window_size = 1):
+    """
+    Returns the indexes of valleys of values in the desired list of values.
+    A value is considered "valley" if it's a local minimum,
+    and if all values in the window (defined by 'window_size') before and after 
+    are strictly monotonous.
+    Used for peak picking in the novelty measure.
+
+    Parameters
+    ----------
+    tab : list of float
+        The list of values to study.
+    window_size : boolean, optional
+        Size of the window around a possible valley to be considered "valley",
+        ie number of consecutive values where the values should decrease (before) and increase (after).
+        The default is 1.
+
+    Returns
+    -------
+    to_return : list of integers
+        The indexes where values are valleys.
+
+    """
+    to_return = []
+    for current_idx in range(window_size, len(tab) - window_size):
+        if is_increasing(tab[current_idx - window_size:current_idx + 1][::-1]) and is_increasing(tab[current_idx:current_idx + window_size + 1]):
+            to_return.append(current_idx)
+    return to_return
+
+def is_increasing(tab):
+    """
+    Tests if the tab values are increasing.
+    Used for peak picking in the novelty measure.
+
+    Parameters
+    ----------
+    tab : list of float
+        The values.
+
+    Returns
+    -------
+    boolean
+        Whether the values are increasing or not.
+
+    """
+    if len(tab) <= 1 or len(np.unique(tab)) == 1:
+        return False
+    for idx in range(len(tab) - 1):
+        if tab[idx] > tab[idx+1]:
+            return False
+    return True
+
+def decreasing_peaks(data):
+    """
+    Returns the peaks indexes of a list of values in their decreasing order of values.
+    Used for peak picking in the novelty measure.
+
+    Parameters
+    ----------
+    data : list of float
+        The values.
+
+    Returns
+    -------
+    list of integers
+        The indexes of the peaks, sorted in their decreasing order of values.
+
+    """
+    peaks_and_value = []
+    for idx in peak_picking(data, window_size = 1):
+        peaks_and_value.append((idx, data[idx]))
+    return sorted(peaks_and_value, key=lambda x:x[1], reverse = True)
+
+def select_highest_peaks_thresholded_indexes(data, percentage = 0.33):
+    """
+    Returns the peaks higher than a percentage of the maximal peak from a list of values.
+    Used for peak picking in the novelty measure.
+    
+    Parameters
+    ----------
+    data : list of floats
+        The values.
+    percentage : float, optional
+        The percentage of the maximal value for a peak to be valid.
+        The default is 0.33.
+
+    Returns
+    -------
+    list of integers
+        Indexes of the valid peaks.
+
+    """
+    peaks = np.array(decreasing_peaks(data))
+    max_peak = peaks[0,1]
+    for idx, peak in enumerate(peaks):
+        if peak[1] < percentage * max_peak:
+            return [int(i) for i in sorted(peaks[:idx, 0])]
+    return [int(i) for i in sorted(peaks[:,0])]
+
+def values_as_slop(value, choice_func = max):
+    """
+    Compute peaks of a value (typically novelty measure)
+    as the difference between absolute peaks and absolute valleys.
+    Function choice_func determines the way of computing this gap.
+    
+    Typically, max will compute peaks as the maximum gap between a peaks and its two closest valleys,
+    whereas min will select the minimal gap.
+    
+    This returns an array containing zeroes where there is no peak in absoluite value,
+    and this new value as a gap computation where there was peaks before.
+
+    Parameters
+    ----------
+    value : array of float
+        The absolute value of the measure.
+    choice_func : function name, optional
+        Type of the function selecting the difference between peaks and valleys.
+        Classical values are "max" for selecting the maximum gap between the peak and both its closest valleys,
+        "min" for the minimum of both gaps, and "mean" (called as_seg.mean) for the mean of both gaps.
+        The default is max.
+
+    Returns
+    -------
+    peak_valley_slop : array of floats
+        The new values of peaks as gaps, and 0 everywhere else.
+
+    """
+    peaks = peak_picking(value, window_size = 1)
+    valleys = valley_picking(value, window_size = 1)
+    peak_valley_slop = np.zeros(len(value))
+    for peak in peaks:
+        i = 0
+        while i < len(valleys) and valleys[i] < peak:
+            i+=1
+        if i == 0:
+            left_valley = 0
+            right_valley = valleys[i]
+        elif i == len(valleys):
+            left_valley = valleys[i - 1]
+            right_valley = 0
+        else:
+            left_valley = valleys[i - 1]
+            right_valley = valleys[i]
+        chosen_valley_value = choice_func(value[left_valley], value[right_valley])
+        peak_valley_slop[peak] = value[peak] - chosen_valley_value
+    return peak_valley_slop
+    
+def mean(val_a, val_b):
+    """
+    A function returning the mean of both values.
+    This function is redeveloped so as to be called as choice_func in the function "values_as_slop()" (see above) in external projects.
+
+    Parameters
+    ----------
+    val_a : float
+        First value.
+    val_b : float
+        Second value.
+
+    Returns
+    -------
+    float: mean of both values.
+
+    """
+    return (val_a + val_b) / 2
```

### Comparing `as_seg-0.1.4/as_seg/model/current_plot.py` & `as_seg-0.1.5/as_seg/model/current_plot.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg/model/errors.py` & `as_seg-0.1.5/as_seg/model/errors.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg/model/features.py` & `as_seg-0.1.5/as_seg/model/features.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg/scripts/default_path.py` & `as_seg-0.1.5/as_seg/scripts/default_path.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,23 +3,32 @@
 Created on Wed Sep 22 17:22:59 2021
 
 Default paths for the different folders.
 Should be changed prior to any computation.
 
 @author: amarmore
 """
+import os
+
+# We suppose that we are in the Notebooks folder,
+# hence data is in the parent folder.
+path_parent_of_data = os.path.dirname(os.getcwd())
+
+# Global
+path_data_persisted = f"{path_parent_of_data}/data/data_persisted"
+
 # RWC
-path_data_persisted_rwc = "C:/Users/amarmore/Desktop/data_persisted" ## Path where pre-computed data on RWC Pop should be stored (spectrograms, NTD, neural networks, etc)
-path_annotation_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/annotations" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
-path_entire_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Entire RWC" ## Path where are stored wav files of RWC
-path_even_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Even songs" ## Path containing only the wav files of songs of odd numbers
-path_odd_songs_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Odd songs" ## Path containing only the wav files of songs of even numbers
-path_debug_rwc = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/debug" ## Debug path, containing only two songs, to fix functions quickly
-path_mirdata_rwc = "C:/Users/amarmore/Desktop/Audio samples/mirdata/RWC Pop/" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
+#path_data_persisted_rwcpop = "C:/Users/amarmore/Desktop/data_persisted/RWC Pop" ## Path where pre-computed data on RWC Pop should be stored (bars, beats, spectrograms, ssm, ...)
+path_annotation_rwcpop = f"{path_parent_of_data}/data/annotations/rwcpop" ## Path of the annotations of RWC Pop. Should be parent folder of "AIST" and/or "MIREX10"
+path_entire_rwcpop = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Entire RWC" ## Path where are stored wav files of RWC
+#path_even_songs_rwcpop = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Even songs" ## Path containing only the wav files of songs of odd numbers
+#path_odd_songs_rwcpop = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/Odd songs" ## Path containing only the wav files of songs of even numbers
+#path_debug_rwcpop = "C:/Users/amarmore/Desktop/Audio samples/RWC Pop/debug" ## Debug path, containing only two songs, to fix functions quickly
+#path_mirdata_rwcpop = "C:/Users/amarmore/Desktop/Audio samples/mirdata/RWC Pop/"
 
 # SALAMI
-path_data_persisted_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami/data_persisted" ## Path where pre-computed data on the SALAMI dataset should be stored (spectrograms, NTD, neural networks, etc)
-path_entire_salami = "C:/Users/amarmore/Desktop/Audio samples/Salami" ## Path where are stored wav files of SALAMI (path where it is downloaded by mirdata also)
+path_data_persisted_salami = f"{path_parent_of_data}/data/annotations/salami" ## Path where pre-computed data on the SALAMI dataset should be stored (bars, beats, spectrograms, ssm, ...)
+path_entire_salami = "C:/Users/amarmore/Desktop/Audio samples/SALAMI" ## Path where are stored wav files of SALAMI (path where it is downloaded by mirdata also)
 
 # Come Together
-come_together = "C:/Users/amarmore/this_folder/The Beatles - Come Together"
-path_data_persisted_come_together = "C:/Users/amarmore/Desktop/data_persisted"
+come_together = "/home/a23marmo/this_folder/The Beatles - Come Together"
+path_data_persisted_come_together = "/home/a23marmo/Bureau/data_persisted/cometogether"
```

### Comparing `as_seg-0.1.4/as_seg/scripts/example.py` & `as_seg-0.1.5/as_seg/example.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.4/as_seg.egg-info/PKG-INFO` & `as_seg-0.1.5/as_seg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-Metadata-Version: 2.1
-Name: as-seg
-Version: 0.1.4
-Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
-Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
-Author: Marmoret Axel
-Author-email: axel.marmoret@imt-atlantique.fr
-License: BSD
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: AUTHORS
-
-# as_seg: module for computing and segmenting autosimilarity matrices. #
-
-Hello, and welcome on this repository!
-
-This project aims at computing autosimilarity matrices, and segmenting them, which consists of the task of structural segmentation.
-
-The current version contains the CBM algorithm [1], along with a (low-effort) implementation of Foote's novelty algorithm [2].
-
-It can be installed using pip as `pip install as-seg`.
-
-This is a first release, and may contain bug. Comments are welcomed!
-
-## Tutorial notebook ##
-
-A tutorial notebook presenting the most important components of this toolbox is available in the folder "Notebooks".
-
-## Experimental notebook ##
-
-Experimental notebooks are available in the folder "Notebooks". They present the code used to compute the main experiments of the paper, in order to improve the reproducibility. Please tell me if any problem would appear when trying to launch them.
-
-## Data ##
-
-Some data is available with the code, in the folder "data". This includes the bar estimates, obtained with the madmom toolbox [3], the Barwise TF matrices, which are the barwise pre-processed versions of the spectrograms we use to estimate boundaries, and the estimated boundaries obtained with the CBM algorithm in the different conditions.
-
-## Software version ##
-
-This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
-
-## How to cite ##
-
-You should cite the package `as_seg`, available on HAL (https://hal.archives-ouvertes.fr/hal-03797507).
-
-Here are two styles of citations:
-
-As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, URL={https://gitlab.inria.fr/amarmore/autosimilarity_segmentation}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
-
-In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices," 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
-
-## Credits ##
-
-Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
-
-The technique in itself was also developed by FrÃ©dÃ©ric Bimbot (<bimbot@irisa.fr>).
-
-## References ##
-[1] A. Marmoret, J.E. Cohen, and F. Bimbot, "Convolutive Block-Matching Segmentation Algorithm with Application to Music Structure Analysis", 2023, to be published at WASPAA 2023.
-
-[2] J. Foote, "Automatic audio segmentation using a measure of audio novelty," in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000, pp. 452â€“455.
-
-[3] BÃ¶ck, S., Korzeniowski, F., SchlÃ¼ter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+Metadata-Version: 2.1
+Name: as-seg
+Version: 0.1.5
+Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
+Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
+Author: Marmoret Axel
+Author-email: axel.marmoret@imt-atlantique.fr
+License: BSD
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS
+
+# as_seg: module for computing and segmenting autosimilarity matrices. #
+
+Hello, and welcome on this repository!
+
+This project aims at computing autosimilarity matrices, and segmenting them, which consists of the task of structural segmentation.
+
+The current version contains the CBM algorithm [1], along with an implementation of Foote's novelty algorithm [2] based on the MSAF toolbox [3].
+
+It can be installed using pip as `pip install as-seg`.
+
+This is a first release, and may contain bug. Comments are welcomed!
+
+## Tutorial notebook ##
+
+A tutorial notebook presenting the most important components of this toolbox is available in the folder "Notebooks".
+
+## Experimental notebook ##
+
+Experimental notebooks are available in the folder "Notebooks". They present the code used to compute the main experiments of the paper, in order to improve the reproducibility. Please tell me if any problem would appear when trying to launch them.
+
+Experimental Notebooks requires some pre-computed data to work, which can be found on zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
+
+## Data ##
+
+Should be obtained from Zenodo: https://zenodo.org/records/10168387. DOI: 10.5281/zenodo.10168386.
+
+## Software version ##
+
+This code was developed with Python 3.8.5, and some external libraries detailed in dependencies.txt. They should be installed automatically if this project is downloaded using pip.
+
+## How to cite ##
+
+You should cite the package `as_seg`, available on HAL (https://hal.archives-ouvertes.fr/hal-03797507).
+
+Here are two styles of citations:
+
+As a bibtex format, this should be cited as: @softwareversion{marmoret2022as_seg, title={as\_seg: module for computing and segmenting autosimilarity matrices}, author={Marmoret, Axel and Cohen, J{\'e}r{\'e}my and Bimbot, Fr{\'e}d{\'e}ric}, LICENSE = {BSD 3-Clause ''New'' or ''Revised'' License}, year={2022}}
+
+In the IEEE style, this should be cited as: A. Marmoret, J.E. Cohen, and F. Bimbot, "as_seg: module for computing and segmenting autosimilarity matrices," 2022, url: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation.
+
+## Credits ##
+
+Code was created by Axel Marmoret (<axel.marmoret@gmail.com>), and strongly supported by Jeremy E. Cohen (<jeremy.cohen@cnrs.fr>).
+
+The technique in itself was also developed by Frédéric Bimbot (<bimbot@irisa.fr>).
+
+## References ##
+[1] A. Marmoret, J.E. Cohen, F. Bimbot. Barwise Music Structure Analysis with the Correlation Block-Matching Segmentation Algorithm. Transactions of the International Society for Music Information Retrieval (TISMIR), 2023, 6 (1), pp.167-185. ⟨10.5334/tismir.167⟩. ⟨hal-04323556⟩, https://hal.science/hal-04323556.
+
+[2] J. Foote, "Automatic audio segmentation using a measure of audio novelty," in: 2000 IEEE Int. Conf. Multimedia and Expo. ICME2000. Proc. Latest Advances in the Fast Changing World of Multimedia, vol. 1, IEEE, 2000, pp. 452–455.
+
+[3] Nieto, O., Bello, J. P., Systematic Exploration Of Computational Music Structure Research. Proc. of the 17th International Society for Music Information Retrieval Conference (ISMIR). New York City, NY, USA, 2016.
+
+[4] Böck, S., Korzeniowski, F., Schlüter, J., Krebs, F., & Widmer, G. (2016, October). Madmom: A new python audio and music signal processing library. In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
+
+
```

### Comparing `as_seg-0.1.4/as_seg.egg-info/SOURCES.txt` & `as_seg-0.1.5/as_seg.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 README.md
 setup.py
 as_seg/CBM_algorithm.py
 as_seg/__init__.py
 as_seg/autosimilarity_computation.py
 as_seg/barwise_input.py
 as_seg/data_manipulation.py
+as_seg/example.py
 as_seg/foote_novelty.py
 as_seg.egg-info/PKG-INFO
 as_seg.egg-info/SOURCES.txt
 as_seg.egg-info/dependency_links.txt
 as_seg.egg-info/requires.txt
 as_seg.egg-info/top_level.txt
 as_seg/model/__init__.py
 as_seg/model/current_plot.py
+as_seg/model/display_results.py
 as_seg/model/errors.py
 as_seg/model/features.py
 as_seg/scripts/__init__.py
 as_seg/scripts/default_path.py
-as_seg/scripts/example.py
 as_seg/scripts/overall_scripts.py
```

### Comparing `as_seg-0.1.4/setup.py` & `as_seg-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="as_seg",
-    version="0.1.4",
+    version="0.1.5",
     author="Marmoret Axel",
     author_email="axel.marmoret@imt-atlantique.fr",
     description="Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.inria.fr/amarmore/autosimilarity_segmentation",
     packages=setuptools.find_packages(),
@@ -21,14 +21,15 @@
         "Intended Audience :: Science/Research",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Programming Language :: Python :: 3.8"
     ],
     license='BSD',
     install_requires=[
         'librosa >= 0.6.0',
+        #'madmom @ git+https://github.com/CPJKU/madmom',
         'madmom >= 0.16.1',
         'matplotlib >= 1.5',
         'mir_eval',
         'mirdata >= 0.3.3',
         'numpy >= 1.8.0,<1.24',
         'pandas',
         'scikit-learn >= 0.17.0',
```

