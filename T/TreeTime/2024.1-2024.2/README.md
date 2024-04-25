# Comparing `tmp/TreeTime-2024.1.tar.gz` & `tmp/TreeTime-2024.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TreeTime-2024.1.tar", last modified: Wed Apr 17 09:16:38 2024, max compression
+gzip compressed data, was "TreeTime-2024.2.tar", last modified: Thu Apr 25 20:10:59 2024, max compression
```

## Comparing `TreeTime-2024.1.tar` & `TreeTime-2024.2.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.782835 TreeTime-2024.1/
--rwxr-x---   0 jacob     (1000) jacob     (1000)    35148 2022-02-22 20:58:49.000000 TreeTime-2024.1/LICENSE.txt
--rwxr-x---   0 jacob     (1000) jacob     (1000)       65 2022-02-22 20:58:49.000000 TreeTime-2024.1/MANIFEST.in
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16376 2024-04-17 09:16:38.782835 TreeTime-2024.1/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)    15794 2024-04-17 08:54:21.000000 TreeTime-2024.1/README.md
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.770835 TreeTime-2024.1/TreeTime.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16376 2024-04-17 09:16:38.000000 TreeTime-2024.1/TreeTime.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7337 2024-04-17 09:16:38.000000 TreeTime-2024.1/TreeTime.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2024-04-17 09:16:38.000000 TreeTime-2024.1/TreeTime.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       48 2024-04-17 09:16:38.000000 TreeTime-2024.1/TreeTime.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        9 2024-04-17 09:16:38.000000 TreeTime-2024.1/TreeTime.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.714835 TreeTime-2024.1/data/
--rwxr-x---   0 jacob     (1000) jacob     (1000)      530 2022-02-22 20:58:49.000000 TreeTime-2024.1/data/Dual-MindMap.empty.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)     1213 2022-02-22 20:58:49.000000 TreeTime-2024.1/data/Example.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)     5407 2022-02-22 20:58:49.000000 TreeTime-2024.1/data/Simple-Task-List.empty.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)    11931 2022-02-22 20:58:49.000000 TreeTime-2024.1/data/Simple-Task-List.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)      358 2022-02-22 20:58:49.000000 TreeTime-2024.1/data/Single-MindMap.empty.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)    20669 2022-06-11 01:35:21.000000 TreeTime-2024.1/data/Tutorial.test.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)    21725 2022-11-10 11:10:48.000000 TreeTime-2024.1/data/Tutorial.trt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6914 2024-02-03 22:48:18.000000 TreeTime-2024.1/data/Work-Plan.trt
--rwxr-x---   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.1/data/treetime-logo.png
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.730835 TreeTime-2024.1/docs/
--rwxr-x---   0 jacob     (1000) jacob     (1000)      398 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/404.html
--rwxr-x---   0 jacob     (1000) jacob     (1000)       14 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/CNAME
--rwxr-x---   0 jacob     (1000) jacob     (1000)     1254 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/Gemfile
--rwxr-x---   0 jacob     (1000) jacob     (1000)     7732 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/Gemfile.lock
--rwxr-x---   0 jacob     (1000) jacob     (1000)      634 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/Makefile
--rw-r--r--   0 jacob     (1000) jacob     (1000)   738301 2023-07-10 16:45:18.000000 TreeTime-2024.1/docs/TreeTime_User-Manual_20223-07-10.pdf
--rw-r--r--   0 jacob     (1000) jacob     (1000)   748236 2024-04-17 09:07:18.000000 TreeTime-2024.1/docs/TreeTime_User-Manual_2024-04-17.pdf
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.710835 TreeTime-2024.1/docs/_build/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.730835 TreeTime-2024.1/docs/_build/doctrees/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.734835 TreeTime-2024.1/docs/_build/doctrees/_site/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6014 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/doctrees/_site/index.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    34221 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/_site/introduction.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    23941 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/_site/releases.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    12837 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/data-fields.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    18099 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/data-format.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)   286937 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6007 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/index.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    35225 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/introduction.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    32603 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/releases.doctree
--rw-r--r--   0 jacob     (1000) jacob     (1000)    28025 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/doctrees/tree-fields.doctree
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.734835 TreeTime-2024.1/docs/_build/html/
--rw-r--r--   0 jacob     (1000) jacob     (1000)      230 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/.buildinfo
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.742835 TreeTime-2024.1/docs/_build/html/_images/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/abcde01.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/abcde011.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/abcde02.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/abcde021.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/linked-trees.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/linked-trees1.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot01.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot011.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot02.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot021.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot03.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot031.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot04.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_images/screenshot041.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.1/docs/_build/html/_images/treetime-logo.png
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.742835 TreeTime-2024.1/docs/_build/html/_site/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5363 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/_site/index.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)    13769 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/html/_site/introduction.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9746 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/html/_site/releases.html
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.742835 TreeTime-2024.1/docs/_build/html/_sources/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.746835 TreeTime-2024.1/docs/_build/html/_sources/_site/
--rw-r--r--   0 jacob     (1000) jacob     (1000)      781 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_sources/_site/index.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7869 2023-05-02 07:40:27.000000 TreeTime-2024.1/docs/_build/html/_sources/_site/introduction.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4043 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/html/_sources/_site/releases.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2861 2024-04-17 09:04:11.000000 TreeTime-2024.1/docs/_build/html/_sources/data-fields.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6071 2024-04-17 08:01:00.000000 TreeTime-2024.1/docs/_build/html/_sources/data-format.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)      826 2023-07-10 16:32:21.000000 TreeTime-2024.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8424 2024-04-17 08:56:49.000000 TreeTime-2024.1/docs/_build/html/_sources/introduction.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5639 2024-04-17 09:01:29.000000 TreeTime-2024.1/docs/_build/html/_sources/releases.rst.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7193 2024-04-17 08:14:16.000000 TreeTime-2024.1/docs/_build/html/_sources/tree-fields.rst.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.750835 TreeTime-2024.1/docs/_build/html/_static/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11185 2024-04-17 09:04:22.000000 TreeTime-2024.1/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 jacob     (1000) jacob     (1000)    15094 2024-04-17 09:04:22.000000 TreeTime-2024.1/docs/_build/html/_static/basic.css
--rw-r--r--   0 jacob     (1000) jacob     (1000)       42 2017-05-15 18:58:47.000000 TreeTime-2024.1/docs/_build/html/_static/custom.css
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4472 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)      329 2024-04-17 09:04:22.000000 TreeTime-2024.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)      286 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/file.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7791 2021-06-13 20:22:59.000000 TreeTime-2024.1/docs/_build/html/_static/forkme_right_darkblue_121621.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4758 2024-04-17 09:04:22.000000 TreeTime-2024.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)       90 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)       90 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5327 2024-04-17 09:04:22.000000 TreeTime-2024.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 jacob     (1000) jacob     (1000)    18931 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5123 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11708 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/html/data-fields.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)    21841 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/html/data-format.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2919 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/genindex.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8939 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/index.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)    14961 2024-04-17 09:04:19.000000 TreeTime-2024.1/docs/_build/html/introduction.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)      352 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/objects.inv
--rw-r--r--   0 jacob     (1000) jacob     (1000)    12602 2024-04-17 09:04:20.000000 TreeTime-2024.1/docs/_build/html/releases.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3196 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/search.html
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16822 2024-04-17 09:04:23.000000 TreeTime-2024.1/docs/_build/html/searchindex.js
--rw-r--r--   0 jacob     (1000) jacob     (1000)    24803 2024-04-17 09:04:20.000000 TreeTime-2024.1/docs/_build/html/tree-fields.html
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.762835 TreeTime-2024.1/docs/_build/latex/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4366 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/LICRcyr2utf8.xdy
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10188 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/LICRlatin2utf8.xdy
--rw-r--r--   0 jacob     (1000) jacob     (1000)    18890 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/LatinRules.xdy
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1549 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/latex/Makefile
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/abcde011.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/abcde021.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)      684 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/latex/latexmkjarc
--rw-r--r--   0 jacob     (1000) jacob     (1000)      405 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/latex/latexmkrc
--rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/linked-trees1.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)      473 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/latex/make.bat
--rw-r--r--   0 jacob     (1000) jacob     (1000)      392 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/python.ist
--rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/screenshot011.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/screenshot021.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/screenshot031.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_build/latex/screenshot041.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    44560 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinx.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     9474 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinx.xdy
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7490 2024-04-17 09:05:33.000000 TreeTime-2024.1/docs/_build/latex/sphinxhighlight.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3256 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxhowto.cls
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10989 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexadmonitions.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)      901 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexcontainers.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4840 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexgraphics.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2066 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexindbibtoc.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5139 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexlists.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)    46048 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexliterals.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4532 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexnumfig.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)    14354 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexobjects.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5066 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexshadowbox.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3445 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexstyleheadings.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3064 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexstylepage.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8589 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatexstyletext.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)    57830 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxlatextables.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4241 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxmanual.cls
--rw-r--r--   0 jacob     (1000) jacob     (1000)      745 2024-04-17 09:05:34.000000 TreeTime-2024.1/docs/_build/latex/sphinxmessages.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2061 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxoptionsgeometry.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1094 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxoptionshyperref.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)    36615 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxpackageboxes.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2590 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxpackagecyrillic.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)    15254 2023-12-19 10:34:25.000000 TreeTime-2024.1/docs/_build/latex/sphinxpackagefootnote.sty
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.1/docs/_build/latex/treetime-logo.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)    12414 2024-04-17 09:05:55.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.aux
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:05:52.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.idx
--rw-r--r--   0 jacob     (1000) jacob     (1000)    33443 2024-04-17 09:05:55.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.log
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6287 2024-04-17 09:05:55.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.out
--rw-r--r--   0 jacob     (1000) jacob     (1000)   748236 2024-04-17 09:05:55.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.pdf
--rw-r--r--   0 jacob     (1000) jacob     (1000)    63140 2024-04-17 09:05:34.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.tex
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4554 2024-04-17 09:05:55.000000 TreeTime-2024.1/docs/_build/latex/treetimeusermanual.toc
--rwxr-x---   0 jacob     (1000) jacob     (1000)     1626 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_config.yml
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.766835 TreeTime-2024.1/docs/_site/
--rwxr-x---   0 jacob     (1000) jacob     (1000)     3150 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/404.html
--rwxr-x---   0 jacob     (1000) jacob     (1000)      634 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/Makefile
--rwxr-x---   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/abcde01.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/abcde02.png
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.766835 TreeTime-2024.1/docs/_site/about/
--rwxr-x---   0 jacob     (1000) jacob     (1000)      523 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/about/index.html
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.710835 TreeTime-2024.1/docs/_site/assets/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.770835 TreeTime-2024.1/docs/_site/assets/css/
--rwxr-x---   0 jacob     (1000) jacob     (1000)    10404 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/assets/css/style.css
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.770835 TreeTime-2024.1/docs/_site/assets/images/
--rwxr-x---   0 jacob     (1000) jacob     (1000)       78 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/assets/images/bg_hr.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)      463 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/assets/images/blacktocat.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)      216 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/assets/images/icon_download.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)    14832 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/assets/images/sprite_download.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)     1925 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/conf.py
--rwxr-x---   0 jacob     (1000) jacob     (1000)      539 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/feed.xml
--rwxr-x---   0 jacob     (1000) jacob     (1000)     9909 2023-05-02 07:40:26.000000 TreeTime-2024.1/docs/_site/index.html
--rwxr-x---   0 jacob     (1000) jacob     (1000)     5859 2024-04-17 08:57:21.000000 TreeTime-2024.1/docs/_site/index.md
--rwxr-x---   0 jacob     (1000) jacob     (1000)      781 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/index.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)     7869 2023-05-02 07:40:27.000000 TreeTime-2024.1/docs/_site/introduction.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)     2082 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/linked-trees.dia
--rwxr-x---   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/linked-trees.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)      795 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/make.bat
--rwxr-x---   0 jacob     (1000) jacob     (1000)     4043 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/releases.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/screenshot01.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/screenshot02.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/screenshot03.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/_site/screenshot04.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/abcde01.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/abcde02.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)      539 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/about.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1946 2024-04-17 08:57:41.000000 TreeTime-2024.1/docs/conf.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2861 2024-04-17 09:04:11.000000 TreeTime-2024.1/docs/data-fields.rst
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6071 2024-04-17 08:01:00.000000 TreeTime-2024.1/docs/data-format.rst
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5859 2023-08-17 16:07:32.000000 TreeTime-2024.1/docs/index.md
--rwxr-x---   0 jacob     (1000) jacob     (1000)      826 2023-07-10 16:32:21.000000 TreeTime-2024.1/docs/index.rst
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8424 2024-04-17 08:56:49.000000 TreeTime-2024.1/docs/introduction.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)    79322 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/kameri-auth.txt
--rwxr-x---   0 jacob     (1000) jacob     (1000)     2082 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/linked-trees.dia
--rwxr-x---   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/linked-trees.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)      795 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/make.bat
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5639 2024-04-17 09:01:29.000000 TreeTime-2024.1/docs/releases.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/screenshot01.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/screenshot02.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/screenshot03.png
--rwxr-x---   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.1/docs/screenshot04.png
--rw-r--r--   0 jacob     (1000) jacob     (1000)     7193 2024-04-17 08:14:16.000000 TreeTime-2024.1/docs/tree-fields.rst
--rwxr-x---   0 jacob     (1000) jacob     (1000)       79 2024-04-17 09:16:38.782835 TreeTime-2024.1/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1858 2024-04-17 08:45:52.000000 TreeTime-2024.1/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.774835 TreeTime-2024.1/treetime/
--rwxr-x---   0 jacob     (1000) jacob     (1000)       97 2022-02-22 20:58:49.000000 TreeTime-2024.1/treetime/__init__.py
--rwxr-x---   0 jacob     (1000) jacob     (1000)      261 2022-03-16 11:29:28.000000 TreeTime-2024.1/treetime/__main__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      265 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/compile-ui.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11721 2024-02-03 22:48:18.000000 TreeTime-2024.1/treetime/item.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    39344 2024-04-17 09:05:13.000000 TreeTime-2024.1/treetime/mainwindow.py
--rwxr-x---   0 jacob     (1000) jacob     (1000)     2563 2022-02-22 20:58:49.000000 TreeTime-2024.1/treetime/test.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-17 09:16:38.782835 TreeTime-2024.1/treetime/themes/
--rw-r--r--   0 jacob     (1000) jacob     (1000)       97 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/dark_branch_full.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       95 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/dark_branch_top.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.1/treetime/themes/dark_triangle_down.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.1/treetime/themes/dark_triangle_down_hover.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/dark_triangle_right.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/dark_triangle_right_hover.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      105 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/dark_twig_empty.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       97 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/light_branch_full.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       95 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/light_branch_top.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.1/treetime/themes/light_triangle_down.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.1/treetime/themes/light_triangle_down_hover.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/light_triangle_right.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/light_triangle_right_hover.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)      105 2023-07-03 09:03:30.000000 TreeTime-2024.1/treetime/themes/light_twig_empty.svg
--rw-r--r--   0 jacob     (1000) jacob     (1000)    49473 2024-02-03 22:48:18.000000 TreeTime-2024.1/treetime/tree.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    89625 2024-02-03 22:51:28.000000 TreeTime-2024.1/treetime/treetime.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.204299 TreeTime-2024.2/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    35148 2022-02-22 20:58:49.000000 TreeTime-2024.2/LICENSE.txt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)       65 2022-02-22 20:58:49.000000 TreeTime-2024.2/MANIFEST.in
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16653 2024-04-25 20:10:59.204299 TreeTime-2024.2/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16071 2024-04-25 19:48:47.000000 TreeTime-2024.2/README.md
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.196299 TreeTime-2024.2/TreeTime.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16653 2024-04-25 20:10:59.000000 TreeTime-2024.2/TreeTime.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7358 2024-04-25 20:10:59.000000 TreeTime-2024.2/TreeTime.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2024-04-25 20:10:59.000000 TreeTime-2024.2/TreeTime.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       48 2024-04-25 20:10:59.000000 TreeTime-2024.2/TreeTime.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        9 2024-04-25 20:10:59.000000 TreeTime-2024.2/TreeTime.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.140301 TreeTime-2024.2/data/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      530 2022-02-22 20:58:49.000000 TreeTime-2024.2/data/Dual-MindMap.empty.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     1213 2022-02-22 20:58:49.000000 TreeTime-2024.2/data/Example.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     5407 2022-02-22 20:58:49.000000 TreeTime-2024.2/data/Simple-Task-List.empty.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    11931 2022-02-22 20:58:49.000000 TreeTime-2024.2/data/Simple-Task-List.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      358 2022-02-22 20:58:49.000000 TreeTime-2024.2/data/Single-MindMap.empty.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    20669 2022-06-11 01:35:21.000000 TreeTime-2024.2/data/Tutorial.test.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    21725 2022-11-10 11:10:48.000000 TreeTime-2024.2/data/Tutorial.trt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6914 2024-02-03 22:48:18.000000 TreeTime-2024.2/data/Work-Plan.trt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.2/data/treetime-logo.png
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.156300 TreeTime-2024.2/docs/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      398 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/404.html
+-rwxr-x---   0 jacob     (1000) jacob     (1000)       14 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/CNAME
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     1254 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/Gemfile
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     7732 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/Gemfile.lock
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      634 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/Makefile
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   738301 2023-07-10 16:45:18.000000 TreeTime-2024.2/docs/TreeTime_User-Manual_20223-07-10.pdf
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   748236 2024-04-17 09:07:18.000000 TreeTime-2024.2/docs/TreeTime_User-Manual_2024-04-17.pdf
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   748369 2024-04-25 20:08:53.000000 TreeTime-2024.2/docs/TreeTime_User-Manual_2024-04-25.pdf
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.136301 TreeTime-2024.2/docs/_build/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.160300 TreeTime-2024.2/docs/_build/doctrees/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.160300 TreeTime-2024.2/docs/_build/doctrees/_site/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6014 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/doctrees/_site/index.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    34221 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/_site/introduction.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    23941 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/_site/releases.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    12837 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/data-fields.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    18099 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/data-format.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   288089 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6007 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    35225 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/introduction.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    33524 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/releases.doctree
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    28025 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/doctrees/tree-fields.doctree
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.160300 TreeTime-2024.2/docs/_build/html/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      230 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/.buildinfo
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.168300 TreeTime-2024.2/docs/_build/html/_images/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/abcde01.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/abcde011.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/abcde02.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/abcde021.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/linked-trees.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/linked-trees1.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot01.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot011.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot02.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot021.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot03.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot031.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot04.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_images/screenshot041.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.2/docs/_build/html/_images/treetime-logo.png
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.168300 TreeTime-2024.2/docs/_build/html/_site/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5363 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_site/index.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    13769 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_site/introduction.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9746 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_site/releases.html
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.168300 TreeTime-2024.2/docs/_build/html/_sources/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.168300 TreeTime-2024.2/docs/_build/html/_sources/_site/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      781 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_sources/_site/index.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7869 2023-05-02 07:40:27.000000 TreeTime-2024.2/docs/_build/html/_sources/_site/introduction.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4043 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/html/_sources/_site/releases.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2861 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/_build/html/_sources/data-fields.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6071 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/_build/html/_sources/data-format.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      826 2023-07-10 16:32:21.000000 TreeTime-2024.2/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8424 2024-04-25 19:32:40.000000 TreeTime-2024.2/docs/_build/html/_sources/introduction.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5906 2024-04-25 19:50:33.000000 TreeTime-2024.2/docs/_build/html/_sources/releases.rst.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7193 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/_build/html/_sources/tree-fields.rst.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.172300 TreeTime-2024.2/docs/_build/html/_static/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11185 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    15094 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_static/basic.css
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       42 2017-05-15 18:58:47.000000 TreeTime-2024.2/docs/_build/html/_static/custom.css
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4472 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      329 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      286 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7791 2021-06-13 20:22:59.000000 TreeTime-2024.2/docs/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4758 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       90 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       90 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5327 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    18931 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5123 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11708 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/data-fields.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    21841 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/data-format.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2919 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/genindex.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8939 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/index.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    14961 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/introduction.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      352 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/objects.inv
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    12910 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/releases.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3196 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/search.html
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16867 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/searchindex.js
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    24803 2024-04-25 20:03:18.000000 TreeTime-2024.2/docs/_build/html/tree-fields.html
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.188300 TreeTime-2024.2/docs/_build/latex/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4366 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/LICRcyr2utf8.xdy
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10188 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/LICRlatin2utf8.xdy
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    18890 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/LatinRules.xdy
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1549 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/latex/Makefile
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/abcde011.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/abcde021.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      684 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/latex/latexmkjarc
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      405 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/latex/latexmkrc
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/linked-trees1.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      473 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/latex/make.bat
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      392 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/python.ist
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/screenshot011.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/screenshot021.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/screenshot031.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_build/latex/screenshot041.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    44560 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinx.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     9474 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinx.xdy
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7490 2024-04-25 20:07:22.000000 TreeTime-2024.2/docs/_build/latex/sphinxhighlight.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3256 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxhowto.cls
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10989 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexadmonitions.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      901 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexcontainers.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4840 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexgraphics.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2066 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexindbibtoc.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5139 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexlists.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    46048 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexliterals.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4532 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexnumfig.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    14354 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexobjects.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5066 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexshadowbox.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3445 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexstyleheadings.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3064 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexstylepage.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8589 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatexstyletext.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    57830 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxlatextables.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4241 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxmanual.cls
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      745 2024-04-25 20:07:23.000000 TreeTime-2024.2/docs/_build/latex/sphinxmessages.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2061 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxoptionsgeometry.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1094 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxoptionshyperref.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    36615 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxpackageboxes.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2590 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxpackagecyrillic.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    15254 2023-12-19 10:34:25.000000 TreeTime-2024.2/docs/_build/latex/sphinxpackagefootnote.sty
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5555 2023-04-26 15:53:38.000000 TreeTime-2024.2/docs/_build/latex/treetime-logo.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    12414 2024-04-25 20:07:50.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.aux
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:07:48.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.idx
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    33443 2024-04-25 20:07:50.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.log
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6287 2024-04-25 20:07:50.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.out
+-rw-r--r--   0 jacob     (1000) jacob     (1000)   748369 2024-04-25 20:07:50.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.pdf
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    63491 2024-04-25 20:07:23.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.tex
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4554 2024-04-25 20:07:50.000000 TreeTime-2024.2/docs/_build/latex/treetimeusermanual.toc
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1600 2024-04-25 19:29:32.000000 TreeTime-2024.2/docs/_config.yml
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.192299 TreeTime-2024.2/docs/_site/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     3150 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/404.html
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      634 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/Makefile
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/abcde01.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/abcde02.png
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.196299 TreeTime-2024.2/docs/_site/about/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      523 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/about/index.html
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.136301 TreeTime-2024.2/docs/_site/assets/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.196299 TreeTime-2024.2/docs/_site/assets/css/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    10404 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/assets/css/style.css
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.196299 TreeTime-2024.2/docs/_site/assets/images/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)       78 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/assets/images/bg_hr.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      463 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/assets/images/blacktocat.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      216 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/assets/images/icon_download.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    14832 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/assets/images/sprite_download.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     1925 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/conf.py
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      539 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/feed.xml
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     9909 2023-05-02 07:40:26.000000 TreeTime-2024.2/docs/_site/index.html
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      781 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/index.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     7869 2023-05-02 07:40:27.000000 TreeTime-2024.2/docs/_site/introduction.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     2082 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/linked-trees.dia
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/linked-trees.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      795 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/make.bat
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     4043 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/releases.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/screenshot01.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/screenshot02.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/screenshot03.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/_site/screenshot04.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     9776 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/abcde01.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     9887 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/abcde02.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      539 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/about.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1946 2024-04-25 19:34:34.000000 TreeTime-2024.2/docs/conf.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2861 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/data-fields.rst
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6071 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/data-format.rst
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5859 2024-04-25 19:34:13.000000 TreeTime-2024.2/docs/index.md
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      826 2023-07-10 16:32:21.000000 TreeTime-2024.2/docs/index.rst
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8424 2024-04-25 19:32:40.000000 TreeTime-2024.2/docs/introduction.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    79322 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/kameri-auth.txt
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     2082 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/linked-trees.dia
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    24220 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/linked-trees.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      795 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/make.bat
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5906 2024-04-25 19:50:33.000000 TreeTime-2024.2/docs/releases.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   190697 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/screenshot01.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   191806 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/screenshot02.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)    68742 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/screenshot03.png
+-rwxr-x---   0 jacob     (1000) jacob     (1000)   144567 2022-02-22 20:58:49.000000 TreeTime-2024.2/docs/screenshot04.png
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7193 2024-04-17 12:01:58.000000 TreeTime-2024.2/docs/tree-fields.rst
+-rwxr-x---   0 jacob     (1000) jacob     (1000)       79 2024-04-25 20:10:59.208299 TreeTime-2024.2/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1858 2024-04-25 19:33:19.000000 TreeTime-2024.2/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.200299 TreeTime-2024.2/treetime/
+-rwxr-x---   0 jacob     (1000) jacob     (1000)       97 2022-02-22 20:58:49.000000 TreeTime-2024.2/treetime/__init__.py
+-rwxr-x---   0 jacob     (1000) jacob     (1000)      261 2022-03-16 11:29:28.000000 TreeTime-2024.2/treetime/__main__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      265 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/compile-ui.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11721 2024-02-03 22:48:18.000000 TreeTime-2024.2/treetime/item.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    45438 2024-04-25 20:09:12.000000 TreeTime-2024.2/treetime/mainwindow.py
+-rwxr-x---   0 jacob     (1000) jacob     (1000)     2563 2022-02-22 20:58:49.000000 TreeTime-2024.2/treetime/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-04-25 20:10:59.204299 TreeTime-2024.2/treetime/themes/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       97 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/dark_branch_full.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       95 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/dark_branch_top.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.2/treetime/themes/dark_triangle_down.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.2/treetime/themes/dark_triangle_down_hover.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/dark_triangle_right.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/dark_triangle_right_hover.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      105 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/dark_twig_empty.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       97 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/light_branch_full.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       95 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/light_branch_top.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.2/treetime/themes/light_triangle_down.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-08-11 11:13:24.000000 TreeTime-2024.2/treetime/themes/light_triangle_down_hover.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/light_triangle_right.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/light_triangle_right_hover.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      105 2023-07-03 09:03:30.000000 TreeTime-2024.2/treetime/themes/light_twig_empty.svg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    55836 2024-04-25 19:29:32.000000 TreeTime-2024.2/treetime/tree.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    89201 2024-04-25 19:29:32.000000 TreeTime-2024.2/treetime/treetime.py
```

### Comparing `TreeTime-2024.1/LICENSE.txt` & `TreeTime-2024.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/PKG-INFO` & `TreeTime-2024.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeTime
-Version: 2024.1
+Version: 2024.2
 Summary: TreeTime is a to-do list manager, test report tool, project manager, family ancestry editor,mind-mapping tool, etc. Using TreeTime you can categorise and organise any data in tree structures.You can define several trees, each with a different structure, on the same data. You can use functions(sums, ratios and means) recursively up the branches of a tree.
 Home-page: https://github.com/jkanev/treetime
 Author: Jacob Kanev
 Author-email: jkanev@zoho.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -118,15 +118,15 @@
 <div id='id-installation'/>
 
 ##  Installation  ##
 [Table of Contents](#id-installation)
 
 ### Using pre-compiled Binaries ###
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
 (If anybody can help building an executable for other platforms I'd be delighted.)
 
 ### Using a PyPi package in Python ###
@@ -221,14 +221,16 @@
 * Done June 2023: Implemented display of tree field definitions and of data field definitions
 * Done July 2023: Release **version 2023.2**
 * Done October 2023: Bugfix: crash when exporting text to clipboard.
 * Done January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 * Done February 2024: Implemented min, max, min-string, max-string fields.
 * Done March 2024: Implemented longtext data field.
 * Done April 2024: Extended documentation on readthedocs.io. Release **version 2024.1**
+* Done April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+* Done April 2024: Release **version 2024.2**
 
 Present
 - Running: Bugfixing
 - Running: Extend documentation on readthedocs.io
 - Running: Implementing continuous text and html export (to use treetime as a meeting note-taking app where participants view an auto-updating html file with the notes)
 - Running: Add more examples and more template data files
 - Running: Implement tree field editing with graphical dialog (add, remove, change tree fields)
```

### Comparing `TreeTime-2024.1/README.md` & `TreeTime-2024.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 <div id='id-installation'/>
 
 ##  Installation  ##
 [Table of Contents](#id-installation)
 
 ### Using pre-compiled Binaries ###
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
 (If anybody can help building an executable for other platforms I'd be delighted.)
 
 ### Using a PyPi package in Python ###
@@ -211,14 +211,16 @@
 * Done June 2023: Implemented display of tree field definitions and of data field definitions
 * Done July 2023: Release **version 2023.2**
 * Done October 2023: Bugfix: crash when exporting text to clipboard.
 * Done January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 * Done February 2024: Implemented min, max, min-string, max-string fields.
 * Done March 2024: Implemented longtext data field.
 * Done April 2024: Extended documentation on readthedocs.io. Release **version 2024.1**
+* Done April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+* Done April 2024: Release **version 2024.2**
 
 Present
 - Running: Bugfixing
 - Running: Extend documentation on readthedocs.io
 - Running: Implementing continuous text and html export (to use treetime as a meeting note-taking app where participants view an auto-updating html file with the notes)
 - Running: Add more examples and more template data files
 - Running: Implement tree field editing with graphical dialog (add, remove, change tree fields)
```

### Comparing `TreeTime-2024.1/TreeTime.egg-info/PKG-INFO` & `TreeTime-2024.2/TreeTime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeTime
-Version: 2024.1
+Version: 2024.2
 Summary: TreeTime is a to-do list manager, test report tool, project manager, family ancestry editor,mind-mapping tool, etc. Using TreeTime you can categorise and organise any data in tree structures.You can define several trees, each with a different structure, on the same data. You can use functions(sums, ratios and means) recursively up the branches of a tree.
 Home-page: https://github.com/jkanev/treetime
 Author: Jacob Kanev
 Author-email: jkanev@zoho.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -118,15 +118,15 @@
 <div id='id-installation'/>
 
 ##  Installation  ##
 [Table of Contents](#id-installation)
 
 ### Using pre-compiled Binaries ###
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
 (If anybody can help building an executable for other platforms I'd be delighted.)
 
 ### Using a PyPi package in Python ###
@@ -221,14 +221,16 @@
 * Done June 2023: Implemented display of tree field definitions and of data field definitions
 * Done July 2023: Release **version 2023.2**
 * Done October 2023: Bugfix: crash when exporting text to clipboard.
 * Done January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 * Done February 2024: Implemented min, max, min-string, max-string fields.
 * Done March 2024: Implemented longtext data field.
 * Done April 2024: Extended documentation on readthedocs.io. Release **version 2024.1**
+* Done April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+* Done April 2024: Release **version 2024.2**
 
 Present
 - Running: Bugfixing
 - Running: Extend documentation on readthedocs.io
 - Running: Implementing continuous text and html export (to use treetime as a meeting note-taking app where participants view an auto-updating html file with the notes)
 - Running: Add more examples and more template data files
 - Running: Implement tree field editing with graphical dialog (add, remove, change tree fields)
```

### Comparing `TreeTime-2024.1/TreeTime.egg-info/SOURCES.txt` & `TreeTime-2024.2/TreeTime.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ./docs/404.html
 ./docs/CNAME
 ./docs/Gemfile
 ./docs/Gemfile.lock
 ./docs/Makefile
 ./docs/TreeTime_User-Manual_20223-07-10.pdf
 ./docs/TreeTime_User-Manual_2024-04-17.pdf
+./docs/TreeTime_User-Manual_2024-04-25.pdf
 ./docs/_config.yml
 ./docs/abcde01.png
 ./docs/abcde02.png
 ./docs/about.md
 ./docs/conf.py
 ./docs/data-fields.rst
 ./docs/data-format.rst
@@ -150,15 +151,14 @@
 ./docs/_site/404.html
 ./docs/_site/Makefile
 ./docs/_site/abcde01.png
 ./docs/_site/abcde02.png
 ./docs/_site/conf.py
 ./docs/_site/feed.xml
 ./docs/_site/index.html
-./docs/_site/index.md
 ./docs/_site/index.rst
 ./docs/_site/introduction.rst
 ./docs/_site/linked-trees.dia
 ./docs/_site/linked-trees.png
 ./docs/_site/make.bat
 ./docs/_site/releases.rst
 ./docs/_site/screenshot01.png
```

### Comparing `TreeTime-2024.1/data/Dual-MindMap.empty.trt` & `TreeTime-2024.2/data/Dual-MindMap.empty.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Example.trt` & `TreeTime-2024.2/data/Example.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Simple-Task-List.empty.trt` & `TreeTime-2024.2/data/Simple-Task-List.empty.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Simple-Task-List.trt` & `TreeTime-2024.2/data/Simple-Task-List.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Tutorial.test.trt` & `TreeTime-2024.2/data/Tutorial.test.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Tutorial.trt` & `TreeTime-2024.2/data/Tutorial.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/Work-Plan.trt` & `TreeTime-2024.2/data/Work-Plan.trt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/data/treetime-logo.png` & `TreeTime-2024.2/data/treetime-logo.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/Gemfile` & `TreeTime-2024.2/docs/Gemfile`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/Gemfile.lock` & `TreeTime-2024.2/docs/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/Makefile` & `TreeTime-2024.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/TreeTime_User-Manual_20223-07-10.pdf` & `TreeTime-2024.2/docs/TreeTime_User-Manual_20223-07-10.pdf`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/TreeTime_User-Manual_2024-04-17.pdf` & `TreeTime-2024.2/docs/TreeTime_User-Manual_2024-04-17.pdf`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/_site/index.doctree` & `TreeTime-2024.2/docs/_build/doctrees/_site/index.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/_site/introduction.doctree` & `TreeTime-2024.2/docs/_build/doctrees/_site/introduction.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/_site/releases.doctree` & `TreeTime-2024.2/docs/_build/doctrees/_site/releases.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/data-fields.doctree` & `TreeTime-2024.2/docs/_build/doctrees/data-fields.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/data-format.doctree` & `TreeTime-2024.2/docs/_build/doctrees/data-format.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/index.doctree` & `TreeTime-2024.2/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/doctrees/introduction.doctree` & `TreeTime-2024.2/docs/_build/doctrees/introduction.doctree`

 * *Files 1% similar despite different names*

```diff
@@ -1240,19 +1240,19 @@
 00004d70: 5f6c 6973 7494 9394 2981 947d 9428 6805  _list...)..}.(h.
 00004d80: 6806 6807 5d94 2868 098c 096c 6973 745f  h.h.].(h...list_
 00004d90: 6974 656d 9493 9429 8194 7d94 2868 0558  item...)..}.(h.X
 00004da0: e101 0000 5769 6e64 6f77 732c 204c 696e  ....Windows, Lin
 00004db0: 7578 3a20 476f 2074 6f20 5b67 6974 6875  ux: Go to [githu
 00004dc0: 622e 636f 6d2f 6a6b 616e 6576 2f74 7265  b.com/jkanev/tre
 00004dd0: 6574 696d 652f 7265 6c65 6173 6573 2f74  etime/releases/t
-00004de0: 6167 2f32 3032 342e 315d 2868 7474 7073  ag/2024.1](https
+00004de0: 6167 2f32 3032 342e 325d 2868 7474 7073  ag/2024.2](https
 00004df0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6b  ://github.com/jk
 00004e00: 616e 6576 2f74 7265 6574 696d 652f 7265  anev/treetime/re
 00004e10: 6c65 6173 6573 2f74 6167 2f32 3032 342e  leases/tag/2024.
-00004e20: 3129 2061 6e64 2064 6f77 6e6c 6f61 6420  1) and download 
+00004e20: 3229 2061 6e64 2064 6f77 6e6c 6f61 6420  2) and download 
 00004e30: 6120 7a69 7070 6564 2070 6163 6b61 6765  a zipped package
 00004e40: 2066 6f72 2057 696e 646f 7773 2031 302c   for Windows 10,
 00004e50: 2036 3420 6269 742c 206f 7220 666f 7220   64 bit, or for 
 00004e60: 4c69 6e75 7820 3634 2062 6974 2066 726f  Linux 64 bit fro
 00004e70: 6d20 7468 6572 652e 2055 6e7a 6970 2069  m there. Unzip i
 00004e80: 7420 696e 746f 2079 6f75 7220 7072 6f67  t into your prog
 00004e90: 7261 6d20 6469 7265 6374 6f72 7920 616e  ram directory an
@@ -1271,19 +1271,19 @@
 00004f60: 722e 6f72 675d 2868 7474 703a 2f2f 7777  r.org](http://ww
 00004f70: 772e 7079 696e 7374 616c 6c65 722e 6f72  w.pyinstaller.or
 00004f80: 6729 292e 0a94 6807 5d94 2868 5029 8194  g))...h.].(hP)..
 00004f90: 7d94 2868 0558 7401 0000 5769 6e64 6f77  }.(h.Xt...Window
 00004fa0: 732c 204c 696e 7578 3a20 476f 2074 6f20  s, Linux: Go to 
 00004fb0: 5b67 6974 6875 622e 636f 6d2f 6a6b 616e  [github.com/jkan
 00004fc0: 6576 2f74 7265 6574 696d 652f 7265 6c65  ev/treetime/rele
-00004fd0: 6173 6573 2f74 6167 2f32 3032 342e 315d  ases/tag/2024.1]
+00004fd0: 6173 6573 2f74 6167 2f32 3032 342e 325d  ases/tag/2024.2]
 00004fe0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
 00004ff0: 636f 6d2f 6a6b 616e 6576 2f74 7265 6574  com/jkanev/treet
 00005000: 696d 652f 7265 6c65 6173 6573 2f74 6167  ime/releases/tag
-00005010: 2f32 3032 342e 3129 2061 6e64 2064 6f77  /2024.1) and dow
+00005010: 2f32 3032 342e 3229 2061 6e64 2064 6f77  /2024.2) and dow
 00005020: 6e6c 6f61 6420 6120 7a69 7070 6564 2070  nload a zipped p
 00005030: 6163 6b61 6765 2066 6f72 2057 696e 646f  ackage for Windo
 00005040: 7773 2031 302c 2036 3420 6269 742c 206f  ws 10, 64 bit, o
 00005050: 7220 666f 7220 4c69 6e75 7820 3634 2062  r for Linux 64 b
 00005060: 6974 2066 726f 6d20 7468 6572 652e 2055  it from there. U
 00005070: 6e7a 6970 2069 7420 696e 746f 2079 6f75  nzip it into you
 00005080: 7220 7072 6f67 7261 6d20 6469 7265 6374  r program direct
@@ -1295,26 +1295,26 @@
 000050e0: 6b61 6765 2074 6f6f 2e20 4164 6420 7468  kage too. Add th
 000050f0: 6520 7072 6f67 7261 6d20 666f 6c64 6572  e program folder
 00005100: 2074 6f20 796f 7572 2070 6174 682e 9468   to your path..h
 00005110: 075d 9428 6816 8c47 5769 6e64 6f77 732c  .].(h..GWindows,
 00005120: 204c 696e 7578 3a20 476f 2074 6f20 5b67   Linux: Go to [g
 00005130: 6974 6875 622e 636f 6d2f 6a6b 616e 6576  ithub.com/jkanev
 00005140: 2f74 7265 6574 696d 652f 7265 6c65 6173  /treetime/releas
-00005150: 6573 2f74 6167 2f32 3032 342e 315d 2894  es/tag/2024.1](.
+00005150: 6573 2f74 6167 2f32 3032 342e 325d 2894  es/tag/2024.2](.
 00005160: 8594 8194 7d94 2868 1b6a 4404 0000 681c  ....}.(h.jD...h.
 00005170: 6803 681d 4e68 1e4e 7562 6809 8c09 7265  h.h.Nh.Nubh...re
 00005180: 6665 7265 6e63 6594 9394 2981 947d 9428  ference...)..}.(
 00005190: 6805 8c36 6874 7470 733a 2f2f 6769 7468  h..6https://gith
 000051a0: 7562 2e63 6f6d 2f6a 6b61 6e65 762f 7472  ub.com/jkanev/tr
 000051b0: 6565 7469 6d65 2f72 656c 6561 7365 732f  eetime/releases/
-000051c0: 7461 672f 3230 3234 2e31 9468 075d 9468  tag/2024.1.h.].h
+000051c0: 7461 672f 3230 3234 2e32 9468 075d 9468  tag/2024.2.h.].h
 000051d0: 168c 3668 7474 7073 3a2f 2f67 6974 6875  ..6https://githu
 000051e0: 622e 636f 6d2f 6a6b 616e 6576 2f74 7265  b.com/jkanev/tre
 000051f0: 6574 696d 652f 7265 6c65 6173 6573 2f74  etime/releases/t
-00005200: 6167 2f32 3032 342e 3194 8594 8194 7d94  ag/2024.1.....}.
+00005200: 6167 2f32 3032 342e 3294 8594 8194 7d94  ag/2024.2.....}.
 00005210: 2868 1b6a 4e04 0000 681c 6803 681d 4e68  (h.jN...h.h.h.Nh
 00005220: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
 00005230: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
 00005240: 7265 6675 7269 946a 5004 0000 7568 2b6a  refuri.jP...uh+j
 00005250: 4c04 0000 681b 6a44 0400 0075 6268 168c  L...h.jD...ubh..
 00005260: 8529 2061 6e64 2064 6f77 6e6c 6f61 6420  .) and download 
 00005270: 6120 7a69 7070 6564 2070 6163 6b61 6765  a zipped package
```

### Comparing `TreeTime-2024.1/docs/_build/doctrees/releases.doctree` & `TreeTime-2024.2/docs/_build/doctrees/releases.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9550 7f00 0000 0000 008c 0f73 7068  ...P.........sph
+00000000: 8005 95e9 8200 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -1479,560 +1479,618 @@
 00005c60: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
 00005c70: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
 00005c80: 295d 9475 682b 685a 681d 682c 681e 4b6a  )].uh+hZh.h,h.Kj
 00005c90: 681b 6abe 0700 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
 00005ca0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
 00005cb0: 295d 9475 682b 6854 681b 6a8d 0700 0068  )].uh+hTh.j....h
 00005cc0: 1c68 0368 1d68 2c68 1e4e 7562 6855 2981  .h.h.h,h.NubhU).
-00005cd0: 947d 9428 6805 8c51 4170 7269 6c20 3230  .}.(h..QApril 20
+00005cd0: 947d 9428 6805 8c50 4170 7269 6c20 3230  .}.(h..PApril 20
 00005ce0: 3234 3a20 4578 7465 6e64 6564 2064 6f63  24: Extended doc
 00005cf0: 756d 656e 7461 7469 6f6e 206f 6e20 7265  umentation on re
 00005d00: 6164 7468 6564 6f63 732e 696f 2e20 5265  adthedocs.io. Re
 00005d10: 6c65 6173 6520 2a2a 7665 7273 696f 6e20  lease **version 
-00005d20: 3230 3234 2e31 2a2a 0a94 6807 5d94 685b  2024.1**..h.].h[
-00005d30: 2981 947d 9428 6805 8c50 4170 7269 6c20  )..}.(h..PApril 
-00005d40: 3230 3234 3a20 4578 7465 6e64 6564 2064  2024: Extended d
-00005d50: 6f63 756d 656e 7461 7469 6f6e 206f 6e20  ocumentation on 
-00005d60: 7265 6164 7468 6564 6f63 732e 696f 2e20  readthedocs.io. 
-00005d70: 5265 6c65 6173 6520 2a2a 7665 7273 696f  Release **versio
-00005d80: 6e20 3230 3234 2e31 2a2a 9468 075d 9428  n 2024.1**.h.].(
-00005d90: 6816 8c3e 4170 7269 6c20 3230 3234 3a20  h..>April 2024: 
-00005da0: 4578 7465 6e64 6564 2064 6f63 756d 656e  Extended documen
-00005db0: 7461 7469 6f6e 206f 6e20 7265 6164 7468  tation on readth
-00005dc0: 6564 6f63 732e 696f 2e20 5265 6c65 6173  edocs.io. Releas
-00005dd0: 6520 9485 9481 947d 9428 681b 6ad9 0700  e .....}.(h.j...
-00005de0: 0068 1c68 0368 1d4e 681e 4e75 626a 4601  .h.h.h.Nh.NubjF.
-00005df0: 0000 2981 947d 9428 6805 8c12 2a2a 7665  ..)..}.(h...**ve
-00005e00: 7273 696f 6e20 3230 3234 2e31 2a2a 9468  rsion 2024.1**.h
-00005e10: 075d 9468 168c 0e76 6572 7369 6f6e 2032  .].h...version 2
-00005e20: 3032 342e 3194 8594 8194 7d94 2868 1b6a  024.1.....}.(h.j
-00005e30: e107 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00005e40: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00005e50: 5d94 6827 5d94 6829 5d94 7568 2b6a 4501  ].h'].h)].uh+jE.
-00005e60: 0000 681b 6ad9 0700 0075 6265 681f 7d94  ..h.j....ubeh.}.
-00005e70: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00005e80: 9468 295d 9475 682b 685a 681d 682c 681e  .h)].uh+hZh.h,h.
-00005e90: 4b6b 681b 6ad5 0700 0075 6261 681f 7d94  Kkh.j....ubah.}.
-00005ea0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00005eb0: 9468 295d 9475 682b 6854 681b 6a8d 0700  .h)].uh+hTh.j...
-00005ec0: 0068 1c68 0368 1d68 2c68 1e4e 7562 6568  .h.h.h.h,h.Nubeh
-00005ed0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00005ee0: 6827 5d94 6829 5d94 6876 6877 7568 2b68  h'].h)].hvhwuh+h
-00005ef0: 4f68 1d68 2c68 1e4b 6868 1b6a 7c07 0000  Oh.h,h.Khh.j|...
-00005f00: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00005f10: 8c04 6964 3130 9461 6823 5d94 6825 5d94  ..id10.ah#].h%].
-00005f20: 8c04 3230 3234 9461 6827 5d94 6829 5d94  ..2024.ah'].h)].
-00005f30: 7568 2b68 0a68 1b68 0c68 1c68 0368 1d68  uh+h.h.h.h.h.h.h
-00005f40: 2c68 1e4b 6675 6268 0b29 8194 7d94 2868  ,h.Kfubh.)..}.(h
-00005f50: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-00005f60: 6805 8c07 5072 6573 656e 7494 6807 5d94  h...Present.h.].
-00005f70: 6816 8c07 5072 6573 656e 7494 8594 8194  h...Present.....
-00005f80: 7d94 2868 1b6a 0c08 0000 681c 6803 681d  }.(h.j....h.h.h.
-00005f90: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00005fa0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00005fb0: 7568 2b68 0f68 1b6a 0908 0000 681c 6803  uh+h.h.j....h.h.
-00005fc0: 681d 682c 681e 4b6e 7562 6850 2981 947d  h.h,h.KnubhP)..}
-00005fd0: 9428 6805 6806 6807 5d94 2868 5529 8194  .(h.h.h.].(hU)..
-00005fe0: 7d94 2868 058c 0942 7567 6669 7869 6e67  }.(h...Bugfixing
-00005ff0: 9468 075d 9468 5b29 8194 7d94 2868 056a  .h.].h[)..}.(h.j
-00006000: 1f08 0000 6807 5d94 6816 8c09 4275 6766  ....h.].h...Bugf
-00006010: 6978 696e 6794 8594 8194 7d94 2868 1b6a  ixing.....}.(h.j
-00006020: 2108 0000 681c 6803 681d 4e68 1e4e 7562  !...h.h.h.Nh.Nub
-00006030: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00006040: 5d94 6827 5d94 6829 5d94 7568 2b68 5a68  ].h'].h)].uh+hZh
-00006050: 1d68 2c68 1e4b 7068 1b6a 1d08 0000 7562  .h,h.Kph.j....ub
-00006060: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00006070: 5d94 6827 5d94 6829 5d94 7568 2b68 5468  ].h'].h)].uh+hTh
-00006080: 1b6a 1a08 0000 681c 6803 681d 682c 681e  .j....h.h.h.h,h.
-00006090: 4e75 6268 5529 8194 7d94 2868 058c 2645  NubhU)..}.(h..&E
-000060a0: 7874 656e 6420 646f 6375 6d65 6e74 6174  xtend documentat
-000060b0: 696f 6e20 6f6e 2072 6561 6474 6865 646f  ion on readthedo
-000060c0: 6373 2e69 6f94 6807 5d94 685b 2981 947d  cs.io.h.].h[)..}
-000060d0: 9428 6805 6a36 0800 0068 075d 9468 168c  .(h.j6...h.].h..
-000060e0: 2645 7874 656e 6420 646f 6375 6d65 6e74  &Extend document
-000060f0: 6174 696f 6e20 6f6e 2072 6561 6474 6865  ation on readthe
-00006100: 646f 6373 2e69 6f94 8594 8194 7d94 2868  docs.io.....}.(h
-00006110: 1b6a 3808 0000 681c 6803 681d 4e68 1e4e  .j8...h.h.h.Nh.N
-00006120: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00006130: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00006140: 5a68 1d68 2c68 1e4b 7168 1b6a 3408 0000  Zh.h,h.Kqh.j4...
-00006150: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00006160: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00006170: 5468 1b6a 1a08 0000 681c 6803 681d 682c  Th.j....h.h.h.h,
-00006180: 681e 4e75 6268 5529 8194 7d94 2868 058c  h.NubhU)..}.(h..
-00006190: 0f41 6464 206d 6f72 6520 6669 656c 6473  .Add more fields
-000061a0: 9468 075d 9468 5b29 8194 7d94 2868 056a  .h.].h[)..}.(h.j
-000061b0: 4d08 0000 6807 5d94 6816 8c0f 4164 6420  M...h.].h...Add 
-000061c0: 6d6f 7265 2066 6965 6c64 7394 8594 8194  more fields.....
-000061d0: 7d94 2868 1b6a 4f08 0000 681c 6803 681d  }.(h.jO...h.h.h.
-000061e0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000061f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00006200: 7568 2b68 5a68 1d68 2c68 1e4b 7268 1b6a  uh+hZh.h,h.Krh.j
-00006210: 4b08 0000 7562 6168 1f7d 9428 6821 5d94  K...ubah.}.(h!].
-00006220: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00006230: 7568 2b68 5468 1b6a 1a08 0000 681c 6803  uh+hTh.j....h.h.
-00006240: 681d 682c 681e 4e75 6268 5529 8194 7d94  h.h,h.NubhU)..}.
-00006250: 2868 058c 2e41 6464 206d 6f72 6520 6578  (h...Add more ex
-00006260: 616d 706c 6573 2061 6e64 206d 6f72 6520  amples and more 
-00006270: 7465 6d70 6c61 7465 2064 6174 6120 6669  template data fi
-00006280: 6c65 7394 6807 5d94 685b 2981 947d 9428  les.h.].h[)..}.(
-00006290: 6805 6a64 0800 0068 075d 9468 168c 2e41  h.jd...h.].h...A
-000062a0: 6464 206d 6f72 6520 6578 616d 706c 6573  dd more examples
-000062b0: 2061 6e64 206d 6f72 6520 7465 6d70 6c61   and more templa
-000062c0: 7465 2064 6174 6120 6669 6c65 7394 8594  te data files...
-000062d0: 8194 7d94 2868 1b6a 6608 0000 681c 6803  ..}.(h.jf...h.h.
-000062e0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-000062f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00006300: 5d94 7568 2b68 5a68 1d68 2c68 1e4b 7368  ].uh+hZh.h,h.Ksh
-00006310: 1b6a 6208 0000 7562 6168 1f7d 9428 6821  .jb...ubah.}.(h!
-00006320: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00006330: 5d94 7568 2b68 5468 1b6a 1a08 0000 681c  ].uh+hTh.j....h.
-00006340: 6803 681d 682c 681e 4e75 6268 5529 8194  h.h.h,h.NubhU)..
-00006350: 7d94 2868 058c 5449 6d70 6c65 6d65 6e74  }.(h..TImplement
-00006360: 2074 7265 6520 6669 656c 6420 6564 6974   tree field edit
-00006370: 696e 6720 7769 7468 2067 7261 7068 6963  ing with graphic
-00006380: 616c 2064 6961 6c6f 6720 2861 6464 2c20  al dialog (add, 
-00006390: 7265 6d6f 7665 2c20 6368 616e 6765 2074  remove, change t
-000063a0: 7265 6520 6669 656c 6473 2994 6807 5d94  ree fields).h.].
-000063b0: 685b 2981 947d 9428 6805 6a7b 0800 0068  h[)..}.(h.j{...h
-000063c0: 075d 9468 168c 5449 6d70 6c65 6d65 6e74  .].h..TImplement
-000063d0: 2074 7265 6520 6669 656c 6420 6564 6974   tree field edit
-000063e0: 696e 6720 7769 7468 2067 7261 7068 6963  ing with graphic
-000063f0: 616c 2064 6961 6c6f 6720 2861 6464 2c20  al dialog (add, 
-00006400: 7265 6d6f 7665 2c20 6368 616e 6765 2074  remove, change t
-00006410: 7265 6520 6669 656c 6473 2994 8594 8194  ree fields).....
-00006420: 7d94 2868 1b6a 7d08 0000 681c 6803 681d  }.(h.j}...h.h.h.
-00006430: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00006440: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00006450: 7568 2b68 5a68 1d68 2c68 1e4b 7468 1b6a  uh+hZh.h,h.Kth.j
-00006460: 7908 0000 7562 6168 1f7d 9428 6821 5d94  y...ubah.}.(h!].
-00006470: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00006480: 7568 2b68 5468 1b6a 1a08 0000 681c 6803  uh+hTh.j....h.h.
-00006490: 681d 682c 681e 4e75 6268 5529 8194 7d94  h.h,h.NubhU)..}.
-000064a0: 2868 058c 5f49 6d70 6c65 6d65 6e74 2064  (h.._Implement d
-000064b0: 6174 6120 6974 656d 2066 6965 6c64 2065  ata item field e
-000064c0: 6469 7469 6e67 2077 6974 6820 6772 6170  diting with grap
-000064d0: 6869 6361 6c20 6469 616c 6f67 2028 6164  hical dialog (ad
-000064e0: 642c 2072 656d 6f76 652c 2063 6861 6e67  d, remove, chang
-000064f0: 6520 6461 7461 2069 7465 6d20 6669 656c  e data item fiel
-00006500: 6473 290a 9468 075d 9468 5b29 8194 7d94  ds)..h.].h[)..}.
-00006510: 2868 058c 5e49 6d70 6c65 6d65 6e74 2064  (h..^Implement d
-00006520: 6174 6120 6974 656d 2066 6965 6c64 2065  ata item field e
-00006530: 6469 7469 6e67 2077 6974 6820 6772 6170  diting with grap
-00006540: 6869 6361 6c20 6469 616c 6f67 2028 6164  hical dialog (ad
-00006550: 642c 2072 656d 6f76 652c 2063 6861 6e67  d, remove, chang
-00006560: 6520 6461 7461 2069 7465 6d20 6669 656c  e data item fiel
-00006570: 6473 2994 6807 5d94 6816 8c5e 496d 706c  ds).h.].h..^Impl
-00006580: 656d 656e 7420 6461 7461 2069 7465 6d20  ement data item 
-00006590: 6669 656c 6420 6564 6974 696e 6720 7769  field editing wi
-000065a0: 7468 2067 7261 7068 6963 616c 2064 6961  th graphical dia
-000065b0: 6c6f 6720 2861 6464 2c20 7265 6d6f 7665  log (add, remove
-000065c0: 2c20 6368 616e 6765 2064 6174 6120 6974  , change data it
-000065d0: 656d 2066 6965 6c64 7329 9485 9481 947d  em fields).....}
-000065e0: 9428 681b 6a94 0800 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-000065f0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00006600: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00006610: 682b 685a 681d 682c 681e 4b75 681b 6a90  h+hZh.h,h.Kuh.j.
-00006620: 0800 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00006630: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00006640: 682b 6854 681b 6a1a 0800 0068 1c68 0368  h+hTh.j....h.h.h
-00006650: 1d68 2c68 1e4e 7562 6568 1f7d 9428 6821  .h,h.Nubeh.}.(h!
-00006660: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00006670: 5d94 6876 6877 7568 2b68 4f68 1d68 2c68  ].hvhwuh+hOh.h,h
-00006680: 1e4b 7068 1b6a 0908 0000 681c 6803 7562  .Kph.j....h.h.ub
-00006690: 6568 1f7d 9428 6821 5d94 8c07 7072 6573  eh.}.(h!]...pres
-000066a0: 656e 7494 6168 235d 9468 255d 948c 0770  ent.ah#].h%]...p
-000066b0: 7265 7365 6e74 9461 6827 5d94 6829 5d94  resent.ah'].h)].
-000066c0: 7568 2b68 0a68 1b68 0c68 1c68 0368 1d68  uh+h.h.h.h.h.h.h
-000066d0: 2c68 1e4b 6e75 6268 0b29 8194 7d94 2868  ,h.Knubh.)..}.(h
-000066e0: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-000066f0: 6805 8c06 4675 7475 7265 9468 075d 9468  h...Future.h.].h
-00006700: 168c 0646 7574 7572 6594 8594 8194 7d94  ...Future.....}.
-00006710: 2868 1b6a b908 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00006720: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00006730: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00006740: 2b68 0f68 1b6a b608 0000 681c 6803 681d  +h.h.j....h.h.h.
-00006750: 682c 681e 4b78 7562 680b 2981 947d 9428  h,h.Kxubh.)..}.(
-00006760: 6805 6806 6807 5d94 2868 1029 8194 7d94  h.h.h.].(h.)..}.
-00006770: 2868 058c 0b4e 6561 7220 4675 7475 7265  (h...Near Future
-00006780: 9468 075d 9468 168c 0b4e 6561 7220 4675  .h.].h...Near Fu
-00006790: 7475 7265 9485 9481 947d 9428 681b 6aca  ture.....}.(h.j.
-000067a0: 0800 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-000067b0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000067c0: 9468 275d 9468 295d 9475 682b 680f 681b  .h'].h)].uh+h.h.
-000067d0: 6ac7 0800 0068 1c68 0368 1d68 2c68 1e4b  j....h.h.h.h,h.K
-000067e0: 7b75 6268 5029 8194 7d94 2868 0568 0668  {ubhP)..}.(h.h.h
-000067f0: 075d 9428 6855 2981 947d 9428 6805 8c19  .].(hU)..}.(h...
-00006800: 496d 706c 656d 656e 7420 7365 6172 6368  Implement search
-00006810: 2066 756e 6374 696f 6e94 6807 5d94 685b   function.h.].h[
-00006820: 2981 947d 9428 6805 6add 0800 0068 075d  )..}.(h.j....h.]
-00006830: 9468 168c 1949 6d70 6c65 6d65 6e74 2073  .h...Implement s
-00006840: 6561 7263 6820 6675 6e63 7469 6f6e 9485  earch function..
-00006850: 9481 947d 9428 681b 6adf 0800 0068 1c68  ...}.(h.j....h.h
-00006860: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00006870: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00006880: 295d 9475 682b 685a 681d 682c 681e 4b7d  )].uh+hZh.h,h.K}
-00006890: 681b 6adb 0800 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
-000068a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000068b0: 295d 9475 682b 6854 681b 6ad8 0800 0068  )].uh+hTh.j....h
-000068c0: 1c68 0368 1d68 2c68 1e4e 7562 6855 2981  .h.h.h,h.NubhU).
-000068d0: 947d 9428 6805 8c9e 496d 706c 656d 656e  .}.(h...Implemen
-000068e0: 7469 6e67 2063 6f6e 7469 6e75 6f75 7320  ting continuous 
-000068f0: 7465 7874 2061 6e64 2068 746d 6c20 6578  text and html ex
-00006900: 706f 7274 2028 746f 2075 7365 2074 7265  port (to use tre
-00006910: 6574 696d 6520 6173 2061 206d 6565 7469  etime as a meeti
-00006920: 6e67 206e 6f74 652d 7461 6b69 6e67 2061  ng note-taking a
-00006930: 7070 2077 6865 7265 2070 6172 7469 6369  pp where partici
-00006940: 7061 6e74 7320 7669 6577 2061 6e20 6175  pants view an au
-00006950: 746f 2d75 7064 6174 696e 6720 6874 6d6c  to-updating html
-00006960: 2066 696c 6520 7769 7468 2074 6865 206e   file with the n
-00006970: 6f74 6573 290a 9468 075d 9468 5b29 8194  otes)..h.].h[)..
-00006980: 7d94 2868 058c 9d49 6d70 6c65 6d65 6e74  }.(h...Implement
-00006990: 696e 6720 636f 6e74 696e 756f 7573 2074  ing continuous t
-000069a0: 6578 7420 616e 6420 6874 6d6c 2065 7870  ext and html exp
-000069b0: 6f72 7420 2874 6f20 7573 6520 7472 6565  ort (to use tree
-000069c0: 7469 6d65 2061 7320 6120 6d65 6574 696e  time as a meetin
-000069d0: 6720 6e6f 7465 2d74 616b 696e 6720 6170  g note-taking ap
-000069e0: 7020 7768 6572 6520 7061 7274 6963 6970  p where particip
-000069f0: 616e 7473 2076 6965 7720 616e 2061 7574  ants view an aut
-00006a00: 6f2d 7570 6461 7469 6e67 2068 746d 6c20  o-updating html 
-00006a10: 6669 6c65 2077 6974 6820 7468 6520 6e6f  file with the no
-00006a20: 7465 7329 9468 075d 9468 168c 9d49 6d70  tes).h.].h...Imp
-00006a30: 6c65 6d65 6e74 696e 6720 636f 6e74 696e  lementing contin
-00006a40: 756f 7573 2074 6578 7420 616e 6420 6874  uous text and ht
-00006a50: 6d6c 2065 7870 6f72 7420 2874 6f20 7573  ml export (to us
-00006a60: 6520 7472 6565 7469 6d65 2061 7320 6120  e treetime as a 
-00006a70: 6d65 6574 696e 6720 6e6f 7465 2d74 616b  meeting note-tak
-00006a80: 696e 6720 6170 7020 7768 6572 6520 7061  ing app where pa
-00006a90: 7274 6963 6970 616e 7473 2076 6965 7720  rticipants view 
-00006aa0: 616e 2061 7574 6f2d 7570 6461 7469 6e67  an auto-updating
-00006ab0: 2068 746d 6c20 6669 6c65 2077 6974 6820   html file with 
-00006ac0: 7468 6520 6e6f 7465 7329 9485 9481 947d  the notes).....}
-00006ad0: 9428 681b 6af6 0800 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00006ae0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00006af0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00006b00: 682b 685a 681d 682c 681e 4b7e 681b 6af2  h+hZh.h,h.K~h.j.
-00006b10: 0800 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00006b20: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00006b30: 682b 6854 681b 6ad8 0800 0068 1c68 0368  h+hTh.j....h.h.h
-00006b40: 1d68 2c68 1e4e 7562 6568 1f7d 9428 6821  .h,h.Nubeh.}.(h!
+00005d20: 3230 3234 2e31 2a2a 9468 075d 9468 5b29  2024.1**.h.].h[)
+00005d30: 8194 7d94 2868 056a d707 0000 6807 5d94  ..}.(h.j....h.].
+00005d40: 2868 168c 3e41 7072 696c 2032 3032 343a  (h..>April 2024:
+00005d50: 2045 7874 656e 6465 6420 646f 6375 6d65   Extended docume
+00005d60: 6e74 6174 696f 6e20 6f6e 2072 6561 6474  ntation on readt
+00005d70: 6865 646f 6373 2e69 6f2e 2052 656c 6561  hedocs.io. Relea
+00005d80: 7365 2094 8594 8194 7d94 2868 1b6a d907  se .....}.(h.j..
+00005d90: 0000 681c 6803 681d 4e68 1e4e 7562 6a46  ..h.h.h.Nh.NubjF
+00005da0: 0100 0029 8194 7d94 2868 058c 122a 2a76  ...)..}.(h...**v
+00005db0: 6572 7369 6f6e 2032 3032 342e 312a 2a94  ersion 2024.1**.
+00005dc0: 6807 5d94 6816 8c0e 7665 7273 696f 6e20  h.].h...version 
+00005dd0: 3230 3234 2e31 9485 9481 947d 9428 681b  2024.1.....}.(h.
+00005de0: 6ae0 0700 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00005df0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00005e00: 255d 9468 275d 9468 295d 9475 682b 6a45  %].h'].h)].uh+jE
+00005e10: 0100 0068 1b6a d907 0000 7562 6568 1f7d  ...h.j....ubeh.}
+00005e20: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005e30: 5d94 6829 5d94 7568 2b68 5a68 1d68 2c68  ].h)].uh+hZh.h,h
+00005e40: 1e4b 6b68 1b6a d507 0000 7562 6168 1f7d  .Kkh.j....ubah.}
+00005e50: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00005e60: 5d94 6829 5d94 7568 2b68 5468 1b6a 8d07  ].h)].uh+hTh.j..
+00005e70: 0000 681c 6803 681d 682c 681e 4e75 6268  ..h.h.h.h,h.Nubh
+00005e80: 5529 8194 7d94 2868 058c df41 7072 696c  U)..}.(h...April
+00005e90: 2032 3032 343a 2052 6573 7472 7563 7475   2024: Restructu
+00005ea0: 7265 6420 6578 706f 7274 2061 7265 612c  red export area,
+00005eb0: 2061 6464 6564 206e 616d 652d 6f6e 6c79   added name-only
+00005ec0: 2065 7870 6f72 742e 204d 6164 6520 616c   export. Made al
+00005ed0: 6c20 6578 706f 7274 206f 7074 696f 6e73  l export options
+00005ee0: 2028 6675 6c6c 2074 7265 6520 2f20 6272   (full tree / br
+00005ef0: 616e 6368 202f 206e 6f64 6520 7769 7468  anch / node with
+00005f00: 2063 6f6e 7465 6374 2920 2861 6c6c 2066   contect) (all f
+00005f10: 6965 6c64 7320 2f20 6e61 6d65 7320 6f6e  ields / names on
+00005f20: 6c79 2920 6176 6169 6c61 626c 6520 666f  ly) available fo
+00005f30: 7220 616c 6c20 6669 6c65 2066 6f72 6d61  r all file forma
+00005f40: 7473 2061 6e64 2066 6f72 2062 6f74 6820  ts and for both 
+00005f50: 6669 6c65 2061 6e64 2063 6c69 7062 6f61  file and clipboa
+00005f60: 7264 2065 7870 6f72 742e 9468 075d 9468  rd export..h.].h
+00005f70: 5b29 8194 7d94 2868 056a fc07 0000 6807  [)..}.(h.j....h.
+00005f80: 5d94 6816 8cdf 4170 7269 6c20 3230 3234  ].h...April 2024
+00005f90: 3a20 5265 7374 7275 6374 7572 6564 2065  : Restructured e
+00005fa0: 7870 6f72 7420 6172 6561 2c20 6164 6465  xport area, adde
+00005fb0: 6420 6e61 6d65 2d6f 6e6c 7920 6578 706f  d name-only expo
+00005fc0: 7274 2e20 4d61 6465 2061 6c6c 2065 7870  rt. Made all exp
+00005fd0: 6f72 7420 6f70 7469 6f6e 7320 2866 756c  ort options (ful
+00005fe0: 6c20 7472 6565 202f 2062 7261 6e63 6820  l tree / branch 
+00005ff0: 2f20 6e6f 6465 2077 6974 6820 636f 6e74  / node with cont
+00006000: 6563 7429 2028 616c 6c20 6669 656c 6473  ect) (all fields
+00006010: 202f 206e 616d 6573 206f 6e6c 7929 2061   / names only) a
+00006020: 7661 696c 6162 6c65 2066 6f72 2061 6c6c  vailable for all
+00006030: 2066 696c 6520 666f 726d 6174 7320 616e   file formats an
+00006040: 6420 666f 7220 626f 7468 2066 696c 6520  d for both file 
+00006050: 616e 6420 636c 6970 626f 6172 6420 6578  and clipboard ex
+00006060: 706f 7274 2e94 8594 8194 7d94 2868 1b6a  port......}.(h.j
+00006070: fe07 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00006080: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00006090: 5d94 6827 5d94 6829 5d94 7568 2b68 5a68  ].h'].h)].uh+hZh
+000060a0: 1d68 2c68 1e4b 6c68 1b6a fa07 0000 7562  .h,h.Klh.j....ub
+000060b0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000060c0: 5d94 6827 5d94 6829 5d94 7568 2b68 5468  ].h'].h)].uh+hTh
+000060d0: 1b6a 8d07 0000 681c 6803 681d 682c 681e  .j....h.h.h.h,h.
+000060e0: 4e75 6268 5529 8194 7d94 2868 058c 2741  NubhU)..}.(h..'A
+000060f0: 7072 696c 2032 3032 343a 2052 656c 6561  pril 2024: Relea
+00006100: 7365 202a 2a76 6572 7369 6f6e 2032 3032  se **version 202
+00006110: 342e 322a 2a0a 9468 075d 9468 5b29 8194  4.2**..h.].h[)..
+00006120: 7d94 2868 058c 2641 7072 696c 2032 3032  }.(h..&April 202
+00006130: 343a 2052 656c 6561 7365 202a 2a76 6572  4: Release **ver
+00006140: 7369 6f6e 2032 3032 342e 322a 2a94 6807  sion 2024.2**.h.
+00006150: 5d94 2868 168c 1441 7072 696c 2032 3032  ].(h...April 202
+00006160: 343a 2052 656c 6561 7365 2094 8594 8194  4: Release .....
+00006170: 7d94 2868 1b6a 1508 0000 681c 6803 681d  }.(h.j....h.h.h.
+00006180: 4e68 1e4e 7562 6a46 0100 0029 8194 7d94  Nh.NubjF...)..}.
+00006190: 2868 058c 122a 2a76 6572 7369 6f6e 2032  (h...**version 2
+000061a0: 3032 342e 322a 2a94 6807 5d94 6816 8c0e  024.2**.h.].h...
+000061b0: 7665 7273 696f 6e20 3230 3234 2e32 9485  version 2024.2..
+000061c0: 9481 947d 9428 681b 6a1d 0800 0068 1c68  ...}.(h.j....h.h
+000061d0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000061e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000061f0: 295d 9475 682b 6a45 0100 0068 1b6a 1508  )].uh+jE...h.j..
+00006200: 0000 7562 6568 1f7d 9428 6821 5d94 6823  ..ubeh.}.(h!].h#
+00006210: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00006220: 2b68 5a68 1d68 2c68 1e4b 6d68 1b6a 1108  +hZh.h,h.Kmh.j..
+00006230: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00006240: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00006250: 2b68 5468 1b6a 8d07 0000 681c 6803 681d  +hTh.j....h.h.h.
+00006260: 682c 681e 4e75 6265 681f 7d94 2868 215d  h,h.Nubeh.}.(h!]
+00006270: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00006280: 9468 7668 7775 682b 684f 681d 682c 681e  .hvhwuh+hOh.h,h.
+00006290: 4b68 681b 6a7c 0700 0068 1c68 0375 6265  Khh.j|...h.h.ube
+000062a0: 681f 7d94 2868 215d 948c 0469 6431 3094  h.}.(h!]...id10.
+000062b0: 6168 235d 9468 255d 948c 0432 3032 3494  ah#].h%]...2024.
+000062c0: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
+000062d0: 680c 681c 6803 681d 682c 681e 4b66 7562  h.h.h.h.h,h.Kfub
+000062e0: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+000062f0: 2868 1029 8194 7d94 2868 058c 0750 7265  (h.)..}.(h...Pre
+00006300: 7365 6e74 9468 075d 9468 168c 0750 7265  sent.h.].h...Pre
+00006310: 7365 6e74 9485 9481 947d 9428 681b 6a48  sent.....}.(h.jH
+00006320: 0800 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00006330: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00006340: 9468 275d 9468 295d 9475 682b 680f 681b  .h'].h)].uh+h.h.
+00006350: 6a45 0800 0068 1c68 0368 1d68 2c68 1e4b  jE...h.h.h.h,h.K
+00006360: 7075 6268 5029 8194 7d94 2868 0568 0668  pubhP)..}.(h.h.h
+00006370: 075d 9428 6855 2981 947d 9428 6805 8c09  .].(hU)..}.(h...
+00006380: 4275 6766 6978 696e 6794 6807 5d94 685b  Bugfixing.h.].h[
+00006390: 2981 947d 9428 6805 6a5b 0800 0068 075d  )..}.(h.j[...h.]
+000063a0: 9468 168c 0942 7567 6669 7869 6e67 9485  .h...Bugfixing..
+000063b0: 9481 947d 9428 681b 6a5d 0800 0068 1c68  ...}.(h.j]...h.h
+000063c0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000063d0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000063e0: 295d 9475 682b 685a 681d 682c 681e 4b72  )].uh+hZh.h,h.Kr
+000063f0: 681b 6a59 0800 0075 6261 681f 7d94 2868  h.jY...ubah.}.(h
+00006400: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00006410: 295d 9475 682b 6854 681b 6a56 0800 0068  )].uh+hTh.jV...h
+00006420: 1c68 0368 1d68 2c68 1e4e 7562 6855 2981  .h.h.h,h.NubhU).
+00006430: 947d 9428 6805 8c26 4578 7465 6e64 2064  .}.(h..&Extend d
+00006440: 6f63 756d 656e 7461 7469 6f6e 206f 6e20  ocumentation on 
+00006450: 7265 6164 7468 6564 6f63 732e 696f 9468  readthedocs.io.h
+00006460: 075d 9468 5b29 8194 7d94 2868 056a 7208  .].h[)..}.(h.jr.
+00006470: 0000 6807 5d94 6816 8c26 4578 7465 6e64  ..h.].h..&Extend
+00006480: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
+00006490: 6e20 7265 6164 7468 6564 6f63 732e 696f  n readthedocs.io
+000064a0: 9485 9481 947d 9428 681b 6a74 0800 0068  .....}.(h.jt...h
+000064b0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000064c0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000064d0: 9468 295d 9475 682b 685a 681d 682c 681e  .h)].uh+hZh.h,h.
+000064e0: 4b73 681b 6a70 0800 0075 6261 681f 7d94  Ksh.jp...ubah.}.
+000064f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00006500: 9468 295d 9475 682b 6854 681b 6a56 0800  .h)].uh+hTh.jV..
+00006510: 0068 1c68 0368 1d68 2c68 1e4e 7562 6855  .h.h.h.h,h.NubhU
+00006520: 2981 947d 9428 6805 8c0f 4164 6420 6d6f  )..}.(h...Add mo
+00006530: 7265 2066 6965 6c64 7394 6807 5d94 685b  re fields.h.].h[
+00006540: 2981 947d 9428 6805 6a89 0800 0068 075d  )..}.(h.j....h.]
+00006550: 9468 168c 0f41 6464 206d 6f72 6520 6669  .h...Add more fi
+00006560: 656c 6473 9485 9481 947d 9428 681b 6a8b  elds.....}.(h.j.
+00006570: 0800 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00006580: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00006590: 9468 275d 9468 295d 9475 682b 685a 681d  .h'].h)].uh+hZh.
+000065a0: 682c 681e 4b74 681b 6a87 0800 0075 6261  h,h.Kth.j....uba
+000065b0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000065c0: 9468 275d 9468 295d 9475 682b 6854 681b  .h'].h)].uh+hTh.
+000065d0: 6a56 0800 0068 1c68 0368 1d68 2c68 1e4e  jV...h.h.h.h,h.N
+000065e0: 7562 6855 2981 947d 9428 6805 8c2e 4164  ubhU)..}.(h...Ad
+000065f0: 6420 6d6f 7265 2065 7861 6d70 6c65 7320  d more examples 
+00006600: 616e 6420 6d6f 7265 2074 656d 706c 6174  and more templat
+00006610: 6520 6461 7461 2066 696c 6573 9468 075d  e data files.h.]
+00006620: 9468 5b29 8194 7d94 2868 056a a008 0000  .h[)..}.(h.j....
+00006630: 6807 5d94 6816 8c2e 4164 6420 6d6f 7265  h.].h...Add more
+00006640: 2065 7861 6d70 6c65 7320 616e 6420 6d6f   examples and mo
+00006650: 7265 2074 656d 706c 6174 6520 6461 7461  re template data
+00006660: 2066 696c 6573 9485 9481 947d 9428 681b   files.....}.(h.
+00006670: 6aa2 0800 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00006680: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00006690: 255d 9468 275d 9468 295d 9475 682b 685a  %].h'].h)].uh+hZ
+000066a0: 681d 682c 681e 4b75 681b 6a9e 0800 0075  h.h,h.Kuh.j....u
+000066b0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000066c0: 255d 9468 275d 9468 295d 9475 682b 6854  %].h'].h)].uh+hT
+000066d0: 681b 6a56 0800 0068 1c68 0368 1d68 2c68  h.jV...h.h.h.h,h
+000066e0: 1e4e 7562 6855 2981 947d 9428 6805 8c54  .NubhU)..}.(h..T
+000066f0: 496d 706c 656d 656e 7420 7472 6565 2066  Implement tree f
+00006700: 6965 6c64 2065 6469 7469 6e67 2077 6974  ield editing wit
+00006710: 6820 6772 6170 6869 6361 6c20 6469 616c  h graphical dial
+00006720: 6f67 2028 6164 642c 2072 656d 6f76 652c  og (add, remove,
+00006730: 2063 6861 6e67 6520 7472 6565 2066 6965   change tree fie
+00006740: 6c64 7329 9468 075d 9468 5b29 8194 7d94  lds).h.].h[)..}.
+00006750: 2868 056a b708 0000 6807 5d94 6816 8c54  (h.j....h.].h..T
+00006760: 496d 706c 656d 656e 7420 7472 6565 2066  Implement tree f
+00006770: 6965 6c64 2065 6469 7469 6e67 2077 6974  ield editing wit
+00006780: 6820 6772 6170 6869 6361 6c20 6469 616c  h graphical dial
+00006790: 6f67 2028 6164 642c 2072 656d 6f76 652c  og (add, remove,
+000067a0: 2063 6861 6e67 6520 7472 6565 2066 6965   change tree fie
+000067b0: 6c64 7329 9485 9481 947d 9428 681b 6ab9  lds).....}.(h.j.
+000067c0: 0800 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+000067d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000067e0: 9468 275d 9468 295d 9475 682b 685a 681d  .h'].h)].uh+hZh.
+000067f0: 682c 681e 4b76 681b 6ab5 0800 0075 6261  h,h.Kvh.j....uba
+00006800: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00006810: 9468 275d 9468 295d 9475 682b 6854 681b  .h'].h)].uh+hTh.
+00006820: 6a56 0800 0068 1c68 0368 1d68 2c68 1e4e  jV...h.h.h.h,h.N
+00006830: 7562 6855 2981 947d 9428 6805 8c5f 496d  ubhU)..}.(h.._Im
+00006840: 706c 656d 656e 7420 6461 7461 2069 7465  plement data ite
+00006850: 6d20 6669 656c 6420 6564 6974 696e 6720  m field editing 
+00006860: 7769 7468 2067 7261 7068 6963 616c 2064  with graphical d
+00006870: 6961 6c6f 6720 2861 6464 2c20 7265 6d6f  ialog (add, remo
+00006880: 7665 2c20 6368 616e 6765 2064 6174 6120  ve, change data 
+00006890: 6974 656d 2066 6965 6c64 7329 0a94 6807  item fields)..h.
+000068a0: 5d94 685b 2981 947d 9428 6805 8c5e 496d  ].h[)..}.(h..^Im
+000068b0: 706c 656d 656e 7420 6461 7461 2069 7465  plement data ite
+000068c0: 6d20 6669 656c 6420 6564 6974 696e 6720  m field editing 
+000068d0: 7769 7468 2067 7261 7068 6963 616c 2064  with graphical d
+000068e0: 6961 6c6f 6720 2861 6464 2c20 7265 6d6f  ialog (add, remo
+000068f0: 7665 2c20 6368 616e 6765 2064 6174 6120  ve, change data 
+00006900: 6974 656d 2066 6965 6c64 7329 9468 075d  item fields).h.]
+00006910: 9468 168c 5e49 6d70 6c65 6d65 6e74 2064  .h..^Implement d
+00006920: 6174 6120 6974 656d 2066 6965 6c64 2065  ata item field e
+00006930: 6469 7469 6e67 2077 6974 6820 6772 6170  diting with grap
+00006940: 6869 6361 6c20 6469 616c 6f67 2028 6164  hical dialog (ad
+00006950: 642c 2072 656d 6f76 652c 2063 6861 6e67  d, remove, chang
+00006960: 6520 6461 7461 2069 7465 6d20 6669 656c  e data item fiel
+00006970: 6473 2994 8594 8194 7d94 2868 1b6a d008  ds).....}.(h.j..
+00006980: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00006990: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000069a0: 6827 5d94 6829 5d94 7568 2b68 5a68 1d68  h'].h)].uh+hZh.h
+000069b0: 2c68 1e4b 7768 1b6a cc08 0000 7562 6168  ,h.Kwh.j....ubah
+000069c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000069d0: 6827 5d94 6829 5d94 7568 2b68 5468 1b6a  h'].h)].uh+hTh.j
+000069e0: 5608 0000 681c 6803 681d 682c 681e 4e75  V...h.h.h.h,h.Nu
+000069f0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00006a00: 255d 9468 275d 9468 295d 9468 7668 7775  %].h'].h)].hvhwu
+00006a10: 682b 684f 681d 682c 681e 4b72 681b 6a45  h+hOh.h,h.Krh.jE
+00006a20: 0800 0068 1c68 0375 6265 681f 7d94 2868  ...h.h.ubeh.}.(h
+00006a30: 215d 948c 0770 7265 7365 6e74 9461 6823  !]...present.ah#
+00006a40: 5d94 6825 5d94 8c07 7072 6573 656e 7494  ].h%]...present.
+00006a50: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
+00006a60: 680c 681c 6803 681d 682c 681e 4b70 7562  h.h.h.h.h,h.Kpub
+00006a70: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+00006a80: 2868 1029 8194 7d94 2868 058c 0646 7574  (h.)..}.(h...Fut
+00006a90: 7572 6594 6807 5d94 6816 8c06 4675 7475  ure.h.].h...Futu
+00006aa0: 7265 9485 9481 947d 9428 681b 6af5 0800  re.....}.(h.j...
+00006ab0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00006ac0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00006ad0: 275d 9468 295d 9475 682b 680f 681b 6af2  '].h)].uh+h.h.j.
+00006ae0: 0800 0068 1c68 0368 1d68 2c68 1e4b 7a75  ...h.h.h.h,h.Kzu
+00006af0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
+00006b00: 9428 6810 2981 947d 9428 6805 8c0b 4e65  .(h.)..}.(h...Ne
+00006b10: 6172 2046 7574 7572 6594 6807 5d94 6816  ar Future.h.].h.
+00006b20: 8c0b 4e65 6172 2046 7574 7572 6594 8594  ..Near Future...
+00006b30: 8194 7d94 2868 1b6a 0609 0000 681c 6803  ..}.(h.j....h.h.
+00006b40: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
 00006b50: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00006b60: 5d94 6876 6877 7568 2b68 4f68 1d68 2c68  ].hvhwuh+hOh.h,h
-00006b70: 1e4b 7d68 1b6a c708 0000 681c 6803 7562  .K}h.j....h.h.ub
-00006b80: 6568 1f7d 9428 6821 5d94 8c0b 6e65 6172  eh.}.(h!]...near
-00006b90: 2d66 7574 7572 6594 6168 235d 9468 255d  -future.ah#].h%]
-00006ba0: 948c 0b6e 6561 7220 6675 7475 7265 9461  ...near future.a
-00006bb0: 6827 5d94 6829 5d94 7568 2b68 0a68 1b6a  h'].h)].uh+h.h.j
-00006bc0: b608 0000 681c 6803 681d 682c 681e 4b7b  ....h.h.h.h,h.K{
-00006bd0: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-00006be0: 5d94 2868 1029 8194 7d94 2868 058c 0a4d  ].(h.)..}.(h...M
-00006bf0: 6964 2046 7574 7572 6594 6807 5d94 6816  id Future.h.].h.
-00006c00: 8c0a 4d69 6420 4675 7475 7265 9485 9481  ..Mid Future....
-00006c10: 947d 9428 681b 6a1b 0900 0068 1c68 0368  .}.(h.j....h.h.h
-00006c20: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00006c30: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00006c40: 9475 682b 680f 681b 6a18 0900 0068 1c68  .uh+h.h.j....h.h
-00006c50: 0368 1d68 2c68 1e4b 8175 6268 5029 8194  .h.h,h.K.ubhP)..
-00006c60: 7d94 2868 0568 0668 075d 9428 6855 2981  }.(h.h.h.].(hU).
-00006c70: 947d 9428 6805 8c48 496d 706c 656d 656e  .}.(h..HImplemen
-00006c80: 7420 6772 6170 6869 6361 6c20 5549 2066  t graphical UI f
-00006c90: 6f72 2065 6469 7469 6e67 2074 7265 6520  or editing tree 
-00006ca0: 6669 656c 6420 616e 6420 6461 7461 2066  field and data f
-00006cb0: 6965 6c64 2064 6566 696e 6974 696f 6e73  ield definitions
-00006cc0: 9468 075d 9468 5b29 8194 7d94 2868 056a  .h.].h[)..}.(h.j
-00006cd0: 2e09 0000 6807 5d94 6816 8c48 496d 706c  ....h.].h..HImpl
-00006ce0: 656d 656e 7420 6772 6170 6869 6361 6c20  ement graphical 
-00006cf0: 5549 2066 6f72 2065 6469 7469 6e67 2074  UI for editing t
-00006d00: 7265 6520 6669 656c 6420 616e 6420 6461  ree field and da
-00006d10: 7461 2066 6965 6c64 2064 6566 696e 6974  ta field definit
-00006d20: 696f 6e73 9485 9481 947d 9428 681b 6a30  ions.....}.(h.j0
-00006d30: 0900 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00006d40: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00006d50: 9468 275d 9468 295d 9475 682b 685a 681d  .h'].h)].uh+hZh.
-00006d60: 682c 681e 4b83 681b 6a2c 0900 0075 6261  h,h.K.h.j,...uba
-00006d70: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00006d80: 9468 275d 9468 295d 9475 682b 6854 681b  .h'].h)].uh+hTh.
-00006d90: 6a29 0900 0068 1c68 0368 1d68 2c68 1e4e  j)...h.h.h.h,h.N
-00006da0: 7562 6855 2981 947d 9428 6805 8ca8 496d  ubhU)..}.(h...Im
-00006db0: 706c 656d 656e 7420 676c 6f62 616c 2066  plement global f
-00006dc0: 756e 6374 696f 6e73 2028 4c69 6e65 6172  unctions (Linear
-00006dd0: 6973 6520 5472 6565 2c20 4c65 7665 6c2d  ise Tree, Level-
-00006de0: 5377 6170 2c20 4d65 7267 6520 6964 656e  Swap, Merge iden
-00006df0: 7469 6361 6c20 5369 626c 696e 6773 2c20  tical Siblings, 
-00006e00: 4d65 7267 6520 4964 656e 7469 6361 6c20  Merge Identical 
-00006e10: 5061 7265 6e74 732f 4368 696c 6472 656e  Parents/Children
-00006e20: 2c20 5265 6d6f 7665 2061 6c6c 204f 7270  , Remove all Orp
-00006e30: 6861 6e73 2c20 496e 7365 7274 2061 6c6c  hans, Insert all
-00006e40: 204f 7270 6861 6e73 2061 7320 4368 696c   Orphans as Chil
-00006e50: 6472 656e 290a 9468 075d 9468 5b29 8194  dren)..h.].h[)..
-00006e60: 7d94 2868 058c a749 6d70 6c65 6d65 6e74  }.(h...Implement
-00006e70: 2067 6c6f 6261 6c20 6675 6e63 7469 6f6e   global function
-00006e80: 7320 284c 696e 6561 7269 7365 2054 7265  s (Linearise Tre
-00006e90: 652c 204c 6576 656c 2d53 7761 702c 204d  e, Level-Swap, M
-00006ea0: 6572 6765 2069 6465 6e74 6963 616c 2053  erge identical S
-00006eb0: 6962 6c69 6e67 732c 204d 6572 6765 2049  iblings, Merge I
-00006ec0: 6465 6e74 6963 616c 2050 6172 656e 7473  dentical Parents
-00006ed0: 2f43 6869 6c64 7265 6e2c 2052 656d 6f76  /Children, Remov
-00006ee0: 6520 616c 6c20 4f72 7068 616e 732c 2049  e all Orphans, I
-00006ef0: 6e73 6572 7420 616c 6c20 4f72 7068 616e  nsert all Orphan
-00006f00: 7320 6173 2043 6869 6c64 7265 6e29 9468  s as Children).h
-00006f10: 075d 9468 168c a749 6d70 6c65 6d65 6e74  .].h...Implement
-00006f20: 2067 6c6f 6261 6c20 6675 6e63 7469 6f6e   global function
-00006f30: 7320 284c 696e 6561 7269 7365 2054 7265  s (Linearise Tre
-00006f40: 652c 204c 6576 656c 2d53 7761 702c 204d  e, Level-Swap, M
-00006f50: 6572 6765 2069 6465 6e74 6963 616c 2053  erge identical S
-00006f60: 6962 6c69 6e67 732c 204d 6572 6765 2049  iblings, Merge I
-00006f70: 6465 6e74 6963 616c 2050 6172 656e 7473  dentical Parents
-00006f80: 2f43 6869 6c64 7265 6e2c 2052 656d 6f76  /Children, Remov
-00006f90: 6520 616c 6c20 4f72 7068 616e 732c 2049  e all Orphans, I
-00006fa0: 6e73 6572 7420 616c 6c20 4f72 7068 616e  nsert all Orphan
-00006fb0: 7320 6173 2043 6869 6c64 7265 6e29 9485  s as Children)..
-00006fc0: 9481 947d 9428 681b 6a47 0900 0068 1c68  ...}.(h.jG...h.h
-00006fd0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00006fe0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00006ff0: 295d 9475 682b 685a 681d 682c 681e 4b84  )].uh+hZh.h,h.K.
-00007000: 681b 6a43 0900 0075 6261 681f 7d94 2868  h.jC...ubah.}.(h
-00007010: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00007020: 295d 9475 682b 6854 681b 6a29 0900 0068  )].uh+hTh.j)...h
-00007030: 1c68 0368 1d68 2c68 1e4e 7562 6568 1f7d  .h.h.h,h.Nubeh.}
-00007040: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00007050: 5d94 6829 5d94 6876 6877 7568 2b68 4f68  ].h)].hvhwuh+hOh
-00007060: 1d68 2c68 1e4b 8368 1b6a 1809 0000 681c  .h,h.K.h.j....h.
-00007070: 6803 7562 6568 1f7d 9428 6821 5d94 8c0a  h.ubeh.}.(h!]...
-00007080: 6d69 642d 6675 7475 7265 9461 6823 5d94  mid-future.ah#].
-00007090: 6825 5d94 8c0a 6d69 6420 6675 7475 7265  h%]...mid future
-000070a0: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
-000070b0: 1b6a b608 0000 681c 6803 681d 682c 681e  .j....h.h.h.h,h.
-000070c0: 4b81 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-000070d0: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
-000070e0: 0a46 6172 2046 7574 7572 6594 6807 5d94  .Far Future.h.].
-000070f0: 6816 8c0a 4661 7220 4675 7475 7265 9485  h...Far Future..
-00007100: 9481 947d 9428 681b 6a6c 0900 0068 1c68  ...}.(h.jl...h.h
-00007110: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00007120: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00007130: 295d 9475 682b 680f 681b 6a69 0900 0068  )].uh+h.h.ji...h
-00007140: 1c68 0368 1d68 2c68 1e4b 8775 6268 5029  .h.h.h,h.K.ubhP)
-00007150: 8194 7d94 2868 0568 0668 075d 9428 6855  ..}.(h.h.h.].(hU
-00007160: 2981 947d 9428 6805 8c33 496d 706c 656d  )..}.(h..3Implem
-00007170: 656e 7420 7361 6665 2075 7361 6765 2062  ent safe usage b
-00007180: 7920 6d75 6c74 6970 6c65 2073 696d 756c  y multiple simul
-00007190: 7461 6e65 6f75 7320 7573 6572 7394 6807  taneous users.h.
-000071a0: 5d94 685b 2981 947d 9428 6805 6a7f 0900  ].h[)..}.(h.j...
-000071b0: 0068 075d 9468 168c 3349 6d70 6c65 6d65  .h.].h..3Impleme
-000071c0: 6e74 2073 6166 6520 7573 6167 6520 6279  nt safe usage by
-000071d0: 206d 756c 7469 706c 6520 7369 6d75 6c74   multiple simult
-000071e0: 616e 656f 7573 2075 7365 7273 9485 9481  aneous users....
-000071f0: 947d 9428 681b 6a81 0900 0068 1c68 0368  .}.(h.j....h.h.h
-00007200: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00007210: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00007220: 9475 682b 685a 681d 682c 681e 4b89 681b  .uh+hZh.h,h.K.h.
-00007230: 6a7d 0900 0075 6261 681f 7d94 2868 215d  j}...ubah.}.(h!]
-00007240: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00007250: 9475 682b 6854 681b 6a7a 0900 0068 1c68  .uh+hTh.jz...h.h
-00007260: 0368 1d68 2c68 1e4e 7562 6855 2981 947d  .h.h,h.NubhU)..}
-00007270: 9428 6805 8c39 496d 706c 656d 656e 7420  .(h..9Implement 
-00007280: 6120 6461 7461 6261 7365 2062 6163 6b65  a database backe
-00007290: 6e64 2069 6e73 7465 6164 206f 6620 7465  nd instead of te
-000072a0: 7874 2066 696c 6520 7374 6f72 6167 6594  xt file storage.
-000072b0: 6807 5d94 685b 2981 947d 9428 6805 6a96  h.].h[)..}.(h.j.
-000072c0: 0900 0068 075d 9468 168c 3949 6d70 6c65  ...h.].h..9Imple
-000072d0: 6d65 6e74 2061 2064 6174 6162 6173 6520  ment a database 
-000072e0: 6261 636b 656e 6420 696e 7374 6561 6420  backend instead 
-000072f0: 6f66 2074 6578 7420 6669 6c65 2073 746f  of text file sto
-00007300: 7261 6765 9485 9481 947d 9428 681b 6a98  rage.....}.(h.j.
-00007310: 0900 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00007320: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00007330: 9468 275d 9468 295d 9475 682b 685a 681d  .h'].h)].uh+hZh.
-00007340: 682c 681e 4b8a 681b 6a94 0900 0075 6261  h,h.K.h.j....uba
-00007350: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00007360: 9468 275d 9468 295d 9475 682b 6854 681b  .h'].h)].uh+hTh.
-00007370: 6a7a 0900 0068 1c68 0368 1d68 2c68 1e4e  jz...h.h.h.h,h.N
-00007380: 7562 6855 2981 947d 9428 6805 8c44 4120  ubhU)..}.(h..DA 
-00007390: 7768 6f6c 6520 6c6f 7420 6f66 206f 7468  whole lot of oth
-000073a0: 6572 2066 616e 6379 2074 6869 6e67 7320  er fancy things 
-000073b0: 7468 6174 2077 696c 6c20 7072 6f62 6162  that will probab
-000073c0: 6c79 206e 6576 6572 2067 6574 2064 6f6e  ly never get don
-000073d0: 650a 9468 075d 9468 5b29 8194 7d94 2868  e..h.].h[)..}.(h
-000073e0: 058c 4341 2077 686f 6c65 206c 6f74 206f  ..CA whole lot o
-000073f0: 6620 6f74 6865 7220 6661 6e63 7920 7468  f other fancy th
-00007400: 696e 6773 2074 6861 7420 7769 6c6c 2070  ings that will p
-00007410: 726f 6261 626c 7920 6e65 7665 7220 6765  robably never ge
-00007420: 7420 646f 6e65 9468 075d 9468 168c 4341  t done.h.].h..CA
-00007430: 2077 686f 6c65 206c 6f74 206f 6620 6f74   whole lot of ot
-00007440: 6865 7220 6661 6e63 7920 7468 696e 6773  her fancy things
-00007450: 2074 6861 7420 7769 6c6c 2070 726f 6261   that will proba
-00007460: 626c 7920 6e65 7665 7220 6765 7420 646f  bly never get do
-00007470: 6e65 9485 9481 947d 9428 681b 6aaf 0900  ne.....}.(h.j...
-00007480: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00007490: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000074a0: 275d 9468 295d 9475 682b 685a 681d 682c  '].h)].uh+hZh.h,
-000074b0: 681e 4b8b 681b 6aab 0900 0075 6261 681f  h.K.h.j....ubah.
-000074c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000074d0: 275d 9468 295d 9475 682b 6854 681b 6a7a  '].h)].uh+hTh.jz
-000074e0: 0900 0068 1c68 0368 1d68 2c68 1e4e 7562  ...h.h.h.h,h.Nub
-000074f0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00007500: 5d94 6827 5d94 6829 5d94 6876 6877 7568  ].h'].h)].hvhwuh
-00007510: 2b68 4f68 1d68 2c68 1e4b 8968 1b6a 6909  +hOh.h,h.K.h.ji.
-00007520: 0000 681c 6803 7562 6568 1f7d 9428 6821  ..h.h.ubeh.}.(h!
-00007530: 5d94 8c0a 6661 722d 6675 7475 7265 9461  ]...far-future.a
-00007540: 6823 5d94 6825 5d94 8c0a 6661 7220 6675  h#].h%]...far fu
-00007550: 7475 7265 9461 6827 5d94 6829 5d94 7568  ture.ah'].h)].uh
-00007560: 2b68 0a68 1b6a b608 0000 681c 6803 681d  +h.h.j....h.h.h.
-00007570: 682c 681e 4b87 7562 6568 1f7d 9428 6821  h,h.K.ubeh.}.(h!
-00007580: 5d94 8c06 6675 7475 7265 9461 6823 5d94  ]...future.ah#].
-00007590: 6825 5d94 8c06 6675 7475 7265 9461 6827  h%]...future.ah'
-000075a0: 5d94 6829 5d94 7568 2b68 0a68 1b68 0c68  ].h)].uh+h.h.h.h
-000075b0: 1c68 0368 1d68 2c68 1e4b 7875 6265 681f  .h.h.h,h.Kxubeh.
-000075c0: 7d94 2868 215d 948c 1468 6973 746f 7279  }.(h!]...history
-000075d0: 2d61 6e64 2d72 6f61 642d 6d61 7094 6168  -and-road-map.ah
-000075e0: 235d 9468 255d 948c 1468 6973 746f 7279  #].h%]...history
-000075f0: 2061 6e64 2072 6f61 6420 6d61 7094 6168   and road map.ah
-00007600: 275d 9468 295d 9475 682b 680a 681b 6803  '].h)].uh+h.h.h.
-00007610: 681c 6803 681d 682c 681e 4b02 7562 6168  h.h.h.h,h.K.ubah
-00007620: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00007630: 6827 5d94 6829 5d94 8c06 736f 7572 6365  h'].h)]...source
-00007640: 9468 2c8c 1474 7261 6e73 6c61 7469 6f6e  .h,..translation
-00007650: 5f70 726f 6772 6573 7394 7d94 288c 0574  _progress.}.(..t
-00007660: 6f74 616c 944b 008c 0a74 7261 6e73 6c61  otal.K...transla
-00007670: 7465 6494 4b00 7575 682b 6801 8c0e 6375  ted.K.uuh+h...cu
-00007680: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
-00007690: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
-000076a0: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
-000076b0: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
-000076c0: 616c 7565 7394 9394 2981 947d 9428 8c06  alues...)..}.(..
-000076d0: 6f75 7470 7574 944e 680f 4e8c 0967 656e  output.Nh.N..gen
-000076e0: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
-000076f0: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
-00007700: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
-00007710: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
-00007720: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
-00007730: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
-00007740: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
-00007750: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
-00007760: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
-00007770: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
-00007780: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
-00007790: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
-000077a0: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
-000077b0: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
-000077c0: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
-000077d0: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
-000077e0: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
-000077f0: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
-00007800: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
-00007810: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
-00007820: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00007830: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
-00007840: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
-00007850: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
-00007860: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00007870: 7294 6a09 0a00 008c 0e65 7272 6f72 5f65  r.j......error_e
-00007880: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
-00007890: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
-000078a0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-000078b0: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
-000078c0: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
-000078d0: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
-000078e0: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
-000078f0: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
-00007900: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
-00007910: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
-00007920: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
-00007930: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
-00007940: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
-00007950: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
-00007960: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
-00007970: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
-00007980: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
-00007990: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
-000079a0: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
-000079b0: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
-000079c0: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
-000079d0: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
-000079e0: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
-000079f0: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
-00007a00: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
-00007a10: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
-00007a20: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
-00007a30: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-00007a40: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
-00007a50: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
-00007a60: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
-00007a70: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
-00007a80: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
-00007a90: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
-00007aa0: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
-00007ab0: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
-00007ac0: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
-00007ad0: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
-00007ae0: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
-00007af0: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
-00007b00: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
-00007b10: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
-00007b20: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
-00007b30: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
-00007b40: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
-00007b50: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
-00007b60: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
-00007b70: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
-00007b80: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
-00007b90: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
-00007ba0: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
-00007bb0: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
-00007bc0: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
-00007bd0: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
-00007be0: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
-00007bf0: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
-00007c00: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
-00007c10: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
-00007c20: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
-00007c30: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
-00007c40: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
-00007c50: 6964 7394 7d94 286a de09 0000 6adb 0900  ids.}.(j....j...
-00007c60: 006a 7907 0000 6a76 0700 0068 7d68 7a68  .jy...jv...h}hzh
-00007c70: e568 e26a c301 0000 6ac0 0100 006a 3902  .h.j....j....j9.
-00007c80: 0000 6a36 0200 006a 7302 0000 6a70 0200  ..j6...js...jp..
-00007c90: 006a 2003 0000 6a1d 0300 006a a805 0000  .j ...j....j....
-00007ca0: 6aa5 0500 006a 4c06 0000 6a49 0600 006a  j....jL...jI...j
-00007cb0: 7107 0000 6a6e 0700 006a 0608 0000 6a03  q...jn...j....j.
-00007cc0: 0800 006a b308 0000 6ab0 0800 006a d609  ...j....j....j..
-00007cd0: 0000 6ad3 0900 006a 1509 0000 6a12 0900  ..j....j....j...
-00007ce0: 006a 6609 0000 6a63 0900 006a ce09 0000  .jf...jc...j....
-00007cf0: 6acb 0900 0075 8c09 6e61 6d65 7479 7065  j....u..nametype
-00007d00: 7394 7d94 286a de09 0000 896a 7907 0000  s.}.(j.....jy...
-00007d10: 8968 7d89 68e5 896a c301 0000 896a 3902  .h}.h..j.....j9.
-00007d20: 0000 896a 7302 0000 896a 2003 0000 896a  ...js....j ....j
-00007d30: a805 0000 896a 4c06 0000 896a 7107 0000  .....jL....jq...
-00007d40: 896a 0608 0000 896a b308 0000 896a d609  .j.....j.....j..
-00007d50: 0000 896a 1509 0000 896a 6609 0000 896a  ...j.....jf....j
-00007d60: ce09 0000 8975 6821 7d94 286a db09 0000  .....uh!}.(j....
-00007d70: 680c 6a76 0700 0068 2d68 7a68 3e68 e268  h.jv...h-hzh>h.h
-00007d80: 806a c001 0000 68e8 6a36 0200 006a c601  .j....h.j6...j..
-00007d90: 0000 6a70 0200 006a 3c02 0000 6a1d 0300  ..jp...j<...j...
-00007da0: 006a 7602 0000 6aa5 0500 006a 2303 0000  .jv...j....j#...
-00007db0: 6a49 0600 006a ab05 0000 6a6e 0700 006a  jI...j....jn...j
-00007dc0: 4f06 0000 6a03 0800 006a 7c07 0000 6ab0  O...j....j|...j.
-00007dd0: 0800 006a 0908 0000 6ad3 0900 006a b608  ...j....j....j..
-00007de0: 0000 6a12 0900 006a c708 0000 6a63 0900  ..j....j....jc..
-00007df0: 006a 1809 0000 6acb 0900 006a 6909 0000  .j....j....ji...
-00007e00: 758c 0d66 6f6f 746e 6f74 655f 7265 6673  u..footnote_refs
-00007e10: 947d 948c 0d63 6974 6174 696f 6e5f 7265  .}...citation_re
-00007e20: 6673 947d 948c 0d61 7574 6f66 6f6f 746e  fs.}...autofootn
-00007e30: 6f74 6573 945d 948c 1161 7574 6f66 6f6f  otes.]...autofoo
-00007e40: 746e 6f74 655f 7265 6673 945d 948c 1073  tnote_refs.]...s
-00007e50: 796d 626f 6c5f 666f 6f74 6e6f 7465 7394  ymbol_footnotes.
-00007e60: 5d94 8c14 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
-00007e70: 6f74 655f 7265 6673 945d 948c 0966 6f6f  ote_refs.]...foo
-00007e80: 746e 6f74 6573 945d 948c 0963 6974 6174  tnotes.]...citat
-00007e90: 696f 6e73 945d 948c 1261 7574 6f66 6f6f  ions.]...autofoo
-00007ea0: 746e 6f74 655f 7374 6172 7494 4b01 8c15  tnote_start.K...
-00007eb0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-00007ec0: 7374 6172 7494 4b00 8c0a 6964 5f63 6f75  start.K...id_cou
-00007ed0: 6e74 6572 948c 0b63 6f6c 6c65 6374 696f  nter...collectio
-00007ee0: 6e73 948c 0743 6f75 6e74 6572 9493 947d  ns...Counter...}
-00007ef0: 946a 170a 0000 4b0a 7385 9452 948c 0e70  .j....K.s..R...p
-00007f00: 6172 7365 5f6d 6573 7361 6765 7394 5d94  arse_messages.].
-00007f10: 8c12 7472 616e 7366 6f72 6d5f 6d65 7373  ..transform_mess
-00007f20: 6167 6573 945d 948c 0b74 7261 6e73 666f  ages.]...transfo
-00007f30: 726d 6572 944e 8c0b 696e 636c 7564 655f  rmer.N..include_
-00007f40: 6c6f 6794 5d94 8c0a 6465 636f 7261 7469  log.]...decorati
-00007f50: 6f6e 944e 681c 6803 7562 2e              on.Nh.h.ub.
+00006b60: 5d94 7568 2b68 0f68 1b6a 0309 0000 681c  ].uh+h.h.j....h.
+00006b70: 6803 681d 682c 681e 4b7d 7562 6850 2981  h.h.h,h.K}ubhP).
+00006b80: 947d 9428 6805 6806 6807 5d94 2868 5529  .}.(h.h.h.].(hU)
+00006b90: 8194 7d94 2868 058c 1949 6d70 6c65 6d65  ..}.(h...Impleme
+00006ba0: 6e74 2073 6561 7263 6820 6675 6e63 7469  nt search functi
+00006bb0: 6f6e 9468 075d 9468 5b29 8194 7d94 2868  on.h.].h[)..}.(h
+00006bc0: 056a 1909 0000 6807 5d94 6816 8c19 496d  .j....h.].h...Im
+00006bd0: 706c 656d 656e 7420 7365 6172 6368 2066  plement search f
+00006be0: 756e 6374 696f 6e94 8594 8194 7d94 2868  unction.....}.(h
+00006bf0: 1b6a 1b09 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00006c00: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00006c10: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00006c20: 5a68 1d68 2c68 1e4b 7f68 1b6a 1709 0000  Zh.h,h.K.h.j....
+00006c30: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00006c40: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00006c50: 5468 1b6a 1409 0000 681c 6803 681d 682c  Th.j....h.h.h.h,
+00006c60: 681e 4e75 6268 5529 8194 7d94 2868 058c  h.NubhU)..}.(h..
+00006c70: 9e49 6d70 6c65 6d65 6e74 696e 6720 636f  .Implementing co
+00006c80: 6e74 696e 756f 7573 2074 6578 7420 616e  ntinuous text an
+00006c90: 6420 6874 6d6c 2065 7870 6f72 7420 2874  d html export (t
+00006ca0: 6f20 7573 6520 7472 6565 7469 6d65 2061  o use treetime a
+00006cb0: 7320 6120 6d65 6574 696e 6720 6e6f 7465  s a meeting note
+00006cc0: 2d74 616b 696e 6720 6170 7020 7768 6572  -taking app wher
+00006cd0: 6520 7061 7274 6963 6970 616e 7473 2076  e participants v
+00006ce0: 6965 7720 616e 2061 7574 6f2d 7570 6461  iew an auto-upda
+00006cf0: 7469 6e67 2068 746d 6c20 6669 6c65 2077  ting html file w
+00006d00: 6974 6820 7468 6520 6e6f 7465 7329 0a94  ith the notes)..
+00006d10: 6807 5d94 685b 2981 947d 9428 6805 8c9d  h.].h[)..}.(h...
+00006d20: 496d 706c 656d 656e 7469 6e67 2063 6f6e  Implementing con
+00006d30: 7469 6e75 6f75 7320 7465 7874 2061 6e64  tinuous text and
+00006d40: 2068 746d 6c20 6578 706f 7274 2028 746f   html export (to
+00006d50: 2075 7365 2074 7265 6574 696d 6520 6173   use treetime as
+00006d60: 2061 206d 6565 7469 6e67 206e 6f74 652d   a meeting note-
+00006d70: 7461 6b69 6e67 2061 7070 2077 6865 7265  taking app where
+00006d80: 2070 6172 7469 6369 7061 6e74 7320 7669   participants vi
+00006d90: 6577 2061 6e20 6175 746f 2d75 7064 6174  ew an auto-updat
+00006da0: 696e 6720 6874 6d6c 2066 696c 6520 7769  ing html file wi
+00006db0: 7468 2074 6865 206e 6f74 6573 2994 6807  th the notes).h.
+00006dc0: 5d94 6816 8c9d 496d 706c 656d 656e 7469  ].h...Implementi
+00006dd0: 6e67 2063 6f6e 7469 6e75 6f75 7320 7465  ng continuous te
+00006de0: 7874 2061 6e64 2068 746d 6c20 6578 706f  xt and html expo
+00006df0: 7274 2028 746f 2075 7365 2074 7265 6574  rt (to use treet
+00006e00: 696d 6520 6173 2061 206d 6565 7469 6e67  ime as a meeting
+00006e10: 206e 6f74 652d 7461 6b69 6e67 2061 7070   note-taking app
+00006e20: 2077 6865 7265 2070 6172 7469 6369 7061   where participa
+00006e30: 6e74 7320 7669 6577 2061 6e20 6175 746f  nts view an auto
+00006e40: 2d75 7064 6174 696e 6720 6874 6d6c 2066  -updating html f
+00006e50: 696c 6520 7769 7468 2074 6865 206e 6f74  ile with the not
+00006e60: 6573 2994 8594 8194 7d94 2868 1b6a 3209  es).....}.(h.j2.
+00006e70: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00006e80: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00006e90: 6827 5d94 6829 5d94 7568 2b68 5a68 1d68  h'].h)].uh+hZh.h
+00006ea0: 2c68 1e4b 8068 1b6a 2e09 0000 7562 6168  ,h.K.h.j....ubah
+00006eb0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00006ec0: 6827 5d94 6829 5d94 7568 2b68 5468 1b6a  h'].h)].uh+hTh.j
+00006ed0: 1409 0000 681c 6803 681d 682c 681e 4e75  ....h.h.h.h,h.Nu
+00006ee0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00006ef0: 255d 9468 275d 9468 295d 9468 7668 7775  %].h'].h)].hvhwu
+00006f00: 682b 684f 681d 682c 681e 4b7f 681b 6a03  h+hOh.h,h.K.h.j.
+00006f10: 0900 0068 1c68 0375 6265 681f 7d94 2868  ...h.h.ubeh.}.(h
+00006f20: 215d 948c 0b6e 6561 722d 6675 7475 7265  !]...near-future
+00006f30: 9461 6823 5d94 6825 5d94 8c0b 6e65 6172  .ah#].h%]...near
+00006f40: 2066 7574 7572 6594 6168 275d 9468 295d   future.ah'].h)]
+00006f50: 9475 682b 680a 681b 6af2 0800 0068 1c68  .uh+h.h.j....h.h
+00006f60: 0368 1d68 2c68 1e4b 7d75 6268 0b29 8194  .h.h,h.K}ubh.)..
+00006f70: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+00006f80: 947d 9428 6805 8c0a 4d69 6420 4675 7475  .}.(h...Mid Futu
+00006f90: 7265 9468 075d 9468 168c 0a4d 6964 2046  re.h.].h...Mid F
+00006fa0: 7574 7572 6594 8594 8194 7d94 2868 1b6a  uture.....}.(h.j
+00006fb0: 5709 0000 681c 6803 681d 4e68 1e4e 7562  W...h.h.h.Nh.Nub
+00006fc0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00006fd0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+00006fe0: 1b6a 5409 0000 681c 6803 681d 682c 681e  .jT...h.h.h.h,h.
+00006ff0: 4b83 7562 6850 2981 947d 9428 6805 6806  K.ubhP)..}.(h.h.
+00007000: 6807 5d94 2868 5529 8194 7d94 2868 058c  h.].(hU)..}.(h..
+00007010: 4849 6d70 6c65 6d65 6e74 2067 7261 7068  HImplement graph
+00007020: 6963 616c 2055 4920 666f 7220 6564 6974  ical UI for edit
+00007030: 696e 6720 7472 6565 2066 6965 6c64 2061  ing tree field a
+00007040: 6e64 2064 6174 6120 6669 656c 6420 6465  nd data field de
+00007050: 6669 6e69 7469 6f6e 7394 6807 5d94 685b  finitions.h.].h[
+00007060: 2981 947d 9428 6805 6a6a 0900 0068 075d  )..}.(h.jj...h.]
+00007070: 9468 168c 4849 6d70 6c65 6d65 6e74 2067  .h..HImplement g
+00007080: 7261 7068 6963 616c 2055 4920 666f 7220  raphical UI for 
+00007090: 6564 6974 696e 6720 7472 6565 2066 6965  editing tree fie
+000070a0: 6c64 2061 6e64 2064 6174 6120 6669 656c  ld and data fiel
+000070b0: 6420 6465 6669 6e69 7469 6f6e 7394 8594  d definitions...
+000070c0: 8194 7d94 2868 1b6a 6c09 0000 681c 6803  ..}.(h.jl...h.h.
+000070d0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000070e0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000070f0: 5d94 7568 2b68 5a68 1d68 2c68 1e4b 8568  ].uh+hZh.h,h.K.h
+00007100: 1b6a 6809 0000 7562 6168 1f7d 9428 6821  .jh...ubah.}.(h!
+00007110: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00007120: 5d94 7568 2b68 5468 1b6a 6509 0000 681c  ].uh+hTh.je...h.
+00007130: 6803 681d 682c 681e 4e75 6268 5529 8194  h.h.h,h.NubhU)..
+00007140: 7d94 2868 058c a849 6d70 6c65 6d65 6e74  }.(h...Implement
+00007150: 2067 6c6f 6261 6c20 6675 6e63 7469 6f6e   global function
+00007160: 7320 284c 696e 6561 7269 7365 2054 7265  s (Linearise Tre
+00007170: 652c 204c 6576 656c 2d53 7761 702c 204d  e, Level-Swap, M
+00007180: 6572 6765 2069 6465 6e74 6963 616c 2053  erge identical S
+00007190: 6962 6c69 6e67 732c 204d 6572 6765 2049  iblings, Merge I
+000071a0: 6465 6e74 6963 616c 2050 6172 656e 7473  dentical Parents
+000071b0: 2f43 6869 6c64 7265 6e2c 2052 656d 6f76  /Children, Remov
+000071c0: 6520 616c 6c20 4f72 7068 616e 732c 2049  e all Orphans, I
+000071d0: 6e73 6572 7420 616c 6c20 4f72 7068 616e  nsert all Orphan
+000071e0: 7320 6173 2043 6869 6c64 7265 6e29 0a94  s as Children)..
+000071f0: 6807 5d94 685b 2981 947d 9428 6805 8ca7  h.].h[)..}.(h...
+00007200: 496d 706c 656d 656e 7420 676c 6f62 616c  Implement global
+00007210: 2066 756e 6374 696f 6e73 2028 4c69 6e65   functions (Line
+00007220: 6172 6973 6520 5472 6565 2c20 4c65 7665  arise Tree, Leve
+00007230: 6c2d 5377 6170 2c20 4d65 7267 6520 6964  l-Swap, Merge id
+00007240: 656e 7469 6361 6c20 5369 626c 696e 6773  entical Siblings
+00007250: 2c20 4d65 7267 6520 4964 656e 7469 6361  , Merge Identica
+00007260: 6c20 5061 7265 6e74 732f 4368 696c 6472  l Parents/Childr
+00007270: 656e 2c20 5265 6d6f 7665 2061 6c6c 204f  en, Remove all O
+00007280: 7270 6861 6e73 2c20 496e 7365 7274 2061  rphans, Insert a
+00007290: 6c6c 204f 7270 6861 6e73 2061 7320 4368  ll Orphans as Ch
+000072a0: 696c 6472 656e 2994 6807 5d94 6816 8ca7  ildren).h.].h...
+000072b0: 496d 706c 656d 656e 7420 676c 6f62 616c  Implement global
+000072c0: 2066 756e 6374 696f 6e73 2028 4c69 6e65   functions (Line
+000072d0: 6172 6973 6520 5472 6565 2c20 4c65 7665  arise Tree, Leve
+000072e0: 6c2d 5377 6170 2c20 4d65 7267 6520 6964  l-Swap, Merge id
+000072f0: 656e 7469 6361 6c20 5369 626c 696e 6773  entical Siblings
+00007300: 2c20 4d65 7267 6520 4964 656e 7469 6361  , Merge Identica
+00007310: 6c20 5061 7265 6e74 732f 4368 696c 6472  l Parents/Childr
+00007320: 656e 2c20 5265 6d6f 7665 2061 6c6c 204f  en, Remove all O
+00007330: 7270 6861 6e73 2c20 496e 7365 7274 2061  rphans, Insert a
+00007340: 6c6c 204f 7270 6861 6e73 2061 7320 4368  ll Orphans as Ch
+00007350: 696c 6472 656e 2994 8594 8194 7d94 2868  ildren).....}.(h
+00007360: 1b6a 8309 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00007370: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00007380: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00007390: 5a68 1d68 2c68 1e4b 8668 1b6a 7f09 0000  Zh.h,h.K.h.j....
+000073a0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000073b0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+000073c0: 5468 1b6a 6509 0000 681c 6803 681d 682c  Th.je...h.h.h.h,
+000073d0: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
+000073e0: 235d 9468 255d 9468 275d 9468 295d 9468  #].h%].h'].h)].h
+000073f0: 7668 7775 682b 684f 681d 682c 681e 4b85  vhwuh+hOh.h,h.K.
+00007400: 681b 6a54 0900 0068 1c68 0375 6265 681f  h.jT...h.h.ubeh.
+00007410: 7d94 2868 215d 948c 0a6d 6964 2d66 7574  }.(h!]...mid-fut
+00007420: 7572 6594 6168 235d 9468 255d 948c 0a6d  ure.ah#].h%]...m
+00007430: 6964 2066 7574 7572 6594 6168 275d 9468  id future.ah'].h
+00007440: 295d 9475 682b 680a 681b 6af2 0800 0068  )].uh+h.h.j....h
+00007450: 1c68 0368 1d68 2c68 1e4b 8375 6268 0b29  .h.h.h,h.K.ubh.)
+00007460: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
+00007470: 2981 947d 9428 6805 8c0a 4661 7220 4675  )..}.(h...Far Fu
+00007480: 7475 7265 9468 075d 9468 168c 0a46 6172  ture.h.].h...Far
+00007490: 2046 7574 7572 6594 8594 8194 7d94 2868   Future.....}.(h
+000074a0: 1b6a a809 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+000074b0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000074c0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+000074d0: 0f68 1b6a a509 0000 681c 6803 681d 682c  .h.j....h.h.h.h,
+000074e0: 681e 4b89 7562 6850 2981 947d 9428 6805  h.K.ubhP)..}.(h.
+000074f0: 6806 6807 5d94 2868 5529 8194 7d94 2868  h.h.].(hU)..}.(h
+00007500: 058c 3349 6d70 6c65 6d65 6e74 2073 6166  ..3Implement saf
+00007510: 6520 7573 6167 6520 6279 206d 756c 7469  e usage by multi
+00007520: 706c 6520 7369 6d75 6c74 616e 656f 7573  ple simultaneous
+00007530: 2075 7365 7273 9468 075d 9468 5b29 8194   users.h.].h[)..
+00007540: 7d94 2868 056a bb09 0000 6807 5d94 6816  }.(h.j....h.].h.
+00007550: 8c33 496d 706c 656d 656e 7420 7361 6665  .3Implement safe
+00007560: 2075 7361 6765 2062 7920 6d75 6c74 6970   usage by multip
+00007570: 6c65 2073 696d 756c 7461 6e65 6f75 7320  le simultaneous 
+00007580: 7573 6572 7394 8594 8194 7d94 2868 1b6a  users.....}.(h.j
+00007590: bd09 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+000075a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000075b0: 5d94 6827 5d94 6829 5d94 7568 2b68 5a68  ].h'].h)].uh+hZh
+000075c0: 1d68 2c68 1e4b 8b68 1b6a b909 0000 7562  .h,h.K.h.j....ub
+000075d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000075e0: 5d94 6827 5d94 6829 5d94 7568 2b68 5468  ].h'].h)].uh+hTh
+000075f0: 1b6a b609 0000 681c 6803 681d 682c 681e  .j....h.h.h.h,h.
+00007600: 4e75 6268 5529 8194 7d94 2868 058c 3949  NubhU)..}.(h..9I
+00007610: 6d70 6c65 6d65 6e74 2061 2064 6174 6162  mplement a datab
+00007620: 6173 6520 6261 636b 656e 6420 696e 7374  ase backend inst
+00007630: 6561 6420 6f66 2074 6578 7420 6669 6c65  ead of text file
+00007640: 2073 746f 7261 6765 9468 075d 9468 5b29   storage.h.].h[)
+00007650: 8194 7d94 2868 056a d209 0000 6807 5d94  ..}.(h.j....h.].
+00007660: 6816 8c39 496d 706c 656d 656e 7420 6120  h..9Implement a 
+00007670: 6461 7461 6261 7365 2062 6163 6b65 6e64  database backend
+00007680: 2069 6e73 7465 6164 206f 6620 7465 7874   instead of text
+00007690: 2066 696c 6520 7374 6f72 6167 6594 8594   file storage...
+000076a0: 8194 7d94 2868 1b6a d409 0000 681c 6803  ..}.(h.j....h.h.
+000076b0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000076c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000076d0: 5d94 7568 2b68 5a68 1d68 2c68 1e4b 8c68  ].uh+hZh.h,h.K.h
+000076e0: 1b6a d009 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
+000076f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00007700: 5d94 7568 2b68 5468 1b6a b609 0000 681c  ].uh+hTh.j....h.
+00007710: 6803 681d 682c 681e 4e75 6268 5529 8194  h.h.h,h.NubhU)..
+00007720: 7d94 2868 058c 4441 2077 686f 6c65 206c  }.(h..DA whole l
+00007730: 6f74 206f 6620 6f74 6865 7220 6661 6e63  ot of other fanc
+00007740: 7920 7468 696e 6773 2074 6861 7420 7769  y things that wi
+00007750: 6c6c 2070 726f 6261 626c 7920 6e65 7665  ll probably neve
+00007760: 7220 6765 7420 646f 6e65 0a94 6807 5d94  r get done..h.].
+00007770: 685b 2981 947d 9428 6805 8c43 4120 7768  h[)..}.(h..CA wh
+00007780: 6f6c 6520 6c6f 7420 6f66 206f 7468 6572  ole lot of other
+00007790: 2066 616e 6379 2074 6869 6e67 7320 7468   fancy things th
+000077a0: 6174 2077 696c 6c20 7072 6f62 6162 6c79  at will probably
+000077b0: 206e 6576 6572 2067 6574 2064 6f6e 6594   never get done.
+000077c0: 6807 5d94 6816 8c43 4120 7768 6f6c 6520  h.].h..CA whole 
+000077d0: 6c6f 7420 6f66 206f 7468 6572 2066 616e  lot of other fan
+000077e0: 6379 2074 6869 6e67 7320 7468 6174 2077  cy things that w
+000077f0: 696c 6c20 7072 6f62 6162 6c79 206e 6576  ill probably nev
+00007800: 6572 2067 6574 2064 6f6e 6594 8594 8194  er get done.....
+00007810: 7d94 2868 1b6a eb09 0000 681c 6803 681d  }.(h.j....h.h.h.
+00007820: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00007830: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00007840: 7568 2b68 5a68 1d68 2c68 1e4b 8d68 1b6a  uh+hZh.h,h.K.h.j
+00007850: e709 0000 7562 6168 1f7d 9428 6821 5d94  ....ubah.}.(h!].
+00007860: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00007870: 7568 2b68 5468 1b6a b609 0000 681c 6803  uh+hTh.j....h.h.
+00007880: 681d 682c 681e 4e75 6265 681f 7d94 2868  h.h,h.Nubeh.}.(h
+00007890: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000078a0: 295d 9468 7668 7775 682b 684f 681d 682c  )].hvhwuh+hOh.h,
+000078b0: 681e 4b8b 681b 6aa5 0900 0068 1c68 0375  h.K.h.j....h.h.u
+000078c0: 6265 681f 7d94 2868 215d 948c 0a66 6172  beh.}.(h!]...far
+000078d0: 2d66 7574 7572 6594 6168 235d 9468 255d  -future.ah#].h%]
+000078e0: 948c 0a66 6172 2066 7574 7572 6594 6168  ...far future.ah
+000078f0: 275d 9468 295d 9475 682b 680a 681b 6af2  '].h)].uh+h.h.j.
+00007900: 0800 0068 1c68 0368 1d68 2c68 1e4b 8975  ...h.h.h.h,h.K.u
+00007910: 6265 681f 7d94 2868 215d 948c 0666 7574  beh.}.(h!]...fut
+00007920: 7572 6594 6168 235d 9468 255d 948c 0666  ure.ah#].h%]...f
+00007930: 7574 7572 6594 6168 275d 9468 295d 9475  uture.ah'].h)].u
+00007940: 682b 680a 681b 680c 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
+00007950: 681e 4b7a 7562 6568 1f7d 9428 6821 5d94  h.Kzubeh.}.(h!].
+00007960: 8c14 6869 7374 6f72 792d 616e 642d 726f  ..history-and-ro
+00007970: 6164 2d6d 6170 9461 6823 5d94 6825 5d94  ad-map.ah#].h%].
+00007980: 8c14 6869 7374 6f72 7920 616e 6420 726f  ..history and ro
+00007990: 6164 206d 6170 9461 6827 5d94 6829 5d94  ad map.ah'].h)].
+000079a0: 7568 2b68 0a68 1b68 0368 1c68 0368 1d68  uh+h.h.h.h.h.h.h
+000079b0: 2c68 1e4b 0275 6261 681f 7d94 2868 215d  ,h.K.ubah.}.(h!]
+000079c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000079d0: 948c 0673 6f75 7263 6594 682c 8c14 7472  ...source.h,..tr
+000079e0: 616e 736c 6174 696f 6e5f 7072 6f67 7265  anslation_progre
+000079f0: 7373 947d 9428 8c05 746f 7461 6c94 4b00  ss.}.(..total.K.
+00007a00: 8c0a 7472 616e 736c 6174 6564 944b 0075  ..translated.K.u
+00007a10: 7568 2b68 018c 0e63 7572 7265 6e74 5f73  uh+h...current_s
+00007a20: 6f75 7263 6594 4e8c 0c63 7572 7265 6e74  ource.N..current
+00007a30: 5f6c 696e 6594 4e8c 0873 6574 7469 6e67  _line.N..setting
+00007a40: 7394 8c11 646f 6375 7469 6c73 2e66 726f  s...docutils.fro
+00007a50: 6e74 656e 6494 8c06 5661 6c75 6573 9493  ntend...Values..
+00007a60: 9429 8194 7d94 288c 066f 7574 7075 7494  .)..}.(..output.
+00007a70: 4e68 0f4e 8c09 6765 6e65 7261 746f 7294  Nh.N..generator.
+00007a80: 4e8c 0964 6174 6573 7461 6d70 944e 8c0b  N..datestamp.N..
+00007a90: 736f 7572 6365 5f6c 696e 6b94 4e8c 0a73  source_link.N..s
+00007aa0: 6f75 7263 655f 7572 6c94 4e8c 0d74 6f63  ource_url.N..toc
+00007ab0: 5f62 6163 6b6c 696e 6b73 948c 0565 6e74  _backlinks...ent
+00007ac0: 7279 948c 1266 6f6f 746e 6f74 655f 6261  ry...footnote_ba
+00007ad0: 636b 6c69 6e6b 7394 4b01 8c0d 7365 6374  cklinks.K...sect
+00007ae0: 6e75 6d5f 7866 6f72 6d94 4b01 8c0e 7374  num_xform.K...st
+00007af0: 7269 705f 636f 6d6d 656e 7473 944e 8c1b  rip_comments.N..
+00007b00: 7374 7269 705f 656c 656d 656e 7473 5f77  strip_elements_w
+00007b10: 6974 685f 636c 6173 7365 7394 4e8c 0d73  ith_classes.N..s
+00007b20: 7472 6970 5f63 6c61 7373 6573 944e 8c0c  trip_classes.N..
+00007b30: 7265 706f 7274 5f6c 6576 656c 944b 028c  report_level.K..
+00007b40: 0a68 616c 745f 6c65 7665 6c94 4b05 8c11  .halt_level.K...
+00007b50: 6578 6974 5f73 7461 7475 735f 6c65 7665  exit_status_leve
+00007b60: 6c94 4b05 8c05 6465 6275 6794 4e8c 0e77  l.K...debug.N..w
+00007b70: 6172 6e69 6e67 5f73 7472 6561 6d94 4e8c  arning_stream.N.
+00007b80: 0974 7261 6365 6261 636b 9488 8c0e 696e  .traceback....in
+00007b90: 7075 745f 656e 636f 6469 6e67 948c 0975  put_encoding...u
+00007ba0: 7466 2d38 2d73 6967 948c 1c69 6e70 7574  tf-8-sig...input
+00007bb0: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00007bc0: 6861 6e64 6c65 7294 8c06 7374 7269 6374  handler...strict
+00007bd0: 948c 0f6f 7574 7075 745f 656e 636f 6469  ...output_encodi
+00007be0: 6e67 948c 0575 7466 2d38 948c 1d6f 7574  ng...utf-8...out
+00007bf0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
+00007c00: 6f72 5f68 616e 646c 6572 946a 450a 0000  or_handler.jE...
+00007c10: 8c0e 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00007c20: 948c 0575 7466 2d38 948c 1c65 7272 6f72  ...utf-8...error
+00007c30: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00007c40: 6861 6e64 6c65 7294 8c10 6261 636b 736c  handler...backsl
+00007c50: 6173 6872 6570 6c61 6365 948c 0d6c 616e  ashreplace...lan
+00007c60: 6775 6167 655f 636f 6465 948c 0265 6e94  guage_code...en.
+00007c70: 8c13 7265 636f 7264 5f64 6570 656e 6465  ..record_depende
+00007c80: 6e63 6965 7394 4e8c 0663 6f6e 6669 6794  ncies.N..config.
+00007c90: 4e8c 0969 645f 7072 6566 6978 9468 068c  N..id_prefix.h..
+00007ca0: 0e61 7574 6f5f 6964 5f70 7265 6669 7894  .auto_id_prefix.
+00007cb0: 8c02 6964 948c 0d64 756d 705f 7365 7474  ..id...dump_sett
+00007cc0: 696e 6773 944e 8c0e 6475 6d70 5f69 6e74  ings.N..dump_int
+00007cd0: 6572 6e61 6c73 944e 8c0f 6475 6d70 5f74  ernals.N..dump_t
+00007ce0: 7261 6e73 666f 726d 7394 4e8c 0f64 756d  ransforms.N..dum
+00007cf0: 705f 7073 6575 646f 5f78 6d6c 944e 8c10  p_pseudo_xml.N..
+00007d00: 6578 706f 7365 5f69 6e74 6572 6e61 6c73  expose_internals
+00007d10: 944e 8c0e 7374 7269 6374 5f76 6973 6974  .N..strict_visit
+00007d20: 6f72 944e 8c0f 5f64 6973 6162 6c65 5f63  or.N.._disable_c
+00007d30: 6f6e 6669 6794 4e8c 075f 736f 7572 6365  onfig.N.._source
+00007d40: 9468 2c8c 0c5f 6465 7374 696e 6174 696f  .h,.._destinatio
+00007d50: 6e94 4e8c 0d5f 636f 6e66 6967 5f66 696c  n.N.._config_fil
+00007d60: 6573 945d 948c 1666 696c 655f 696e 7365  es.]...file_inse
+00007d70: 7274 696f 6e5f 656e 6162 6c65 6494 888c  rtion_enabled...
+00007d80: 0b72 6177 5f65 6e61 626c 6564 944b 018c  .raw_enabled.K..
+00007d90: 116c 696e 655f 6c65 6e67 7468 5f6c 696d  .line_length_lim
+00007da0: 6974 944d 1027 8c0e 7065 705f 7265 6665  it.M.'..pep_refe
+00007db0: 7265 6e63 6573 944e 8c0c 7065 705f 6261  rences.N..pep_ba
+00007dc0: 7365 5f75 726c 948c 1868 7474 7073 3a2f  se_url...https:/
+00007dd0: 2f70 6570 732e 7079 7468 6f6e 2e6f 7267  /peps.python.org
+00007de0: 2f94 8c15 7065 705f 6669 6c65 5f75 726c  /...pep_file_url
+00007df0: 5f74 656d 706c 6174 6594 8c08 7065 702d  _template...pep-
+00007e00: 2530 3464 948c 0e72 6663 5f72 6566 6572  %04d...rfc_refer
+00007e10: 656e 6365 7394 4e8c 0c72 6663 5f62 6173  ences.N..rfc_bas
+00007e20: 655f 7572 6c94 8c26 6874 7470 733a 2f2f  e_url..&https://
+00007e30: 6461 7461 7472 6163 6b65 722e 6965 7466  datatracker.ietf
+00007e40: 2e6f 7267 2f64 6f63 2f68 746d 6c2f 948c  .org/doc/html/..
+00007e50: 0974 6162 5f77 6964 7468 944b 088c 1d74  .tab_width.K...t
+00007e60: 7269 6d5f 666f 6f74 6e6f 7465 5f72 6566  rim_footnote_ref
+00007e70: 6572 656e 6365 5f73 7061 6365 9489 8c10  erence_space....
+00007e80: 7379 6e74 6178 5f68 6967 686c 6967 6874  syntax_highlight
+00007e90: 948c 046c 6f6e 6794 8c0c 736d 6172 745f  ...long...smart_
+00007ea0: 7175 6f74 6573 9488 8c13 736d 6172 7471  quotes....smartq
+00007eb0: 756f 7465 735f 6c6f 6361 6c65 7394 5d94  uotes_locales.].
+00007ec0: 8c1d 6368 6172 6163 7465 725f 6c65 7665  ..character_leve
+00007ed0: 6c5f 696e 6c69 6e65 5f6d 6172 6b75 7094  l_inline_markup.
+00007ee0: 898c 0e64 6f63 7469 746c 655f 7866 6f72  ...doctitle_xfor
+00007ef0: 6d94 898c 0d64 6f63 696e 666f 5f78 666f  m....docinfo_xfo
+00007f00: 726d 944b 018c 1273 6563 7473 7562 7469  rm.K...sectsubti
+00007f10: 746c 655f 7866 6f72 6d94 898c 0d69 6d61  tle_xform....ima
+00007f20: 6765 5f6c 6f61 6469 6e67 948c 046c 696e  ge_loading...lin
+00007f30: 6b94 8c10 656d 6265 645f 7374 796c 6573  k...embed_styles
+00007f40: 6865 6574 9489 8c15 636c 6f61 6b5f 656d  heet....cloak_em
+00007f50: 6169 6c5f 6164 6472 6573 7365 7394 888c  ail_addresses...
+00007f60: 1173 6563 7469 6f6e 5f73 656c 665f 6c69  .section_self_li
+00007f70: 6e6b 9489 8c03 656e 7694 4e75 628c 0872  nk....env.Nub..r
+00007f80: 6570 6f72 7465 7294 4e8c 1069 6e64 6972  eporter.N..indir
+00007f90: 6563 745f 7461 7267 6574 7394 5d94 8c11  ect_targets.]...
+00007fa0: 7375 6273 7469 7475 7469 6f6e 5f64 6566  substitution_def
+00007fb0: 7394 7d94 8c12 7375 6273 7469 7475 7469  s.}...substituti
+00007fc0: 6f6e 5f6e 616d 6573 947d 948c 0872 6566  on_names.}...ref
+00007fd0: 6e61 6d65 7394 7d94 8c06 7265 6669 6473  names.}...refids
+00007fe0: 947d 948c 076e 616d 6569 6473 947d 9428  .}...nameids.}.(
+00007ff0: 6a1a 0a00 006a 170a 0000 6a79 0700 006a  j....j....jy...j
+00008000: 7607 0000 687d 687a 68e5 68e2 6ac3 0100  v...h}hzh.h.j...
+00008010: 006a c001 0000 6a39 0200 006a 3602 0000  .j....j9...j6...
+00008020: 6a73 0200 006a 7002 0000 6a20 0300 006a  js...jp...j ...j
+00008030: 1d03 0000 6aa8 0500 006a a505 0000 6a4c  ....j....j....jL
+00008040: 0600 006a 4906 0000 6a71 0700 006a 6e07  ...jI...jq...jn.
+00008050: 0000 6a42 0800 006a 3f08 0000 6aef 0800  ..jB...j?...j...
+00008060: 006a ec08 0000 6a12 0a00 006a 0f0a 0000  .j....j....j....
+00008070: 6a51 0900 006a 4e09 0000 6aa2 0900 006a  jQ...jN...j....j
+00008080: 9f09 0000 6a0a 0a00 006a 070a 0000 758c  ....j....j....u.
+00008090: 096e 616d 6574 7970 6573 947d 9428 6a1a  .nametypes.}.(j.
+000080a0: 0a00 0089 6a79 0700 0089 687d 8968 e589  ....jy....h}.h..
+000080b0: 6ac3 0100 0089 6a39 0200 0089 6a73 0200  j.....j9....js..
+000080c0: 0089 6a20 0300 0089 6aa8 0500 0089 6a4c  ..j ....j.....jL
+000080d0: 0600 0089 6a71 0700 0089 6a42 0800 0089  ....jq....jB....
+000080e0: 6aef 0800 0089 6a12 0a00 0089 6a51 0900  j.....j.....jQ..
+000080f0: 0089 6aa2 0900 0089 6a0a 0a00 0089 7568  ..j.....j.....uh
+00008100: 217d 9428 6a17 0a00 0068 0c6a 7607 0000  !}.(j....h.jv...
+00008110: 682d 687a 683e 68e2 6880 6ac0 0100 0068  h-hzh>h.h.j....h
+00008120: e86a 3602 0000 6ac6 0100 006a 7002 0000  .j6...j....jp...
+00008130: 6a3c 0200 006a 1d03 0000 6a76 0200 006a  j<...j....jv...j
+00008140: a505 0000 6a23 0300 006a 4906 0000 6aab  ....j#...jI...j.
+00008150: 0500 006a 6e07 0000 6a4f 0600 006a 3f08  ...jn...jO...j?.
+00008160: 0000 6a7c 0700 006a ec08 0000 6a45 0800  ..j|...j....jE..
+00008170: 006a 0f0a 0000 6af2 0800 006a 4e09 0000  .j....j....jN...
+00008180: 6a03 0900 006a 9f09 0000 6a54 0900 006a  j....j....jT...j
+00008190: 070a 0000 6aa5 0900 0075 8c0d 666f 6f74  ....j....u..foot
+000081a0: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
+000081b0: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
+000081c0: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
+000081d0: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
+000081e0: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
+000081f0: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
+00008200: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
+00008210: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
+00008220: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
+00008230: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
+00008240: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
+00008250: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
+00008260: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
+00008270: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
+00008280: 756e 7465 7294 9394 7d94 6a53 0a00 004b  unter...}.jS...K
+00008290: 0a73 8594 5294 8c0e 7061 7273 655f 6d65  .s..R...parse_me
+000082a0: 7373 6167 6573 945d 948c 1274 7261 6e73  ssages.]...trans
+000082b0: 666f 726d 5f6d 6573 7361 6765 7394 5d94  form_messages.].
+000082c0: 8c0b 7472 616e 7366 6f72 6d65 7294 4e8c  ..transformer.N.
+000082d0: 0b69 6e63 6c75 6465 5f6c 6f67 945d 948c  .include_log.]..
+000082e0: 0a64 6563 6f72 6174 696f 6e94 4e68 1c68  .decoration.Nh.h
+000082f0: 0375 622e                                .ub.
```

### Comparing `TreeTime-2024.1/docs/_build/doctrees/tree-fields.doctree` & `TreeTime-2024.2/docs/_build/doctrees/tree-fields.doctree`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/abcde01.png` & `TreeTime-2024.2/docs/_build/html/_images/abcde01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/abcde011.png` & `TreeTime-2024.2/docs/_build/html/_images/abcde011.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/abcde02.png` & `TreeTime-2024.2/docs/_build/html/_images/abcde02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/abcde021.png` & `TreeTime-2024.2/docs/_build/html/_images/abcde021.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/linked-trees.png` & `TreeTime-2024.2/docs/_build/html/_images/linked-trees.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/linked-trees1.png` & `TreeTime-2024.2/docs/_build/html/_images/linked-trees1.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot01.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot011.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot011.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot02.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot021.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot021.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot03.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot03.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot031.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot031.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot04.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot04.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/screenshot041.png` & `TreeTime-2024.2/docs/_build/html/_images/screenshot041.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_images/treetime-logo.png` & `TreeTime-2024.2/docs/_build/html/_images/treetime-logo.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_site/index.html` & `TreeTime-2024.2/docs/_build/html/_site/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="../">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Content &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Content &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="../_static/alabaster.css?v=cb25574f" />
-    <script src="../_static/documentation_options.js?v=db884f6e"></script>
+    <script src="../_static/documentation_options.js?v=ec70c504"></script>
     <script src="../_static/doctools.js?v=888ff710"></script>
     <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
    
   <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/_site/introduction.html` & `TreeTime-2024.2/docs/_build/html/_site/introduction.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="../">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Introduction &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Introduction &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="../_static/alabaster.css?v=cb25574f" />
-    <script src="../_static/documentation_options.js?v=db884f6e"></script>
+    <script src="../_static/documentation_options.js?v=ec70c504"></script>
     <script src="../_static/doctools.js?v=888ff710"></script>
     <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
    
   <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/_site/releases.html` & `TreeTime-2024.2/docs/_build/html/_site/releases.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="../">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>History and Road Map &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>History and Road Map &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="../_static/alabaster.css?v=cb25574f" />
-    <script src="../_static/documentation_options.js?v=db884f6e"></script>
+    <script src="../_static/documentation_options.js?v=ec70c504"></script>
     <script src="../_static/doctools.js?v=888ff710"></script>
     <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
    
   <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/_site/index.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/_site/index.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/_site/introduction.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/_site/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/_site/releases.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/_site/releases.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/data-fields.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/data-fields.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/data-format.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/data-format.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/index.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/introduction.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/introduction.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 Installation
 ------------
 
 Using pre-compiled Binaries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run *TreeTime* or *TreeTime.exe* from the new folder. Unzip the data package too. Add the program folder to your path.
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run *TreeTime* or *TreeTime.exe* from the new folder. Unzip the data package too. Add the program folder to your path.
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
   (If anybody can help building an executable for other platforms I'd be delighted.)
 
 Using a PyPi package in Python
```

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/releases.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/releases.rst.txt`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,16 @@
 2024
 ----
 
 * January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 * February 2024: Implemented min, max, min-string, max-string fields.
 * March 2024: Implemented longtext data field.
 * April 2024: Extended documentation on readthedocs.io. Release **version 2024.1**
+* April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+* April 2024: Release **version 2024.2**
 
 Present
 -------
 
 * Bugfixing
 * Extend documentation on readthedocs.io
 * Add more fields
```

### Comparing `TreeTime-2024.1/docs/_build/html/_sources/tree-fields.rst.txt` & `TreeTime-2024.2/docs/_build/html/_sources/tree-fields.rst.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/alabaster.css` & `TreeTime-2024.2/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/basic.css` & `TreeTime-2024.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/doctools.js` & `TreeTime-2024.2/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/forkme_right_darkblue_121621.png` & `TreeTime-2024.2/docs/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/language_data.js` & `TreeTime-2024.2/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/pygments.css` & `TreeTime-2024.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/searchtools.js` & `TreeTime-2024.2/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/_static/sphinx_highlight.js` & `TreeTime-2024.2/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/html/data-fields.html` & `TreeTime-2024.2/docs/_build/html/data-fields.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Data Fields &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Data Fields &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Tree Fields" href="tree-fields.html" />
     <link rel="prev" title="Data Format" href="data-format.html" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/data-format.html` & `TreeTime-2024.2/docs/_build/html/data-format.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Data Format &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Data Format &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Data Fields" href="data-fields.html" />
     <link rel="prev" title="Introduction" href="introduction.html" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/genindex.html` & `TreeTime-2024.2/docs/_build/html/genindex.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Index &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/index.html` & `TreeTime-2024.2/docs/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Content &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Content &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Introduction" href="introduction.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `TreeTime-2024.1/docs/_build/html/introduction.html` & `TreeTime-2024.2/docs/_build/html/introduction.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Introduction &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Introduction &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Data Format" href="data-format.html" />
     <link rel="prev" title="Content" href="index.html" />
    
@@ -100,15 +100,15 @@
 <p>A data file can be created by saving the currently open file to a copy. The button ‘Save As’ saves the current state. All write operations will be on the new file.</p>
 </section>
 <section id="installation">
 <h2>Installation<a class="headerlink" href="#installation" title="Link to this heading">¶</a></h2>
 <section id="using-pre-compiled-binaries">
 <h3>Using pre-compiled Binaries<a class="headerlink" href="#using-pre-compiled-binaries" title="Link to this heading">¶</a></h3>
 <ul>
-<li><p>Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](<a class="reference external" href="https://github.com/jkanev/treetime/releases/tag/2024.1">https://github.com/jkanev/treetime/releases/tag/2024.1</a>) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run <em>TreeTime</em> or <em>TreeTime.exe</em> from the new folder. Unzip the data package too. Add the program folder to your path.</p>
+<li><p>Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](<a class="reference external" href="https://github.com/jkanev/treetime/releases/tag/2024.2">https://github.com/jkanev/treetime/releases/tag/2024.2</a>) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run <em>TreeTime</em> or <em>TreeTime.exe</em> from the new folder. Unzip the data package too. Add the program folder to your path.</p>
 <p>Executable bundles have been created with pyinstaller ([www.pyinstaller.org](<a class="reference external" href="http://www.pyinstaller.org">http://www.pyinstaller.org</a>)).</p>
 </li>
 <li><p>Mac: Mac users please use the Python code (see below). There is no executable for Mac.
 (If anybody can help building an executable for other platforms I’d be delighted.)</p></li>
 </ul>
 </section>
 <section id="using-a-pypi-package-in-python">
```

#### html2text {}

```diff
@@ -93,16 +93,16 @@
 All write operations will be performed on that copy. This is to create a new
 file from a basically empty ‘trt’ file that has a pre-defined data structure.
 A data file can be created by saving the currently open file to a copy. The
 button ‘Save As’ saves the current state. All write operations will be on the
 new file.
 ********** IInnssttaallllaattiioonn_?¶ **********
 ******** UUssiinngg pprree--ccoommppiilleedd BBiinnaarriieess_?¶ ********
-    * Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1]
-      (_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_k_a_n_e_v_/_t_r_e_e_t_i_m_e_/_r_e_l_e_a_s_e_s_/_t_a_g_/_2_0_2_4_._1) and download a
+    * Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2]
+      (_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_k_a_n_e_v_/_t_r_e_e_t_i_m_e_/_r_e_l_e_a_s_e_s_/_t_a_g_/_2_0_2_4_._2) and download a
       zipped package for Windows 10, 64 bit, or for Linux 64 bit from there.
       Unzip it into your program directory and run TTrreeeeTTiimmee or TTrreeeeTTiimmee..eexxee
       from the new folder. Unzip the data package too. Add the program folder
       to your path.
       Executable bundles have been created with pyinstaller (
       [www.pyinstaller.org](_h_t_t_p_:_/_/_w_w_w_._p_y_i_n_s_t_a_l_l_e_r_._o_r_g)).
     * Mac: Mac users please use the Python code (see below). There is no
```

### Comparing `TreeTime-2024.1/docs/_build/html/releases.html` & `TreeTime-2024.2/docs/_build/html/releases.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>History and Road Map &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>History and Road Map &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="Tree Fields" href="tree-fields.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
@@ -141,14 +141,16 @@
 <section id="id10">
 <h2>2024<a class="headerlink" href="#id10" title="Link to this heading">¶</a></h2>
 <ul class="simple">
 <li><p>January 2024: Changed node symbol to small circle in text eport (after asking users on social media).</p></li>
 <li><p>February 2024: Implemented min, max, min-string, max-string fields.</p></li>
 <li><p>March 2024: Implemented longtext data field.</p></li>
 <li><p>April 2024: Extended documentation on readthedocs.io. Release <strong>version 2024.1</strong></p></li>
+<li><p>April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.</p></li>
+<li><p>April 2024: Release <strong>version 2024.2</strong></p></li>
 </ul>
 </section>
 <section id="present">
 <h2>Present<a class="headerlink" href="#present" title="Link to this heading">¶</a></h2>
 <ul class="simple">
 <li><p>Bugfixing</p></li>
 <li><p>Extend documentation on readthedocs.io</p></li>
```

#### html2text {}

```diff
@@ -96,14 +96,19 @@
 ********** 22002244_?¶ **********
     * January 2024: Changed node symbol to small circle in text eport (after
       asking users on social media).
     * February 2024: Implemented min, max, min-string, max-string fields.
     * March 2024: Implemented longtext data field.
     * April 2024: Extended documentation on readthedocs.io. Release vveerrssiioonn
       22002244..11
+    * April 2024: Restructured export area, added name-only export. Made all
+      export options (full tree / branch / node with contect) (all fields /
+      names only) available for all file formats and for both file and
+      clipboard export.
+    * April 2024: Release vveerrssiioonn 22002244..22
 ********** PPrreesseenntt_?¶ **********
     * Bugfixing
     * Extend documentation on readthedocs.io
     * Add more fields
     * Add more examples and more template data files
     * Implement tree field editing with graphical dialog (add, remove, change
       tree fields)
```

### Comparing `TreeTime-2024.1/docs/_build/html/search.html` & `TreeTime-2024.2/docs/_build/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Search &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
     
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
```

### Comparing `TreeTime-2024.1/docs/_build/html/searchindex.js` & `TreeTime-2024.2/docs/_build/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -198,15 +198,15 @@
         "instanc": [1, 6],
         "might": [1, 6],
         "see": [1, 3, 4, 6, 8],
         "taxonomi": [1, 6],
         "habitat": [1, 6],
         "contin": [1, 6],
         "countri": [1, 6],
-        "area": [1, 6],
+        "area": [1, 6, 7],
         "switch": [1, 6],
         "both": [1, 2, 6, 7],
         "view": [1, 6, 7, 8],
         "dai": [1, 6],
         "breakdown": [1, 6],
         "compani": [1, 6],
         "overview": [1, 6, 8],
@@ -618,14 +618,17 @@
         "breez": 7,
         "symbol": 7,
         "circl": 7,
         "eport": 7,
         "ask": 7,
         "social": 7,
         "media": 7,
+        "restructur": 7,
+        "full": 7,
+        "contect": 7,
         "continu": 7,
         "meet": 7,
         "take": 7,
         "app": 7,
         "particip": 7,
         "ui": 7,
         "input": 8,
@@ -773,14 +776,18 @@
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 4,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx": 60
     },
     "alltitles": {
+        "Content": [
+            [0, "content"],
+            [5, "content"]
+        ],
         "Introduction": [
             [1, "introduction"],
             [6, "introduction"]
         ],
         "Concept": [
             [1, "concept"],
             [6, "concept"]
@@ -912,18 +919,14 @@
         ],
         "Data Item Definition": [
             [4, "data-item-definition"]
         ],
         "The Data Pool": [
             [4, "the-data-pool"]
         ],
-        "Content": [
-            [5, "content"],
-            [0, "content"]
-        ],
         "2022": [
             [7, "id8"]
         ],
         "2023": [
             [7, "id9"]
         ],
         "2024": [
```

### Comparing `TreeTime-2024.1/docs/_build/html/tree-fields.html` & `TreeTime-2024.2/docs/_build/html/tree-fields.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Tree Fields &#8212; TreeTime User Manual 2024.1 documentation</title>
+    <title>Tree Fields &#8212; TreeTime User Manual 2024.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=b3523f8e" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=cb25574f" />
-    <script src="_static/documentation_options.js?v=db884f6e"></script>
+    <script src="_static/documentation_options.js?v=ec70c504"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="History and Road Map" href="releases.html" />
     <link rel="prev" title="Data Fields" href="data-fields.html" />
```

### Comparing `TreeTime-2024.1/docs/_build/latex/LICRcyr2utf8.xdy` & `TreeTime-2024.2/docs/_build/latex/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/LICRlatin2utf8.xdy` & `TreeTime-2024.2/docs/_build/latex/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/LatinRules.xdy` & `TreeTime-2024.2/docs/_build/latex/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/Makefile` & `TreeTime-2024.2/docs/_build/latex/Makefile`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/abcde011.png` & `TreeTime-2024.2/docs/_build/latex/abcde011.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/abcde021.png` & `TreeTime-2024.2/docs/_build/latex/abcde021.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/latexmkjarc` & `TreeTime-2024.2/docs/_build/latex/latexmkjarc`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/linked-trees1.png` & `TreeTime-2024.2/docs/_build/latex/linked-trees1.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/screenshot011.png` & `TreeTime-2024.2/docs/_build/latex/screenshot011.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/screenshot021.png` & `TreeTime-2024.2/docs/_build/latex/screenshot021.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/screenshot031.png` & `TreeTime-2024.2/docs/_build/latex/screenshot031.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/screenshot041.png` & `TreeTime-2024.2/docs/_build/latex/screenshot041.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinx.sty` & `TreeTime-2024.2/docs/_build/latex/sphinx.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinx.xdy` & `TreeTime-2024.2/docs/_build/latex/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxhighlight.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxhighlight.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxhowto.cls` & `TreeTime-2024.2/docs/_build/latex/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexadmonitions.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexcontainers.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexgraphics.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexindbibtoc.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexlists.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexliterals.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexnumfig.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexobjects.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexshadowbox.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexstyleheadings.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexstylepage.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatexstyletext.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxlatextables.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxmanual.cls` & `TreeTime-2024.2/docs/_build/latex/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxmessages.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxmessages.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxoptionsgeometry.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxoptionshyperref.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxpackageboxes.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxpackageboxes.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxpackagecyrillic.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/sphinxpackagefootnote.sty` & `TreeTime-2024.2/docs/_build/latex/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/treetime-logo.png` & `TreeTime-2024.2/docs/_build/latex/treetime-logo.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.aux` & `TreeTime-2024.2/docs/_build/latex/treetimeusermanual.aux`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 \newlabel{releases:id7}{{5.1.7}{22}{2021}{subsection.5.1.7}{}}
 \@writefile{toc}{\contentsline {subsection}{\numberline {5.1.8}2022}{23}{subsection.5.1.8}\protected@file@percent }
 \newlabel{releases:id8}{{5.1.8}{23}{2022}{subsection.5.1.8}{}}
 \@writefile{toc}{\contentsline {subsection}{\numberline {5.1.9}2023}{23}{subsection.5.1.9}\protected@file@percent }
 \newlabel{releases:id9}{{5.1.9}{23}{2023}{subsection.5.1.9}{}}
 \@writefile{toc}{\contentsline {section}{\numberline {5.2}2024}{23}{section.5.2}\protected@file@percent }
 \newlabel{releases:id10}{{5.2}{23}{2024}{section.5.2}{}}
-\@writefile{toc}{\contentsline {section}{\numberline {5.3}Present}{23}{section.5.3}\protected@file@percent }
-\newlabel{releases:present}{{5.3}{23}{Present}{section.5.3}{}}
+\@writefile{toc}{\contentsline {section}{\numberline {5.3}Present}{24}{section.5.3}\protected@file@percent }
+\newlabel{releases:present}{{5.3}{24}{Present}{section.5.3}{}}
 \@writefile{toc}{\contentsline {section}{\numberline {5.4}Future}{24}{section.5.4}\protected@file@percent }
 \newlabel{releases:future}{{5.4}{24}{Future}{section.5.4}{}}
 \@writefile{toc}{\contentsline {subsection}{\numberline {5.4.1}Near Future}{24}{subsection.5.4.1}\protected@file@percent }
 \newlabel{releases:near-future}{{5.4.1}{24}{Near Future}{subsection.5.4.1}{}}
 \@writefile{toc}{\contentsline {subsection}{\numberline {5.4.2}Mid Future}{24}{subsection.5.4.2}\protected@file@percent }
 \newlabel{releases:mid-future}{{5.4.2}{24}{Mid Future}{subsection.5.4.2}{}}
 \@writefile{toc}{\contentsline {subsection}{\numberline {5.4.3}Far Future}{24}{subsection.5.4.3}\protected@file@percent }
```

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.log` & `TreeTime-2024.2/docs/_build/latex/treetimeusermanual.log`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-This is pdfTeX, Version 3.141592653-2.6-1.40.25 (TeX Live 2023/Debian) (preloaded format=pdflatex 2024.1.2)  17 APR 2024 11:05
+This is pdfTeX, Version 3.141592653-2.6-1.40.25 (TeX Live 2023/Debian) (preloaded format=pdflatex 2024.1.2)  25 APR 2024 22:07
 entering extended mode
  restricted \write18 enabled.
  %&-line parsing enabled.
 **treetimeusermanual.tex
 (./treetimeusermanual.tex
 LaTeX2e <2023-11-01>
 L3 programming layer <2023-11-09>
@@ -961,14 +961,14 @@
  72i,12n,79p,962b,703s stack positions out of 10000i,1000n,20000p,200000b,200000s
 </usr/share/texmf/fonts/type1/public/tex-gyre/qhvb.pfb></usr/share/texmf/font
 s/type1/public/tex-gyre/qhvbi.pfb></usr/share/texmf/fonts/type1/public/tex-gyre
 /qtmb.pfb></usr/share/texmf/fonts/type1/public/tex-gyre/qtmbi.pfb></usr/share/t
 exmf/fonts/type1/public/tex-gyre/qtmr.pfb></usr/share/texmf/fonts/type1/public/
 tex-gyre/qtmri.pfb></usr/share/texlive/texmf-dist/fonts/type1/public/txfonts/t1
 xtt.pfb>
-Output written on treetimeusermanual.pdf (28 pages, 748236 bytes).
+Output written on treetimeusermanual.pdf (28 pages, 748369 bytes).
 PDF statistics:
  496 PDF objects out of 1000 (max. 8388607)
  437 compressed objects within 5 object streams
  96 named destinations out of 1000 (max. 500000)
  541 words of extra memory for PDF output out of 10000 (max. 10000000)
```

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.out` & `TreeTime-2024.2/docs/_build/latex/treetimeusermanual.out`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.pdf` & `TreeTime-2024.2/docs/TreeTime_User-Manual_2024-04-25.pdf`

 * *Files 4% similar despite different names*

#### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.pdf` & `TreeTime-2024.2/docs/TreeTime_User-Manual_2024-04-25.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Jacob Kanev'
-CreationDate: "D:20240417110552+02'00'"
+CreationDate: "D:20240425220748+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240417110552+02'00'"
+ModDate: "D:20240425220748+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.25 (TeX Live 2023/Debian) kpathsea version 6.3.5'
 Producer: 'pdfTeX-1.40.25'
 Subject: ''
 Title: 'TreeTime User Manual'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 TreeTime User Manual
-Release 2024.1
+Release 2024.2
 
 Jacob Kanev
 
-Apr 17, 2024
+Apr 25, 2024
 
 CONTENTS
 
 1
 
 Introduction
 1.1 Concept . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -108,30 +108,30 @@
 5.2 2024 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 5.3 Present . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 5.4 Future . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 21
 21
 23
-23
+24
 24
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 TreeTime is a general data organisation, management and analysis tool using linked trees instead of flat lists of tables. A
 tree is a hierarchical structure that arranges your data into units and sub-units. Mathematical functions (sum, difference,
 mean, ratio) can be calculated recursively. Linked trees are distinct trees that share data between them. In TreeTime, a
 data object is part of several trees at the same time. TreeTime is a time planner, a to-do list manager, a test report tool,
 a project planner, a family ancestry editor, a mind-mapping tool, and similar.
 
 CONTENTS
 
 1
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 2
 
 CONTENTS
 
 CHAPTER
 
@@ -157,15 +157,15 @@
 1.1.2 What are linked Trees?
 The core concept of TreeTime are linked trees. Linked trees are separate trees that share the same data. One piece of
 information (a node) can be in several trees at the same time, but in different place of the tree. As a single tree is a way
 of sorting information, different linked trees sort the same data in different ways.
 
 3
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 In Tree 1, Node E is right at the bottom, as a child of B and a grandchild of A. In Tree 2 it is a child of D.
 In TreeTime, a node or item can hold different information like text, numbers, dates, internet links. These are saved in
 the item’s fields.
 Here we have a field we call “value”. Each node in all trees has a value field that can hold a number (like a cell in a
 spread sheet). The node A has the value=1, B=2, etc. In addition we have a field we call “Sum”. Its content is calculated
 automatically, summing up the item’s own value plus the values of all children. In TreeTime, looking at item E and
@@ -173,15 +173,15 @@
 
 Clicking on the other tab shows the second tree while the same items stays selected:
 
 4
 
 Chapter 1. Introduction
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 Note how the values are summed up the branches. Apart from sums, TreeTime also offers means, ratios, or differences,
 using different combinations of parent, child, or sibling fields.
 Linked trees are a natural and powerful way to structure data. If you, for instance, organise information
 about animals, you might want to see the animal’s taxonomy (kingdom/class/family/species), but also their habitat (continent/country/area), and switch between both views. If you organise tasks, you could switch between
 a year/quarter/week/day breakdown, a company/department/team/person tree, and a product/project/package/task
 overview.
@@ -201,15 +201,15 @@
 Access each single tree by clicking a tab on the main tree-view widget (the picture above shows the tree Time Plan, the
 picture below the tree Projects).
 
 1.2. Basic Use
 
 5
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 Branches and children can be sorted, branches can be folded and unfolded. Data content is shown via analytic fields
 that are defined per tree. In the example project you will see a sum, a percentage, and text display.
 Add, move and remove single nodes and complete branches by using the buttons on the left. Change the name of a node
 by selecting the node and editing the name in the top of the edit grid in the middle. Change all other values (numbers
 or text) by clicking into the field and start typing.
 The parents of an item are listed underneath the item name. Each tree has a separate line. Change the position of a
@@ -219,41 +219,41 @@
 TreeTime lets you select different themes and will try to use the default colours that are defined with your operating
 system.
 
 6
 
 Chapter 1. Introduction
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 1.3 Data Files
 The data in TreeTime is stored in a plain text file, marked with a ‘trt’ file ending (‘trt’ for ‘TreeTime’).
 The button ‘Load File’ will open an existing ‘trt’ file. After this, all changes are written to that file. There is no ‘Save’
 button, changes are written to the file immediately.
 The button ‘New From Template’ opens an existing data file, creates a copy, and saves this copy. A data file can be
 created by copying the currently open file. All write operations will be performed on that copy. This is to create a new
 file from a basically empty ‘trt’ file that has a pre-defined data structure.
 A data file can be created by saving the currently open file to a copy. The button ‘Save As’ saves the current state. All
 write operations will be on the new file.
 
 1.4 Installation
 1.4.1 Using pre-compiled Binaries
-• Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/
-releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there.
+• Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/
+releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there.
 Unzip it into your program directory and run TreeTime or TreeTime.exe from the new folder. Unzip the data
 package too. Add the program folder to your path.
 Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 • Mac: Mac users please use the Python code (see below). There is no executable for Mac. (If anybody can help
 building an executable for other platforms I’d be delighted.)
 
 1.3. Data Files
 
 7
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 1.4.2 Using a PyPi package in Python
 1. If you don’t have it yet, install python3
 2. Install PyQt6 – on an elevated command prompt (Windows), or on the standard command line (Mac,
 Linux), type:
 pip install PyQt6
 3. Install TreeTime – on an elevated command prompt (Windows), or on the standard command line (Mac,
@@ -320,15 +320,15 @@
 parent-fields []
 field "Sum"
 field-type "sum"
 (continues on next page)
 
 9
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 (continued from previous page)
 
 own-fields ["value"]
 child-fields ["Sum"]
 sibling-fields []
 parent-fields []
@@ -368,15 +368,15 @@
 field-type "sum"
 (continues on next page)
 
 10
 
 Chapter 2. Data Format
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 (continued from previous page)
 
 own-fields ["value"]
 child-fields ["Sum"]
 sibling-fields []
 parent-fields []
@@ -414,15 +414,15 @@
 fields {"value": {"content": 5, "type": "integer"}}
 trees [[0, 0, 1], [0, 1]]
 
 2.3. Data Item Definition
 
 11
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 The content here is the actual content in the field. The tree structure is stored in the last line:
 trees [[0, 0, 1], [0, 1]]
 This is an array of arrays, each of which is a path in the tree. In the example above the node can be found following
 the path 0-0-1 in the first tree starting at the root node, and 0-1 in the second tree. Children are numbered using fixed
 indexes, starting at 0. A path of 0-0-1 means: My node is the second child (-1) of the first child (-0-1) of the first child
 (0-0-1) of the root node in the (first) tree. And in the second tree, the path 0-1 says the node is the second child of the
@@ -456,15 +456,15 @@
 3.3 longtext
 Quite long text.:
 "details": {"content": "We discussed the following...", "type": "longtext"}
 Identical to the text field, but in the GUI there are 25 lines and a scrollbar.
 
 13
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 3.4 url
 A URl of any type (file, http, . . . ).:
 "external link": {"content": "https://tree-time.info", "type": "url"}
 In the GUI there’s a text field and a button saying “Open”. Clicking the button will use the the content of the text
 field and call the open method defined in the operating system (e.g. a content of “https://tree-time.info” or “file:
 ///home/myself/downloads/pass-word.info.html” would be opened with your default web browser).
@@ -521,15 +521,15 @@
 sibling-fields []
 parent-fields []
 The tree field “Progress” is a ratio, defined as parameter1 / (parameter2 + parameter3 + . . . ). In the tree view it will be
 displayed as a percentage. It shows the ratio of the tree fields “Spent Hours” / “Planned Hours”.
 
 15
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 4.2 string
 The simple display of the content of one or multiple data fields or tree fields. Syntax:
 field "Name"
 field-type "string"
 own-fields ["field1"]
 child-fields []
@@ -564,15 +564,15 @@
 sibling-fields [...]
 parent-fields [...]
 
 16
 
 Chapter 4. Tree Fields
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 were “field1”, “field2”, “field3”, . . . , are the names of data or tree fields.
 Result: A list like value1, value2, value3, value4, where each value is the value of at least on input field and each value
 is listed only once, sorted alphabetically.
 
 4.7 sum-time
 Same as “sum”, but will show the result as hour format, e.g. the value 1.5 will be displayed and exported as 1:30:00.
@@ -603,15 +603,15 @@
 were “field1”, “field2”, “field3”, . . . , are the names of data or tree fields.
 Result: The value (field1 + field2 + field3 + . . . ) / N, where N is the number of fields.
 
 4.7. sum-time
 
 17
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 4.11 mean-percent
 Same as “mean”, but will show the result as a percentage, e.g. the value 0.75 will show as 75 %.
 
 4.12 min
 The minimum. Syntax:
 field "Name"
@@ -644,15 +644,15 @@
 parent-fields [...]
 were “field1”, “field2”, “field3”, . . . , are the names of data or tree fields.
 Result: The value field1 / (field2 + field3 + . . . ), where N is the number of fields.
 18
 
 Chapter 4. Tree Fields
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 4.17 ratio-percent
 Same as “ratio”, but displayed as percentage (e.g., 0.75 is displayed as 75 %).
 
 4.18 node-name
 The name of the node’s parent in another tree. Syntax:
 field "Name"
@@ -683,15 +683,15 @@
 Same as “node-name”, but instead of the paren’t name, the entire path is shown, using “|” as delimiter (e.g. “Coding |
 Open Source | TreeTime”).
 
 4.17. ratio-percent
 
 19
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 20
 
 Chapter 4. Tree Fields
 
 CHAPTER
 
@@ -721,15 +721,15 @@
 single drop down lists.
 • October: Re-furbished the GUI and removed a couple of bugs. Slighty changed the data file format. Implemented
 theme selection. Tested pyqtdeploy for deployment instead of pyinstaller. Updated the description.
 • November: Released version 2018-10
 
 21
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 5.1.5 2019
 • January: Implemented new field type “URL”
 
 5.1.6 2020
 • June: Fixed problem with protected cells (typing into a cell without data could cause a crash), and fixed file
 selection dialog (now only offers .trt files).
@@ -762,15 +762,15 @@
 • September: Added new export option “Text to Clipboard”
 • November: Added new export option “Html (List) to File”
 • December: Added two primitive template files (a text-only single tree and dual tree mindmap)
 22
 
 Chapter 5. History and Road Map
 
-TreeTime User Manual, Release 2024.1
+TreeTime User Manual, Release 2024.2
 
 • December: Released version 2021.9
 
 5.1.8 2022
 • March: Fixed crash bug on non-export
 • March 2022: Improved sorting and grouping in html export, changed to five columns
 • June 2022: Added a tutorial file
@@ -790,29 +790,32 @@
 • October 2023: Fixed crash when exporting text to clipboard.
 
 5.2 2024
 • January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 • February 2024: Implemented min, max, min-string, max-string fields.
 • March 2024: Implemented longtext data field.
 • April 2024: Extended documentation on readthedocs.io. Release version 2024.1
+• April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node
+with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+• April 2024: Release version 2024.2
+
+5.2. 2024
+
+23
+
+TreeTime User Manual, Release 2024.2
 
 5.3 Present
 • Bugfixing
 • Extend documentation on readthedocs.io
 • Add more fields
 • Add more examples and more template data files
 • Implement tree field editing with graphical dialog (add, remove, change tree fields)
 • Implement data item field editing with graphical dialog (add, remove, change data item fields)
 
-5.2. 2024
-
-23
-
-TreeTime User Manual, Release 2024.1
-
 5.4 Future
 5.4.1 Near Future
 • Implement search function
 • Implementing continuous text and html export (to use treetime as a meeting note-taking app where participants
 view an auto-updating html file with the notes)
 
 5.4.2 Mid Future
```

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.tex` & `TreeTime-2024.2/docs/_build/latex/treetimeusermanual.tex`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 
 \usepackage{sphinxmessages}
 \setcounter{tocdepth}{1}
 
 
 
 \title{TreeTime User Manual}
-\date{Apr 17, 2024}
-\release{2024.1}
+\date{Apr 25, 2024}
+\release{2024.2}
 \author{Jacob Kanev}
 \newcommand{\sphinxlogo}{\vbox{}}
 \renewcommand{\releasename}{Release}
 \makeindex
 \begin{document}
 
 \ifdefined\shorthandoff
@@ -224,15 +224,15 @@
 \section{Installation}
 \label{\detokenize{introduction:installation}}
 
 \subsection{Using pre\sphinxhyphen{}compiled Binaries}
 \label{\detokenize{introduction:using-pre-compiled-binaries}}\begin{itemize}
 \item {} 
 \sphinxAtStartPar
-Windows, Linux: Go to {[}github.com/jkanev/treetime/releases/tag/2024.1{]}(\sphinxurl{https://github.com/jkanev/treetime/releases/tag/2024.1}) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run \sphinxstyleemphasis{TreeTime} or \sphinxstyleemphasis{TreeTime.exe} from the new folder. Unzip the data package too. Add the program folder to your path.
+Windows, Linux: Go to {[}github.com/jkanev/treetime/releases/tag/2024.2{]}(\sphinxurl{https://github.com/jkanev/treetime/releases/tag/2024.2}) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run \sphinxstyleemphasis{TreeTime} or \sphinxstyleemphasis{TreeTime.exe} from the new folder. Unzip the data package too. Add the program folder to your path.
 
 \sphinxAtStartPar
 Executable bundles have been created with pyinstaller ({[}www.pyinstaller.org{]}(\sphinxurl{http://www.pyinstaller.org})).
 
 \item {} 
 \sphinxAtStartPar
 Mac: Mac users please use the Python code (see below). There is no executable for Mac.
@@ -1193,14 +1193,22 @@
 \sphinxAtStartPar
 March 2024: Implemented longtext data field.
 
 \item {} 
 \sphinxAtStartPar
 April 2024: Extended documentation on readthedocs.io. Release \sphinxstylestrong{version 2024.1}
 
+\item {} 
+\sphinxAtStartPar
+April 2024: Restructured export area, added name\sphinxhyphen{}only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+
+\item {} 
+\sphinxAtStartPar
+April 2024: Release \sphinxstylestrong{version 2024.2}
+
 \end{itemize}
 
 
 \section{Present}
 \label{\detokenize{releases:present}}\begin{itemize}
 \item {} 
 \sphinxAtStartPar
```

### Comparing `TreeTime-2024.1/docs/_build/latex/treetimeusermanual.toc` & `TreeTime-2024.2/docs/_build/latex/treetimeusermanual.toc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
 \contentsline {subsection}{\numberline {5.1.4}2018}{21}{subsection.5.1.4}%
 \contentsline {subsection}{\numberline {5.1.5}2019}{22}{subsection.5.1.5}%
 \contentsline {subsection}{\numberline {5.1.6}2020}{22}{subsection.5.1.6}%
 \contentsline {subsection}{\numberline {5.1.7}2021}{22}{subsection.5.1.7}%
 \contentsline {subsection}{\numberline {5.1.8}2022}{23}{subsection.5.1.8}%
 \contentsline {subsection}{\numberline {5.1.9}2023}{23}{subsection.5.1.9}%
 \contentsline {section}{\numberline {5.2}2024}{23}{section.5.2}%
-\contentsline {section}{\numberline {5.3}Present}{23}{section.5.3}%
+\contentsline {section}{\numberline {5.3}Present}{24}{section.5.3}%
 \contentsline {section}{\numberline {5.4}Future}{24}{section.5.4}%
 \contentsline {subsection}{\numberline {5.4.1}Near Future}{24}{subsection.5.4.1}%
 \contentsline {subsection}{\numberline {5.4.2}Mid Future}{24}{subsection.5.4.2}%
 \contentsline {subsection}{\numberline {5.4.3}Far Future}{24}{subsection.5.4.3}%
```

### Comparing `TreeTime-2024.1/docs/_config.yml` & `TreeTime-2024.2/docs/_config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # in the templates via {{ site.myvariable }}.
 title: TreeTime
 email: jkanev@zoho.com
 description: >- # this means to ignore newlines until "baseurl:"
   Take notes. Track tasks. Plan projects. Organize knowledge. Using trees:<br/>
 baseurl: "" # the subpath of your site, e.g. /blog
 url: "http://tree-time.info" # the base hostname & protocol for your site, e.g. http://example.com
-twitter_username: j_kanev
 github_username:  jkanev
 logo: https://raw.githubusercontent.com/jkanev/treetime/master/data/treetime-logo.png
 
 # Build settings
 markdown: kramdown
 theme: jekyll-theme-slate
 plugins:
```

### Comparing `TreeTime-2024.1/docs/_site/404.html` & `TreeTime-2024.2/docs/_site/404.html`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/Makefile` & `TreeTime-2024.2/docs/_site/Makefile`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/abcde01.png` & `TreeTime-2024.2/docs/_site/abcde01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/abcde02.png` & `TreeTime-2024.2/docs/_site/abcde02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/about/index.html` & `TreeTime-2024.2/docs/_site/about/index.html`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/assets/css/style.css` & `TreeTime-2024.2/docs/_site/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/assets/images/sprite_download.png` & `TreeTime-2024.2/docs/_site/assets/images/sprite_download.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/conf.py` & `TreeTime-2024.2/docs/_site/conf.py`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/feed.xml` & `TreeTime-2024.2/docs/_site/feed.xml`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/index.html` & `TreeTime-2024.2/docs/_site/index.html`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/index.md` & `TreeTime-2024.2/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [TreeTime Documentation](https://treetime-data-manager.readthedocs.io/en/latest) on readthedocs.io is constantly being kept up to date.
 
 ## Get TreeTime ##
 
 #### Unpack-and-run Zip Files ####
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run _TreeTime_ or _TreeTime.exe_ from the new folder. Unzip the data package too. Add the program folder to your path.  
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
 (If anybody can help building an executable for other platforms I'd be delighted.)
 
 #### Python / PyPi ####
```

### Comparing `TreeTime-2024.1/docs/_site/index.rst` & `TreeTime-2024.2/docs/_site/index.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/introduction.rst` & `TreeTime-2024.2/docs/_site/introduction.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/linked-trees.dia` & `TreeTime-2024.2/docs/_site/linked-trees.dia`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/linked-trees.png` & `TreeTime-2024.2/docs/_site/linked-trees.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/make.bat` & `TreeTime-2024.2/docs/_site/make.bat`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/releases.rst` & `TreeTime-2024.2/docs/_site/releases.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/screenshot01.png` & `TreeTime-2024.2/docs/_site/screenshot01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/screenshot02.png` & `TreeTime-2024.2/docs/_site/screenshot02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/screenshot03.png` & `TreeTime-2024.2/docs/_site/screenshot03.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/_site/screenshot04.png` & `TreeTime-2024.2/docs/_site/screenshot04.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/abcde01.png` & `TreeTime-2024.2/docs/abcde01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/abcde02.png` & `TreeTime-2024.2/docs/abcde02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/about.md` & `TreeTime-2024.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/conf.py` & `TreeTime-2024.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'TreeTime User Manual'
 copyright = 'CC BY-SA 4.0,  Jacob Kanev'
 author = 'Jacob Kanev'
 
 # The full version, including alpha/beta/rc tags
-release = '2024.1'
+release = '2024.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `TreeTime-2024.1/docs/data-fields.rst` & `TreeTime-2024.2/docs/data-fields.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/data-format.rst` & `TreeTime-2024.2/docs/data-format.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/index.rst` & `TreeTime-2024.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/introduction.rst` & `TreeTime-2024.2/docs/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 Installation
 ------------
 
 Using pre-compiled Binaries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.1](https://github.com/jkanev/treetime/releases/tag/2024.1) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run *TreeTime* or *TreeTime.exe* from the new folder. Unzip the data package too. Add the program folder to your path.
+- Windows, Linux: Go to [github.com/jkanev/treetime/releases/tag/2024.2](https://github.com/jkanev/treetime/releases/tag/2024.2) and download a zipped package for Windows 10, 64 bit, or for Linux 64 bit from there. Unzip it into your program directory and run *TreeTime* or *TreeTime.exe* from the new folder. Unzip the data package too. Add the program folder to your path.
   
   Executable bundles have been created with pyinstaller ([www.pyinstaller.org](http://www.pyinstaller.org)).
 
 - Mac: Mac users please use the Python code (see below). There is no executable for Mac.
   (If anybody can help building an executable for other platforms I'd be delighted.)
 
 Using a PyPi package in Python
```

### Comparing `TreeTime-2024.1/docs/kameri-auth.txt` & `TreeTime-2024.2/docs/kameri-auth.txt`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/linked-trees.dia` & `TreeTime-2024.2/docs/linked-trees.dia`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/linked-trees.png` & `TreeTime-2024.2/docs/linked-trees.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/make.bat` & `TreeTime-2024.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/releases.rst` & `TreeTime-2024.2/docs/releases.rst`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,16 @@
 2024
 ----
 
 * January 2024: Changed node symbol to small circle in text eport (after asking users on social media).
 * February 2024: Implemented min, max, min-string, max-string fields.
 * March 2024: Implemented longtext data field.
 * April 2024: Extended documentation on readthedocs.io. Release **version 2024.1**
+* April 2024: Restructured export area, added name-only export. Made all export options (full tree / branch / node with contect) (all fields / names only) available for all file formats and for both file and clipboard export.
+* April 2024: Release **version 2024.2**
 
 Present
 -------
 
 * Bugfixing
 * Extend documentation on readthedocs.io
 * Add more fields
```

### Comparing `TreeTime-2024.1/docs/screenshot01.png` & `TreeTime-2024.2/docs/screenshot01.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/screenshot02.png` & `TreeTime-2024.2/docs/screenshot02.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/screenshot03.png` & `TreeTime-2024.2/docs/screenshot03.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/screenshot04.png` & `TreeTime-2024.2/docs/screenshot04.png`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/docs/tree-fields.rst` & `TreeTime-2024.2/docs/tree-fields.rst`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/setup.py` & `TreeTime-2024.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='TreeTime',
-    version='2024.1',
+    version='2024.2',
     description='TreeTime is a to-do list manager, test report tool, project manager, family ancestry editor,'
                 'mind-mapping tool, etc. Using TreeTime you can categorise and organise any data in tree structures.'
                 'You can define several trees, each with a different structure, on the same data. You can use functions'
                 '(sums, ratios and means) recursively up the branches of a tree.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jacob Kanev',
```

### Comparing `TreeTime-2024.1/treetime/item.py` & `TreeTime-2024.2/treetime/item.py`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/treetime/mainwindow.py` & `TreeTime-2024.2/treetime/mainwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,71 @@
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(MainWindow.sizePolicy().hasHeightForWidth())
         MainWindow.setSizePolicy(sizePolicy)
         self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.formLayout_2 = QtWidgets.QFormLayout(self.centralwidget)
         self.formLayout_2.setObjectName("formLayout_2")
-        self.toolBox = QtWidgets.QToolBox(parent=self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Expanding)
+        self.splitter = QtWidgets.QSplitter(parent=self.centralwidget)
+        self.splitter.setCursor(QtGui.QCursor(QtCore.Qt.CursorShape.ArrowCursor))
+        self.splitter.setLineWidth(0)
+        self.splitter.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self.splitter.setOpaqueResize(True)
+        self.splitter.setHandleWidth(10)
+        self.splitter.setChildrenCollapsible(False)
+        self.splitter.setObjectName("splitter")
+        self.tableWidget = QtWidgets.QTableWidget(parent=self.splitter)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.toolBox.sizePolicy().hasHeightForWidth())
-        self.toolBox.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.tableWidget.sizePolicy().hasHeightForWidth())
+        self.tableWidget.setSizePolicy(sizePolicy)
+        self.tableWidget.setMinimumSize(QtCore.QSize(300, 0))
+        self.tableWidget.setBaseSize(QtCore.QSize(300, 0))
+        self.tableWidget.setMidLineWidth(0)
+        self.tableWidget.setShowGrid(False)
+        self.tableWidget.setWordWrap(True)
+        self.tableWidget.setRowCount(23)
+        self.tableWidget.setColumnCount(5)
+        self.tableWidget.setObjectName("tableWidget")
+        self.tableWidget.horizontalHeader().setVisible(False)
+        self.tableWidget.horizontalHeader().setCascadingSectionResizes(False)
+        self.tableWidget.horizontalHeader().setDefaultSectionSize(10)
+        self.tableWidget.horizontalHeader().setMinimumSectionSize(10)
+        self.tableWidget.horizontalHeader().setSortIndicatorShown(True)
+        self.tableWidget.horizontalHeader().setStretchLastSection(False)
+        self.tableWidget.verticalHeader().setVisible(False)
+        self.tableWidget.verticalHeader().setCascadingSectionResizes(True)
+        self.tabWidget = QtWidgets.QTabWidget(parent=self.splitter)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.tabWidget.sizePolicy().hasHeightForWidth())
+        self.tabWidget.setSizePolicy(sizePolicy)
+        self.tabWidget.setMinimumSize(QtCore.QSize(500, 0))
+        self.tabWidget.setBaseSize(QtCore.QSize(500, 0))
+        self.tabWidget.setDocumentMode(False)
+        self.tabWidget.setObjectName("tabWidget")
+        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.splitter)
+        self.toolBox = QtWidgets.QToolBox(parent=self.centralwidget)
         self.toolBox.setMinimumSize(QtCore.QSize(250, 0))
         self.toolBox.setMaximumSize(QtCore.QSize(16777215, 16777215))
         self.toolBox.setToolTip("")
         self.toolBox.setObjectName("toolBox")
         self.pageFile = QtWidgets.QWidget()
         self.pageFile.setGeometry(QtCore.QRect(0, 0, 250, 760))
         self.pageFile.setObjectName("pageFile")
         self.formLayout = QtWidgets.QFormLayout(self.pageFile)
         self.formLayout.setFieldGrowthPolicy(QtWidgets.QFormLayout.FieldGrowthPolicy.ExpandingFieldsGrow)
         self.formLayout.setObjectName("formLayout")
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.formLayout.setItem(0, QtWidgets.QFormLayout.ItemRole.SpanningRole, spacerItem)
         self.label_8 = QtWidgets.QLabel(parent=self.pageFile)
         self.label_8.setWordWrap(True)
+        self.label_8.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.NoTextInteraction)
         self.label_8.setObjectName("label_8")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.label_8)
         self.labelCurrentFile = QtWidgets.QLabel(parent=self.pageFile)
         self.labelCurrentFile.setEnabled(True)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Ignored, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
@@ -53,15 +90,15 @@
         self.labelCurrentFile.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setItalic(True)
         self.labelCurrentFile.setFont(font)
         self.labelCurrentFile.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.labelCurrentFile.setWordWrap(True)
         self.labelCurrentFile.setOpenExternalLinks(True)
-        self.labelCurrentFile.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse)
+        self.labelCurrentFile.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.NoTextInteraction)
         self.labelCurrentFile.setObjectName("labelCurrentFile")
         self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.labelCurrentFile)
         spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.formLayout.setItem(3, QtWidgets.QFormLayout.ItemRole.SpanningRole, spacerItem1)
         self.label_5 = QtWidgets.QLabel(parent=self.pageFile)
         font = QtGui.QFont()
         font.setBold(True)
@@ -86,30 +123,67 @@
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_11.setFont(font)
         self.label_11.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.label_11.setObjectName("label_11")
         self.formLayout.setWidget(9, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.label_11)
-        self.radioButtonExportBranch = QtWidgets.QRadioButton(parent=self.pageFile)
+        self.groupBoxSource = QtWidgets.QGroupBox(parent=self.pageFile)
+        self.groupBoxSource.setFlat(True)
+        self.groupBoxSource.setCheckable(False)
+        self.groupBoxSource.setObjectName("groupBoxSource")
+        self.gridLayout = QtWidgets.QGridLayout(self.groupBoxSource)
+        self.gridLayout.setObjectName("gridLayout")
+        self.radioButtonExportTree = QtWidgets.QRadioButton(parent=self.groupBoxSource)
+        self.radioButtonExportTree.setMinimumSize(QtCore.QSize(0, 0))
+        self.radioButtonExportTree.setObjectName("radioButtonExportTree")
+        self.gridLayout.addWidget(self.radioButtonExportTree, 0, 1, 1, 1)
+        self.radioButtonExportBranch = QtWidgets.QRadioButton(parent=self.groupBoxSource)
         self.radioButtonExportBranch.setChecked(True)
         self.radioButtonExportBranch.setObjectName("radioButtonExportBranch")
-        self.formLayout.setWidget(10, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.radioButtonExportBranch)
-        self.radioButtonExportTree = QtWidgets.QRadioButton(parent=self.pageFile)
-        self.radioButtonExportTree.setObjectName("radioButtonExportTree")
-        self.formLayout.setWidget(11, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.radioButtonExportTree)
+        self.gridLayout.addWidget(self.radioButtonExportBranch, 0, 0, 1, 1)
+        self.radioButtonThisNodeWithContext = QtWidgets.QRadioButton(parent=self.groupBoxSource)
+        self.radioButtonThisNodeWithContext.setObjectName("radioButtonThisNodeWithContext")
+        self.gridLayout.addWidget(self.radioButtonThisNodeWithContext, 1, 0, 1, 2)
+        self.formLayout.setWidget(10, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.groupBoxSource)
+        self.groupBoxExport = QtWidgets.QGroupBox(parent=self.pageFile)
+        self.groupBoxExport.setFlat(True)
+        self.groupBoxExport.setObjectName("groupBoxExport")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBoxExport)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.radioButtonExportAllFields = QtWidgets.QRadioButton(parent=self.groupBoxExport)
+        self.radioButtonExportAllFields.setChecked(True)
+        self.radioButtonExportAllFields.setObjectName("radioButtonExportAllFields")
+        self.gridLayout_2.addWidget(self.radioButtonExportAllFields, 0, 0, 1, 1)
+        self.radioButtonExportNamesOnly = QtWidgets.QRadioButton(parent=self.groupBoxExport)
+        self.radioButtonExportNamesOnly.setObjectName("radioButtonExportNamesOnly")
+        self.gridLayout_2.addWidget(self.radioButtonExportNamesOnly, 0, 1, 1, 1)
+        self.formLayout.setWidget(11, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.groupBoxExport)
+        self.groupBoxExportTarget = QtWidgets.QGroupBox(parent=self.pageFile)
+        self.groupBoxExportTarget.setFlat(True)
+        self.groupBoxExportTarget.setObjectName("groupBoxExportTarget")
+        self.gridLayout_3 = QtWidgets.QGridLayout(self.groupBoxExportTarget)
+        self.gridLayout_3.setObjectName("gridLayout_3")
+        self.radioButtonExportToFile = QtWidgets.QRadioButton(parent=self.groupBoxExportTarget)
+        self.radioButtonExportToFile.setChecked(True)
+        self.radioButtonExportToFile.setObjectName("radioButtonExportToFile")
+        self.gridLayout_3.addWidget(self.radioButtonExportToFile, 0, 0, 1, 1)
+        self.radioButtonExportToClipboard = QtWidgets.QRadioButton(parent=self.groupBoxExportTarget)
+        self.radioButtonExportToClipboard.setObjectName("radioButtonExportToClipboard")
+        self.gridLayout_3.addWidget(self.radioButtonExportToClipboard, 0, 1, 1, 1)
+        self.formLayout.setWidget(12, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.groupBoxExportTarget)
         self.label_6 = QtWidgets.QLabel(parent=self.pageFile)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_6.sizePolicy().hasHeightForWidth())
         self.label_6.setSizePolicy(sizePolicy)
         self.label_6.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_6.setObjectName("label_6")
-        self.formLayout.setWidget(12, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
+        self.formLayout.setWidget(13, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
         self.comboBoxExportDepth = QtWidgets.QComboBox(parent=self.pageFile)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.comboBoxExportDepth.sizePolicy().hasHeightForWidth())
         self.comboBoxExportDepth.setSizePolicy(sizePolicy)
         self.comboBoxExportDepth.setObjectName("comboBoxExportDepth")
@@ -120,32 +194,49 @@
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
         self.comboBoxExportDepth.addItem("")
-        self.formLayout.setWidget(12, QtWidgets.QFormLayout.ItemRole.FieldRole, self.comboBoxExportDepth)
-        self.pushButtonExportTxt = QtWidgets.QPushButton(parent=self.pageFile)
-        self.pushButtonExportTxt.setObjectName("pushButtonExportTxt")
-        self.formLayout.setWidget(13, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonExportTxt)
-        self.pushButtonExportCsv = QtWidgets.QPushButton(parent=self.pageFile)
-        self.pushButtonExportCsv.setObjectName("pushButtonExportCsv")
-        self.formLayout.setWidget(14, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonExportCsv)
-        self.pushButtonExportHtmlTiles = QtWidgets.QPushButton(parent=self.pageFile)
-        self.pushButtonExportHtmlTiles.setObjectName("pushButtonExportHtmlTiles")
-        self.formLayout.setWidget(15, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonExportHtmlTiles)
-        self.pushButtonClipBoardTxt = QtWidgets.QPushButton(parent=self.pageFile)
-        self.pushButtonClipBoardTxt.setObjectName("pushButtonClipBoardTxt")
-        self.formLayout.setWidget(17, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonClipBoardTxt)
+        self.formLayout.setWidget(13, QtWidgets.QFormLayout.ItemRole.FieldRole, self.comboBoxExportDepth)
+        self.labelExportFileDescription = QtWidgets.QLabel(parent=self.pageFile)
+        self.labelExportFileDescription.setObjectName("labelExportFileDescription")
+        self.formLayout.setWidget(15, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.labelExportFileDescription)
+        self.labelCurrentExportFile = QtWidgets.QLabel(parent=self.pageFile)
+        font = QtGui.QFont()
+        font.setItalic(True)
+        font.setKerning(True)
+        self.labelCurrentExportFile.setFont(font)
+        self.labelCurrentExportFile.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.labelCurrentExportFile.setWordWrap(True)
+        self.labelCurrentExportFile.setOpenExternalLinks(True)
+        self.labelCurrentExportFile.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.NoTextInteraction)
+        self.labelCurrentExportFile.setObjectName("labelCurrentExportFile")
+        self.formLayout.setWidget(16, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.labelCurrentExportFile)
+        self.pushButtonExport = QtWidgets.QPushButton(parent=self.pageFile)
+        self.pushButtonExport.setObjectName("pushButtonExport")
+        self.formLayout.setWidget(17, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonExport)
         spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.formLayout.setItem(18, QtWidgets.QFormLayout.ItemRole.SpanningRole, spacerItem3)
-        self.pushButtonExportHtmlList = QtWidgets.QPushButton(parent=self.pageFile)
-        self.pushButtonExportHtmlList.setObjectName("pushButtonExportHtmlList")
-        self.formLayout.setWidget(16, QtWidgets.QFormLayout.ItemRole.SpanningRole, self.pushButtonExportHtmlList)
+        self.formLayout.setItem(23, QtWidgets.QFormLayout.ItemRole.SpanningRole, spacerItem3)
+        self.comboBoxExportFormat = QtWidgets.QComboBox(parent=self.pageFile)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.comboBoxExportFormat.sizePolicy().hasHeightForWidth())
+        self.comboBoxExportFormat.setSizePolicy(sizePolicy)
+        self.comboBoxExportFormat.setObjectName("comboBoxExportFormat")
+        self.comboBoxExportFormat.addItem("")
+        self.comboBoxExportFormat.addItem("")
+        self.comboBoxExportFormat.addItem("")
+        self.comboBoxExportFormat.addItem("")
+        self.formLayout.setWidget(14, QtWidgets.QFormLayout.ItemRole.FieldRole, self.comboBoxExportFormat)
+        self.label_15 = QtWidgets.QLabel(parent=self.pageFile)
+        self.label_15.setObjectName("label_15")
+        self.formLayout.setWidget(14, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_15)
         self.toolBox.addItem(self.pageFile, "")
         self.pageEdit = QtWidgets.QWidget()
         self.pageEdit.setGeometry(QtCore.QRect(0, 0, 250, 760))
         self.pageEdit.setMinimumSize(QtCore.QSize(200, 716))
         self.pageEdit.setObjectName("pageEdit")
         self.formLayout1 = QtWidgets.QFormLayout(self.pageEdit)
         self.formLayout1.setFieldGrowthPolicy(QtWidgets.QFormLayout.FieldGrowthPolicy.ExpandingFieldsGrow)
@@ -341,103 +432,76 @@
         self.label_7 = QtWidgets.QLabel(parent=self.pageSettings)
         self.label_7.setObjectName("label_7")
         self.verticalLayout_2.addWidget(self.label_7)
         spacerItem17 = QtWidgets.QSpacerItem(20, 136, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_2.addItem(spacerItem17)
         self.toolBox.addItem(self.pageSettings, "")
         self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.toolBox)
-        self.splitter = QtWidgets.QSplitter(parent=self.centralwidget)
-        self.splitter.setCursor(QtGui.QCursor(QtCore.Qt.CursorShape.ArrowCursor))
-        self.splitter.setLineWidth(0)
-        self.splitter.setOrientation(QtCore.Qt.Orientation.Horizontal)
-        self.splitter.setOpaqueResize(True)
-        self.splitter.setHandleWidth(10)
-        self.splitter.setChildrenCollapsible(False)
-        self.splitter.setObjectName("splitter")
-        self.tableWidget = QtWidgets.QTableWidget(parent=self.splitter)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tableWidget.sizePolicy().hasHeightForWidth())
-        self.tableWidget.setSizePolicy(sizePolicy)
-        self.tableWidget.setMinimumSize(QtCore.QSize(300, 0))
-        self.tableWidget.setBaseSize(QtCore.QSize(300, 0))
-        self.tableWidget.setMidLineWidth(0)
-        self.tableWidget.setShowGrid(False)
-        self.tableWidget.setWordWrap(True)
-        self.tableWidget.setRowCount(23)
-        self.tableWidget.setColumnCount(5)
-        self.tableWidget.setObjectName("tableWidget")
-        self.tableWidget.horizontalHeader().setVisible(False)
-        self.tableWidget.horizontalHeader().setCascadingSectionResizes(False)
-        self.tableWidget.horizontalHeader().setDefaultSectionSize(10)
-        self.tableWidget.horizontalHeader().setMinimumSectionSize(10)
-        self.tableWidget.horizontalHeader().setSortIndicatorShown(True)
-        self.tableWidget.horizontalHeader().setStretchLastSection(False)
-        self.tableWidget.verticalHeader().setVisible(False)
-        self.tableWidget.verticalHeader().setCascadingSectionResizes(True)
-        self.tabWidget = QtWidgets.QTabWidget(parent=self.splitter)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.tabWidget.sizePolicy().hasHeightForWidth())
-        self.tabWidget.setSizePolicy(sizePolicy)
-        self.tabWidget.setMinimumSize(QtCore.QSize(500, 0))
-        self.tabWidget.setBaseSize(QtCore.QSize(500, 0))
-        self.tabWidget.setDocumentMode(False)
-        self.tabWidget.setObjectName("tabWidget")
-        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.splitter)
         MainWindow.setCentralWidget(self.centralwidget)
         self.actionQuit = QtGui.QAction(parent=MainWindow)
         self.actionQuit.setObjectName("actionQuit")
 
         self.retranslateUi(MainWindow)
-        self.toolBox.setCurrentIndex(1)
         self.tabWidget.setCurrentIndex(-1)
+        self.toolBox.setCurrentIndex(1)
         self.actionQuit.triggered.connect(MainWindow.close) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "Tree Time"))
+        self.tableWidget.setSortingEnabled(False)
         self.label_8.setText(_translate("MainWindow", "Connected to Data File:"))
         self.labelCurrentFile.setToolTip(_translate("MainWindow", "The current data file. All changes made are silently written to this file."))
         self.labelCurrentFile.setText(_translate("MainWindow", "[current file name]"))
         self.label_5.setText(_translate("MainWindow", "Load and Save"))
         self.pushButtonNewFromTemplate.setToolTip(_translate("MainWindow", "<b>Create a new tree sheet from a template file</b><br/><br/>• Lets you choose a template in a file dialog, then choose a file location for your new file.<br/>• Changes are silently written to the new file."))
         self.pushButtonNewFromTemplate.setText(_translate("MainWindow", "New from Template"))
         self.pushButtonLoadFile.setToolTip(_translate("MainWindow", "<b>Load an existing tree sheet</b><br/><br/>Subsequent changes will be written silently to the loaded file."))
         self.pushButtonLoadFile.setText(_translate("MainWindow", "Load File"))
         self.pushButtonSaveToFile.setToolTip(_translate("MainWindow", "<b>Save the current file to a new location</b><br/><br/>Subsequent changes will be written silently to the new location."))
         self.pushButtonSaveToFile.setText(_translate("MainWindow", "Save As"))
         self.label_11.setText(_translate("MainWindow", "Export"))
-        self.radioButtonExportBranch.setText(_translate("MainWindow", "Selected Branch"))
-        self.radioButtonExportTree.setText(_translate("MainWindow", "Entire tree"))
+        self.radioButtonExportTree.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export the entire tree</span></p><p>Export all branches to file or clipboard.</p></body></html>"))
+        self.radioButtonExportTree.setText(_translate("MainWindow", "Whole tree"))
+        self.radioButtonExportBranch.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export selected branch</span></p><p>The selected node and all its children will be exported to file or clipboard.</p></body></html>"))
+        self.radioButtonExportBranch.setText(_translate("MainWindow", "This branch"))
+        self.radioButtonThisNodeWithContext.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export the current node</span></p><p>The selected node will be exported to file or clipboard, inside a collapsed tree showing only direct parents and their siblings. The collapsed tree starts at the root node, or at the level set in the <span style=\" font-style:italic;\">depth </span>box.</p></body></html>"))
+        self.radioButtonThisNodeWithContext.setText(_translate("MainWindow", "This node with context"))
+        self.radioButtonExportAllFields.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export all fields</span></p><p>All tree fields visible in the GUI will be exported.</p></body></html>"))
+        self.radioButtonExportAllFields.setText(_translate("MainWindow", "All fields"))
+        self.radioButtonExportNamesOnly.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export only names</span></p><p>No fields, only node names, will be exported.</p></body></html>"))
+        self.radioButtonExportNamesOnly.setText(_translate("MainWindow", "Names only"))
+        self.radioButtonExportToFile.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export to file.</span></p><p>The export will be saved in a file. When clicking [Export], a file dialog opens to select a target file.</p></body></html>"))
+        self.radioButtonExportToFile.setText(_translate("MainWindow", "To file"))
+        self.radioButtonExportToClipboard.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export to clipboard.</span></p><p>When the [Export] button is clicked, the exported data will be in the clipboard and can be pasted (Menu/Paste or Ctrl+V) it into any document.</p></body></html>"))
+        self.radioButtonExportToClipboard.setText(_translate("MainWindow", "To clipboard"))
         self.label_6.setText(_translate("MainWindow", "Depth  "))
-        self.comboBoxExportDepth.setToolTip(_translate("MainWindow", "<b>Select a level down to which the current branch is copied</b>"))
+        self.comboBoxExportDepth.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select a level down to which the current branch is copied.</span></p><p>For the options &quot;This branch&quot; and &quot;Whole tree&quot; this will show the respective level of children.</p><p>For the option &quot;This node with content&quot; this will show the summary path starting at the respective level, counting from the top.</p></body></html>"))
         self.comboBoxExportDepth.setItemText(0, _translate("MainWindow", "all levels"))
         self.comboBoxExportDepth.setItemText(1, _translate("MainWindow", "1 level"))
         self.comboBoxExportDepth.setItemText(2, _translate("MainWindow", "2 levels"))
         self.comboBoxExportDepth.setItemText(3, _translate("MainWindow", "3 levels"))
         self.comboBoxExportDepth.setItemText(4, _translate("MainWindow", "4 levels"))
         self.comboBoxExportDepth.setItemText(5, _translate("MainWindow", "5 levels"))
         self.comboBoxExportDepth.setItemText(6, _translate("MainWindow", "6 levels"))
         self.comboBoxExportDepth.setItemText(7, _translate("MainWindow", "7 levels"))
         self.comboBoxExportDepth.setItemText(8, _translate("MainWindow", "8 levels"))
         self.comboBoxExportDepth.setItemText(9, _translate("MainWindow", "9 levels"))
         self.comboBoxExportDepth.setItemText(10, _translate("MainWindow", "10 levels"))
-        self.pushButtonExportTxt.setToolTip(_translate("MainWindow", "<b>Export the current branch to a text file</b><br/><br/>• The file will contain all tree fields.<br/>• Text graphics show the tree structure."))
-        self.pushButtonExportTxt.setText(_translate("MainWindow", "Text to File"))
-        self.pushButtonExportCsv.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export the current branch or tree to a CSV file</span><br/><br/>• The file will contain all tree fields.<br/>• The first field (&quot;Tree&quot;) shows the tree structure.</p><p>• The second field (&quot;Name&quot;) shows the name.</p></body></html>"))
-        self.pushButtonExportCsv.setText(_translate("MainWindow", "CSV to File"))
-        self.pushButtonExportHtmlTiles.setToolTip(_translate("MainWindow", "<b>Export the current tree to a text file.</b><br/><br/>• The file will contain all tree fields.<br/>• Text graphics show the tree structure."))
-        self.pushButtonExportHtmlTiles.setText(_translate("MainWindow", "HTML (Tiles) to File"))
-        self.pushButtonClipBoardTxt.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export the current tree as text to the clipboard.</span><br/><br/>• The file will contain all tree fields.<br/>• Text graphics show the tree structure.</p></body></html>"))
-        self.pushButtonClipBoardTxt.setText(_translate("MainWindow", "Text to Clipboard"))
-        self.pushButtonExportHtmlList.setText(_translate("MainWindow", "HTML (List) to File"))
+        self.labelExportFileDescription.setText(_translate("MainWindow", "Last exported file:"))
+        self.labelCurrentExportFile.setText(_translate("MainWindow", "[last exported file name]"))
+        self.pushButtonExport.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Export.</span><br/>Starts the export to a file after showing a file selection dialog, or to the clipboard.</p></body></html>"))
+        self.pushButtonExport.setText(_translate("MainWindow", "Export"))
+        self.comboBoxExportFormat.setToolTip(_translate("MainWindow", "<html><head/><body><p><span style=\" font-weight:600;\">Select export file format</span></p><p>• HTML (Tiles) — html file, nodes are tiles within tiles<br/>• HTML (List) — html file, nodes are list lines<br/>• Text/Unicode — pure text file with text graphics<br/>• CSV — csv file with heading, first column is the tree structure, next are name and fields<p></body></html>"))
+        self.comboBoxExportFormat.setItemText(0, _translate("MainWindow", "HTML (Tiles)"))
+        self.comboBoxExportFormat.setItemText(1, _translate("MainWindow", "HTML (List)"))
+        self.comboBoxExportFormat.setItemText(2, _translate("MainWindow", "Text/Unicode"))
+        self.comboBoxExportFormat.setItemText(3, _translate("MainWindow", "CSV"))
+        self.label_15.setText(_translate("MainWindow", "Format"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.pageFile), _translate("MainWindow", "File"))
         self.label.setText(_translate("MainWindow", "Insert New Nodes"))
         self.pushButtonNewChild.setToolTip(_translate("MainWindow", "<b>Create a new item and link it as a child to the selected node</b><br/><br/>Only this tree will be affected."))
         self.pushButtonNewChild.setText(_translate("MainWindow", "New Child"))
         self.pushButtonNewSibling.setToolTip(_translate("MainWindow", "<b>Create a new item and link it as a sibling next to the selected node</b><br/><br/>Only this tree will be affected."))
         self.pushButtonNewSibling.setText(_translate("MainWindow", "New Sibling"))
         self.pushButtonNewParent.setToolTip(_translate("MainWindow", "<b>Create a new item and insert it as a parent above the selected node</b><br/><br/>Only this tree will be affected."))
@@ -485,14 +549,13 @@
         self.toolBox.setItemText(self.toolBox.indexOf(self.pageStructure), _translate("MainWindow", "View Form"))
         self.label_9.setText(_translate("MainWindow", "Look and Feel"))
         self.label_10.setText(_translate("MainWindow", "About"))
         self.label_7.setText(_translate("MainWindow", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
 "p, li { white-space: pre-wrap; }\n"
 "</style></head><body style=\" font-family:\'Noto Sans\'; font-size:10pt; font-weight:400; font-style:normal;\">\n"
-"<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">     TreeTime 2024.1</p>\n"
+"<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">     TreeTime 2024.2</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">     Official website:<br />     <a href=\"https://github.com/jkanev/treetime\"><span style=\" text-decoration: underline; color:#2980b9;\">tree-time.info</span></a></p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">     Updates and source code:<br />     <a href=\"https://github.com/jkanev/treetime\"><span style=\" text-decoration: underline; color:#2980b9;\">github.com/jkanev/treetime</span></a></p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">    Documentation:<br />     <a href=\"https://treetime-data-manager.readthedocs.io\"><span style=\" text-decoration: underline; color:#2980b9;\">treetime-data-manager.</span></a><br />     <a href=\"https://treetime-data-manager.readthedocs.io\"><span style=\" text-decoration: underline; color:#2980b9;\">readthedocs.io</span></a></p></body></html>"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.pageSettings), _translate("MainWindow", "Settings"))
-        self.tableWidget.setSortingEnabled(False)
         self.actionQuit.setText(_translate("MainWindow", "Quit"))
```

### Comparing `TreeTime-2024.1/treetime/test.py` & `TreeTime-2024.2/treetime/test.py`

 * *Files identical despite different names*

### Comparing `TreeTime-2024.1/treetime/tree.py` & `TreeTime-2024.2/treetime/tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -499,14 +499,43 @@
         :return: Array with text wrapped at 70 chars, preserving newlines, but trimming space (no double new lines)
         """
         lines = []
         for line in [s.strip() for s in raw_lines.split('\n')]:
             lines += wrap(line, 70) or '\n'
         return lines
 
+    def _evaluateContext(self, fields, context):
+        """
+        Helper function, calculates fieds, context, and whether we're in the current node, based on the context path.
+        :param fields: the initial "fields" variable. If the context is "False", that variable will be
+            returned in the "fields" return value unchanged. This is important in non-context display settings.
+        :param context: The path of the node that is to be displayed as "node with context".
+        :return: fields, children, context_current - three bools indicating whether the calling node should display
+            its children (yes, if it is a sibling in the ancestry path, otherwise no), its fields (yes, if it is the
+            target node and we have fields enabled in the gui, otherwise no), and whether it is the target
+            node (interesting for separate css things)
+        """
+        children = True
+        fields_local = fields
+        context_current = False
+        if context:
+            fields_local = False
+            children = False
+
+            # display children if we're a direct ancestor
+            if len(self.path) <= len(context) and self.path == context[:len(self.path)]:
+                children = True
+
+                # display fields if we're the actual target node
+                if len(self.path) == len(context):
+                    fields_local = fields
+                    context_current = True
+
+        return fields_local, children, context_current
+
     def map(self, function, parameter, depthFirst):
         ''' Applies the function to each node in the tree. The function must receive one parameter and return one
         parameter. The return value is used as parameter for the next function call. The value Parameter is used in the
         first call.'''
         
         # if depthFirst then recurse first and apply later
         if depthFirst:
@@ -542,15 +571,15 @@
             s += " [" + name + "] " + str(field.getString())
         print(s)
         
         # recurse
         for i in range(len(self.children)):
             self.children[i].printForest(indent + 1)
 
-    def to_csv(self, first=True, depth=-1):
+    def to_csv(self, fields=True, context=False, first=True, depth=-1):
         """
         Create a csv representation of the current branch.
         :fieldOrder: The order of fields in the tree
         :first: If this is the first call (first=True), add a title line with field names,
                 on recursive calls (=False) don't
         :depth: A number listing how many levels should be in the export
         :return: CSV. Quotes become double-quotes, fields with commas, line breaks or quotes are quoted,
@@ -565,14 +594,16 @@
 
         def clean_field(text):
             text.replace('"', '""')
             if '"' in text or '\n' in text or ',' in text:
                 text = '"' + text + '"'
             return text
 
+        # evaluate context
+        fields_local, children, context_current = self._evaluateContext(fields, context)
         csv = ""
 
         # find root node
         tree = self
         while tree.parent.parent is not None:
             tree = tree.parent
 
@@ -596,35 +627,33 @@
         field += self.name
         csv += clean_field(field) + ','
 
         # add node name
         csv += self.name
 
         # add fields
-        for f in tree.fieldOrder:
-            csv += ',' + clean_field(self.fields[f].getString())
+        if fields_local:
+            for f in tree.fieldOrder:
+                csv += ',' + clean_field(self.fields[f].getString())
         csv += '\n'
 
         # add children
-        if depth:
-            sorted_children = sorted(self.children, key=lambda c: c.name)
-        else:
-            sorted_children = []
-        if len(sorted_children):
-            for i in range(len(sorted_children)):
-                csv += sorted_children[i].to_csv(first=False, depth=depth-1)
+        if depth and children:
+            for c in sorted(self.children, key=lambda x: x.name):
+                csv += c.to_csv(first=False, fields=fields, context=context, depth=depth - 1)
 
         # return
         return csv
 
-    def to_txt(self, lastitem=[], depth=-1):
+    def to_txt(self, fields=True, context=False, lastitem=[], depth=-1):
         """
         Create a text representation of the current branch.
         :param lastitem: A list of booleans showing whether the great-grandparent, grandparent, parent, is the
                          last item of the list of siblings
+        :param fields: if true, all fields are included, if false, only node names are exported (no fields)
         :return: a string like this:
 
                     █ abc
                       def
 
                     █ abc
                     │ def
@@ -646,17 +675,20 @@
                        │
                        ┕━━█ abc
                             def
         """
 
         text = ""
 
+        # evaluate context
+        fields_local, children, context_current = self._evaluateContext(fields, context)
+
         # create leading tree graphics
         # please pay attention: The spaces in the graphic strings are special unicode figure spaces
-        if self.children and depth:
+        if children and self.children and depth:
             pre_node_prefix = ""
             first_line_prefix = "●  "
             line_prefix = "│  "
         else:
             pre_node_prefix = ""
             first_line_prefix = "●  "
             line_prefix = "   "
@@ -691,61 +723,66 @@
             line = line == '\n' and line or line + '\n'
             if first:
                 text += first_line_prefix + line
                 first = False
             else:
                 text += line_prefix + "    " + line
 
-        for name, field in self.fields.items():
+        if fields_local:
+            for name, field in self.fields.items():
 
-            # wrap field content, larger bits of text start with a newline
-            lines = Node._wrap_lines(field.getString())
+                # wrap field content, larger bits of text start with a newline
+                lines = Node._wrap_lines(field.getString())
 
-            # empty array if only whitespace content
-            if lines == ['\n']:
-                lines = []
-
-            if len(lines) > 1:
-                lines = [''] + lines
-
-            # assemble final text with tree decorations
-            first = True
-            for line in lines:
-                line = line == '\n' and line or line + '\n'
-                if first:
-                    text += line_prefix + name + ": " + line
-                    first = False
-                else:
-                    text += line_prefix + "    " + line
+                # empty array if only whitespace content
+                if lines == ['\n']:
+                    lines = []
+
+                if len(lines) > 1:
+                    lines = [''] + lines
+
+                # assemble final text with tree decorations
+                first = True
+                for line in lines:
+                    line = line == '\n' and line or line + '\n'
+                    if first:
+                        text += line_prefix + name + ": " + line
+                        first = False
+                    else:
+                        text += line_prefix + "    " + line
 
         # recurse
-        if depth:
+        if children and depth:
             sorted_children = sorted(self.children, key=lambda c: c.name)
         else:
             sorted_children = []
         if len(sorted_children) > 1:
             childprefix = lastitem.copy()
             childprefix.append(False)
             for i in range(len(sorted_children)-1):
-                text += sorted_children[i].to_txt(childprefix, depth-1)
+                text += sorted_children[i].to_txt(fields=fields, context=context, lastitem=childprefix, depth=depth-1)
         if len(sorted_children):
             childprefix = lastitem.copy()
             childprefix.append(True)
-            text += sorted_children[-1].to_txt(childprefix, depth-1)
+            text += sorted_children[-1].to_txt(fields=fields, context=context, lastitem=childprefix, depth=depth-1)
 
         # return
         return text
 
-    def to_html(self, header=False, footer=False, style='tiles', background='blue', depth=-1, current_depth=0):
+    def to_html(self, header=False, footer=False, fields=True, context=False, style='tiles', background='blue',
+                depth=-1, current_depth=0):
+
+        # evaluate context
+        fields_local, children, context_current = self._evaluateContext(fields, context)
 
         # background colours
         next_background = {'blue': 'green', 'green': 'red', 'red': 'blue'}
 
         # page header
-        if header and style=='tiles':
+        if header and style == 'tiles' and not context:
             html = '<!DOCTYPE html><html lang="en"><meta charset="utf-8"><title>TreeTime Export</title><style>' \
                    'body {font-family: sans-serif; color: black; background-color: white; font-size: 0.8em;} '\
                    'em {color: #555;}' \
                    'div.red {background-color: rgba(80, 0, 0, 0.03);}' \
                    'div.green {background-color: rgba(0, 80, 0, 0.03);}' \
                    'div.blue {background-color: rgba(0, 0, 80, 0.03);}' \
                    'div.node {position: relative; float: left; border: 1px solid; margin: 0.6em; padding: 0.6em; width: min-content; border-radius: 1em; border-color: #CCC;}' \
@@ -767,14 +804,45 @@
                    'div.mean {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
                    'div.mean-percent {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
                    'div.ratio {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
                    'div.ratio-percent {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
                    'div.node-name {position: relative; float: left; width: 10em; margin: 0.3em; padding: 0.3em; }' \
                    'div.node-path {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
                    '</style></head><body>'
+        elif header and style == 'tiles' and context:
+            html = '<!DOCTYPE html><html lang="en"><meta charset="utf-8"><title>TreeTime Export</title><style>' \
+                   'body {font-family: sans-serif; color: black; background-color: white; font-size: 1.2em;} ' \
+                   'em {color: #555;}' \
+                   'div.red {background-color: rgba(80, 0, 0, 0.03);}' \
+                   'div.green {background-color: rgba(0, 80, 0, 0.03);}' \
+                   'div.blue {background-color: rgba(0, 0, 80, 0.03);}' \
+                   'div.node {position: relative; float: left; border: 1px solid; margin: 0.6em; padding: 0.6em; width: min-content; border-radius: 1em; border-color: #CCC;}' \
+                   'div.name {padding: 0.2em; margin: 0.2em; position: relative; float: left; width: 12em;} ' \
+                   'div.name_current {padding: 0.2em; margin: 0.2em; position: relative; float: left; width: 48.5em;} ' \
+                   'div.fields {position: relative; float: left; clear: left; width: 74em; border-top: 1px solid; border-color: #808080;} ' \
+                   'div.children {position: relative; float: left; clear: left; width: max-content;} ' \
+                   'div.string {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.min-string {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.max-string {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.set {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.text {position: relative; float: left; width: 40em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.url {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.sum {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.sum-time {position: relative; float: left; width: 10em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.difference {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.difference-time {position: relative; float: left; width: 10em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.min {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.max {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.mean {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.mean-percent {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.ratio {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.ratio-percent {position: relative; float: left; width: 5em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.node-name {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
+                   'div.node-path {position: relative; float: left; width: 40em; margin: 0.3em; padding: 0.3em; }' \
+                   '</style></head><body>'
         elif header and style == 'list':
             html = '<!DOCTYPE html><html lang="en"><meta charset="utf-8"><title>TreeTime Export</title><style>' \
                    'body {font-family: sans-serif; color: black; background-color: white; font-size: 0.8em;} ' \
                    'em {color: #555;}' \
                    'div.red {background-color: rgba(80, 0, 0, 0.03);}' \
                    'div.green {background-color: rgba(0, 80, 0, 0.03);}' \
                    'div.blue {background-color: rgba(0, 0, 80, 0.03);}' \
@@ -802,75 +870,89 @@
                    'div.node-path {position: relative; float: left; width: 20em; margin: 0.3em; padding: 0.3em; }' \
                    '</style></head><body>'
         else:
             html = ''
 
         # node header
         html += '<div class="node {}">'.format(background)
-        needed_columns = 1    # the amount of columns needed by this child
+        needed_columns = context_current and 5 or 1    # the amount of columns needed by this child
 
         # node name
-        font_size = 1.0 + 1.0 / (1.0 + current_depth)
+        if context:
+            if context_current:
+                font_size = 1.5
+            else:
+                font_size = 0.5 + 1.0 / (2.0 + max((len(context) - len(self.path)), 0))  # 1 em for target, decay to 0.5
+        else:
+            font_size = 1.0 + 1.0 / (1.0 + current_depth)  # start with 2 em, exponentially decay to 0.5 em
         if style == 'tiles':
-            html += '<div class="name" style="font-size: {:0.2f}em">{}</div>'.format(font_size, self.name)
+            if context_current:
+                html += '<div class="name_current" style="font-size: {:0.2f}em">{}</div>'.format(font_size, self.name)
+            else:
+                html += '<div class="name" style="font-size: {:0.2f}em">{}</div>'.format(font_size, self.name)
         if style == 'list':
             html += '<div class="name" style="font-size: {:0.2f}em; ' \
                     'width: {:0.2f}em;">{}</div>'.format(font_size, (20.0 - (1.2*current_depth))/font_size, self.name)
 
         # node fields
-        html += '<div class="fields">'
+        if fields_local:
+            html += '<div class="fields">'
+            for name, field in self.fields.items():
+                content = field.getString().strip()
+                if content or (style == 'list'):   # in tile mode empty fields are hidden, in list mode always displayed
+                    content = content.replace('\n', '<br/>')
+                    if field.fieldType == "url":
+                        html += '<div class="{}"><em>{}</em><br/><a href="{}">{}</a></div>'.format(
+                            field.fieldType, name, content, len(content) > 40 and content[:37]+"..." or content)
+                    else:
+                        html += '<div class="{}"><em>{}</em><br/>{}</div>'.format(field.fieldType, name, content)
+            html += '</div>'
 
-        for name, field in self.fields.items():
-            content = field.getString().strip()
-            if content or (style == 'list'):   # in tile mode empty fields are hidden, in list mode always displayed
-                content = content.replace('\n', '<br/>')
-                if field.fieldType == "url":
-                    html += '<div class="{}"><em>{}</em><br/><a href="{}">{}</a></div>'.format(
-                        field.fieldType, name, content, len(content) > 40 and content[:37]+"..." or content)
-                else:
-                    html += '<div class="{}"><em>{}</em><br/>{}</div>'.format(field.fieldType, name, content)
-        html += '</div>'
+        child_html = ""
 
         # children
-        child_count = 0
-        sorted_children = sorted(self.children, key=lambda c: c.name)
-        group_open = False
-        for i in range(len(sorted_children)):
-
-            # write next child
-            background = next_background[background]
-            child_columns = 1     # number of columns needed by child sub-branch
-            if depth:
-                child_columns, child_html = sorted_children[i].to_html(background=background, depth=depth-1,
-                                                                       current_depth=current_depth+1, style=style)
-
-            # start new child group on first child in group of 5, or if child needs more columns than available
-            if child_columns > 5-child_count:
-                child_count = 0
-            if child_count == 0:
-                if group_open:
+        if children:
+
+            child_count = 0
+            sorted_children = sorted(self.children, key=lambda c: c.name)
+            group_open = False
+            for i in range(len(sorted_children)):
+
+                # write next child
+                background = next_background[background]
+                child_columns = 1     # number of columns needed by child sub-branch
+                if depth:
+                    child_columns, child_html = sorted_children[i].to_html(background=background, depth=depth-1,
+                                                                           fields=fields, context=context,
+                                                                           current_depth=current_depth+1, style=style)
+
+                # start new child group on first child in group of 5, or if child needs more columns than available
+                if child_columns > 5-child_count:
+                    child_count = 0
+                if child_count == 0:
+                    if group_open:
+                        html += '</div>'
+                    html += '<div class="children">'
+                    group_open = True
+
+                # add html to main html
+                html += child_html
+                child_count += child_columns
+                needed_columns = max(needed_columns, min(child_count, 5))
+
+                # close child group after fourth child of after node with children
+                if child_count >= 5:
+                    child_count = 0
+                if child_count == 0:
                     html += '</div>'
-                html += '<div class="children">'
-                group_open = True
+                    group_open = False
 
-            # add html to main html
-            html += child_html
-            child_count += child_columns
-            needed_columns = max(needed_columns, min(child_count, 5))
-
-            # close child group after fourth child of after node with children
-            if child_count >= 5:
-                child_count = 0
-            if child_count == 0:
+            # node footer
+            if group_open:
                 html += '</div>'
-                group_open = False
-
-        # node footer
-        if group_open:
-            html += '</div>'
         html += "</div>"
 
         # page footer
         if footer:
             html += '</body></html>'
 
         # finished.
@@ -1145,15 +1227,15 @@
             n = item.trees[treeindex][0]
             while n >= len(self.children):
                 self.addChild()
             self.children[n].createPathTo(item, treeindex, 1, self.fields)
 
     def findNode(self, path):
         """
-        Sort the item into the forest, creating existing nodes on the fly if missing.
+        Find the node at a given path. Calls the respective function of the Node class.
         """
 
         # per tree: loop over all nodes, creating if necessary
         return super().findNode(path, 0)
 
     def writeToString(self):
         string = "tree " + json.dumps(self.name) + "\n"
```

### Comparing `TreeTime-2024.1/treetime/treetime.py` & `TreeTime-2024.2/treetime/treetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -398,19 +398,15 @@
         self.pushButtonCopyNodeChild.clicked.connect(lambda: self.createNode("child", True))
         self.pushButtonCopyNodeSibling.clicked.connect(lambda: self.createNode("sibling", True))
         self.pushButtonCopyNodeParent.clicked.connect(lambda: self.createNode("parent", True))
         self.pushButtonCopyBranchSibling.clicked.connect(lambda: self.createNode("sibling", True, True))
         self.pushButtonNewFromTemplate.clicked.connect(self.pushButtonNewFromTemplateClicked)
         self.pushButtonLoadFile.clicked.connect(self.pushButtonLoadFileClicked)
         self.pushButtonSaveToFile.clicked.connect(self.pushButtonSaveToFileClicked)
-        self.pushButtonExportTxt.clicked.connect(self.pushButtonExportTxtClicked)
-        self.pushButtonClipBoardTxt.clicked.connect(self.pushButtonClipBoardTxtClicked)
-        self.pushButtonExportCsv.clicked.connect(self.pushButtonExportCsvClicked)
-        self.pushButtonExportHtmlList.clicked.connect(lambda: self.pushButtonExportHtmlClicked(style='list'))
-        self.pushButtonExportHtmlTiles.clicked.connect(lambda: self.pushButtonExportHtmlClicked(style='tiles'))
+        self.pushButtonExport.clicked.connect(self.pushButtonExportClicked)
         self.pushButtonRemoveNode.clicked.connect(self.pushButtonRemoveNodeClicked)
         self.pushButtonDeleteNode.clicked.connect(self.pushButtonDeleteNodeClicked)
         self.pushButtonRemoveBranch.clicked.connect(lambda: self.moveCurrentItemToNewParent(self.currentTree, None))
         self.pushButtonDeleteBranch.clicked.connect(self.pushButtonDeleteBranchClicked)
         self.pushButtonDataFields.clicked.connect(self.pushButtonDataFieldsClicked)
         self.pushButtonTreeFields.clicked.connect(self.pushButtonTreeFieldsClicked)
         self.tableWidget.cellChanged.connect(self.tableWidgetCellChanged)
@@ -437,14 +433,17 @@
         self.gridInitialised = False
         self.editMode = 'content'     # one of 'content', 'tree', or 'data'
 
         # init application settings
         print("loading system settings...")
         self.settings = QtCore.QSettings('FreeSoftware', 'TreeTime')
 
+        # show last exported file
+        self.labelCurrentExportFile.setText(self.settings.value('exportFile') or "[last exported file]")
+
         # load last file
         print("opening last file...")
         if filename:
             loadFile = filename
         else:
             loadFile = self.settings.value('lastFile')
 
@@ -496,19 +495,15 @@
         self.pushButtonCopyNodeChild.setEnabled(state)
         self.pushButtonCopyNodeSibling.setEnabled(state)
         self.pushButtonCopyNodeParent.setEnabled(state)
         self.pushButtonCopyBranchSibling.setEnabled(state)
         self.pushButtonNewFromTemplate.setEnabled(state)
         self.pushButtonLoadFile.setEnabled(state)
         self.pushButtonSaveToFile.setEnabled(state)
-        self.pushButtonExportTxt.setEnabled(state)
-        self.pushButtonClipBoardTxt.setEnabled(state)
-        self.pushButtonExportCsv.setEnabled(state)
-        self.pushButtonExportHtmlList.setEnabled(state)
-        self.pushButtonExportHtmlTiles.setEnabled(state)
+        self.pushButtonExport.setEnabled(state)
         self.pushButtonRemoveNode.setEnabled(state)
         self.pushButtonDeleteNode.setEnabled(state)
         self.pushButtonRemoveBranch.setEnabled(state)
         self.pushButtonDeleteBranch.setEnabled(state)
         self.pushButtonDataFields.setEnabled(state)
         self.pushButtonTreeFields.setEnabled(state)
 
@@ -693,74 +688,14 @@
         if file != '':
             self.loadFile(file)
             self.setWindowTitle("TreeTime - " + file)
             self.settings.setValue('fileDir', os.path.dirname(file))
             self.settings.setValue('lastFile', file)
             self.labelCurrentFile.setText(file)
 
-    def pushButtonExportCsvClicked(self):
-        """
-        Callback for the csv export. Asks for a file name, then writes branch text export into it.
-        """
-        if self.currentItem:
-            fileDir = self.settings.value('fileDir') or ''
-            file = QtWidgets.QFileDialog.getSaveFileName(self, "Export to Plain Text", fileDir, 'CSV (Comma-separated Values) Files (*.csv)')[0]
-            if file != '':
-                with open(file, "w") as f:
-
-                    # get depth
-                    depth = self.comboBoxExportDepth.currentIndex() - 1
-
-                    # export current branch
-                    if self.radioButtonExportBranch.isChecked():
-                        currentNode = self.currentItem.viewNodes[self.currentTree]
-                        csv = currentNode.to_csv(depth=depth)
-                        f.write(csv)
-
-                    # export entire tree
-                    if self.radioButtonExportTree.isChecked():
-                        rootNode = self.forest.children[self.currentTree]
-                        children = sorted(rootNode.children, key=lambda a: a.name)
-                        first = True
-                        for c in children:
-                            f.write(c.to_csv( first=first, depth=depth))
-                            first = False
-
-    def pushButtonClipBoardTxtClicked(self):
-        """
-        Callback for the txt clipboard export. Writes branch text export into clipboard.
-        """
-        if self.currentItem:
-
-            # get depth
-            depth = self.comboBoxExportDepth.currentIndex() - 1
-            txt = ''
-
-            # export current branch
-            if self.radioButtonExportBranch.isChecked():
-                currentNode = self.currentItem.viewNodes[self.currentTree]
-                txt += currentNode.to_txt(depth=depth)
-
-            # export entire tree
-            if self.radioButtonExportTree.isChecked():
-                rootNode = self.forest.children[self.currentTree]
-                children = sorted(rootNode.children, key=lambda a: a.name)
-                for c in children:
-                    txt += '\n'
-                    txt += c.to_txt(depth=depth)
-                    txt += '\n'
-
-            # save to clipboard
-            clipboard = QGuiApplication.clipboard()
-            clipboard.setText(txt, QClipboard.Mode.Clipboard)
-            clipboard.setText(txt, QClipboard.Mode.FindBuffer)
-            if clipboard.supportsSelection():
-                clipboard.setText(txt, QClipboard.Mode.Selection)
-            time.sleep(0.001)
-
     def pushButtonDataFieldsClicked(self):
         """
         Callback for the data field edit button. Toggles the tree-field edit mode.
         """
         if self.editMode == 'data':
             self.changeEditMode('content')
         else:
@@ -771,80 +706,134 @@
         Callback for the data field edit button. Toggles the tree-field edit mode.
         """
         if self.editMode == 'tree':
             self.changeEditMode('content')
         else:
             self.changeEditMode('tree')
 
-    def pushButtonExportTxtClicked(self):
+    def pushButtonExportClicked(self):
         """
-        Callback for the txt export. Asks for a file name, then writes branch text export into it.
+        Callback for the text/html/csv export. Asks for a file name, then writes branch text export into it.
         """
+
         if self.currentItem:
-            fileDir = self.settings.value('fileDir') or ''
-            file = QtWidgets.QFileDialog.getSaveFileName(self, "Export to Plain Text", fileDir, 'Text Files (*.txt)')[0]
-            if file != '':
-                with open(file, "w") as f:
 
-                    # get depth
-                    depth = self.comboBoxExportDepth.currentIndex() - 1
+            # read file format
+            exportFormat = self.comboBoxExportFormat.currentText()
+            allFields = self.radioButtonExportAllFields.isChecked()
+
+            # Select target file or cancel
+            exportToFile = self.radioButtonExportToFile.isChecked()
+            file = ""
+            if exportToFile:
+                extensions = {
+                    "HTML (Tiles)": "HTML Files (*.html)",
+                    "HTML (List)": "HTML Files (*.html)",
+                    "Text/Unicode": "Text Files (*.txt)",
+                    "CSV": "CSV (Comma-separated Values) Files (*.csv)"
+                }
+                fileDir = os.path.dirname(self.settings.value('exportFile')) or ''
+                file = QtWidgets.QFileDialog.getSaveFileName(self, "Export to " + exportFormat, fileDir,
+                                                             extensions[exportFormat])[0]
+                if not file:
+                    return
 
-                    # export current branch
-                    if self.radioButtonExportBranch.isChecked():
-                        currentNode = self.currentItem.viewNodes[self.currentTree]
-                        txt = currentNode.to_txt(depth=depth)
-                        f.write(txt)
-
-                    # export entire tree
-                    if self.radioButtonExportTree.isChecked():
-                        rootNode = self.forest.children[self.currentTree]
-                        children = sorted(rootNode.children, key=lambda a: a.name)
-                        for c in children:
-                            f.write('\n')
-                            f.write(c.to_txt(depth=depth))
-                            f.write('\n')
+            # The target string for file write / clipboard write
+            data = ""
+            depth = self.comboBoxExportDepth.currentIndex() - 1
 
-    def pushButtonExportHtmlClicked(self, style):
-        """
-        Callback for the html export. Asks for a file name, then writes branch html export into it.
-        """
-        if self.currentItem:
-            fileDir = self.settings.value('fileDir') or ''
-            file = QtWidgets.QFileDialog.getSaveFileName(self, "Export to HTML", fileDir, 'HTML Files (*.html)')[0]
-            if file != '':
-                with open(file, "w") as f:
+            # export current branch
+            if self.radioButtonExportBranch.isChecked():
 
-                    # get depth
-                    depth = self.comboBoxExportDepth.currentIndex() - 1
+                currentNode = self.currentItem.viewNodes[self.currentTree]
+                if currentNode:
 
-                    # export current branch
-                    if self.radioButtonExportBranch.isChecked():
-                        currentNode = self.currentItem.viewNodes[self.currentTree]
-                        if currentNode:
-                            dummy, txt = currentNode.to_html(header=True, footer=True, depth=depth, style=style)
+                    # write to data string
+                    if exportFormat == "CSV":
+                        data = currentNode.to_csv(depth=depth, fields=allFields)
+                    elif exportFormat == "Text/Unicode":
+                        data = currentNode.to_txt(depth=depth, fields=allFields)
+                    elif exportFormat == "HTML (List)":
+                        dummy, data = currentNode.to_html(header=True, footer=True, depth=depth, fields=allFields,
+                                                          style='list')
+                    else:
+                        dummy, data = currentNode.to_html(header=True, footer=True, depth=depth, fields=allFields,
+                                                          style='tiles')
+                else:
+                    data = ("No branch selected, export is empty")
+
+            # export entire tree
+            elif self.radioButtonExportTree.isChecked():
+
+                # pick up the source
+                rootNode = self.forest.children[self.currentTree]
+                children = sorted(rootNode.children, key=lambda a: a.name)
+
+                # write data string
+                if exportFormat == "CSV":
+                    first = True
+                    for c in children:
+                        data += c.to_csv(first=first, depth=depth, fields=allFields)
+                        first = False
+                elif exportFormat == "Text/Unicode":
+                    for c in children:
+                        data += '\n'
+                        data += c.to_txt(depth=depth, fields=allFields)
+                        data += '\n'
+                else:
+                    next_background = {'blue': 'green', 'green': 'red', 'red': 'blue'}
+                    background = 'blue'
+                    style = (exportFormat == "HTML (List)" and "list") or "tiles"
+                    for c in range(0, len(children)):
+                        if c == 0:
+                            background = next_background[background]
+                            data += children[c].to_html(header=True, background=background, depth=depth,
+                                                        fields=allFields, style=style)[1]
+                        elif c == len(children) - 1:
+                            background = next_background[background]
+                            data += children[c].to_html(footer=True, background=background, depth=depth,
+                                                        fields=allFields, style=style)[1]
                         else:
-                            txt = ("No branch selected, export is empty")
-                        f.write(txt)
+                            background = next_background[background]
+                            data += children[c].to_html(background=background, depth=depth,
+                                                        fields=allFields, style=style)[1]
+
+            # export current node with context
+            else:
+                path = self.currentItem.trees[self.currentTree]
+                currentNode = self.forest.children[self.currentTree].findNode(path[:1])
+                if currentNode:
+
+                    # write to data string
+                    if exportFormat == "CSV":
+                        data = currentNode.to_csv(depth=depth, fields=allFields, context=path)
+                    elif exportFormat == "Text/Unicode":
+                        data = currentNode.to_txt(depth=depth, fields=allFields, context=path)
+                    elif exportFormat == "HTML (List)":
+                        dummy, data = currentNode.to_html(header=True, footer=True, depth=depth, context=path,
+                                                          fields=allFields, style='list')
+                    else:
+                        dummy, data = currentNode.to_html(header=True, footer=True, depth=depth, context=path,
+                                                          fields=allFields, style='tiles')
+                else:
+                    data = ("No branch selected, export is empty")
 
-                    # export entire tree
-                    if self.radioButtonExportTree.isChecked():
-                        rootNode = self.forest.children[self.currentTree]
-                        children = sorted(rootNode.children, key=lambda a: a.name)
-                        next_background = {'blue': 'green', 'green': 'red', 'red': 'blue'}
-                        background = 'blue'
-                        for c in range(0, len(children)):
-                            if c == 0:
-                                background = next_background[background]
-                                f.write(children[c].to_html(header=True, background=background, depth=depth, style=style)[1])
-                            elif c == len(children)-1:
-                                background = next_background[background]
-                                f.write(children[c].to_html(footer=True, background=background, depth=depth, style=style)[1])
-                            else:
-                                background = next_background[background]
-                                f.write(children[c].to_html(background=background, depth=depth, style=style)[1])
+            # save to file or to clipboard
+            if exportToFile:
+                with open(file, "w") as f:
+                    f.write(data)
+                self.labelCurrentExportFile.setText(file)
+                self.settings.setValue("exportFile", file)
+            else:
+                clipboard = QGuiApplication.clipboard()
+                clipboard.setText(data, QClipboard.Mode.Clipboard)
+                clipboard.setText(data, QClipboard.Mode.FindBuffer)
+                if clipboard.supportsSelection():
+                    clipboard.setText(data, QClipboard.Mode.Selection)
+                time.sleep(0.001)
 
     def pushButtonNewFromTemplateClicked(self):
         """
         Callback for the new-from-template button. Loads new file and immediately saves it to a different file.
         """
 
         # First load template file
```

