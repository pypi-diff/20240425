# Comparing `tmp/splicekit-0.5.1.tar.gz` & `tmp/splicekit-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.5.1.tar", last modified: Wed Feb  7 10:18:55 2024, max compression
+gzip compressed data, was "splicekit-0.6.tar", last modified: Thu Apr 25 08:53:31 2024, max compression
```

## Comparing `splicekit-0.5.1.tar` & `splicekit-0.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.225529 splicekit-0.5.1/
--rw-r--r--   0 rotg     (2023757) games       (20)     4737 2024-02-07 10:18:55.221412 splicekit-0.5.1/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)     4096 2023-11-27 13:00:07.000000 splicekit-0.5.1/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2024-02-07 10:18:55.225652 splicekit-0.5.1/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1242 2023-12-01 11:09:11.000000 splicekit-0.5.1/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.132593 splicekit-0.5.1/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    21467 2024-02-01 14:14:53.000000 splicekit-0.5.1/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.153585 splicekit-0.5.1/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5750 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.155104 splicekit-0.5.1/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1443 2024-01-25 15:46:58.000000 splicekit-0.5.1/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.210988 splicekit-0.5.1/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      930 2023-11-30 15:16:11.000000 splicekit-0.5.1/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     7454 2024-02-07 07:23:48.000000 splicekit-0.5.1/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    25165 2024-02-07 10:17:13.000000 splicekit-0.5.1/splicekit/core/annotation.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     2535 2024-01-15 15:34:47.000000 splicekit-0.5.1/splicekit/core/comps_edgeR.R
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-09-05 12:26:35.000000 splicekit-0.5.1/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6755 2024-02-07 07:23:35.000000 splicekit-0.5.1/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    31588 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     7143 2024-02-07 07:23:58.000000 splicekit-0.5.1/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    10009 2024-01-19 10:48:53.000000 splicekit-0.5.1/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2745 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    17593 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    39867 2024-01-18 12:54:08.000000 splicekit-0.5.1/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1969 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2441 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    11910 2024-01-16 11:39:03.000000 splicekit-0.5.1/splicekit/core/report.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1235 2024-02-05 15:53:20.000000 splicekit-0.5.1/splicekit/folders.setup
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.212355 splicekit-0.5.1/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26727 2024-01-25 11:30:26.000000 splicekit-0.5.1/splicekit/judge/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.215289 splicekit-0.5.1/splicekit/report/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13300 2024-01-30 14:43:56.000000 splicekit-0.5.1/splicekit/report/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5412 2024-01-12 08:54:37.000000 splicekit-0.5.1/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5716 2024-02-01 14:12:40.000000 splicekit-0.5.1/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1976 2024-01-16 12:00:37.000000 splicekit-0.5.1/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2024-02-07 10:18:39.000000 splicekit-0.5.1/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-02-07 10:18:55.220014 splicekit-0.5.1/splicekit.egg-info/
--rw-r--r--   0 rotg     (2023757) games       (20)     4737 2024-02-07 10:18:54.000000 splicekit-0.5.1/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      874 2024-02-07 10:18:54.000000 splicekit-0.5.1/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2024-02-07 10:18:54.000000 splicekit-0.5.1/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-11-23 10:29:09.000000 splicekit-0.5.1/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)      120 2024-02-07 10:18:54.000000 splicekit-0.5.1/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2024-02-07 10:18:54.000000 splicekit-0.5.1/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.492697 splicekit-0.6/
+-rw-r--r--   0 rotg     (2023757) games       (20)     5381 2024-04-25 08:53:31.492095 splicekit-0.6/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     4742 2024-04-25 08:51:36.000000 splicekit-0.6/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2024-04-25 08:53:31.492803 splicekit-0.6/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1242 2023-12-01 11:09:11.000000 splicekit-0.6/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.471412 splicekit-0.6/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    21688 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.475483 splicekit-0.6/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5750 2024-01-12 08:54:37.000000 splicekit-0.6/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.476470 splicekit-0.6/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1443 2024-02-07 14:52:24.000000 splicekit-0.6/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.487804 splicekit-0.6/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1085 2024-03-05 15:05:12.000000 splicekit-0.6/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7463 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    24716 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/annotation.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     2535 2024-03-12 14:12:01.000000 splicekit-0.6/splicekit/core/comps_edgeR.R
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-09-05 12:26:35.000000 splicekit-0.6/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6484 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    28547 2024-04-12 13:02:19.000000 splicekit-0.6/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7153 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10024 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2745 2024-01-12 08:54:37.000000 splicekit-0.6/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18646 2024-04-25 08:52:04.000000 splicekit-0.6/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37200 2024-04-12 12:30:37.000000 splicekit-0.6/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1908 2024-04-12 12:12:52.000000 splicekit-0.6/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2488 2024-04-17 07:34:48.000000 splicekit-0.6/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9035 2024-04-16 09:47:05.000000 splicekit-0.6/splicekit/core/report.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1264 2024-02-15 12:48:03.000000 splicekit-0.6/splicekit/folders.setup
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.488871 splicekit-0.6/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26727 2024-02-07 14:52:24.000000 splicekit-0.6/splicekit/judge/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.489918 splicekit-0.6/splicekit/june/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8908 2024-04-12 13:07:48.000000 splicekit-0.6/splicekit/june/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.490968 splicekit-0.6/splicekit/report/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    22825 2024-03-26 11:12:29.000000 splicekit-0.6/splicekit/report/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5412 2024-01-12 08:54:37.000000 splicekit-0.6/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5829 2024-03-15 14:26:18.000000 splicekit-0.6/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1976 2024-01-16 12:00:37.000000 splicekit-0.6/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        4 2024-04-25 08:52:50.000000 splicekit-0.6/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2024-04-25 08:53:31.474954 splicekit-0.6/splicekit.egg-info/
+-rw-r--r--   0 rotg     (2023757) games       (20)     5381 2024-04-25 08:53:31.471981 splicekit-0.6/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      901 2024-04-25 08:53:31.472888 splicekit-0.6/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2024-04-25 08:53:31.473441 splicekit-0.6/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-11-23 10:29:09.000000 splicekit-0.6/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)      120 2024-04-25 08:53:31.474386 splicekit-0.6/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2024-04-25 08:53:31.475045 splicekit-0.6/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.5.1/PKG-INFO` & `splicekit-0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.5.1
+Version: 0.6
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -21,14 +21,18 @@
 Requires-Dist: requests
 Requires-Dist: rangehttpserver
 
 ## splicekit: an integrative toolkit for splicing analysis from short-read RNA-seq
 
 <b>splicekit</b> is a modular platform for splicing analysis from short-read RNA-seq datasets. The platform also integrates an JBrowse2 instance, [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
+Check a short video presentation about splicekit (poster) at ECCB 2023 on Youtube:
+
+[<img src="media/splicekit_youtube.jpg" width=300>](https://youtu.be/P1m73usZ3lc?si=HBJxWOkUajObFpu1)
+
 ## Quick start
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute:
@@ -37,21 +41,15 @@
 
 Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 <details>
 <summary>Installing splicekit directly from the GitHub repository</summary>
 
 ```
-# move to HOME folder (for example)
-cd ~
-# clone the repository
-git clone git@github.com:bedapub/splicekit.git
-# adjust PYTHONPATH and PATH
-export PYTHONPATH=$PYTHONPATH:~/splicekit
-export PATH=$PATH:~/splicekit/splicekit
+pip install git+https://github.com/bedapub/splicekit.git@main
 ```
 </details>
 
 <details>
 <summary>If you already have aligned reads in BAM files</summary>
 
 All you need is `samples.tab` (note that this is a <b>TAB delimited file</b>) and `splicekit.config` in one folder (check [datasets](datasets) for examples).
@@ -66,53 +64,66 @@
 ## Documentation
 
 * [PDF reference manual](https://github.com/bedapub/splicekit/raw/main/docs/splicekit_docs.pdf)
 * [Google docs](https://docs.google.com/document/d/15ZRCeK8xyg3klLktZSHZ9k__Xw_BZRn_Q-J4W35JNnQ/edit?usp=sharing) of the above PDF (comment if you like)
 
 ## Changelog<a name="changelog"></a>
 
-**v0.4.9**: released in November 2023
+**v0.6**: released in April 2024
+
+* updated reports
+* JUNE analysis (junction-events to classify skipped and mutually exclusive exons)
+
+<details>
+<summary>Past changenotes (click to view)</summary>
+
+<b>v0.4.9</b>: released in November 2023
+
 * added rMATS analysis for splicing events
 * added Docker container that can be directly imported to singularity via ghcr.io
 * fixed dependencies
 * other small fixes
 
-<details>
-<summary><b>v0.4</b>: released in May 2023 (click to show details)</summary>
+<b>v0.4</b>: released in May 2023
 
 * added singularity container with all dependencies
 * added local integrated JBrowse2
 * cluster or desktop runs
 * scanRBP and bootstrap analysis of RNA-protein binding
 * further development and integration with pybio
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+<b>v0.3</b>: released in January 2023 (click to show details)
 
 * re-coded junction analysis
   * independent junctions parsing from provided bam files
   * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
 * clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
 * added *first_exon* annotation for junctions touching annotated first exons of transcripts
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+<b>v0.2</b>: released in October 2022
 
 * software architecture restructure with python modules
 * filtering of lowly expressed features by edgeR
 * DonJuan analysis (junction-anchor analysis)
 * more advanced motif analysis with DREME
 * filtering regulated junctions with regulated donors
-</details>
 
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+<b>v0.1</b>: released in July 2022
 
 * initial version of splicekit
 * parsing of junction and exon counts
 * computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
 * basic motif analysis
+
 </details>
+
+## Citing and Contact<a name="citation"></a>
+
+If you find **splicekit** useful in your work and research, please cite:
+
+Gregor Rot, Arne Wehling, Roland Schmucki, Nikolaos Berntenis, Jitao David Zhang, Martin Ebeling<br>
+<a href='https://www.biorxiv.org/content/10.1101/2023.05.25.542256v1' target='_biorxiv'>splicekit: a comprehensive toolkit for splicing analysis from short-read RNA-seq</a><br>
+bioRxiv, 2023.05. 25.542256
+
+In case of questions, issues and other ideas, please use the <a href='https://github.com/bedapub/splicekit/issues'>GitHub Issues</a> or write directly to <a href='mailto:gregor.rot@gmail.com'>Gregor Rot</a>.
```

### Comparing `splicekit-0.5.1/README.md` & `splicekit-0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 <picture><img src="media/splicekit_logo.png" height="30"/></picture>
 ## splicekit: an integrative toolkit for splicing analysis from short-read RNA-seq
 
 <b>splicekit</b> is a modular platform for splicing analysis from short-read RNA-seq datasets. The platform also integrates an JBrowse2 instance, [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
+Check a short video presentation about splicekit (poster) at ECCB 2023 on Youtube:
+
+[<img src="media/splicekit_youtube.jpg" width=300>](https://youtu.be/P1m73usZ3lc?si=HBJxWOkUajObFpu1)
+
 ## Quick start
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute:
@@ -15,21 +19,15 @@
 
 Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 <details>
 <summary>Installing splicekit directly from the GitHub repository</summary>
 
 ```
-# move to HOME folder (for example)
-cd ~
-# clone the repository
-git clone git@github.com:bedapub/splicekit.git
-# adjust PYTHONPATH and PATH
-export PYTHONPATH=$PYTHONPATH:~/splicekit
-export PATH=$PATH:~/splicekit/splicekit
+pip install git+https://github.com/bedapub/splicekit.git@main
 ```
 </details>
 
 <details>
 <summary>If you already have aligned reads in BAM files</summary>
 
 All you need is `samples.tab` (note that this is a <b>TAB delimited file</b>) and `splicekit.config` in one folder (check [datasets](datasets) for examples).
@@ -44,53 +42,66 @@
 ## Documentation
 
 * [PDF reference manual](https://github.com/bedapub/splicekit/raw/main/docs/splicekit_docs.pdf)
 * [Google docs](https://docs.google.com/document/d/15ZRCeK8xyg3klLktZSHZ9k__Xw_BZRn_Q-J4W35JNnQ/edit?usp=sharing) of the above PDF (comment if you like)
 
 ## Changelog<a name="changelog"></a>
 
-**v0.4.9**: released in November 2023
+**v0.6**: released in April 2024
+
+* updated reports
+* JUNE analysis (junction-events to classify skipped and mutually exclusive exons)
+
+<details>
+<summary>Past changenotes (click to view)</summary>
+
+<b>v0.4.9</b>: released in November 2023
+
 * added rMATS analysis for splicing events
 * added Docker container that can be directly imported to singularity via ghcr.io
 * fixed dependencies
 * other small fixes
 
-<details>
-<summary><b>v0.4</b>: released in May 2023 (click to show details)</summary>
+<b>v0.4</b>: released in May 2023
 
 * added singularity container with all dependencies
 * added local integrated JBrowse2
 * cluster or desktop runs
 * scanRBP and bootstrap analysis of RNA-protein binding
 * further development and integration with pybio
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+<b>v0.3</b>: released in January 2023 (click to show details)
 
 * re-coded junction analysis
   * independent junctions parsing from provided bam files
   * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
 * clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
 * added *first_exon* annotation for junctions touching annotated first exons of transcripts
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+<b>v0.2</b>: released in October 2022
 
 * software architecture restructure with python modules
 * filtering of lowly expressed features by edgeR
 * DonJuan analysis (junction-anchor analysis)
 * more advanced motif analysis with DREME
 * filtering regulated junctions with regulated donors
-</details>
 
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+<b>v0.1</b>: released in July 2022
 
 * initial version of splicekit
 * parsing of junction and exon counts
 * computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
 * basic motif analysis
+
 </details>
+
+## Citing and Contact<a name="citation"></a>
+
+If you find **splicekit** useful in your work and research, please cite:
+
+Gregor Rot, Arne Wehling, Roland Schmucki, Nikolaos Berntenis, Jitao David Zhang, Martin Ebeling<br>
+<a href='https://www.biorxiv.org/content/10.1101/2023.05.25.542256v1' target='_biorxiv'>splicekit: a comprehensive toolkit for splicing analysis from short-read RNA-seq</a><br>
+bioRxiv, 2023.05. 25.542256
+
+In case of questions, issues and other ideas, please use the <a href='https://github.com/bedapub/splicekit/issues'>GitHub Issues</a> or write directly to <a href='mailto:gregor.rot@gmail.com'>Gregor Rot</a>.
```

### Comparing `splicekit-0.5.1/setup.py` & `splicekit-0.6/setup.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/__init__.py` & `splicekit-0.6/splicekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 if not os.path.exists("splicekit.config"):
     print("splicekit | please run splicekit in a folder with splicekit.config present")
     sys.exit(0)
 
 print("splicekit | loading splicekit.config")
 import splicekit.config as config
+print("splicekit | ", config.platform, " detected")
 print("splicekit | loading splicekit.core")
 import splicekit.core as core
 print("splicekit | loading splicekit.core.annotation")
 import splicekit.core.annotation
 print("splicekit | loading splicekit.core.features")
 import splicekit.core.features
 print("splicekit | loading splicekit.core.exons")
@@ -39,14 +40,16 @@
 import splicekit.core.juan
 print("splicekit | loading splicekit.judge")
 import splicekit.judge
 print("splicekit | loading splicekit.core.delta_dar")
 import splicekit.core.delta_dar
 print("splicekit | loading splicekit.clusterlogfc")
 import splicekit.clusterlogfc
+print("splicekit | loading splicekit.june")
+import splicekit.june
 print("splicekit | loading splicekit.report")
 import splicekit.report
 
 # initialization (triggered once on "import splicekit")
 splicekit.core.annotation.compounds = {}
 splicekit.core.annotation.samples = set()
 splicekit.core.annotation.comparisons = []
@@ -84,15 +87,15 @@
     if splicekit.config.platform=="cluster":
         os.system('export BSUB_QUIET=Y; jobs=( $(ls jobs/count_junctions/*.job) ); g=10; for((i=0; i < ${#jobs[@]}; i+=g)); do part=( "${jobs[@]:i:g}" ); for job_fname in ${part[*]}; do echo "splicekit | features | junctions | submitted $job_fname"; bsub -M 8GB -K < ${job_fname} & done; wait; echo "splicekit | features | junctions | processing next 10"; done; echo "splicekit | features | junctions | processing complete"')
         os.system("export BSUB_QUIET=Y; bsub -q short -M 16GB -o /dev/null -e /dev/null -K python -c 'import splicekit; splicekit.core.junctions.make_master()'; wait;") # run make master as cluster job
     if splicekit.config.platform=="desktop":
         splicekit.core.mprocess("jobs/count_junctions/process.sh")
         splicekit.core.junctions.make_master()
     if splicekit.config.platform=="SLURM":
-        os.system("jobs=( $(ls jobs/count_junctions/*.job) ); g=10; " "for((i=0; i < ${#jobs[@]}; i+=g)); do " "part=( \"${jobs[@]:i:g}\" ); " "for job_fname in ${part[*]}; do " "echo \"splicekit | features | junctions | submitted $job_fname\"; " "sbatch --mem=8G --parsable ${job_fname} & " "done; wait; " "echo \"splicekit | features | junctions | processing next 10\"; " "done; " "echo \"splicekit | features | junctions | processing complete\"")
+        os.system("jobs=( $(ls jobs/count_junctions/*.job) ); g=10; " "for((i=0; i < ${#jobs[@]}; i+=g)); do " "part=( \"${jobs[@]:i:g}\" ); " "for job_fname in ${part[*]}; do " "echo \"splicekit | features | junctions | submitted $job_fname\"; " "sbatch --mem=8G --open-mode=append ${job_fname} & " "done; wait; " "echo \"splicekit | features | junctions | processing next 10\"; " "done; " "echo \"splicekit | features | junctions | processing complete\"")
         os.system("sbatch --partition=short --mem=16G --output=/dev/null --error=/dev/null " "--wrap=\"python -c 'import splicekit; splicekit.core.junctions.make_master()'\"")
 
 def junctions():
     splicekit.core.annotation.make_comparisons()
     splicekit.core.junctions.junctions_per_sample()
     splicekit.core.features.load_genes()
     splicekit.core.features.read_junctions()
@@ -260,20 +263,24 @@
 def rmats():
     if splicekit.config.platform=="cluster":
         os.system('export BSUB_QUIET=Y; jobs=( $(ls jobs/rmats/*.job) ); g=10; for((i=0; i < ${#jobs[@]}; i+=g)); do part=( "${jobs[@]:i:g}" ); for job_fname in ${part[*]}; do echo "[splicekit.rmats] submitted $job_fname"; bsub -M 8GB -K < ${job_fname} & done; wait; echo "[splicekit.rmats] processing next 10"; done; echo "[splicekit.rmats] processing complete"')
     if splicekit.config.platform=="desktop":
         splicekit.core.mprocess("jobs/rmats/process.sh")
     if splicekit.config.platform=="SLURM":
         os.system('jobs=( $(ls jobs/rmats/*.job) ); g=10; for((i=0; i < ${#jobs[@]}; i+=g)); do part=( "${jobs[@]:i:g}" ); job_ids=(); for job_fname in "${part[@]}"; do echo "[splicekit.rmats] submitted $job_fname"; job_id=$(sbatch --mem=8G --parsable ${job_fname}); job_ids+=($job_id); done; for job_id in "${job_ids[@]}"; do scontrol show job $job_id | grep -q "JobState=COMPLETED" || scontrol wait job $job_id; done; echo "[splicekit.rmats] processing next 10"; done; echo "[splicekit.rmats] processing complete"')
-    
+
+def june_process():
+    splicekit.june.process()
 
 def process(force=False):
     setup()
     annotation()
     features()
     edgeR()
     juan()
     judge_process()
     motifs()
     promisc()
     clusterlogfc_process()
+    june_process()
+    splicekit.report.process()
     jbrowse2_process(force_samples=force, force_annotation=force)
```

### Comparing `splicekit-0.5.1/splicekit/clusterlogfc/__init__.py` & `splicekit-0.6/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/config/__init__.py` & `splicekit-0.6/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/core/__init__.py` & `splicekit-0.6/splicekit/core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,7 +37,12 @@
 
     for task in tasks:
         q.put(task)
 
     q.join()
     print("splicekit | done multicore ({num_worker_threads}) processing: {fname}")
 
+def smart_number_format(number):
+    if abs(number) < 0.0001 or abs(number) >= 1e4:
+        return f"{number:.4e}"
+    else:
+        return f"{number:.4f}"
```

### Comparing `splicekit-0.5.1/splicekit/core/anchors.py` & `splicekit-0.6/splicekit/core/anchors.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,18 @@
     for anchor_type in ["donor", "acceptor"]:
         gtf_fname = f"reference/{anchor_type}_anchors.gtf.gz"
         bam_dir = f"{config.bam_path}" # files inside end with <sample_id>.bam
         out_dir = f'data/sample_{anchor_type}_anchors_data'
         jobs_dir = f'jobs/count_{anchor_type}_anchors'
         logs_dir = f'logs/count_{anchor_type}_anchors'
 
-        if config.platform == 'SLURM':
+        if splicekit.config.platform == 'SLURM':
 
             job_anchors="""
- #!/bin/bash
+#!/bin/bash
 #SBATCH --job-name={anchor_type}_anchors_{sample_id}  # Job name
 #SBATCH --ntasks=12                                   # Number of tasks
 #SBATCH --nodes=1                                     # All tasks on one node
 #SBATCH --partition=short                             # Select queue
 #SBATCH --output={logs_dir}/{anchor_type}_anchors_{sample_id}.out # Output file
 #SBATCH --error={logs_dir}/{anchor_type}_anchors_{sample_id}.err  # Error file
```

### Comparing `splicekit-0.5.1/splicekit/core/annotation.py` & `splicekit-0.6/splicekit/core/annotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 import subprocess
 import sys
 import splicekit.config as config
 import splicekit.core.annotation as annotation
 import splicekit.core as core
 import splicekit
 
-# dictionary of last nucleotide of first exon of transcripts
-# used to annotate junctions hitting 5'UTR / alternative 5'UTR
-# -> promoter changes
-# annotation.first_exons[(chr, strand, pos)] = (transcript_id, gene_id)
-
 def short_names(text):
     result = text
     if getattr(config, "short_names", None) == None:
         return result
     for from_text, to_text, replace_type in config.short_names:
         if replace_type=="complete":
             if text==from_text:
@@ -31,33 +26,27 @@
     if type(item) is tuple:
         item_process = item[0]
     else:
         item_process = item
     for splitter in [" ", "_", "-"]:
         item_temp = item_process.split(splitter)
         # separates the string by splitter
-        # find the first element that could be casted to integer and return (integer, string_without_element)
+        # find first element that casts to int and return (int, str_without_element)
         if len(item_temp)>1:
             for item_index_test in range(0, len(item_temp)):
                 if item_temp[item_index_test].isdigit():
                     return (int(item_temp[item_index_test]), splitter.join(item_temp[:item_index_test]+item_temp[item_index_test+1:]))
     if item_process.isdigit():
         return int(item_process)
     else:
         return item_process
 
 def sort_readout_id(data):
     return sorted(data, key=break_readout_id)
 
-def to_int(el):
-    try:
-        return int(el)
-    except:
-        return el
-
 class Cmd():
     # Interface for running commands from Python.
     def __init__(self, command):
         self.command = command
         self.returncode = None
         self.process = subprocess.Popen(['/bin/sh', '-c', command], stdout=subprocess.PIPE, stderr=subprocess.PIPE) # -cl and bash was original
         self.pid = self.process.pid
@@ -70,15 +59,18 @@
 def make_comparisons():
     if not os.path.exists("samples.tab"):
         return
     annotation.comparisons = []
     annotation.treatments = {}
     samples = set()
     f = open("samples.tab")
-    header = f.readline().replace("\r", "").replace("\n", "").split("\t")
+    r = f.readline()
+    while r.startswith("#"):
+        r = f.readline()
+    header = r.replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     separates = set()
     while r:
         if r.startswith("#"):
             r = f.readline()
             continue
         r = r.replace("\r", "").replace("\n", "").split("\t")
@@ -86,16 +78,15 @@
         sample_id = data[config.sample_column]
         samples.add(sample_id)
         treatment_id = data[config.treatment_column]
         separates.add(data.get(config.separate_column, ""))
         annotation.treatments.setdefault(treatment_id, []).append((sample_id, treatment_id, data.get(config.separate_column, ""), data.get(config.group_column, "")))
         r = f.readline()
     f.close()
-    # sort by sample ID
-    for treatment, data in annotation.treatments.items():
+    for treatment, data in annotation.treatments.items(): # sort by sample ID
         try:
             annotation.treatments[treatment] = sort_readout_id(data)
         except:
             pass
     dmso_hash = {}
     dmso_letter = "A"
     # sometimes the separates set was reshufled
@@ -138,15 +129,15 @@
     try:
         annotation.samples = sort_readout_id(annotation.samples)
     except:
         pass
     annotation.samples = [str(el) for el in annotation.samples]
 
 def write_comparisons():
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
         job_rmats="""
 #!/bin/bash
 #SBATCH --job-name={job_name}                        # Job name
 #SBATCH --ntasks=1                                   # Number of tasks
 #SBATCH --mem=8G                                     # Allocate memory
 #SBATCH --nodes=1                                    # All tasks on one node
 #SBATCH --partition=short                            # Select queue
@@ -210,32 +201,30 @@
         row = [comparison_name, ",".join(str(el) for el in control_ids), ",".join(str(el) for el in test_ids), control_group_id, test_group_id]
         comps_table.write("\t".join(row) + "\n") 
     comps_table.close()
     write_edgeR_jobs()
     write_mds_job()
 
 def write_edgeR_jobs():
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
             job_edgeR="""
 #!/bin/bash
 #SBATCH --job-name={job_name}                                     # Job name
 #SBATCH --ntasks=1                                                # Number of tasks
 #SBATCH --nodes=1                                                 # All tasks on one node
 #SBATCH --mem=8G                                                  # Allocate memory
 #SBATCH --partition=short                                         # Select queue
 #SBATCH --output=logs/edgeR/{atype}/{comparison_name}.out         # Output file
 #SBATCH --error=logs/edgeR/{atype}/{comparison_name}.err          # Error file
 
 module load R
 {container} R --no-save --args {input_folder} {atype} {control_name} {test_name} {comparison_name} {sample_membership} {filter_low} < {core_path}/comps_edgeR.R
     """
-        
 
     else:
-
         job_edgeR="""
 #!/bin/bash
 #BSUB -J {job_name}                                     # job name
 #BSUB -n 1                                              # number of tasks
 #BSUB -R "span[hosts=1]"                                # allocate hosts
 #BSUB -M {memory}                                       # allocate memory
 #BSUB -q {queue}                                        # select queue
@@ -252,19 +241,17 @@
     fsh_donor_anchors = open(f"jobs/edgeR/donor_anchors/process.sh", "wt")
     fsh_acceptor_anchors = open(f"jobs/edgeR/acceptor_anchors/process.sh", "wt")
     fsh_genes = open(f"jobs/edgeR/genes/process.sh", "wt")
     sample_membership = {}
     for (comparison_name, control_set, test_set, control_group_id, test_group_id) in annotation.comparisons:
         for (sample_id, _, _, _) in control_set:
             # in some rare cases, the same sample can be part of diverse control groups
-            #assert(sample_membership.get(sample_id, None) in [None, control_group_id])
             sample_membership[sample_id] = control_group_id
         for (sample_id, _, _, _) in test_set:
             # in some rare cases, the same sample can be part of diverse test groups
-            #assert(sample_membership.get(sample_id, None) in [None, test_group_id])
             sample_membership[sample_id] = test_group_id
     sample_membership = [sample_membership[sample_id] for sample_id in annotation.samples]
     for (comparison_name, control_set, test_set, control_group_id, test_group_id) in annotation.comparisons:
         control_name = control_group_id
         test_name = test_group_id
         fout_exons = open(f"jobs/edgeR/exons/{comparison_name}.job", "wt")
         fout_junctions = open(f"jobs/edgeR/junctions/{comparison_name}.job", "wt")
@@ -328,15 +315,15 @@
 
     fsh_exons.close()
     fsh_junctions.close()
     fsh_donor_anchors.close()
     fsh_acceptor_anchors.close()
 
 def write_mds_job():
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
             job_mds="""
 #!/bin/bash
 #SBATCH --job-name=edgeR_mds                                      # Job name
 #SBATCH --ntasks=1                                                # Number of tasks
 #SBATCH --nodes=1                                                 # All tasks on one node
 #SBATCH --mem=8G                                                  # Allocate memory
 #SBATCH --partition=short                                         # Select queue
@@ -366,19 +353,17 @@
     job_sh_mds="""{container} R --no-save --args {input_folder} {sample_membership} {filter_low} < {core_path}/comps_edgeR_mds.R"""
     fsh_mds = open(f"jobs/edgeR/mds/process.sh", "wt")
     fout_mds = open(f"jobs/edgeR/mds/mds.job", "wt")
     sample_membership = {}
     for (comparison_name, control_set, test_set, control_group_id, test_group_id) in annotation.comparisons:
         for (sample_id, _, _, _) in control_set:
             # in some rare cases, the same sample can be part of diverse control groups
-            #assert(sample_membership.get(sample_id, None) in [None, control_group_id])
             sample_membership[sample_id] = control_group_id
         for (sample_id, _, _, _) in test_set:
             # in some rare cases, the same sample can be part of diverse test groups
-            #assert(sample_membership.get(sample_id, None) in [None, test_group_id])
             sample_membership[sample_id] = test_group_id
     sample_membership = [sample_membership[sample_id] for sample_id in annotation.samples]
     try:
         filter_low = splicekit.config.filter_low
     except:
         filter_low = "filter_low"
 
@@ -448,25 +433,29 @@
         temp[group_id] = row
     for group_id in master_order:
         row = temp[group_id]
         f.write("\t".join([str(el) for el in row])+"\n")
     f.close()
 
 def bam_count():
-    return
-    fout = open("annotation/bam_counts.tab", "wt")
-    fout.write("\t".join([config.sample_column, "bam_count"]) + "\n")
+    if os.path.exists("annotation/bam_counts.tab"):
+        return
+    counts = []
     f = open("samples.tab")
     header = f.readline().replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         data = dict(zip(header, r))
         bam_fname = os.path.join(config.bam_path, data[config.sample_column]+".bam")
         output = subprocess.check_output(f"samtools view -@ 4 -c {bam_fname}", shell=True)
         count = int(output.decode().split("\n")[0])
-        print(f"splicekit | bam read counts: {data['readout_id']}, bam file {bam_fname}, counts = {count}")
+        print(f"splicekit | bam read counts: {data[splicekit.config.sample_column]}, bam file {bam_fname}, counts = {count}")
         row = [data[config.sample_column], count]
-        fout.write("\t".join([str(x) for x in row]) + "\n")
+        counts.append(row)
         r = f.readline()
     f.close()
+    fout = open("annotation/bam_counts.tab", "wt")
+    fout.write("\t".join([config.sample_column, "bam_count"]) + "\n")
+    for row in counts:
+        fout.write("\t".join([str(x) for x in row]) + "\n")
     fout.close()
```

### Comparing `splicekit-0.5.1/splicekit/core/comps_edgeR.R` & `splicekit-0.6/splicekit/core/comps_edgeR.R`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/core/delta_dar.py` & `splicekit-0.6/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/core/exons.py` & `splicekit-0.6/splicekit/core/exons.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 # splicekit exons module
-# generate exon count data
-# use featureCounts and provided gtf file + bam files
+# generate exon count data using featureCounts and the provided bams+gtf
 
 import os
 import sys
 import splicekit.config as config
 import gzip
 
 def write_exons_gtf():
 
     def make_row(r):
-        chr = r[0]
-        start = int(r[3]) # ! GTF file to GTF file, no change of coordinates here
-        stop = int(r[4]) # ! GTF file to GTF file, no change of coordinates here
-        strand = r[6]
+        chr, strand = r[0], r[6]
+        start, stop = int(r[3]), int(r[4]) # ! GTF file to GTF file, no change of coordinates here
         attributes = r[-1].split(";")
         new_attributes = []
         for att in attributes:
-            att = att.lstrip(" ")
-            att = att.split(" ")
+            att = att.lstrip(" ").split(" ")
             name, val = att[0], " ".join(att[1:])
-            name = name.lstrip(" ")
-            name = name.rstrip(" ")
+            name = name.lstrip(" ").rstrip(" ")
             if name in ["gene_id", "gene_name", "transcript_id"]:
-                val = val.lstrip(" ")
-                val = val.rstrip(" ")
-                val = val[1:-1] # remove quotes
+                val = val.lstrip(" ").rstrip(" ")[1:-1] # remove quotes
                 new_attributes.append(f"{name}={val}")
         exon_id = f"{chr}{strand}_{start}_{stop}"
-        new_attributes.append("exon_id="+exon_id)
+        new_attributes.append(f"exon_id={exon_id}")
         attributes_str = '; '.join(new_attributes)
         row = '\t'.join([chr, 'splicekit', "exon", str(start), str(stop), '.', strand, '0', attributes_str])+'\n'
         return row
 
     """
-    create exons.gtf to parse to featureCount jobs
-    we need 9 columns https://www.ensembl.org/info/website/upload/gff.html/
-    <seqname> <source> <feature> <start> <end> <score> <strand> <frame> [attributes]
+    * create exons.gtf as input to featureCount
+    * 9 columns https://www.ensembl.org/info/website/upload/gff.html/
+    * <seqname> <source> <feature> <start> <end> <score> <strand> <frame> [attributes]
     """
     # iterate over original gtf file
     gtf_file = gzip.open(config.gtf_path, 'rt')
     r = gtf_file.readline()
     exons_file = gzip.open("reference/exons.gtf.gz", "wt")
     while r:
         if r.startswith("#"):
@@ -54,32 +47,29 @@
         exons_file.write(row)
         r = gtf_file.readline()
     gtf_file.close()
     exons_file.close()
 
 def write_jobs_featureCounts(library_type='single-end', library_strand='NONE'):
     """
-    This function write a featureCounts job per comparison for every bamfile it can find
-    It takes in two parameters:
-        library_type: str
-        library_strand: str
-    Both are needed to call featureCounts correctly (see string formating with library_type_insert and library_strand_insert variables)
+    * write a featureCounts job per comparison for every bam file
+    * input parameters: library_type:str and library_strand:str
+    * both needed to call featureCounts correctly (see string formating with library_type_insert and library_strand_insert variables)
     """
 
-    #translate to be used in featureCoutns command
     library_type_insert = {"single-end":"", "paired-end":"-p "}[library_type]
     library_strand_insert = {"FIRST_READ_TRANSCRIPTION_STRAND":1, "SINGLE_STRAND":1, "SINGLE_REVERSE":1, "SECOND_READ_TRANSCRIPTION_STRAND":2, "NONE":0}[library_strand]
     
     gtf_fname = f"reference/exons.gtf.gz"
     bam_dir = f"{config.bam_path}" # files inside end with <sample_id>.bam
     out_dir = f'data/sample_exons_data'
     jobs_dir = f'jobs/count_exons'
     logs_dir = f'logs/count_exons'
 
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
         job_exons="""
 #!/bin/bash
 #SBATCH --job-name=count_exons_{sample_id}            # Job name
 #SBATCH --ntasks=12                                   # Number of tasks
 #SBATCH --nodes=1                                     # All tasks on one node
 #SBATCH --partition=short                             # Select queue
 #SBATCH --output={logs_dir}/exons_{sample_id}.out     # Output file
```

### Comparing `splicekit-0.5.1/splicekit/core/features.py` & `splicekit-0.6/splicekit/core/features.py`

 * *Files 21% similar despite different names*

```diff
@@ -86,32 +86,29 @@
                     current_len = abs(current_exon_start - current_exon_stop + 1)
                     new_len = abs(exon_start - exon_stop + 1)
                     if new_len>current_len:
                         store_data = False
                 if store_data:
                     annotation_data[chr, strand, exon_stop] = (transcript_id, gene_id, exon_start, exon_stop)
 
-    # save last nucleotide of first/second exon of each transcript)
+    # save last nucleotide of first exon of each transcript
     print(f"{module_name} saving last nucleotide of first/second exon of each transcript")
     annotation.first_exons = {}
     identify_exons(transcript_exons, annotation.first_exons, 0)
-    #annotation.second_exons = {}
-    #identify_exons(transcript_exons, annotation.second_exons, 1)
     
     print(f"{module_name} reading junctions and anchors annotation from: reference/junctions.tab.gz")
     f = gzip.open("reference/junctions.tab.gz", "rt")
     header = f.readline().replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         data = dict(zip(header, r))
         gene_id = data["gene_id"]
         gene = annotation.genes.get(gene_id, {})
-        gene["chr"] = data["chr"]
-        gene["strand"] = data["strand"]
+        gene["chr"], gene["strand"] = data["chr"], data["strand"]
         # junctions
         annotation.junctions_genes[data["junction_id"]] = gene_id
         junctions = gene.get("junctions", {})
         junction_start, junction_stop = int(data["junction_id"].split("_")[-2]), int(data["junction_id"].split("_")[-1])
         junctions[data["junction_id"]] = {"start":junction_start, "stop":junction_stop} # + sample counts later
         gene["junctions"] = junctions
         # anchors
@@ -136,50 +133,46 @@
         f = gzip.open(f"data/sample_junctions_data/sample_{sample_id}.tab.gz", "rt")
         r = f.readline() # header
         r = f.readline()
         while r:
             r = r.replace("\r", "").replace("\n", "").split("\t")
             junction_id = r[0]
             coords = junction_id.split('_')
-            start = int(coords[-2])
-            stop = int(coords[-1])
-            strand = coords[-3][-1]
-            chr = '_'.join(coords[:-2])[:-1]            
+            start, stop = int(coords[-2]), int(coords[-1])
+            chr, strand = '_'.join(coords[:-2])[:-1], coords[-3][-1]
             raw_count = int(r[-1])
             gene_id = annotation.junctions_genes[junction_id]
             gene = annotation.genes.get(gene_id, {})
             junctions = gene.get("junctions", {})
             junctions.setdefault(junction_id, {})[sample_id] = raw_count # sample counts dict
             gene["junctions"] = junctions
             annotation.genes[gene_id] = gene
             r = f.readline()
         count += 1
         print(f"{module_name} junction read OK, sample={sample_id}, from=data/sample_junctions_data/sample_{sample_id}.tab {count}/{count_all}")
         f.close()
 
 def read_anchors(anchor_type):
     """
-    # Description
-    Read anchors sample raw counts and populate the annotation.genes ["anchors"] field.
-    The input is read from the output of juan scripts (data/sample_anchors_data) producing anchor read counts.
+    * read anchors sample raw counts and populate the annotation.genes ["anchors"] field
+    * input is read from the output of juan scripts (data/sample_anchors_data) producing anchor read counts
     """
+
     count = 0
     count_all = len(annotation.samples)
     for sample_id in annotation.samples:
         f = gzip.open(f"data/sample_{anchor_type}_anchors_data/sample_{sample_id}.tab.gz", "rt")
         r = f.readline() # header
         r = f.readline()
         while r:
             r = r.replace("\r", "").replace("\n", "").split("\t")
             anchor_id = r[0]
             coords = anchor_id.split('_')
-            start = int(coords[-2]) - 1 # reports by featureCounts are on 1-indexed gtf regions, convert back
-            stop = int(coords[-1]) - 1 # reports by featureCounts are on 1-indexed gtf regions, convert back
-            strand = coords[-3][-1]
-            chr = '_'.join(coords[:-2])[:-1]
+            start, stop = int(coords[-2])-1, int(coords[-1])-1 # reports by featureCounts are on 1-indexed gtf regions, convert back
+            chr, strand = '_'.join(coords[:-2])[:-1], coords[-3][-1]
             anchor_id = f"{chr}{strand}_{start}_{stop}" # reconstruct anchor_id with 0-indexed coords
             raw_count = int(r[-1])
             if anchor_type=="donor":
                 gene_id = annotation.donor_anchors_genes[anchor_id]
             if anchor_type=="acceptor":
                 gene_id = annotation.acceptor_anchors_genes[anchor_id]
             gene = annotation.genes.get(gene_id, {})
@@ -190,32 +183,29 @@
             r = f.readline()
         count += 1
         print(f"{module_name} anchors read OK, sample={sample_id}, from=data/sample_{anchor_type}_anchors_data/sample_{sample_id}.tab.gz {count}/{count_all}")
         f.close()
 
 def read_exons():
     """
-    # Description
-    Read exons sample raw counts and populate the annotation.genes ["exons"] field.
-    The input is read from data/sample_exons_data
+    * read exons sample raw counts and populate the annotation.genes ["exons"] field
+    * input is read from data/sample_exons_data
     """
     count = 0
     count_all = len(annotation.samples)
     for sample_id in annotation.samples:
         f = gzip.open(f"data/sample_exons_data/sample_{sample_id}.tab.gz", "rt")
         r = f.readline() # header
         r = f.readline()
         while r:
             r = r.replace("\r", "").replace("\n", "").split("\t")
             exon_id = r[0]
             coords = exon_id.split('_')
-            start = int(coords[-2])-1 # reports by featureCounts are on 1-indexed gtf regions, convert back
-            stop = int(coords[-1])-1 # reports by featureCounts are on 1-indexed gtf regions, convert back
-            strand = coords[-3][-1]
-            chr = '_'.join(coords[:-2])[:-1]      
+            start, stop = int(coords[-2])-1, int(coords[-1])-1 # reports by featureCounts are on 1-indexed gtf regions, convert back
+            chr, strand = '_'.join(coords[:-2])[:-1], coords[-3][-1]
             exon_id = f"{chr}{strand}_{start}_{stop}" # reconstruct exon_id with 0-indexed coords
             raw_count = int(r[-1])
             gene_id = annotation.exons_genes[exon_id]
             gene = annotation.genes.get(gene_id, {})
             exons = gene.get("exons", {})
             exons.setdefault(exon_id, {})[sample_id] = raw_count # sample counts dict
             gene["exons"] = exons
@@ -223,17 +213,16 @@
             r = f.readline()
         count += 1
         print(f"{module_name} exons read OK, sample={sample_id}, from=data/sample_exons_data/sample_{sample_id}.tab.gz, ({count}/{count_all})")
         f.close()
 
 def read_genes():
     """
-    # Description
-    Read gene sample raw counts and populate the annotation.genes ["genes"] field.
-    The input is read from data/sample_genes_data
+    * read gene sample raw counts and populate the annotation.genes ["genes"] field
+    * input is read from data/sample_genes_data
     """
     count = 0
     count_all = len(annotation.samples)
     for sample_id in annotation.samples:
         f = gzip.open(f"data/sample_genes_data/sample_{sample_id}.tab.gz", "rt")
         r = f.readline() # header
         r = f.readline()
@@ -250,25 +239,19 @@
             r = f.readline()
         count += 1
         print(f"{module_name} genes read OK, sample={sample_id}, from=data/sample_genes_data/sample_{sample_id}.tab.gz, ({count}/{count_all}")
         f.close()
 
 def save_comps_feature_data(feature_type):
     """
-    # Description
-    Take files from data/samples_{feature_type}_data/*.tab and read in the counts
-    Write the data/comparison_{feature_type}_data files
-
-    # Parameters
-    feature_type = exons, junctions, donor_anchors, acceptor_anchors
-
-    # Structure and debug
-    comp1 = [(36, 'DMSO', 'DMSO_rep1'), (48, 'DMSO', 'DMSO_rep1'), (60, 'DMSO', 'DMSO_rep1'), (72, 'DMSO', 'DMSO_rep1'), (84, 'DMSO', 'DMSO_rep1'), (96, 'DMSO', 'DMSO_rep1'), (132, 'DMSO', 'DMSO_rep1'), (144, 'DMSO', 'DMSO_rep1'), (156, 'DMSO', 'DMSO_rep1'), (168, 'DMSO', 'DMSO_rep1'), (180, 'DMSO', 'DMSO_rep1'), (192, 'DMSO', 'DMSO_rep1'), (228, 'DMSO', 'DMSO_rep2'), (240, 'DMSO', 'DMSO_rep2'), (252, 'DMSO', 'DMSO_rep2'), (264, 'DMSO', 'DMSO_rep2'), (276, 'DMSO', 'DMSO_rep2'), (288, 'DMSO', 'DMSO_rep2'), (324, 'DMSO', 'DMSO_rep2'), (336, 'DMSO', 'DMSO_rep2'), (348, 'DMSO', 'DMSO_rep2'), (360, 'DMSO', 'DMSO_rep2'), (372, 'DMSO', 'DMSO_rep2'), (384, 'DMSO', 'DMSO_rep2'), (420, 'DMSO', 'DMSO_rep3'), (432, 'DMSO', 'DMSO_rep3'), (444, 'DMSO', 'DMSO_rep3'), (456, 'DMSO', 'DMSO_rep3'), (468, 'DMSO', 'DMSO_rep3'), (480, 'DMSO', 'DMSO_rep3'), (516, 'DMSO', 'DMSO_rep3'), (528, 'DMSO', 'DMSO_rep3'), (540, 'DMSO', 'DMSO_rep3'), (552, 'DMSO', 'DMSO_rep3'), (564, 'DMSO', 'DMSO_rep3'), (576, 'DMSO', 'DMSO_rep3')]
-    comp2 = [(1, 'RO7282701', 'RO7282701-000-001_rep1'), (193, 'RO7282701', 'RO7282701-000-001_rep2'), (385, 'RO7282701', 'RO7282701-000-001_rep3')]
+    * take files from data/samples_{feature_type}_data/*.tab and read in the counts
+    * write the data/comparison_{feature_type}_data files
+    * feature_type = exons, junctions, donor_anchors, acceptor_anchors
     """
+
     count = 0
     count_all = len(annotation.comparisons)
     for (comp_name, comp1, comp2, _, _) in annotation.comparisons:
         fout = gzip.open(f"data/comparison_{feature_type}_data/{comp_name}.tab.gz", "wt")
         header = ["gene_id", "gene_name", "chr", "strand", "feature_start", "feature_stop", "length", "feature_id"]
         for (sample_id, compound, rep, _) in comp2:
             header.append("{sample}_{compound}".format(sample=sample_id, compound=compound))
@@ -353,15 +336,16 @@
         for feature_id, feature_data in gene_data[feature_type].items():
             # propagate gene start stop from gene object to count object
             if feature_type=="genes" and feature_id in ["start", "stop"]:
                 continue
             if feature_type=="genes":
                 feature_data["start"] = gene_data["genes"]["start"]
                 feature_data["stop"] = gene_data["genes"]["stop"]
-            row = [gene_id, "{symbol}\t{chr}\t{strand}\t{feature_start}\t{feature_stop}\t{length}".format(chr=gene_data["chr"], strand=gene_data["strand"], symbol=gene_data["gene_name"], feature_start=feature_data["start"], feature_stop=feature_data["stop"], length=feature_data["stop"]-feature_data["start"]+1)]
+            feature_len = feature_data["stop"]-feature_data["start"]+1
+            row = [gene_id, f"{gene_data['gene_name']}\t{gene_data['chr']}\t{gene_data['strand']}\t{feature_data['start']}\t{feature_data['stop']}\t{feature_len}"]
             row.append(feature_id)
             for sample_id in annotation.samples:
                 row.append(feature_data.get(sample_id, 0))
             fout.write("\t".join(str(el) for el in row)+"\n")
     fout.close()
 
 def add_psi_cluster():
@@ -376,17 +360,16 @@
         for (comp_name, comp1, comp2, _, _) in annotation.comparisons:
             command = "python -c 'import splicekit; splicekit.core.features.add_psi(\"" + comp_name + "\")'"
             os.system(command)
 
 def add_psi(comp_name):
     read_length = 150
     """
-    # Description
-    Adds delta_PSI to exon results tables
-    Reference: https://currentprotocols.onlinelibrary.wiley.com/doi/full/10.1002/0471142905.hg1116s87
+    * adds delta_PSI to exon results tables
+    * reference: https://currentprotocols.onlinelibrary.wiley.com/doi/full/10.1002/0471142905.hg1116s87
 
     IR = IR_exon / (exon_length + read_length - 1) # reads covering the exon
     ER = ER_exon / (read_length - 1) # reads skipping the exon
     PSI = IR / (IR+ER) * 100
     """
 
     def find_junctions(data, chr, strand, feature_start, feature_stop):
@@ -465,20 +448,18 @@
     fout_exons.close()
     os.system(f"mv data/comparison_exons_data/{comp_name}.tab.gz.temp data/comparison_exons_data/{comp_name}.tab.gz")
     print(f"{module_name} added PSI for comparison_exons_data/{comp_name}.tab.gz")
     return True    
 
 def add_dai():
     """
-    Description
-    -----------
-    Adds delta_DAI to junction results tables
-    donor_DAI = control_donor / (control_donor + test_donor)
-    acceptor_DAI = control_acceptor / (control_acceptor + test_acceptor)
-    delta_DAI = (donor_DAI - acceptor_DAI) * 100
+    * adds delta_DAI to junction results tables
+    * donor_DAI = control_donor / (control_donor + test_donor)
+    * acceptor_DAI = control_acceptor / (control_acceptor + test_acceptor)
+    * delta_DAI = (donor_DAI - acceptor_DAI) * 100
     """
 
     count = 0
     count_all = len(annotation.comparisons)
     # read junctions, donors, anchors mapping
     mapping_junction_donor = {}
     mapping_junction_acceptor = {}
@@ -581,29 +562,8 @@
             fout_junctions.write("\t".join(str(data_out[h]) for h in header_out) + "\n")
             r = fin_junctions.readline()
         fin_junctions.close()
         fout_junctions.close()
         count += 1
         os.system(f"mv data/comparison_junctions_data/{comp_name}.tab.gz.temp data/comparison_junctions_data/{comp_name}.tab.gz")
         print(f"{module_name} Added DAI for comparison_junctions_data/{comp_name}.tab.gz ({count}/{count_all}")
-    return True    
-
-def save_feature_data(feature_type, filter=None):
-    count = 0
-    count_all = len(annotation.samples)
-    for sample_id in annotation.samples:
-        if filter==None:
-            fname = f"data/sample_{feature_type}_data/sample_{sample_id}.tab.gz"
-        else:
-            fname = f"data/sample_{feature_type}_data/sample_{sample_id}.tab.gz.filtered"
-        fout = gzip.open(fname, "wt")
-        for gene_id, gene_data in annotation.genes.items():
-            if gene_data.get(feature_type, None)==None:
-                continue
-            for (feature_start, feature_stop), feature_data in gene_data[feature_type].items():
-                row = ["{gene_id}_{gene_name}:{feature_start}-{feature_stop}".format(gene_id=gene_id, gene_name=gene_data["gene_name"], feature_start=feature_start, feature_stop=feature_stop), feature_data.get(sample_id, 0)]
-                filter_key = "{chr}:{feature_start}-{feature_stop}".format(chr=gene_data["chr"], feature_start=feature_start, feature_stop=feature_stop)
-                if filter==None or filter_key not in filter:
-                    fout.write("\t".join(str(el) for el in row)+"\n")
-        fout.close()
-        count += 1
-        print(f"{module_name} saved {feature_type} data, sample={sample_id}, file={fname} ({count}/{count_all}")
+    return True
```

### Comparing `splicekit-0.5.1/splicekit/core/genes.py` & `splicekit-0.6/splicekit/core/genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     
     gtf_fname = f"reference/genes.gtf.gz"
     bam_dir = f"{config.bam_path}" # files inside end with <sample_id>.bam
     out_dir = f"data/sample_genes_data"
     jobs_dir = f"jobs/count_genes"
     logs_dir = f"logs/count_genes"
 
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
         job_genes="""
 #!/bin/bash
 #SBATCH --job-name=count_genes_{sample_id}            # Job name
 #SBATCH --ntasks=12                                   # Number of tasks
 #SBATCH --nodes=1                                     # All tasks on one node
 #SBATCH --partition=short                             # Select queue
 #SBATCH --output={logs_dir}/genes_{sample_id}.out     # Output file
```

### Comparing `splicekit-0.5.1/splicekit/core/jbrowse2.py` & `splicekit-0.6/splicekit/core/jbrowse2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         print(f"{module_desc} http://{ip_addr}:{config.jbrowse2_port}/jbrowse2/?config=splicekit_data/config.json")
         httpd.serve_forever()
 
 def setup():
     if not os.path.exists("jbrowse2"):
         os.makedirs("jbrowse2")
     if not os.path.exists("jbrowse2/version.txt"):
-        os.system("wget https://github.com/GMOD/jbrowse-components/releases/download/v2.4.2/jbrowse-web-v2.4.2.zip -O jbrowse2/jbrowse-web-v2.4.2.zip")
-        os.system("unzip -qq -d jbrowse2 -o jbrowse2/jbrowse-web-v2.4.2.zip")
-        os.system("rm jbrowse2/jbrowse-web-v2.4.2.zip")
+        os.system("wget https://github.com/GMOD/jbrowse-components/releases/download/v2.10.3/jbrowse-web-v2.10.3.zip -O jbrowse2/jbrowse-web-v2.10.3.zip")
+        os.system("unzip -qq -d jbrowse2 -o jbrowse2/jbrowse-web-v2.10.3.zip")
+        os.system("rm jbrowse2/jbrowse-web-v2.10.3.zip")
 
 # JBrowse2 part
 
 # for every bam file create bigwig and cram file plus a bed file that shows the junctions
 bam_dir = config.bam_path
 container = config.container
 try:
@@ -52,15 +52,15 @@
         os.system(f"{container} samtools faidx {genome_fa}")
         print(f"{module_desc} done indexing genome: {genome_fa}")
 
 def write_sample_jobs(force_samples):
     os.system("rm -r jobs/jobs_jbrowse/* >/dev/null 2>&1") # clean up previous jobs
 
     # create bigwig and then cram files
-    if config.platform == 'SLURM':
+    if splicekit.config.platform == 'SLURM':
         job_bw="""
 #!/bin/bash
 #SBATCH --job-name={sample}_jbrowse               # Job name
 #SBATCH --ntasks=4                               # Number of tasks
 #SBATCH --nodes=1                                # All tasks on one node
 #SBATCH --partition=short                        # Select queue
 #SBATCH --output=logs/logs_jbrowse/{sample}.out  # Output file
```

### Comparing `splicekit-0.5.1/splicekit/core/juan.py` & `splicekit-0.6/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/core/junctions.py` & `splicekit-0.6/splicekit/core/junctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,38 +98,62 @@
             factor = {"NN":0, "NA":1, "AN":1, "AA":2}[annotation]
             gene_len = gene_stop-gene_start+1
             detected_genes.append((factor + 1.0/gene_len, gene_id, gene_name, strand, annotation))
     detected_genes.sort(reverse=True)
     return detected_genes
 
 def make_jobs():
-    job_junctions="""
+    if splicekit.config.platform == 'SLURM':
+        job_junctions = """
+#!/bin/bash
+#SBATCH --job-name={job_name}                     # Job name
+#SBATCH --ntasks=1                                 # number of tasks
+#SBATCH --nodes=1                                  # Allocate all tasks in 1 node
+#SBATCH --mem=4GB                                  # Memory
+#SBATCH --partition=short                          # Select partition/queue
+#SBATCH --output=logs/count_junctions/{sample_id}.out     # Output file
+#SBATCH --error=logs/count_junctions/{sample_id}.err      # Error file
+
+python {core_path}/junctions.py {bam_fname} data/sample_junctions_data/sample_{sample_id}
+"""
+    else:
+        job_junctions = """
 #!/bin/bash
 #BSUB -J {job_name}                               # Job name
 #BSUB -n 1                                        # number of tasks
 #BSUB -R "span[hosts=1]"                          # Allocate all tasks in 1 host
 #BSUB -M 4GB                                      # Memory
 #BSUB -q short                                    # Select queue
 #BSUB -o logs/count_junctions/{sample_id}.out     # Output file
 #BSUB -e logs/count_junctions/{sample_id}.err     # Error file
 
 python {core_path}/junctions.py {bam_fname} data/sample_junctions_data/sample_{sample_id}
 """
 
-    job_sh_junctions="""python {core_path}/junctions.py {bam_fname} data/sample_junctions_data/sample_{sample_id}"""
+    job_sh_junctions = """python {core_path}/junctions.py {bam_fname} data/sample_junctions_data/sample_{sample_id}"""
 
     fsh = open("jobs/count_junctions/process.sh", "wt")
+
     for sample_id in splicekit.core.annotation.samples:
-        core_path=os.path.dirname(splicekit.core.__file__)
+        core_path = os.path.dirname(splicekit.core.__file__)
         bam_fname = f"{splicekit.config.bam_path}/{sample_id}.bam"
         f = open("jobs/count_junctions/sample_{sample_id}.job".format(sample_id=sample_id), "wt")
         f.write(job_junctions.format(sample_id=sample_id, core_path=core_path, bam_fname=bam_fname, job_name="count_junctions_{sample_id}".format(sample_id=sample_id)))
         f.close()
         fsh.write(job_sh_junctions.format(sample_id=sample_id, core_path=core_path, bam_fname=bam_fname)+"\n")
+
     fsh.close()
+
+    for sample_id in splicekit.core.annotation.samples:
+        with open("jobs/count_junctions/sample_{sample_id}.job".format(sample_id=sample_id), "r") as file:
+            content = file.read()
+
+        with open("jobs/count_junctions/sample_{sample_id}.job".format(sample_id=sample_id), "w") as file:
+            file.write(content.replace("\n", "", 1))
+
     
 def detect_junctions(database, positions, cigar, read, pair=None, stats=False):
     junctions_stats = []
     chr = read.reference_name
     strand = "-" if read.is_reverse else "+"
     if pair==1 and splicekit.config.library_strand=="SECOND_READ_TRANSCRIPTION_STRAND": # paired-end, second read is in transcription direction, reverse first read
         strand = {"+":"-", "-":"+"}[strand]
```

### Comparing `splicekit-0.5.1/splicekit/core/motifs.py` & `splicekit-0.6/splicekit/core/motifs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # splicekit motifs module
-# retrieve sequence patterns and construct sequence logos
-# prepare FASTA for scanRBP and DREME
-# html reports
 
 import pybio
 import math
 import gzip
 import random
 random.seed(42)
 import numpy as np
@@ -28,14 +25,17 @@
 logFC_thresh = 1 # threshold for events to be considered by effect size
 motif_FDR = 0.05 # we use this threshold for motifs
 
 # scan / motif areas
 scanRBP_area = 100 # feature_site-scanRBP_area ... feature_site+scanRBP_area
 splice_sites_area = (-2, 6) # take -2 ... 6 around splice site (donor or acceptor)
 
+# data types
+dtypes = ["PWM"] # also CLIP
+
 # criteria is split by feature type, data read-in from "results/results_edgeR_{feature_type}_all.tab"
 motif_criteria = {}
 
 # (criteria_name, donor/acceptor, actual criteria)
 # note that criteria_name must be unique across all feature types
 motif_criteria["junctions"] = []
 motif_criteria["junctions"].append(("juan_up_donor", "donor", f"float(data['fdr'])<{motif_FDR} and float(data['donor_anchor_logfc'])>{logFC_thresh}"))
@@ -58,18 +58,17 @@
 # exons_donors sites
 motif_criteria["exons"] = []
 motif_criteria["exons"].append(("exons_up", "donor", f"float(data['fdr'])<{motif_FDR} and float(data['logFC'])>{logFC_thresh}"))
 motif_criteria["exons"].append(("exons_down", "donor", f"float(data['fdr'])<{motif_FDR} and float(data['logFC'])<-{logFC_thresh}"))
 motif_criteria["exons"].append(("exons_up_controls", "donor", f"float(data['fdr'])>0.5 and float(data['logFC'])>0"))
 motif_criteria["exons"].append(("exons_down_controls", "donor", f"float(data['fdr'])>0.5 and float(data['logFC'])<0"))
 
+# format (name is used for output folder name): (name, criteria_name1, criteria_name2)
 # dreme positive sequences = criteria_name1
 # dreme negative sequences = criteria_name2
-# format of tuples (name is used for output folder name):
-# (name, criteria_name1, criteria_name2)
 dreme_criteria = []
 dreme_criteria.append(("junctions_up_donor", "junctions_up_donor", "junctions_up_donor_controls"))
 dreme_criteria.append(("junctions_down_donor", "junctions_down_donor", "junctions_down_donor_controls"))
 dreme_criteria.append(("juan_up_donor", "juan_up_donor", "juan_controls"))
 dreme_criteria.append(("juan_down_donor", "juan_down_donor", "juan_controls"))
 dreme_criteria.append(("juan_irr_donor", "juan_irr_donor", "juan_controls"))
 
@@ -183,38 +182,24 @@
                     coords = data["feature_id"].split('_')
                     start = int(coords[-2])
                     stop = int(coords[-1])
                     strand = coords[-3][-1]
                     chr = '_'.join(coords[:-2])[:-1]
                     if comparison_counts.get((criteria_name, data["comparison"]), 0)<1000: # no more than 1000 sequences per criteria per comparison
                         comparison_counts[(criteria_name, data["comparison"])] = comparison_counts.setdefault((criteria_name, data["comparison"]), 0) + 1
-                        if seq_field=="donor":
-                            donor_site = start if strand=="+" and feature_type=="junctions" else stop
-                            start_pos = donor_site - scanRBP_area
-                            stop_pos = donor_site + scanRBP_area
-                            donor_seq = pybio.core.genomes.seq_direct(config.species, chr, strand, start_pos, stop_pos, genome_version=config.genome_version)
-                            #fasta_id = f"{chr}{strand}_{start_pos}_{stop_pos}"
-                            fasta_id = f"{chr}{strand}_{donor_site}"
-                            result_data = scanRBP_data.get((criteria_name, data["comparison"]), {})
-                            result_data.setdefault(fasta_id, {})
-                            result_data[fasta_id]["seq"] = donor_seq
-                            result_data[fasta_id].setdefault("result_list", set()).add(data["result_id"])
-                            scanRBP_data[(criteria_name, data["comparison"])] = result_data
-                        if seq_field=="acceptor":
-                            acceptor_site = stop if strand=="+" and feature_type=="junctions" else start
-                            start_pos = acceptor_site - scanRBP_area
-                            stop_pos = acceptor_site + scanRBP_area
-                            acceptor_seq = pybio.core.genomes.seq_direct(config.species, chr, strand, start_pos, stop_pos, genome_version=config.genome_version)
-                            #fasta_id = f"{chr}{strand}_{start_pos}_{stop_pos}"
-                            fasta_id = f"{chr}{strand}_{acceptor_site}"
-                            result_data = scanRBP_data.get((criteria_name, data["comparison"]), {})
-                            result_data[fasta_id] = {}
-                            result_data[fasta_id]["seq"] = acceptor_seq
-                            result_data[fasta_id].setdefault("result_list", set()).add(data["result_id"])
-                            scanRBP_data[(criteria_name, data["comparison"])] = result_data
+                        splice_site = start if strand=="+" and feature_type=="junctions" else stop
+                        start_pos = splice_site - scanRBP_area
+                        stop_pos = splice_site + scanRBP_area
+                        splice_seq = pybio.core.genomes.seq_direct(config.species, chr, strand, start_pos, stop_pos, genome_version=config.genome_version)
+                        fasta_id = f"{chr}{strand}_{splice_site}"
+                        result_data = scanRBP_data.get((criteria_name, data["comparison"]), {})
+                        result_data.setdefault(fasta_id, {})
+                        result_data[fasta_id]["seq"] = splice_seq
+                        result_data[fasta_id].setdefault("result_list", set()).add(data["result_id"])
+                        scanRBP_data[(criteria_name, data["comparison"])] = result_data
             r = f.readline()
         f.close()
 
         for (criteria_name, comparison), result_data in scanRBP_data.items():
             if criteria_name not in scanRBP_to_process:
                 continue
             print(f"{module_name} make_scanRBP | {comparison}: {criteria_name} {feature_type}")
@@ -223,14 +208,31 @@
             for fasta_id, data in result_data.items():
                 result_list = " ".join(list(data["result_list"]))
                 seq = data["seq"]
                 f.write(f">{fasta_id} {result_list}\n{seq}\n")
             f.close()
             os.system(f"scanRBP {fasta_fname} --output_folder results/motifs/scanRBP/data -nonzero -protein {config.protein}")
 
+def scanRBP_dreme():
+    for cdata in splicekit.core.annotation.comparisons:
+        comparison = cdata[0]
+        for dtype in dtypes:
+            for (cname, signal_up, signal_down, control_up, control_down) in scanRBP_pairs:
+                up_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{signal_up}_scanRBP.fasta"
+                down_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{signal_down}_scanRBP.fasta"
+                upcontrol_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{control_up}_scanRBP.fasta"
+                downcontrol_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{control_down}_scanRBP.fasta"
+
+                command = f"dreme -png -norc -p {up_fasta} -n {upcontrol_fasta} -oc results/motifs/scanRBP/{comparison}_{signal_up}"
+                os.system(command)
+
+                command = f"dreme -png -norc -p {down_fasta} -n {downcontrol_fasta} -oc results/motifs/scanRBP/{comparison}_{signal_down}"
+                os.system(command)
+    return True
+
 def smooth(y, box_pts):
     box = np.ones(box_pts)/box_pts
     y_smooth = np.convolve(y, box, mode='same')
     return y_smooth
 
 def bootstrap_logfc(matrix_signal, matrix_control, smoothing=6, iterations=1000):
     def matrix_vector(matrix):
@@ -280,104 +282,73 @@
             id = f.id.replace("+", "plus").replace("-", "minus").split(" ")[0]
             if dtype=="PWM":
                 scanRBP_fname = f"results/motifs/scanRBP/data/pwm_{id}.tab.gz"
             elif dtype=="CLIP":
                 scanRBP_fname = f"results/motifs/scanRBP/data/{id}_CLIP.tab"
             df = pd.read_csv(scanRBP_fname, sep='\t', header=0, index_col=0)
             data = list(df.loc[protein])
-            #data = [x if x>=0 else 0 for x in data]
-            data = [1 if x>0 else 0 for x in data]
+            data = [1 if x>0 else 0 for x in data] # data = [x if x>=0 else 0 for x in data]
             rows.append(id_original)
             matrix.append(data)
             if vector==[]:
                 vector=data
             else:
                 vector = [e1+e2 for e1,e2 in zip(vector, data)]
         return matrix, vector, rows
 
     for cdata in splicekit.core.annotation.comparisons:
         comparison = cdata[0]
-        #for dtype in ["CLIP", "PWM"]:
-        for dtype in ["PWM"]:
+        for dtype in dtypes:
             for (cname, signal_up, signal_down, control_up, control_down) in scanRBP_pairs:
                 up_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{signal_up}_scanRBP.fasta"
                 down_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{signal_down}_scanRBP.fasta"
                 upcontrol_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{control_up}_scanRBP.fasta"
                 downcontrol_fasta = f"results/motifs/scanRBP/fasta/{comparison}_{control_down}_scanRBP.fasta"
                 if not os.path.exists(up_fasta) or not os.path.exists(down_fasta) or not os.path.exists(upcontrol_fasta) or not os.path.exists(downcontrol_fasta):
                     continue
                 print(f"{module_name} plot_scanRBP | processing {cname} {comparison} {dtype}")
                 matrix_up, vector_up, rows_up = read_matrix_vector(up_fasta, dtype=dtype)
                 matrix_down, vector_down, rows_down = read_matrix_vector(down_fasta, dtype=dtype)
                 matrix_upcontrol, vector_upcontrol, rows_upcontrol = read_matrix_vector(upcontrol_fasta, dtype=dtype)
                 matrix_downcontrol, vector_downcontrol, rows_downcontrol = read_matrix_vector(downcontrol_fasta, dtype=dtype)
 
                 bootup = bootstrap_logfc(matrix_up, matrix_upcontrol, smoothing=smoothing, iterations=100000)
-                value_up = bootup[0]
+                logfc_value_up = bootup[0]
                 bootup.sort(reverse=True)
-                index_up = bootup.index(value_up)
-                print(f"{module_name} plot_scanRBP up logFC=", value_up)
-                print(f"{module_name} plot_scanRBP] p-value up = ", index_up/float(len(bootup)))
+                index_up = bootup.index(logfc_value_up)
+                print(f"{module_name} plot_scanRBP | up logFC = ", logfc_value_up)
+                print(f"{module_name} plot_scanRBP | p-value up = ", index_up/float(len(bootup)))
                 up_file = open(f"results/motifs/scanRBP/{comparison}_{signal_up}_bootstrap.tab", "wt")
-                up_file.write(f"logFC\t{value_up}\np_value\t{index_up/float(len(bootup))}")
+                up_file.write(f"logFC\t{logfc_value_up}\np_value\t{index_up/float(len(bootup))}")
                 up_file.close()
+                p_value_up = index_up/float(len(bootup))
 
                 bootdown = bootstrap_logfc(matrix_down, matrix_downcontrol, smoothing=smoothing, iterations=100000)
-                value_down = bootdown[0]
+                logfc_value_down = bootdown[0]
                 bootdown.sort(reverse=True)
-                index_down = bootdown.index(value_down)
-                print(f"{module_name} plot_scanRBP | down logFC=", value_down)
+                index_down = bootdown.index(logfc_value_down)
+                print(f"{module_name} plot_scanRBP | down logFC = ", logfc_value_down)
                 print(f"{module_name} plot_scanRBP | p-value down = ", index_down/float(len(bootdown)))
+                print()
                 down_file = open(f"results/motifs/scanRBP/{comparison}_{signal_down}_bootstrap.tab", "wt")
-                down_file.write(f"logFC\t{value_down}\np_value\t{index_down/float(len(bootdown))}")
+                down_file.write(f"logFC\t{logfc_value_down}\np_value\t{index_down/float(len(bootdown))}")
                 down_file.close()
-
-                # heatmap
-                """
-                for htype, matrix_data, rows_data in [("up", matrix_up, rows_up), ("down", matrix_down, rows_down)]:
-                    data = pd.DataFrame(matrix_data, index=rows_data)
-                    plt.figure()
-                    sns.set(font="Arial")
-                    sns.set(font_scale=0.4)
-                    sns.set_style("dark")
-                    sns.set_style("ticks")
-                    if htype=="up":
-                        rdgn = sns.diverging_palette(h_neg=130, h_pos=10, s=99, l=55, sep=3, as_cmap=True)
-                    if htype=="down":
-                        rdgn = sns.diverging_palette(h_neg=250, h_pos=250, s=99, l=55, sep=3, as_cmap=True)
-                    optional_params = {"linewidths":0.0}
-                    optional_params["col_cluster"] = False
-                    optional_params["annot"] = False
-                    optional_params["center"] = 0
-                    optional_params["fmt"] = ".0f"
-                    optional_params["figsize"] = (10,3)
-                    optional_params["yticklabels"] = True
-                    optional_params["xticklabels"] = False
-                    optional_params["cmap"] = rdgn
-                    optional_params["cbar_pos"] = None
-                    fig = sns.clustermap(data, **optional_params)
-                    fig.ax_col_dendrogram.set_visible(False)
-                    plt.tight_layout() 
-                    plt.savefig(f"results/motifs/scanRBP/heatmap_{protein_label}_{comparison}_{dtype}_{htype}_{cname}.png", dpi=300)
-                    plt.close()
-                """
+                p_value_down = index_down/float(len(bootdown))
 
                 plt.figure(figsize=(10,3))
-                sns.set(font="Arial")
-                sns.set(font_scale=0.6)
-                sns.set_style("dark")
-                sns.set_style("ticks")
+                sns.set(font="Arial"); sns.set(font_scale=0.6); sns.set_style("dark"); sns.set_style("ticks")
 
                 vector_up = [e1/len(matrix_up) for e1 in vector_up] # normalize
                 vector_up = smooth(vector_up, smoothing)[25:-25]
                 x = list(range(len(vector_up)))
                 middle = int(len(x)/2)
                 x = [el-middle for el in x]
                 fig = sns.lineplot(data={"x":x, "y":vector_up}, x="x", y="y", linewidth=2, color='r')
                 fig.fill_between(x, vector_up, color='#fb6767')
+
                 fig.set(xlabel=f"distance from site [nt]", ylabel='fraction of sites (RBP binding)')
                 fig.spines['left'].set_linewidth(0.5)
                 fig.spines['left'].set_color('#333333')
                 fig.spines['bottom'].set_linewidth(0.5)
                 fig.spines['bottom'].set_color('#333333')
                 fig.spines['top'].set_linewidth(0.5)
                 fig.spines['top'].set_color('#333333')
@@ -395,53 +366,45 @@
                 fig = sns.lineplot(data={"x":x, "y":vector_down}, x="x", y="y", linewidth=2, color='b')
                 fig.fill_between(x, vector_down, color='#6767fb')
 
                 # plot the controls
                 vector_upcontrol = [e1/len(matrix_upcontrol) for e1 in vector_upcontrol] # normalize
                 vector_upcontrol = smooth(vector_upcontrol, smoothing)[25:-25]
                 fig = sns.lineplot(data={"x":x, "y":vector_upcontrol}, x="x", y="y", linewidth=2, color='#ffab40')
-                #fig.fill_between(x, vector_upcontrol, color='#fb6767')
 
                 vector_downcontrol = [e1/len(matrix_downcontrol) for e1 in vector_downcontrol] # normalize
                 vector_downcontrol = smooth(vector_downcontrol, smoothing)[25:-25]
                 vector_downcontrol = [-e1 for e1 in vector_downcontrol]
                 fig = sns.lineplot(data={"x":x, "y":vector_downcontrol}, x="x", y="y", linewidth=2, color='#ffab40')
-                #fig.fill_between(x, vector_downcontrol, color='#6767fb')
 
                 plt.plot([-80, 80], [0, 0], color='#999999', linestyle='--', linewidth=0.3, alpha=0.5)
                 plt.plot([0, 0], [-max_val, max_val], color='#999999', linestyle='--', linewidth=0.3, alpha=0.5)
                 fig.set(ylim=(-max_val, max_val))
                 fig.set(xlim=(-80, 80))
-                plt.title(f"{dtype} {protein_label}, FDR<0.05, up={len(matrix_up)}, down={len(matrix_down)}, up_control={len(matrix_upcontrol)}, down_control={len(matrix_downcontrol)}, smoothing={smoothing}")
+
+                # make pvalue label
+                p_value_up = "<1e-5" if p_value_up==0 else f"{p_value_up:.3}"
+                p_value_down = "<1e-5" if p_value_down==0 else f"{p_value_down:.3}"
+
+                plt.title(f"{protein_label} {comparison} {dtype} {cname}, FDR<0.05, up=(#{len(matrix_up)}, logfc={logfc_value_up:.3}, pval={p_value_up}), down=(#{len(matrix_down)}, logfc={logfc_value_down:.3}, pval={p_value_down}), #up_control={len(matrix_upcontrol)}, #down_control={len(matrix_downcontrol)}, smoothing={smoothing}")
                 plt.tight_layout() 
                 plt.savefig(f"results/motifs/scanRBP/{protein_label}_{comparison}_{dtype}_{cname}.png", dpi=300)
                 plt.close()
 
-                """
-                logfc = float(sum(vector_up))/sum(vector_upcontrol)
-                logfc = math.log(logfc, 2)
-                print(logfc)
-
-                logfc = float(sum(vector_down))/sum(vector_downcontrol)
-                logfc = math.log(logfc, 2)
-                print(logfc)
-                """
-
-
 feature_added = {} # do not add sequences for the same donor/acceptor site multiple times (e.g. several junctions can represent the same donor site)
 treatment_seq_bytype = {}
 def make_logos():
     print(f"{module_name} make_logos | start")
 
     # evaluetes criteria from motif_criteria (see top of file) and distributes sequences accordingly
     # write fasta files
     # produces report in images and html
 
     for feature_type, mcriteria in motif_criteria.items():
-        h_donors = {} # handle to fasta donor sequence files
+        h_donors = {} # handle for fasta donor sequence files
         f = gzip.open(f"results/edgeR/{feature_type}_results_complete.tab.gz", "rt")
         header = f.readline().replace("\r", "").replace("\n", "").split("\t")
         r = f.readline()
         while r:
             r = r.replace("\r", "").replace("\n", "").split("\t")
             data = dict(zip(header, r))
             fdr = float(data["fdr"])
@@ -457,15 +420,15 @@
                     donor_site, acceptor_site = stop, start
             if feature_type in ["exons", "donor_anchors"]:
                 if strand=="+":
                     donor_site, acceptor_site = stop, start
                 else:
                     donor_site, acceptor_site = start, stop
             donor_seq = pybio.core.genomes.seq(config.species, chr, strand, donor_site, splice_sites_area[0], splice_sites_area[1], genome_version=config.genome_version)
-            if donor_seq.find("N")!=-1: # ignore sequences containing N
+            if donor_seq.find("N")!=-1: # ignore sequences with N
                 r = f.readline()
                 continue
             acceptor_seq = pybio.core.genomes.seq(config.species, chr, strand, acceptor_site, splice_sites_area[0], splice_sites_area[1], genome_version=config.genome_version)
             donor_id = f"{chr}{strand}_{donor_site}"
             acceptor_id = f"{chr}{strand}_{acceptor_site}"
             treatment = data["treatment"]
 
@@ -483,15 +446,14 @@
             # add sequences to each motif_criteria, if the criteria is met (eval)
             for cryteria_name, seq_field, criteria in mcriteria:
                 try: # because some anchors are not reported (too low expression or other reasons), data["fdr_anchor"] is sometimes empty for a junction
                     criteria_met = eval(criteria)
                 except:
                     criteria_met = False
 
-                #if criteria_met:
                 if criteria_met and donor_id not in feature_added.get((cryteria_name, seq_field, data["comparison"]), set()):
                     temp = treatment_seq_bytype.get(cryteria_name, {})
                     if seq_field=="donor":
                         temp_seq = donor_seq
                     if seq_field=="acceptor":
                         temp_seq = acceptor_seq
                     temp.setdefault(treatment, []).append(temp_seq)
@@ -505,15 +467,14 @@
                     feature_set = feature_added.get((cryteria_name, seq_field, data["comparison"]), set())
                     if seq_field=="donor":
                         feature_set.add(donor_id)
                     if seq_field=="acceptor":
                         feature_set.add(acceptor_id)
                     feature_added[(cryteria_name, seq_field, data["comparison"])] = feature_set
 
-
             temp = treatment_seq_bytype.get(f"{feature_type}_all", {})
             temp.setdefault(treatment, []).append(donor_seq)
             temp.setdefault("overall", []).append(donor_seq)
             treatment_seq_bytype[f"{feature_type}_all"] = temp
             r = f.readline()
         f.close()
         for f_name, f_handle in h_donors.items():
@@ -588,23 +549,14 @@
     print(f"{module_name} dreme | start")
     for comparison in splicekit.core.annotation.comparisons:
         comp_id = comparison[0]
         for dreme_name, dreme_positive, dreme_negative in dreme_criteria:
             command = f"{splicekit.config.container} dreme -png -k 7 -norc -m 5 -p results/motifs/fasta/{comp_id}_{dreme_positive}.fasta -n results/motifs/fasta/{comp_id}_{dreme_negative}.fasta -oc results/motifs/dreme/{comp_id}_{dreme_name}"
             os.system(command)
 
-        # for feature_type, mcriteria in motif_criteria.items():
-        #     for (criteria_name, _, _) in mcriteria:
-        #         if criteria_name.endswith("_controls"):
-        #             continue
-        #         if os.path.exists(f"results/motifs/fasta/{feature_type}_donor_controls.fasta"):
-        #             if os.path.exists(f"results/motifs/fasta/{comp_id}_{criteria_name}.fasta"):
-        #                 command = f"{splicekit.config.container} dreme -png -k 7 -norc -m 5 -p results/motifs/fasta/{comp_id}_{criteria_name}.fasta -n results/motifs/fasta/{feature_type}_donor_controls.fasta -oc results/motifs/dreme/{comp_id}_{criteria_name}"
-        #                 os.system(command)
-
 def make_distance():
     print(f"{module_name} make_distance | start")
     len_background, background = get_background()
     for feature_type in motif_criteria.keys():
         treatment_seq = treatment_seq_bytype.get(f"{feature_type}_all", {}) # use all to do the clustering and dendrogram
         f = open(f"results/motifs/{feature_type}_donor_pattern_dm.tab", "wt")
         f.write("\t".join(["treatment1", "treatment2", "donnor_pattern_distance"]) + "\n")
@@ -736,11 +688,12 @@
         f.write(html_code.format(cluster_blocks="\n".join(cluster_blocks)))
         f.close()
 
 def process():
     if config.scanRBP:
         make_scanRBP()
         plot_scanRBP()
+        scanRBP_dreme()
     make_logos()
     dreme()
     make_distance()
-    cluster()
+    cluster()
```

### Comparing `splicekit-0.5.1/splicekit/core/patterns.py` & `splicekit-0.6/splicekit/core/patterns.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,20 @@
             r = r.replace("\r", "").replace("\n", "").split("\t")
             data_new = dict(zip(header_new, r))
             coords = data_new["feature_id"].split('_')
             start = int(coords[-2])
             stop = int(coords[-1])
             strand = coords[-3][-1]
             chr = '_'.join(coords[:-2])[:-1]
-            if strand=="+":
-                donor_site, acceptor_site = start, stop
-            else:
-                donor_site, acceptor_site = stop, start
+            donor_site, acceptor_site = (start, stop) if strand=="+" else (stop, start)
             donor_seq = pybio.core.genomes.seq(config.species, chr, strand, donor_site, pattern_area[0], pattern_area[1], genome_version=config.genome_version)
             acceptor_seq = pybio.core.genomes.seq(config.species, chr, strand, acceptor_site, pattern_area[0], pattern_area[1], genome_version=config.genome_version)
             data_new["donor_pattern"] = donor_seq
             data_new["acceptor_pattern"] = acceptor_seq
             fout.write("\t".join(str(data_new[h]) for h in header_new) + "\n")
             r = fin.readline()
         fout.close()
         fin.close()
         os.system(f"mv results/edgeR/{fname}.tab.gz.temp results/edgeR/{fname}.tab.gz")
+        
     process_file(f"junctions_results_fdr005")
     process_file(f"junctions_results_complete")
```

### Comparing `splicekit-0.5.1/splicekit/core/promisc.py` & `splicekit-0.6/splicekit/core/promisc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 import splicekit.core.annotation as annotation
 import splicekit.config as config
 import gzip
 
+module_name = "splicekit | promisc |"
+
 def toint(temp):
     try:
         temp = str(int(temp))
         return temp
     except:
         return temp
 
@@ -30,15 +32,15 @@
         r = f.readline()
     f.close()
 
     # update results table
     count = 1
     for id, data in results.items():
         if count%100==0:
-            print("[promisc] processed {a}/{b} ({c}% done)".format(a=count, b=len(results), c="%.2f" % (count/len(results)*100)))
+            print("{module_name} processed {a}/{b} ({c}% done)".format(module_name=module_name, a=count, b=len(results), c="%.2f" % (count/len(results)*100)))
         count += 1
         for rid, rdata in results.items():
             if same_junction(data, rdata):
                 results[id][rdata["comparison"]+"_junction"] = 1
 
     reported_junction = {}
     fout_junction = gzip.open("results/junctions_promisc.tab.gz", "wt")
@@ -55,12 +57,11 @@
         for hid in header[7:]:
             row_junction.append(data.get(hid+"_junction", ""))
         row_sum_junction = sum([1 for el in row_junction if el==1])
         row_junction.insert(6, row_sum_junction)
         if reported_junction.get(tuple(row_junction[:6]), None)==None:
             temp_junction.append((row_sum_junction, row_junction))
             reported_junction[tuple(row_junction[:6])] = 1
-    # junction level
     temp_junction.sort(reverse=True)
     for row_sum, row in temp_junction:
         fout_junction.write("\t".join([str(el) for el in row]) + "\n")
     fout_junction.close()
```

### Comparing `splicekit-0.5.1/splicekit/folders.setup` & `splicekit-0.6/splicekit/folders.setup`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 results/motifs/dreme
 results/motifs/fasta
 results/motifs/images
 results/motifs
 results/motifs/scanRBP
 results/motifs/scanRBP/data
 results/motifs/scanRBP/fasta
+results/motifs/scanRBP/dreme
 results/dge
 results/judge
 results/judge/plots
 results/judge/data
 results/splicemap
 results/edgeR
 results/edgeR/junctions
```

### Comparing `splicekit-0.5.1/splicekit/judge/__init__.py` & `splicekit-0.6/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/splicecompare` & `splicekit-0.6/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit/splicekit` & `splicekit-0.6/splicekit/splicekit`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   
   -- Splicing analyses
      edgeR             run edgeR analyses on junctions, exons and anchors
      judge             run juDGE plot analysis
      promisc           promiscuity analysis: genes and their junctions changes across conditions
      clusterlogfc      log fold-change clusters of significant changes (FDR<0.05) on junction, exon, gene level
      rmats             process data with rMATS
+     june              junction-event (junE) analysis
 
   -- scanRBP, motif and sequence analyses
      motifs            run motif and scanRBP analysis
 
   -- JBrowse2 genomic browser
      jbrowse2 [process | start] processes (creates) all required JBrowse2 files and/or starts JBrowse2 web server
 
@@ -145,14 +146,16 @@
     splicekit.clusterlogfc_process()
 elif args.command[0]=="process":
     splicekit.process(force=args.force)
 elif args.command[0]=="judge":
     splicekit.judge_process()
 elif args.command[0]=="juan":
     splicekit.juan()
+elif args.command[0]=="june":
+    splicekit.june_process()
 elif args.command[0]=="rmats":
     splicekit.rmats()
 elif args.command[0] in ["jbrowse2", "jbrowse"]:
     if len(args.command)>1:
         if args.command[1]=="process":
             splicekit.jbrowse2_process(force_samples=args.force, force_annotation=args.force)
         if args.command[1]=="start":
```

### Comparing `splicekit-0.5.1/splicekit/splicekit.config.template` & `splicekit-0.6/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.5.1/splicekit.egg-info/PKG-INFO` & `splicekit-0.6/splicekit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.5.1
+Version: 0.6
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -21,14 +21,18 @@
 Requires-Dist: requests
 Requires-Dist: rangehttpserver
 
 ## splicekit: an integrative toolkit for splicing analysis from short-read RNA-seq
 
 <b>splicekit</b> is a modular platform for splicing analysis from short-read RNA-seq datasets. The platform also integrates an JBrowse2 instance, [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
+Check a short video presentation about splicekit (poster) at ECCB 2023 on Youtube:
+
+[<img src="media/splicekit_youtube.jpg" width=300>](https://youtu.be/P1m73usZ3lc?si=HBJxWOkUajObFpu1)
+
 ## Quick start
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
 Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute:
@@ -37,21 +41,15 @@
 
 Another suggestion is to install inside a virtual environment (using `virtualenv`).
 
 <details>
 <summary>Installing splicekit directly from the GitHub repository</summary>
 
 ```
-# move to HOME folder (for example)
-cd ~
-# clone the repository
-git clone git@github.com:bedapub/splicekit.git
-# adjust PYTHONPATH and PATH
-export PYTHONPATH=$PYTHONPATH:~/splicekit
-export PATH=$PATH:~/splicekit/splicekit
+pip install git+https://github.com/bedapub/splicekit.git@main
 ```
 </details>
 
 <details>
 <summary>If you already have aligned reads in BAM files</summary>
 
 All you need is `samples.tab` (note that this is a <b>TAB delimited file</b>) and `splicekit.config` in one folder (check [datasets](datasets) for examples).
@@ -66,53 +64,66 @@
 ## Documentation
 
 * [PDF reference manual](https://github.com/bedapub/splicekit/raw/main/docs/splicekit_docs.pdf)
 * [Google docs](https://docs.google.com/document/d/15ZRCeK8xyg3klLktZSHZ9k__Xw_BZRn_Q-J4W35JNnQ/edit?usp=sharing) of the above PDF (comment if you like)
 
 ## Changelog<a name="changelog"></a>
 
-**v0.4.9**: released in November 2023
+**v0.6**: released in April 2024
+
+* updated reports
+* JUNE analysis (junction-events to classify skipped and mutually exclusive exons)
+
+<details>
+<summary>Past changenotes (click to view)</summary>
+
+<b>v0.4.9</b>: released in November 2023
+
 * added rMATS analysis for splicing events
 * added Docker container that can be directly imported to singularity via ghcr.io
 * fixed dependencies
 * other small fixes
 
-<details>
-<summary><b>v0.4</b>: released in May 2023 (click to show details)</summary>
+<b>v0.4</b>: released in May 2023
 
 * added singularity container with all dependencies
 * added local integrated JBrowse2
 * cluster or desktop runs
 * scanRBP and bootstrap analysis of RNA-protein binding
 * further development and integration with pybio
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+<b>v0.3</b>: released in January 2023 (click to show details)
 
 * re-coded junction analysis
   * independent junctions parsing from provided bam files
   * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
 * clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
 * added *first_exon* annotation for junctions touching annotated first exons of transcripts
 * extended documentation of concepts, analysis and results
-</details>
 
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+<b>v0.2</b>: released in October 2022
 
 * software architecture restructure with python modules
 * filtering of lowly expressed features by edgeR
 * DonJuan analysis (junction-anchor analysis)
 * more advanced motif analysis with DREME
 * filtering regulated junctions with regulated donors
-</details>
 
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+<b>v0.1</b>: released in July 2022
 
 * initial version of splicekit
 * parsing of junction and exon counts
 * computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
 * basic motif analysis
+
 </details>
+
+## Citing and Contact<a name="citation"></a>
+
+If you find **splicekit** useful in your work and research, please cite:
+
+Gregor Rot, Arne Wehling, Roland Schmucki, Nikolaos Berntenis, Jitao David Zhang, Martin Ebeling<br>
+<a href='https://www.biorxiv.org/content/10.1101/2023.05.25.542256v1' target='_biorxiv'>splicekit: a comprehensive toolkit for splicing analysis from short-read RNA-seq</a><br>
+bioRxiv, 2023.05. 25.542256
+
+In case of questions, issues and other ideas, please use the <a href='https://github.com/bedapub/splicekit/issues'>GitHub Issues</a> or write directly to <a href='mailto:gregor.rot@gmail.com'>Gregor Rot</a>.
```

### Comparing `splicekit-0.5.1/splicekit.egg-info/SOURCES.txt` & `splicekit-0.6/splicekit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 splicekit/core/juan.py
 splicekit/core/junctions.py
 splicekit/core/motifs.py
 splicekit/core/patterns.py
 splicekit/core/promisc.py
 splicekit/core/report.py
 splicekit/judge/__init__.py
+splicekit/june/__init__.py
 splicekit/report/__init__.py
```

