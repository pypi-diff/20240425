# Comparing `tmp/phamclust-1.2.0.tar.gz` & `tmp/phamclust-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phamclust-1.2.0.tar", last modified: Wed Mar  6 20:38:18 2024, max compression
+gzip compressed data, was "phamclust-1.3.0.tar", last modified: Thu Apr 25 20:39:38 2024, max compression
```

## Comparing `phamclust-1.2.0.tar` & `phamclust-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-03-06 20:38:18.538081 phamclust-1.2.0/
--rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2024-01-30 13:49:10.000000 phamclust-1.2.0/LICENSE
--rw-r--r--   0 cgauthier   (501) staff       (20)     6818 2024-03-06 20:38:18.537871 phamclust-1.2.0/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)     5537 2024-02-08 20:03:52.000000 phamclust-1.2.0/README.md
--rw-r--r--   0 cgauthier   (501) staff       (20)       89 2024-01-30 13:49:10.000000 phamclust-1.2.0/pyproject.toml
--rw-r--r--   0 cgauthier   (501) staff       (20)     1400 2024-03-06 20:38:18.539101 phamclust-1.2.0/setup.cfg
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-03-06 20:38:18.527345 phamclust-1.2.0/src/
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-03-06 20:38:18.532721 phamclust-1.2.0/src/phamclust/
--rw-r--r--   0 cgauthier   (501) staff       (20)       69 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/__init__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)      130 2024-03-05 13:51:35.000000 phamclust-1.2.0/src/phamclust/__main__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     3888 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/blastn.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     5822 2024-02-08 20:03:52.000000 phamclust-1.2.0/src/phamclust/cli.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     1911 2024-02-21 18:41:57.000000 phamclust-1.2.0/src/phamclust/clustering.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/fasta.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     6803 2024-01-30 15:25:50.000000 phamclust-1.2.0/src/phamclust/genome.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2473 2024-03-06 18:11:58.000000 phamclust-1.2.0/src/phamclust/heatmap.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)    23877 2024-03-06 20:21:38.000000 phamclust-1.2.0/src/phamclust/matrix.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/metrics.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/parallel_process.py
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-03-06 20:38:18.536026 phamclust-1.2.0/src/phamclust/scripts/
--rw-r--r--   0 cgauthier   (501) staff       (20)        0 2024-03-05 13:49:45.000000 phamclust-1.2.0/src/phamclust/scripts/__init__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     3721 2024-02-21 18:53:55.000000 phamclust-1.2.0/src/phamclust/scripts/benchmark.py
--rw-r--r--   0 cgauthier   (501) staff       (20)    19843 2024-03-06 20:38:01.000000 phamclust-1.2.0/src/phamclust/scripts/phamclust.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2024-01-30 13:49:10.000000 phamclust-1.2.0/src/phamclust/statistics.py
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-03-06 20:38:18.536910 phamclust-1.2.0/src/phamclust.egg-info/
--rw-r--r--   0 cgauthier   (501) staff       (20)     6818 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)      678 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/SOURCES.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)        1 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/dependency_links.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)      109 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/entry_points.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)      136 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/requires.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)       10 2024-03-06 20:38:18.000000 phamclust-1.2.0/src/phamclust.egg-info/top_level.txt
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.194760 phamclust-1.3.0/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2024-01-30 13:49:10.000000 phamclust-1.3.0/LICENSE
+-rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-25 20:39:38.194611 phamclust-1.3.0/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)     9457 2024-04-25 20:17:00.000000 phamclust-1.3.0/README.md
+-rw-r--r--   0 cgauthier   (501) staff       (20)       89 2024-01-30 13:49:10.000000 phamclust-1.3.0/pyproject.toml
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1400 2024-04-25 20:39:38.195264 phamclust-1.3.0/setup.cfg
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.179794 phamclust-1.3.0/src/
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.189913 phamclust-1.3.0/src/phamclust/
+-rw-r--r--   0 cgauthier   (501) staff       (20)       69 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)      130 2024-03-05 13:51:35.000000 phamclust-1.3.0/src/phamclust/__main__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     5478 2024-04-25 20:19:39.000000 phamclust-1.3.0/src/phamclust/blastn.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6397 2024-04-25 18:43:50.000000 phamclust-1.3.0/src/phamclust/cli.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1911 2024-02-21 18:41:57.000000 phamclust-1.3.0/src/phamclust/clustering.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/fasta.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6803 2024-01-30 15:25:50.000000 phamclust-1.3.0/src/phamclust/genome.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     4534 2024-04-25 20:00:07.000000 phamclust-1.3.0/src/phamclust/heatmap.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)    23449 2024-04-21 20:44:13.000000 phamclust-1.3.0/src/phamclust/matrix.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/metrics.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/parallel_process.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.193623 phamclust-1.3.0/src/phamclust/scripts/
+-rw-r--r--   0 cgauthier   (501) staff       (20)        0 2024-03-05 13:49:45.000000 phamclust-1.3.0/src/phamclust/scripts/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     3657 2024-03-06 21:02:43.000000 phamclust-1.3.0/src/phamclust/scripts/benchmark.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)    21143 2024-04-25 20:17:04.000000 phamclust-1.3.0/src/phamclust/scripts/phamclust.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/statistics.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.193998 phamclust-1.3.0/src/phamclust.egg-info/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)      678 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/SOURCES.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)        1 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/dependency_links.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)      109 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/entry_points.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)      136 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/requires.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       10 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/top_level.txt
```

### Comparing `phamclust-1.2.0/LICENSE` & `phamclust-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/PKG-INFO` & `phamclust-1.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 1.2.0
+Version: 1.3.0
 Summary: Cluster genomes based on gene phamily data
 Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,27 +18,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: joblib>=1.3.0
+Requires-Dist: joblib~=1.4.0
 Requires-Dist: kaleido~=0.2.0
 Requires-Dist: numpy~=1.24.0
 Requires-Dist: pandas~=2.0.0
 Requires-Dist: parasail~=1.3.0
 Requires-Dist: plotly~=5.18.0
 Requires-Dist: psutil~=5.9.0
 Requires-Dist: scikit-learn~=1.3.0
 Requires-Dist: scipy~=1.10.0
 
 # phamclust
 
-PhamClust is a tool for performing gene phamily based clustering of bacteriophage genomes. It makes use of a novel genome similarity index, the proteomic equivalence quotient (PEQ) to cluster genomes according to their global similarity. A manuscript describing it in detail has been submitted for publication at mSphere.
+PhamClust is a tool for performing gene phamily based clustering of bacteriophage genomes. It makes use of a novel genome 
+similarity index, the proteomic equivalence quotient (PEQ) to cluster genomes according to their global similarity. It was 
+[published in mSphere](https://doi.org/10.1128/msystems.00443-23) in 2023.
 
 # Installation
 
 The most straightforward way to install PhamClust is from the Python Package Index (PyPI): `pip install phamclust`
 
 # Usage
 
@@ -58,52 +60,123 @@
   -h, --help            show this help message and exit
   -g, --genome-dir      interpret `infile` as a directory of genome FASTA files instead of TSV
   -d, --debug           increase verbosity of logging for debug purposes
   -n, --no-sub          do not perform sub-clustering
   -r, --remove-tmp      remove temporary files (not recommended if repeated runs are planned on the same dataset)
   -t , --threads        number of CPU cores to use [default: 16]
 
-clustering arguments::
+clustering arguments:
   -k , --k-min          minimum cluster size to perform subclustering [default: 6]
   -s , --sub-thresh     similarity threshold to use for sub-clustering [default: 0.6]
   -sl , --sub-linkage   linkage type to use for sub-clustering [default: single]
   -c , --clu-thresh     similarity threshold to use for clustering [default: 0.25]
   -cl , --clu-linkage   linkage type to use for clustering [default: average]
   -nr , --nr-thresh     similarity threshold above which to pre-group very similar genomes that must be clustered together [default: 0.75]
   -nl , --nr-linkage    linkage type to use for pre-grouping very similar genomes [default: complete]
   -m , --metric         relatedness index to use for pairwise genome comparisons [default: peq]
+  
+heatmap arguments:
+  -hc , --heatmap-colors
+                        comma-separated list of 2 or 3 colors to use in heatmaps [default: red,yellow,green]
+  -hm , --heatmap-midpoint
+                        midpoint to use for color gradient in heatmaps [default: same as clustering threshold]
 
 Available metrics:
 
     Acronym     Name                                Reference
 (1) gcs         gene content similarity             https://doi.org/10.1038/nmicrobiol.2017.112
 (2) jc          jaccard coefficient                 https://doi.org/10.1111/j.1469-8137.1912.tb05611.x
 (3) pocp        percentage of conserved proteins    https://doi.org/10.1128/JB.01688-14
 (4) af          alignment fraction                  https://doi.org/10.1093/nar/gkv657
 (5) aai         average aminoacid identity          https://doi.org/10.1073/pnas.0409727102
 (6) peq         proteomic equivalence quotient      https://doi.org/10.1128/msystems.00443-23
 ```
 
-PhamClust takes an input filepath and an output filepath as its primary arguments. By default, the input path is assumed to be a TSV file mapping genome names/identifiers to pham identifiers and translations.
+PhamClust takes an input filepath and an output filepath as its primary arguments. By default, the input path is 
+assumed to be a TSV file mapping genome names/identifiers to pham identifiers and translations.
 
-If the `-g/--genome-dir` argument is provided, PhamClust interprets the input filepath as a directory containing one FASTA file per genome, with headers structured as in the example below:
+If the `-g/--genome-dir` argument is provided, PhamClust interprets the input filepath as a directory containing 
+one FASTA file per genome, with headers structured as in the example below:
 
 ```
 >name=Bipper|pham=pham_1|n=1
 MTAPLLQSVTADDGNMITVPTLQFTRWLDETRDKVIGADGAPDPVRDPMSAYRYLKGRRSVIEGAARQRPMLRLFDKNMDPIAQIAGERLASVEEMMSDSGQANVVLRYDNWLTDFILHQTKIHEDLHLVVDPNPTNRTWRTRWGGKITGINAKRDSSGIHTLELEAISNRQHAKHMLFASNPVFPPEIQLPKMWVLPGNTRTILSISMFVNLARRFFPLLSIPTNIFNPMAWVNGWGAGLDPLMWPLQVAFVNPLLDQSRLSVLGSSWTDWHTAMDSMLKDAGVLFRAYTWLTEDADTPHTELVDMVRGLGPLQDTVDNLTRPHRNCVVFALEDKSGVQGPTGTAADGVINLIGATADDMITETLFNLDRDGDGETDPIFRKLLGVAPEKPKTIWYDGQFSGIIESEIRRHKGPVKKIHTGGRSPSILNQAQTYAIRYALSQLAQVISYGIGAYQQYGTEGLDNLYQGQLDNTLFAWQAFDDPIRALQTGDMAWQEHFERGSGTAYTLSGIVTLRVGHYKTRAWQGFTVKVVNGRPHAVDVDITLGDRAGFEQGGIIFVDQITAIKRSWSRTEPVTVQLSIGDDQDKEDPAARGLRAIQAVWTTLGMLLGEGTIF
 >name=Bipper|pham=pham_37|n=1
 MTSPSGVAVAALKGHTKPRLYTPPLAVNCNIWIAPELSCPCGCGLHAGTSWGFDCIDFLTNVLKWQLIPYQRWLYIHALEKGPGGEGFRFKTLVILIARQNGKTQWLRGLGLWRLYLDSRGRSSPDCPAAKTVVIAAQGLEYAEGTLGEVVNDVKECRALKREFLRHRQTNGKHAMLLSGRRSWRAVAANRKGGRSMSVDLAELDELREHHDWLAWNAITPTTQARQYSQNVAASNAGDKRSVVLRSLRDGAMAKILARDTEDTKTGLFEYSAPQDANPLERKYWPMANPALGYLPGHDEDALAAKAEAMADNMAGFVTEHLCQWVDTLLPGVMPMEDWNATTDPESRRAEGAPVYAAVDVSHSRSKAYIAVASRRSDGLLHVEVVAAHRGTDWVVPWFKARPGKFVAVAVQARGCPASDLIEPLTEAGVPVMELGGAELVRGAGGVLFDGIRKHAIWHRPSPALDTAAKGTVSRSLGGDTWVLDRKNSPVDAAPLVACAAAAWAEGQGPMVPDKVPEVHEWPDEEEIAEWEKELDELQ
 ...
 ```
 
-If a genome encodes more than one copy of a pham (namely, paralogs), each copy after the first should increment the value of `n`.
+If a genome encodes more than one copy of a pham (namely, paralogs), each copy after the first should increment 
+the value of `n`.
 
-Six metrics are available for calculating intergenomic similarities (single-CPU processing speeds estimated in parentheses): 
+Six metrics are available for calculating intergenomic similarities (processing speeds estimated in parentheses 
+as the number of genome pairs calculated per second on an M1 Macbook Pro):
 
 1. Gene Content Similarity (gcs)                    (>100,000 pairs/second)
 2. Jaccard Coefficient (jc)                         (>55,000 pairs/second)
 3. Percentage of Conserved Proteins (pocp)          (>25,000 pairs/second)
 4. Alignment Fraction (AF)                          (>15,000 pairs/second)
 5. Average Aminoacid Identity (aai)                 (~500 pairs/second)
 6. Proteomic Equivalence Quotient (peq)             (~475 pairs/second)
 
-Because of how cheap the first four metrics are, the maximum parallelization benefit is seen with just 4 CPU cores for datasets consisting of fewer than 2,500 genomes. The last two metrics are considerably more expensive to calculate, and will see benefit from as many physical cores are available on your machine (i.e., core count, not thread count). 
+Because of how cheap the first four metrics are, the maximum parallelization benefit is seen with just 4 CPU 
+cores for datasets consisting of fewer than 2,500 genomes. The last two metrics are considerably more expensive 
+to calculate, and will see benefit from as many physical cores are available on your machine (i.e., core count, 
+not thread count), as long as there is enough system memory. 
+
+# Heatmap settings
+
+Among the outputs from PhamClust are per-cluster matrix heatmaps that nicely illustrate the pairwise similarities 
+within clusters/subclusters.
+
+For reasonably small datasets (those with fewer than 1000 genomes), a heatmap will also be drawn for the complete 
+dataset matrix.
+
+Two commandline arguments can be used to alter the appearance of these heatmaps. The `-hc/--heatmap-colors` 
+argument allows you to specify either two or three colors that define the heatmap colorscheme. By default, a 
+3-point gradient is used, where the lowest similarity genome pairs are in red, intermediate similarity genomes 
+pairs are in yellow, and the highest-similarity genome pairs are green. This default behavior is the same as 
+invoking phamclust with `-hc red,yellow,green`. Another visually appealing option might be a 2-color gradient
+from white (0% similar) to green (100% identical), which could be applied with `-hc white,green`.
+
+Any valid CSS named colors can be used:
+
+                aliceblue, antiquewhite, aqua, aquamarine, azure,
+                beige, bisque, black, blanchedalmond, blue,
+                blueviolet, brown, burlywood, cadetblue,
+                chartreuse, chocolate, coral, cornflowerblue,
+                cornsilk, crimson, cyan, darkblue, darkcyan,
+                darkgoldenrod, darkgray, darkgrey, darkgreen,
+                darkkhaki, darkmagenta, darkolivegreen, darkorange,
+                darkorchid, darkred, darksalmon, darkseagreen,
+                darkslateblue, darkslategray, darkslategrey,
+                darkturquoise, darkviolet, deeppink, deepskyblue,
+                dimgray, dimgrey, dodgerblue, firebrick,
+                floralwhite, forestgreen, fuchsia, gainsboro,
+                ghostwhite, gold, goldenrod, gray, grey, green,
+                greenyellow, honeydew, hotpink, indianred, indigo,
+                ivory, khaki, lavender, lavenderblush, lawngreen,
+                lemonchiffon, lightblue, lightcoral, lightcyan,
+                lightgoldenrodyellow, lightgray, lightgrey,
+                lightgreen, lightpink, lightsalmon, lightseagreen,
+                lightskyblue, lightslategray, lightslategrey,
+                lightsteelblue, lightyellow, lime, limegreen,
+                linen, magenta, maroon, mediumaquamarine,
+                mediumblue, mediumorchid, mediumpurple,
+                mediumseagreen, mediumslateblue, mediumspringgreen,
+                mediumturquoise, mediumvioletred, midnightblue,
+                mintcream, mistyrose, moccasin, navajowhite, navy,
+                oldlace, olive, olivedrab, orange, orangered,
+                orchid, palegoldenrod, palegreen, paleturquoise,
+                palevioletred, papayawhip, peachpuff, peru, pink,
+                plum, powderblue, purple, red, rosybrown,
+                royalblue, saddlebrown, salmon, sandybrown,
+                seagreen, seashell, sienna, silver, skyblue,
+                slateblue, slategray, slategrey, snow, springgreen,
+                steelblue, tan, teal, thistle, tomato, turquoise,
+                violet, wheat, white, whitesmoke, yellow,
+                yellowgreen
+
+For 3-point color scales, the `-hm/--heatmap-midpoint` argument can be used to adjust the similarity threshold 
+where the middle color goes. For example, to highlight diversity within clusters (i.e., dissimilarity between 
+subclusters), a midpoint at the subcluster threshold would maximize contrast between intra-subcluster and 
+inter-subcluster similarity values.
```

### Comparing `phamclust-1.2.0/setup.cfg` & `phamclust-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_files = LICENSE
 name = phamclust
-version = 1.2.0
+version = 1.3.0
 author = Christian Gauthier
 author_email = chg60@pitt.edu
 description = Cluster genomes based on gene phamily data
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/chg60/phamclust
 project_urls = 
@@ -27,15 +27,15 @@
 
 [options]
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	joblib>=1.3.0
+	joblib~=1.4.0
 	kaleido~=0.2.0
 	numpy~=1.24.0
 	pandas~=2.0.0
 	parasail~=1.3.0
 	plotly~=5.18.0
 	psutil~=5.9.0
 	scikit-learn~=1.3.0
```

### Comparing `phamclust-1.2.0/src/phamclust/cli.py` & `phamclust-1.3.0/src/phamclust/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     while mem - main / cpus < per_core:
         cpus -= 1
 
     return cpus
 
 
+COLORS = "red,yellow,green"
 CPUS = recommended_cpus()
 EPILOG = """
 Available metrics:
 
     Acronym     Name                                Reference
 (1) gcs         gene content similarity             \
 https://doi.org/10.1038/nmicrobiol.2017.112
@@ -47,20 +48,20 @@
 https://doi.org/10.1093/nar/gkv657
 (5) aai         average aminoacid identity          \
 https://doi.org/10.1073/pnas.0409727102
 (6) peq         proteomic equivalence quotient      \
 https://doi.org/10.1128/msystems.00443-23
 """
 LINKAGES = {"single", "average", "complete"}
-METRICS = {"gcs": gene_content_similarity,
-           "jc": jaccard_coefficient,
+METRICS = {"gcs":  gene_content_similarity,
+           "jc":   jaccard_coefficient,
            "pocp": percentage_of_conserved_proteins,
-           "af": alignment_fraction,
-           "aai": average_aminoacid_identity,
-           "peq": proteomic_equivalence_quotient}
+           "af":   alignment_fraction,
+           "aai":  average_aminoacid_identity,
+           "peq":  proteomic_equivalence_quotient}
 K_MIN = 6                       # Minimum size of cluster to sub-cluster
 METRIC = "peq"                  # Default metric
 NR_THRESH = 0.75                # Default 1st iteration cluster threshold
 NR_LINKAGE = "complete"         # Default 1st iteration cluster linkage
 CLU_THRESH = 0.25               # Default 2nd iteration cluster threshold
 CLU_LINKAGE = "average"         # Default 2nd iteration cluster linkage
 SUB_THRESH = 0.6                # Default subclustering threshold
@@ -112,14 +113,25 @@
                    type=str, choices=LINKAGES, default=NR_LINKAGE, metavar="",
                    help=f"linkage type to use for pre-grouping very similar "
                         f"genomes [default: {NR_LINKAGE}]")
     c.add_argument("-m", "--metric",
                    type=str, choices=METRICS, default=METRIC, metavar="",
                    help=f"relatedness index to use for pairwise genome "
                         f"comparisons [default: {METRIC}]")
+
+    h = p.add_argument_group("heatmap arguments:")
+    h.add_argument("-hc", "--heatmap-colors",
+                   type=str, default=COLORS, metavar="",
+                   help=f"comma-separated list of 2 or 3 colors to use in "
+                        f"heatmaps [default: %(default)s]")
+    h.add_argument("-hm", "--heatmap-midpoint",
+                   type=float, default=None, metavar="",
+                   help=f"midpoint to use for color gradient in heatmaps "
+                        f"[default: same as clustering threshold]")
+
     p.add_argument("-d", "--debug", action="store_true",
                    help=f"increase verbosity of logging for debug purposes")
     p.add_argument("-n", "--no-sub", action="store_true",
                    help="do not perform sub-clustering")
     p.add_argument("-r", "--remove-tmp", action="store_true",
                    help=f"remove temporary files (not recommended if repeated "
                         f"runs are planned on the same dataset)")
```

### Comparing `phamclust-1.2.0/src/phamclust/clustering.py` & `phamclust-1.3.0/src/phamclust/clustering.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust/fasta.py` & `phamclust-1.3.0/src/phamclust/fasta.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust/genome.py` & `phamclust-1.3.0/src/phamclust/genome.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust/matrix.py` & `phamclust-1.3.0/src/phamclust/matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -463,25 +463,17 @@
     # <<< End sanity checks <<<
 
     # <<< Initialize distance matrix, populate the diagonal for "free" >>>
     matrix = SymMatrix(nodes=[g.name for g in genomes], is_distance=as_distance)
     for genome in genomes:
         matrix.set_weight(genome.name, genome.name, 1.0 - as_distance)
 
-    # TODO: when version 1.4 is formally released, bump joblib in requirements
-    #  and remove try/except initialization in favor of 1.4-only!
     # Initialize parallel runner - disable memory mapping
-    try:
-        # joblib version must be at least 1.4 to support this better approach
-        runner = joblib.Parallel(n_jobs=cpus, return_as="generator_unordered",
-                                 max_nbytes=None)
-    except ValueError:
-        # joblib version 1.3 roll back to this approach
-        runner = joblib.Parallel(n_jobs=cpus, return_as="generator",
-                                 max_nbytes=None)
+    runner = joblib.Parallel(n_jobs=cpus, return_as="generator_unordered",
+                             max_nbytes=None)
 
     # Determine how many batches to chunk the data into - target
     # 10,000 calculations per cpu per batch
     stride = int(len(genomes) // (n_pairs / (10000 * cpus)))
     iter_order = [i for i in _outside_in_index_iterator(len(genomes))]
     batches = [iter_order[i:i+stride] for i in range(0, len(genomes), stride)]
     for batch_indices in batches:
@@ -615,15 +607,15 @@
     # Analyze diagonal: all values should be the same
     if len(diagonal) > 1:
         raise ValueError(f"values on matrix diagonal should be identical")
 
     # Analyze diagonal: should be either 0.0 (distance) or 1.0 (similarity)
     if sum(diagonal) == 0.0:
         is_distance = True
-    elif sum(diagonal) == 1.0:
+    elif sum(diagonal) == len(diagonal):
         is_distance = False
     else:
         raise ValueError(f"values on matrix diagonal can only be 0.0 or 1.0")
 
     # Create the matrix
     matrix = SymMatrix(names, is_distance=is_distance)
     for i, (target, row) in enumerate(read_squareform(filepath)):
@@ -639,15 +631,15 @@
     :param filepath: the file to read the squareform matrix from
     :type filepath: pathlib.Path
     :rtype: typing.Generator[tuple[str, list[float]]]
     """
     with open(filepath, "r") as squareform_reader:
         next(squareform_reader)     # skip first line, only has matrix size
         for row in squareform_reader:
-            row = row.rstrip().split()
+            row = row.rstrip().split("\t")
             name = row[0]
             row = [float(x) for x in row[1:]]
             yield name, row
 
 
 def matrix_to_squareform(matrix, filepath, lower_triangle=False):
     """Write matrix to a file, as a squareform matrix.
@@ -669,15 +661,15 @@
 
         for i, (source, row) in enumerate(matrix.iterrows()):
             if not lower_triangle:
                 row = "\t".join([f"{x:.6f}" for x in row])
             else:
                 row = "\t".join([f"{x:.6f}" for x in row[:i + 1]])
 
-            squareform_writer.write(f"{source:<24}\t{row}\n")
+            squareform_writer.write(f"{source}\t{row}\n")
 
     return filepath
 
 
 def _get_tree_order(matrix):
     """Return the distance-sorted leaf (node) order for a given matrix.
```

### Comparing `phamclust-1.2.0/src/phamclust/metrics.py` & `phamclust-1.3.0/src/phamclust/metrics.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust/parallel_process.py` & `phamclust-1.3.0/src/phamclust/parallel_process.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust/scripts/benchmark.py` & `phamclust-1.3.0/src/phamclust/scripts/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import argparse
 import datetime
 import pathlib
 import random
 
 from phamclust.cli import METRICS
 from phamclust.matrix import matrix_de_novo, matrix_to_squareform
-from phamclust.__main__ import load_genomes_from_tsv
+from phamclust.scripts.phamclust import load_genomes_from_tsv
 
 # Common values that might be found/used on modern commodity hardware
 CPUS = [1, 2, 4, 6, 8, 12, 16]
 
-# RefSeq phages number ~5,000, so these are realistic test numbers
-SAMPLE_SIZES = [500, 1000, 2000, 3000]
+SAMPLE_SIZES = [2000, 1000, 500]
 
 # Default: run each test this many times to get representative outcomes
 ITER = 3
 
 # Random seed
 SEED = 42
```

### Comparing `phamclust-1.2.0/src/phamclust/scripts/phamclust.py` & `phamclust-1.3.0/src/phamclust/scripts/phamclust.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 import shutil
 import sys
 
 from phamclust.cli import parse_args, METRICS
 from phamclust.clustering import hierarchical_clustering
 from phamclust.genome import Genome
-from phamclust.heatmap import draw_heatmap
+from phamclust.heatmap import draw_heatmap, CSS_COLORS
 from phamclust.matrix import matrix_de_novo, matrix_to_squareform, \
     matrix_from_squareform, matrix_to_adjacency
 
 LOG_STR_FMT = "phamclust: %(asctime)s.%(msecs)03d: %(levelname)s: %(message)s"
 LOG_TIME_FMT = "%H:%M:%S"
 
 
@@ -135,15 +135,15 @@
     none_diff = empty_cnt - 0
 
     return cell_diff, diag_diff, none_diff
 
 
 def phamclust(infile, outdir, is_genome_dir, metric, nr_distance, nr_linkage,
               clu_distance, clu_linkage, sub_distance, sub_linkage, k_min,
-              no_sub, cpus, rm_tmp, debug):
+              no_sub, colors, midpoint, cpus, rm_tmp, debug):
     """Main program for phamclust.
 
     :param infile: input TSV file mapping phage-to-pham-to-translation
     :type infile: pathlib.Path
     :param outdir: output directory where files should be written
     :type outdir: pathlib.Path
     :param is_genome_dir: indicate that infile should instead be
@@ -169,14 +169,18 @@
     :param sub_linkage: hierarchical clustering linkage type to use for
         sub-clustering genome clusters
     :type sub_linkage: str
     :param k_min: minimum size of cluster to perform sub-clustering on
     :type k_min: int
     :param no_sub: indicate that sub-clustering should not be performed
     :type no_sub: bool
+    :param colors: colors to use in heatmaps
+    :type colors: list[str]
+    :param midpoint: midpoint of the color gradient in heatmaps
+    :type midpoint: float
     :param cpus: number of CPUs to use for distance calculations
     :type cpus: int
     :param rm_tmp: remove temporary files when done
     :type rm_tmp: bool
     :param debug: indicate if logging should be set to DEBUG level
     :type debug: bool
     """
@@ -196,14 +200,16 @@
     logging.info(f"sub link:   {sub_linkage}")
     logging.info(f"clu dist:   {clu_distance}")
     logging.info(f"clu link:   {clu_linkage}")
     logging.info(f"nr dist:    {nr_distance}")
     logging.info(f"nr link:    {nr_linkage}")
     logging.info(f"metric:     {metric}")
     logging.info(f"cpus:       {cpus}")
+    logging.info(f"colors:     {','.join(colors)}")
+    logging.info(f"midpoint:   {midpoint}")
 
     # Parse genomes from TSV-formatted infile
     logging.info(f"====================")
     logging.info(f" 1: parsing genomes ")
     logging.info(f"====================")
     if is_genome_dir:
         genomes = load_genomes_from_fasta_dir(infile)
@@ -349,47 +355,45 @@
             genome_file = genome_dir.joinpath(f"{genome.name}.faa")
             genome.save(genome_file)
             logging.debug(f"wrote genome to {genome_file}")
 
         if no_sub or len(clu_mat) < k_min:
             logging.debug(f"not sub-clustering {len(clu_mat)} genomes")
 
-            # Re-order matrix in order of proximity to the medoid; convert to
-            # similarity matrix
-            # order = [clu_mat.medoid[0]]
-            # order.extend(clu_mat.nearest_neighbors(order[0], threshold=1.0))
+            # Re-order matrix in distance tree order
             clu_mat.reorder()
             clu_mat.invert()
             matrix_to_squareform(clu_mat, cluster_matfile)
-            draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap)
-            draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap2)
+            draw_heatmap(clu_mat, colors=colors, midpoint=midpoint,
+                         filename=cluster_heatmap)
+            draw_heatmap(clu_mat, colors=colors, midpoint=midpoint,
+                         filename=cluster_heatmap2)
             continue
         else:
             sub_mats = hierarchical_clustering(clu_mat, eps=sub_distance,
                                                linkage=sub_linkage)
             sub_mats = sorted(sub_mats, reverse=True)
             order = list()
             for j, sub_mat in enumerate(sub_mats):
                 sub_matfile = cluster_dir.joinpath(
                     f"subcluster_{j+1}_similarity.tsv")
-                # _ord = [sub_mat.medoid[0]]
-                # _ord.extend(sub_mat.nearest_neighbors(_ord[0], threshold=1.0))
-                # order.extend(_ord)
                 # Can't re-order a matrix with only a single node, and order
                 # doesn't matter for just 2 nodes
                 if len(sub_mat) > 2:
                     sub_mat.reorder()
                 order.extend(sub_mat.nodes)
                 sub_mat.invert()
                 matrix_to_squareform(sub_mat, sub_matfile)
             clu_mat.reorder(order)
             clu_mat.invert()
             matrix_to_squareform(clu_mat, cluster_matfile)
-            draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap)
-            draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap2)
+            draw_heatmap(clu_mat, colors=colors, midpoint=midpoint,
+                         filename=cluster_heatmap)
+            draw_heatmap(clu_mat, colors=colors, midpoint=midpoint,
+                         filename=cluster_heatmap2)
             continue
 
     # Make a toplevel directory for singletons, with nested genome dir
     if single_mats:
         single_dir = tmp_clusters.joinpath(f"singletons")
         if single_dir.is_dir():
             logging.debug(f"removing old singleton directory {single_dir}")
@@ -416,25 +420,29 @@
     dataset_order = list()
     for clu_mat in sorted(clu_mats, reverse=True):
         dataset_order.extend(clu_mat.nodes)
     for single_mat in single_mats:
         dataset_order.extend(single_mat.nodes)
 
     dataset_html = tmp_clusters.joinpath(f"{metric}_heatmap.html")
+    dataset_svg = tmp_clusters.joinpath(f"{metric}_heatmap.svg")
     dist_mat.reorder(dataset_order)
 
-    logging.info(f"convert to similarity matrix for easier visualization")
+    logging.info(f"cast to similarity matrix for easier visualization")
     dist_mat.invert()
 
-    if len(dist_mat) > 5000:
+    if len(dist_mat) > 1500:
         logging.info(f"full pairwise matrix is too large to visualize")
     else:
         logging.info(f"drawing heatmap HTML and saving to {dataset_html}")
-        draw_heatmap(dist_mat, midpoint=1.0 - clu_distance,
+        draw_heatmap(dist_mat, colors=colors, midpoint=1.0 - clu_distance,
                      filename=dataset_html)
+        logging.info(f"drawing heatmap SVG and saving to {dataset_svg}")
+        draw_heatmap(dist_mat, colors=colors, midpoint=1.0 - clu_distance,
+                     filename=dataset_svg)
 
     # Copy output files to output directory
     logging.info(f"========================")
     logging.info(f" 6: move output files   ")
     logging.info(f"========================")
     logging.info(f"removing contents from existing output directory {outdir}")
     for fp in outdir.iterdir():
@@ -488,26 +496,49 @@
     if args.debug:
         log_level = logging.DEBUG
 
     logging.basicConfig(filename=logfile, filemode="w", level=log_level,
                         format=LOG_STR_FMT, datefmt=LOG_TIME_FMT)
     logging.getLogger().addHandler(logging.StreamHandler(sys.stdout))
 
+    # sanity-check colors - must be a list of either 2 or 3 valid colors
+    colors = args.heatmap_colors.split(",")
+    if not 2 <= len(colors) <= 3:
+        logging.error(f"expected either two or three colors, got {len(colors)}")
+        sys.exit(1)
+    if len(colors) == 2:
+        logging.warning("2-color scale ignores `--heatmap-midpoint`")
+
+    valid_colors = []
+    for color in colors:
+        if color not in CSS_COLORS:
+            logging.error(f"unknown color specified: '{color}'")
+            continue
+        valid_colors.append(color)
+    if len(valid_colors) != len(colors):
+        logging.error(f"got {len(colors) - len(valid_colors)} unrecognized "
+                      f"colors")
+        logging.error(f"valid colors:")
+        logging.error(f"{' '.join(CSS_COLORS)}")
+        sys.exit(1)
+
     # Run PhamClust!
     phamclust(infile=args.infile,
               outdir=args.outdir,
               is_genome_dir=args.genome_dir,
               metric=args.metric,
               nr_distance=round(1.0 - args.nr_thresh, 6),
               nr_linkage=args.nr_linkage,
               clu_distance=round(1.0 - args.clu_thresh, 6),
               clu_linkage=args.clu_linkage,
               sub_distance=round(1.0 - args.sub_thresh, 6),
               sub_linkage=args.sub_linkage,
               k_min=max([1, args.k_min]),
+              colors=valid_colors,
+              midpoint=round(args.heatmap_midpoint, 6),
               cpus=args.threads,
               no_sub=args.no_sub,
               rm_tmp=args.remove_tmp,
               debug=args.debug)
 
 
 if __name__ == "__main__":
```

### Comparing `phamclust-1.2.0/src/phamclust/statistics.py` & `phamclust-1.3.0/src/phamclust/statistics.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.2.0/src/phamclust.egg-info/PKG-INFO` & `phamclust-1.3.0/src/phamclust.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 1.2.0
+Version: 1.3.0
 Summary: Cluster genomes based on gene phamily data
 Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,27 +18,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: joblib>=1.3.0
+Requires-Dist: joblib~=1.4.0
 Requires-Dist: kaleido~=0.2.0
 Requires-Dist: numpy~=1.24.0
 Requires-Dist: pandas~=2.0.0
 Requires-Dist: parasail~=1.3.0
 Requires-Dist: plotly~=5.18.0
 Requires-Dist: psutil~=5.9.0
 Requires-Dist: scikit-learn~=1.3.0
 Requires-Dist: scipy~=1.10.0
 
 # phamclust
 
-PhamClust is a tool for performing gene phamily based clustering of bacteriophage genomes. It makes use of a novel genome similarity index, the proteomic equivalence quotient (PEQ) to cluster genomes according to their global similarity. A manuscript describing it in detail has been submitted for publication at mSphere.
+PhamClust is a tool for performing gene phamily based clustering of bacteriophage genomes. It makes use of a novel genome 
+similarity index, the proteomic equivalence quotient (PEQ) to cluster genomes according to their global similarity. It was 
+[published in mSphere](https://doi.org/10.1128/msystems.00443-23) in 2023.
 
 # Installation
 
 The most straightforward way to install PhamClust is from the Python Package Index (PyPI): `pip install phamclust`
 
 # Usage
 
@@ -58,52 +60,123 @@
   -h, --help            show this help message and exit
   -g, --genome-dir      interpret `infile` as a directory of genome FASTA files instead of TSV
   -d, --debug           increase verbosity of logging for debug purposes
   -n, --no-sub          do not perform sub-clustering
   -r, --remove-tmp      remove temporary files (not recommended if repeated runs are planned on the same dataset)
   -t , --threads        number of CPU cores to use [default: 16]
 
-clustering arguments::
+clustering arguments:
   -k , --k-min          minimum cluster size to perform subclustering [default: 6]
   -s , --sub-thresh     similarity threshold to use for sub-clustering [default: 0.6]
   -sl , --sub-linkage   linkage type to use for sub-clustering [default: single]
   -c , --clu-thresh     similarity threshold to use for clustering [default: 0.25]
   -cl , --clu-linkage   linkage type to use for clustering [default: average]
   -nr , --nr-thresh     similarity threshold above which to pre-group very similar genomes that must be clustered together [default: 0.75]
   -nl , --nr-linkage    linkage type to use for pre-grouping very similar genomes [default: complete]
   -m , --metric         relatedness index to use for pairwise genome comparisons [default: peq]
+  
+heatmap arguments:
+  -hc , --heatmap-colors
+                        comma-separated list of 2 or 3 colors to use in heatmaps [default: red,yellow,green]
+  -hm , --heatmap-midpoint
+                        midpoint to use for color gradient in heatmaps [default: same as clustering threshold]
 
 Available metrics:
 
     Acronym     Name                                Reference
 (1) gcs         gene content similarity             https://doi.org/10.1038/nmicrobiol.2017.112
 (2) jc          jaccard coefficient                 https://doi.org/10.1111/j.1469-8137.1912.tb05611.x
 (3) pocp        percentage of conserved proteins    https://doi.org/10.1128/JB.01688-14
 (4) af          alignment fraction                  https://doi.org/10.1093/nar/gkv657
 (5) aai         average aminoacid identity          https://doi.org/10.1073/pnas.0409727102
 (6) peq         proteomic equivalence quotient      https://doi.org/10.1128/msystems.00443-23
 ```
 
-PhamClust takes an input filepath and an output filepath as its primary arguments. By default, the input path is assumed to be a TSV file mapping genome names/identifiers to pham identifiers and translations.
+PhamClust takes an input filepath and an output filepath as its primary arguments. By default, the input path is 
+assumed to be a TSV file mapping genome names/identifiers to pham identifiers and translations.
 
-If the `-g/--genome-dir` argument is provided, PhamClust interprets the input filepath as a directory containing one FASTA file per genome, with headers structured as in the example below:
+If the `-g/--genome-dir` argument is provided, PhamClust interprets the input filepath as a directory containing 
+one FASTA file per genome, with headers structured as in the example below:
 
 ```
 >name=Bipper|pham=pham_1|n=1
 MTAPLLQSVTADDGNMITVPTLQFTRWLDETRDKVIGADGAPDPVRDPMSAYRYLKGRRSVIEGAARQRPMLRLFDKNMDPIAQIAGERLASVEEMMSDSGQANVVLRYDNWLTDFILHQTKIHEDLHLVVDPNPTNRTWRTRWGGKITGINAKRDSSGIHTLELEAISNRQHAKHMLFASNPVFPPEIQLPKMWVLPGNTRTILSISMFVNLARRFFPLLSIPTNIFNPMAWVNGWGAGLDPLMWPLQVAFVNPLLDQSRLSVLGSSWTDWHTAMDSMLKDAGVLFRAYTWLTEDADTPHTELVDMVRGLGPLQDTVDNLTRPHRNCVVFALEDKSGVQGPTGTAADGVINLIGATADDMITETLFNLDRDGDGETDPIFRKLLGVAPEKPKTIWYDGQFSGIIESEIRRHKGPVKKIHTGGRSPSILNQAQTYAIRYALSQLAQVISYGIGAYQQYGTEGLDNLYQGQLDNTLFAWQAFDDPIRALQTGDMAWQEHFERGSGTAYTLSGIVTLRVGHYKTRAWQGFTVKVVNGRPHAVDVDITLGDRAGFEQGGIIFVDQITAIKRSWSRTEPVTVQLSIGDDQDKEDPAARGLRAIQAVWTTLGMLLGEGTIF
 >name=Bipper|pham=pham_37|n=1
 MTSPSGVAVAALKGHTKPRLYTPPLAVNCNIWIAPELSCPCGCGLHAGTSWGFDCIDFLTNVLKWQLIPYQRWLYIHALEKGPGGEGFRFKTLVILIARQNGKTQWLRGLGLWRLYLDSRGRSSPDCPAAKTVVIAAQGLEYAEGTLGEVVNDVKECRALKREFLRHRQTNGKHAMLLSGRRSWRAVAANRKGGRSMSVDLAELDELREHHDWLAWNAITPTTQARQYSQNVAASNAGDKRSVVLRSLRDGAMAKILARDTEDTKTGLFEYSAPQDANPLERKYWPMANPALGYLPGHDEDALAAKAEAMADNMAGFVTEHLCQWVDTLLPGVMPMEDWNATTDPESRRAEGAPVYAAVDVSHSRSKAYIAVASRRSDGLLHVEVVAAHRGTDWVVPWFKARPGKFVAVAVQARGCPASDLIEPLTEAGVPVMELGGAELVRGAGGVLFDGIRKHAIWHRPSPALDTAAKGTVSRSLGGDTWVLDRKNSPVDAAPLVACAAAAWAEGQGPMVPDKVPEVHEWPDEEEIAEWEKELDELQ
 ...
 ```
 
-If a genome encodes more than one copy of a pham (namely, paralogs), each copy after the first should increment the value of `n`.
+If a genome encodes more than one copy of a pham (namely, paralogs), each copy after the first should increment 
+the value of `n`.
 
-Six metrics are available for calculating intergenomic similarities (single-CPU processing speeds estimated in parentheses): 
+Six metrics are available for calculating intergenomic similarities (processing speeds estimated in parentheses 
+as the number of genome pairs calculated per second on an M1 Macbook Pro):
 
 1. Gene Content Similarity (gcs)                    (>100,000 pairs/second)
 2. Jaccard Coefficient (jc)                         (>55,000 pairs/second)
 3. Percentage of Conserved Proteins (pocp)          (>25,000 pairs/second)
 4. Alignment Fraction (AF)                          (>15,000 pairs/second)
 5. Average Aminoacid Identity (aai)                 (~500 pairs/second)
 6. Proteomic Equivalence Quotient (peq)             (~475 pairs/second)
 
-Because of how cheap the first four metrics are, the maximum parallelization benefit is seen with just 4 CPU cores for datasets consisting of fewer than 2,500 genomes. The last two metrics are considerably more expensive to calculate, and will see benefit from as many physical cores are available on your machine (i.e., core count, not thread count). 
+Because of how cheap the first four metrics are, the maximum parallelization benefit is seen with just 4 CPU 
+cores for datasets consisting of fewer than 2,500 genomes. The last two metrics are considerably more expensive 
+to calculate, and will see benefit from as many physical cores are available on your machine (i.e., core count, 
+not thread count), as long as there is enough system memory. 
+
+# Heatmap settings
+
+Among the outputs from PhamClust are per-cluster matrix heatmaps that nicely illustrate the pairwise similarities 
+within clusters/subclusters.
+
+For reasonably small datasets (those with fewer than 1000 genomes), a heatmap will also be drawn for the complete 
+dataset matrix.
+
+Two commandline arguments can be used to alter the appearance of these heatmaps. The `-hc/--heatmap-colors` 
+argument allows you to specify either two or three colors that define the heatmap colorscheme. By default, a 
+3-point gradient is used, where the lowest similarity genome pairs are in red, intermediate similarity genomes 
+pairs are in yellow, and the highest-similarity genome pairs are green. This default behavior is the same as 
+invoking phamclust with `-hc red,yellow,green`. Another visually appealing option might be a 2-color gradient
+from white (0% similar) to green (100% identical), which could be applied with `-hc white,green`.
+
+Any valid CSS named colors can be used:
+
+                aliceblue, antiquewhite, aqua, aquamarine, azure,
+                beige, bisque, black, blanchedalmond, blue,
+                blueviolet, brown, burlywood, cadetblue,
+                chartreuse, chocolate, coral, cornflowerblue,
+                cornsilk, crimson, cyan, darkblue, darkcyan,
+                darkgoldenrod, darkgray, darkgrey, darkgreen,
+                darkkhaki, darkmagenta, darkolivegreen, darkorange,
+                darkorchid, darkred, darksalmon, darkseagreen,
+                darkslateblue, darkslategray, darkslategrey,
+                darkturquoise, darkviolet, deeppink, deepskyblue,
+                dimgray, dimgrey, dodgerblue, firebrick,
+                floralwhite, forestgreen, fuchsia, gainsboro,
+                ghostwhite, gold, goldenrod, gray, grey, green,
+                greenyellow, honeydew, hotpink, indianred, indigo,
+                ivory, khaki, lavender, lavenderblush, lawngreen,
+                lemonchiffon, lightblue, lightcoral, lightcyan,
+                lightgoldenrodyellow, lightgray, lightgrey,
+                lightgreen, lightpink, lightsalmon, lightseagreen,
+                lightskyblue, lightslategray, lightslategrey,
+                lightsteelblue, lightyellow, lime, limegreen,
+                linen, magenta, maroon, mediumaquamarine,
+                mediumblue, mediumorchid, mediumpurple,
+                mediumseagreen, mediumslateblue, mediumspringgreen,
+                mediumturquoise, mediumvioletred, midnightblue,
+                mintcream, mistyrose, moccasin, navajowhite, navy,
+                oldlace, olive, olivedrab, orange, orangered,
+                orchid, palegoldenrod, palegreen, paleturquoise,
+                palevioletred, papayawhip, peachpuff, peru, pink,
+                plum, powderblue, purple, red, rosybrown,
+                royalblue, saddlebrown, salmon, sandybrown,
+                seagreen, seashell, sienna, silver, skyblue,
+                slateblue, slategray, slategrey, snow, springgreen,
+                steelblue, tan, teal, thistle, tomato, turquoise,
+                violet, wheat, white, whitesmoke, yellow,
+                yellowgreen
+
+For 3-point color scales, the `-hm/--heatmap-midpoint` argument can be used to adjust the similarity threshold 
+where the middle color goes. For example, to highlight diversity within clusters (i.e., dissimilarity between 
+subclusters), a midpoint at the subcluster threshold would maximize contrast between intra-subcluster and 
+inter-subcluster similarity values.
```

### Comparing `phamclust-1.2.0/src/phamclust.egg-info/SOURCES.txt` & `phamclust-1.3.0/src/phamclust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

