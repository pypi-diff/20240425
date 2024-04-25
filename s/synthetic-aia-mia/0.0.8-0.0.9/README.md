# Comparing `tmp/synthetic_aia_mia-0.0.8.tar.gz` & `tmp/synthetic_aia_mia-0.0.9.tar.gz`

## Comparing `synthetic_aia_mia-0.0.8.tar` & `synthetic_aia_mia-0.0.9.tar`

### file list

```diff
@@ -1,128 +1,139 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/.gitlab-ci.yml
--rw-r--r--   0        0        0   158065 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/aia_soft.log
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/conf.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/make.bat
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/synthetic.fetch_data.rst
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/synthetic.generator.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/synthetic.predictor.rst
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/synthetic.rst
--rw-r--r--   0        0        0   173815 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.doctree
--rw-r--r--   0        0        0    28619 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.fetch_data.doctree
--rw-r--r--   0        0        0     8790 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.generator.doctree
--rw-r--r--   0        0        0    49626 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.predictor.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    11070 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/genindex.html
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/index.html
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/objects.inv
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/search.html
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/synthetic.fetch_data.html
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/synthetic.generator.html
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/synthetic.html
--rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/synthetic.predictor.html
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/index.html
--rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/adult.html
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/split.html
--rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/utk.html
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/generator/example.html
--rw-r--r--   0        0        0    37239 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/predictor/adult.html
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_sources/synthetic.fetch_data.rst.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_sources/synthetic.generator.rst.txt
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_sources/synthetic.predictor.rst.txt
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_sources/synthetic.rst.txt
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0   288304 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/IEEEtran.cls
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/background.tex
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/biblio.bib
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/compile.sh
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/conclusion.tex
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/introduction.tex
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/list_of_conf_journals
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.aux
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.bbl
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.blg
--rw-r--r--   0        0        0    26312 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.log
--rw-r--r--   0        0        0    88773 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.pdf
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.tex
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/main.toc
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/methodology.tex
--rwxr-xr-x   0        0        0      133 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/pdfcompress.sh
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/related.tex
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/results.tex
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/figure/tikz/data.tex
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/figure/tikz/data_flow/step1.tex
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/figure/tikz/data_flow/step2.tex
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/figure/tikz/data_flow/step3.tex
--rw-r--r--   0        0        0   764784 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/conference-latex-template_10-17-19.zip
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/.DS_Store
--rw-r--r--   0        0        0   288304 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran.cls
--rw-r--r--   0        0        0   671626 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran_HOWTO.pdf
--rw-r--r--   0        0        0   125971 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.pdf
--rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.tex
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/fig1.png
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/remove_cache.sh
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/aia/__init__.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/aia/soft.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/experiments/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/experiments/__main__.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/experiments/adult.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/__init__.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/adult.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/split.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/utk.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/generator/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/generator/adult.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/generator/example.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/metrics/__init__.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/mia/__init__.py
--rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/mia/ml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/predictor/__init__.py
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/predictor/adult.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/predictor/utk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/__init__.py
--rw-r--r--   0        0        0   126428 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/aia_soft.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/aia/__init__.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/aia/aia_soft.log
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/aia/hard.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/aia/soft.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/data_management/__init__.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/data_management/dataset.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/data_management/fetch.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/data_management/split.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/experiement/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/experiement/adult.py
--rw-r--r--   0        0        0   532736 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/experiement/aia_soft.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/experiement/mia.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/generator/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/generator/adult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/metrics/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/metrics/metrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/mia/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/mia/ml.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/mia/random_fusion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/predictor/__init__.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/predictor/adult_nn.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/predictor/stop_train_condition.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/test/predictor/utk_nn
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/.gitignore
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/README.md
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0   158065 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/aia_soft.log
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/synthetic.fetch_data.rst
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/synthetic.generator.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/synthetic.predictor.rst
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/synthetic.rst
+-rw-r--r--   0        0        0   173815 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.doctree
+-rw-r--r--   0        0        0    28619 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.fetch_data.doctree
+-rw-r--r--   0        0        0     8790 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.generator.doctree
+-rw-r--r--   0        0        0    49626 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.predictor.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    11070 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/index.html
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/search.html
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/synthetic.fetch_data.html
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/synthetic.generator.html
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/synthetic.html
+-rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/synthetic.predictor.html
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/index.html
+-rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/adult.html
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/split.html
+-rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/utk.html
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/generator/example.html
+-rw-r--r--   0        0        0    37239 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/predictor/adult.html
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_sources/synthetic.fetch_data.rst.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_sources/synthetic.generator.rst.txt
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_sources/synthetic.predictor.rst.txt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_sources/synthetic.rst.txt
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0   288304 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/IEEEtran.cls
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/background.tex
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/biblio.bib
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/compile.sh
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/conclusion.tex
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/introduction.tex
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/list_of_conf_journals
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.aux
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.bbl
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.blg
+-rw-r--r--   0        0        0    26312 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.log
+-rw-r--r--   0        0        0    88773 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.pdf
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.tex
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/main.toc
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/methodology.tex
+-rwxr-xr-x   0        0        0      133 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/pdfcompress.sh
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/related.tex
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/results.tex
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/figure/tikz/data.tex
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/figure/tikz/data_flow/step1.tex
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/figure/tikz/data_flow/step2.tex
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/figure/tikz/data_flow/step3.tex
+-rw-r--r--   0        0        0   764784 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/conference-latex-template_10-17-19.zip
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/.DS_Store
+-rw-r--r--   0        0        0   288304 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran.cls
+-rw-r--r--   0        0        0   671626 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran_HOWTO.pdf
+-rw-r--r--   0        0        0   125971 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.pdf
+-rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.tex
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/fig1.png
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/remove_cache.sh
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/aia/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/aia/soft.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/experiments/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/experiments/__main__.py
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/experiments/adult.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/__init__.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/adult.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/split.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/utk.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/generator/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/generator/adult.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/generator/example.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/metrics/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/mia/__init__.py
+-rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/mia/ml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/predictor/__init__.py
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/predictor/adult.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/predictor/utk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aaaaaaaaaaaa
+-rw-r--r--   0        0        0   177011 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia_soft.log
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/log
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/remove_cache.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/after
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/aia_soft.log
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/before
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/hard.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/high_lvl_interface.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/label_encoder.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/log
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/aia/soft.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/data_management/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/data_management/dataset.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/data_management/fetch.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/data_management/split.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/__init__.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/aaaaaaaaaaaa
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/adult.py
+-rw-r--r--   0        0        0    67602 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/aia_soft.log
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/bbaaa
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/experiement/out
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/generator/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/generator/adult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/metrics/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/mia/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/mia/ml.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/mia/random_fusion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/predictor/__init__.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/predictor/adult_nn.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/predictor/stop_train_condition.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/test/predictor/utk_nn
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 synthetic_aia_mia-0.0.9/PKG-INFO
```

### Comparing `synthetic_aia_mia-0.0.8/aia_soft.log` & `synthetic_aia_mia-0.0.9/aia_soft.log`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/Makefile` & `synthetic_aia_mia-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/conf.py` & `synthetic_aia_mia-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/make.bat` & `synthetic_aia_mia-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/synthetic.fetch_data.rst` & `synthetic_aia_mia-0.0.9/docs/synthetic.fetch_data.rst`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/environment.pickle` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/index.doctree` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.doctree` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.doctree`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.fetch_data.doctree` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.fetch_data.doctree`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.generator.doctree` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.generator.doctree`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/doctrees/synthetic.predictor.doctree` & `synthetic_aia_mia-0.0.9/docs/build/doctrees/synthetic.predictor.doctree`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/genindex.html` & `synthetic_aia_mia-0.0.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/index.html` & `synthetic_aia_mia-0.0.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/objects.inv` & `synthetic_aia_mia-0.0.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/py-modindex.html` & `synthetic_aia_mia-0.0.9/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/search.html` & `synthetic_aia_mia-0.0.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/searchindex.js` & `synthetic_aia_mia-0.0.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/synthetic.fetch_data.html` & `synthetic_aia_mia-0.0.9/docs/build/html/synthetic.fetch_data.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/synthetic.generator.html` & `synthetic_aia_mia-0.0.9/docs/build/html/synthetic.generator.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/synthetic.html` & `synthetic_aia_mia-0.0.9/docs/build/html/synthetic.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/synthetic.predictor.html` & `synthetic_aia_mia-0.0.9/docs/build/html/synthetic.predictor.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/index.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/adult.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/adult.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/split.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/split.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/fetch_data/utk.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/fetch_data/utk.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/generator/example.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/generator/example.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_modules/synthetic/predictor/adult.html` & `synthetic_aia_mia-0.0.9/docs/build/html/_modules/synthetic/predictor/adult.html`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_sources/synthetic.fetch_data.rst.txt` & `synthetic_aia_mia-0.0.9/docs/build/html/_sources/synthetic.fetch_data.rst.txt`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/alabaster.css` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/basic.css` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/doctools.js` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/language_data.js` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/pygments.css` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/searchtools.js` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/docs/build/html/_static/sphinx_highlight.js` & `synthetic_aia_mia-0.0.9/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/IEEEtran.cls` & `synthetic_aia_mia-0.0.9/paper/IEEEtran.cls`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/background.tex` & `synthetic_aia_mia-0.0.9/paper/background.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/biblio.bib` & `synthetic_aia_mia-0.0.9/paper/biblio.bib`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.aux` & `synthetic_aia_mia-0.0.9/paper/main.aux`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.bbl` & `synthetic_aia_mia-0.0.9/paper/main.bbl`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.blg` & `synthetic_aia_mia-0.0.9/paper/main.blg`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.log` & `synthetic_aia_mia-0.0.9/paper/main.log`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.pdf` & `synthetic_aia_mia-0.0.9/paper/main.pdf`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.tex` & `synthetic_aia_mia-0.0.9/paper/main.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/main.toc` & `synthetic_aia_mia-0.0.9/paper/main.toc`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/methodology.tex` & `synthetic_aia_mia-0.0.9/paper/methodology.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/figure/tikz/data.tex` & `synthetic_aia_mia-0.0.9/paper/figure/tikz/data.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/figure/tikz/data_flow/step1.tex` & `synthetic_aia_mia-0.0.9/paper/figure/tikz/data_flow/step1.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/figure/tikz/data_flow/step3.tex` & `synthetic_aia_mia-0.0.9/paper/figure/tikz/data_flow/step3.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/conference-latex-template_10-17-19.zip` & `synthetic_aia_mia-0.0.9/paper/template/conference-latex-template_10-17-19.zip`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/.DS_Store` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/.DS_Store`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran.cls` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran.cls`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran_HOWTO.pdf` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/IEEEtran_HOWTO.pdf`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.pdf` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.pdf`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.tex` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/conference_101719.tex`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/paper/template/Conference-LaTeX-template_10-17-19/fig1.png` & `synthetic_aia_mia-0.0.9/paper/template/Conference-LaTeX-template_10-17-19/fig1.png`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/aia/__init__.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/aia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
     def fit(self, dadata):
         """Fit a neural network to predict sensitive attribute from soft labels.
 
         :param dadata: Auxiliary data for aia training.
         :type dadata: fetch_data.Dataset
         """
+        print(dadata.load())
         self.model["race"].fit(dadata, "race")
         self.model["sex"].fit(dadata, "sex")
 
     def predict(self, dadata):
         """Use previously trained neural network to infer senstivies attribute and append prediction to input data.
 
         :param dadata: Auxiliary data for aia evaluation.
```

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/aia/soft.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/mia/ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Define structures to manage and interface a fully connected neural network for attribute inference attack using soft labels."""
+"""Define structures to manage and interface a fully connected neural network for membership inference attack."""
 
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import StratifiedKFold
 from sklearn.preprocessing import StandardScaler
 from functools import partial
 import tempfile
 import os
-import logging
-logging.basicConfig(filename='aia_soft.log', encoding='utf-8', level=logging.DEBUG)
 
 #Pytorch 
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.utils.data import Dataset
 
@@ -28,17 +26,17 @@
     """Pytorch dataset to handle aia with soft labels."""
     def __init__(self, data):
         """Make data conversion for pytorch integration.
 
         :param data: dataset to convert.
         :type data: pandas.dataframe
         """
-        y = data["attribute"].to_numpy()
+        y = data["member"].to_numpy()
         self.y = torch.from_numpy(y).type(torch.float)
-        self.x = torch.from_numpy(data[["soft0","soft1"]].to_numpy()).type(torch.float)
+        self.x = torch.from_numpy(data["loss"].to_numpy().reshape(-1,1)).type(torch.float)
 
     def __len__(self):
         """Length of dataset."""
         return len(self.y)
 
     def __getitem__(self, idx):
         """Fetch ith data point.
@@ -81,40 +79,36 @@
         :rtype: torch.tensor
         """
         x = self.fc1(x)
         x = self.relu(x)
         x = self.fc2(x)
         x = self.relu(x)
         x = self.fc3(x)
-        x = self.sigmoid(x)
+        #x = self.sigmoid(x)
         return x
 
-class AiaNN:
+class MiaNN:
     """Wrapper arround pytorch neural network. Interfare for hyper parameter optimisation using raytune."""
     def __init__(self):
         self.trained = False
 
-    def fit(self, dadata, attrib):
+    def fit(self, dadata):
         """Train and tune hyper parameters.
         
-        :parameter data: Dataset the will be split for training and hyper parameter tuning. Dataset must contain columns called "soft0" and "soft1" used as features.
+        :parameter data: Dataset the will be split for training and hyper parameter tuning. Dataset must contain columns called "loss" used as features and "member" used as labels.
         :type dadata: fetch_data.Dataset
-        :param attrib: Sensitive attribute to attack. A column of dadata.
-        :type attrib: str
         """
 
-        data = dadata.load()[["soft0", "soft1",attrib]]
-        x = data[["soft0", "soft1"]].to_numpy()
+        data = dadata.load()[["loss","member"]]
+        x = data["loss"].to_numpy().reshape(-1,1)
         self.scaler = StandardScaler()
         self.scaler.fit(x)
         x = self.scaler.transform(x)
-        x = pd.DataFrame(x,columns=["soft0", "soft1"])
+        x = pd.DataFrame(x,columns=["loss"])
         data.replace(x,inplace=True)
-        data.rename({attrib:"attribute"},axis=1,inplace=True)
-        self.attrib = attrib
 
         search_space = {
                 "l1": tune.choice([2 ** i for i in range(9)]),
                 "l2": tune.choice([2 ** i for i in range(9)]),
                 "lr": tune.loguniform(1e-4, 1e-1),
                 "batch_size": tune.choice([8, 16, 32, 64, 128])
                 }
@@ -133,28 +127,26 @@
 
         tune_config = tune.TuneConfig(
                 num_samples=20,
                 scheduler=asha_scheduler,
                 search_alg=hyperopt_search
                 )
 
-        logging.debug(data)
         tuner = tune.Tuner(
                 partial(_train,data=data,stand_alone=False),
                 tune_config=tune_config,
                 run_config=train.RunConfig(stop=_stop_train)
                 )
 
         results = tuner.fit()
 
         #Real training on full train dataset (no validation)
         #Using best hyper parameters 
         best_result = results.get_best_result("loss","min")
-        num_mod = len(np.unique(data["attribute"].to_numpy()))
-        best_trained_model = TabularNN(2,best_result.config["l1"], best_result.config["l2"],num_mod)
+        best_trained_model = TabularNN(1,best_result.config["l1"], best_result.config["l2"],2)
         device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
         checkpoint_path = os.path.join(best_result.checkpoint.to_directory(), "checkpoint.pt")
 
         model_state, optimizer_state = torch.load(checkpoint_path)
         best_trained_model.load_state_dict(model_state)
         
@@ -162,42 +154,42 @@
         self.trained=True
 
     def predict(self, dadata):
         """Use a trained TabularNN to predict label of dataset.
 
         :param dadata: Dataset to evaluate.
         :type dadata: fetch_data.Dataset
-        :return: Input dataset completed with hard labels, soft labels and loss.
+        :return: Input dataset completed with mia result as a column called "mia".
         :rtype: fetch_data.Dataset
         """
         if not(self.trained):
             raise AssertionError(f"{self} must be trained prioir to predict")
         with torch.no_grad():
             criterion = nn.CrossEntropyLoss()
             data = dadata.load()
-            x = data[["soft0", "soft1"]].to_numpy()
+            x = data["loss"].to_numpy().reshape(-1,1)
             x = self.scaler.transform(x)
             x = torch.from_numpy(x).float()
             output = self.model(x)
             yhard = np.argmax(output,axis=1)
-        data[self.attrib+"_soft"] = yhard
+        data["mia"] = yhard
         dadata.update(data)
         return dadata
 
 
 def _pandas_to_dataset(data):
     """Split pands dataset into training and validation and convert into pytorch dataset.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
     :return: Training and validation dataset (train,validation).
     :rtype: tuple of torch.utils.data.dataset
     """
     skf = StratifiedKFold(shuffle=True,random_state=123)
-    for train,validation in skf.split(data,data["attribute"]):
+    for train,validation in skf.split(data,data["member"]):
         pass
     train_dataset = AiaDataset(data.iloc[train])
     validation_dataset = AiaDataset(data.iloc[validation])
     return train_dataset, validation_dataset
 
         
 def _stop_train(trial_id, result):
@@ -225,16 +217,15 @@
     """Train TabularNN with ray_tune hyper parameter tuning.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
     :param stand_alone: (Optional default=False) If True _train does not use ray.tune and return the trained model.
     :type return_model: bool
     """
-    num_mod = len(np.unique(data["attribute"].to_numpy()))
-    net = TabularNN(2,config["l1"],config["l2"],num_mod)
+    net = TabularNN(1,config["l1"],config["l2"],2)
 
     device = "cpu"
     if torch.cuda.is_available():
         device = "cuda:0"
     net.to(device)
 
     criterion = nn.CrossEntropyLoss()
```

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/experiments/adult.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/experiments/adult.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,29 @@
         metrics[attrib] = {}
         for labtype in ["hard","soft"]:
             metrics[attrib][labtype] = {}
             for metric in metric_lst:
                 metrics[attrib][labtype][metric] = []
 
     data = dadata.load()
+    with open("aaaaaaaaaaaa", "w") as f:
+        f.write(str(data))
+
     skf = StratifiedKFold(random_state=123, shuffle=True)
-    data_train = Dataset()
-    data_test = Dataset()
-    for train,test in skf.split(data,data["PINCP"]):
-        data_train.update(data.iloc[train])
-        data_test.update(data.iloc[test])
-        aia = Aia()
-        aia.fit(data_train)
-        pred = aia.predict(data_test)
-        for attrib in ["sex", "race"]:
+    for attrib in ["sex","race"]:
+        for train,test in skf.split(data,data[attrib]):
+            data_train = Dataset()
+            data_test = Dataset()
+
+
+            data_train.update((data.iloc[train]).reset_index(drop=True))
+            data_test.update((data.iloc[test]).reset_index(drop=True))
+            aia = Aia()
+            aia.fit(data_train)
+            pred = aia.predict(data_test)
             for labtype in ["hard","soft"]:
                 for metric in metric_lst:
                     value = balanced_accuracy(pred, attrib, f"{attrib}_{labtype}")
                     metrics[attrib][labtype][metric] += [value]
 
     return metrics
```

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/__init__.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/__init__.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/adult.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/adult.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/split.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/split.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/fetch_data/utk.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/fetch_data/utk.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/generator/adult.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/generator/adult.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/generator/example.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/generator/example.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/metrics/__init__.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/mia/__init__.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/mia/__init__.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/mia/ml.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/predictor/adult.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Define structures to manage and interface a fully connected neural network for membership inference attack."""
+"""Define structures to manage and interface a fully connected neural network for adult."""
 
 import numpy as np
-import pandas as pd
 from sklearn.model_selection import StratifiedKFold
 from sklearn.preprocessing import StandardScaler
+import pandas as pd
 from functools import partial
 import tempfile
 import os
 
 #Pytorch 
 import torch
 import torch.nn as nn
@@ -18,25 +18,25 @@
 from ray import train, tune
 from ray.tune.schedulers import ASHAScheduler
 from ray.tune.search.hyperopt import HyperOptSearch
 from ray.train import Checkpoint
 
 from ..fetch_data import Dataset
 
-class AiaDataset(Dataset):
-    """Pytorch dataset to handle aia with soft labels."""
+class AdultDataset(Dataset):
+    """Pytorch dataset to handle adult data."""
     def __init__(self, data):
         """Make data conversion for pytorch integration.
 
         :param data: dataset to convert.
         :type data: pandas.dataframe
         """
-        y = data["member"].to_numpy()
-        self.y = torch.from_numpy(y).type(torch.float)
-        self.x = torch.from_numpy(data["loss"].to_numpy().reshape(-1,1)).type(torch.float)
+        y = data["PINCP"].to_numpy()
+        self.y = torch.from_numpy(y).type(torch.float) 
+        self.x = torch.from_numpy(data.drop("PINCP", axis=1).to_numpy()).type(torch.float)
 
     def __len__(self):
         """Length of dataset."""
         return len(self.y)
 
     def __getitem__(self, idx):
         """Fetch ith data point.
@@ -79,35 +79,36 @@
         :rtype: torch.tensor
         """
         x = self.fc1(x)
         x = self.relu(x)
         x = self.fc2(x)
         x = self.relu(x)
         x = self.fc3(x)
-        x = self.sigmoid(x)
+        #x = self.sigmoid(x)
         return x
 
-class MiaNN:
+class AdultNN:
     """Wrapper arround pytorch neural network. Interfare for hyper parameter optimisation using raytune."""
     def __init__(self):
         self.trained = False
 
     def fit(self, dadata):
         """Train and tune hyper parameters.
         
-        :parameter data: Dataset the will be split for training and hyper parameter tuning. Dataset must contain columns called "loss" used as features and "member" used as labels.
+        :parameter data: Dataset the will be split for training and hyper parameter tuning. Dataset must contain a column called "PINCP" used as training label.
         :type dadata: fetch_data.Dataset
         """
 
-        data = dadata.load()[["loss","member"]]
-        x = data["loss"].to_numpy().reshape(-1,1)
+        data = dadata.load()
+        x = data.drop("PINCP",axis=1).to_numpy()
+        self.columns = data.columns.drop("PINCP")
         self.scaler = StandardScaler()
         self.scaler.fit(x)
         x = self.scaler.transform(x)
-        x = pd.DataFrame(x,columns=["loss"])
+        x = pd.DataFrame(x,columns=data.columns.drop("PINCP"))
         data.replace(x,inplace=True)
 
         search_space = {
                 "l1": tune.choice([2 ** i for i in range(9)]),
                 "l2": tune.choice([2 ** i for i in range(9)]),
                 "lr": tune.loguniform(1e-4, 1e-1),
                 "batch_size": tune.choice([8, 16, 32, 64, 128])
@@ -138,61 +139,65 @@
                 )
 
         results = tuner.fit()
 
         #Real training on full train dataset (no validation)
         #Using best hyper parameters 
         best_result = results.get_best_result("loss","min")
-        best_trained_model = TabularNN(1,best_result.config["l1"], best_result.config["l2"],2)
-        device = "cuda:0" if torch.cuda.is_available() else "cpu"
+        best_trained_model = TabularNN(len(data.columns)-1,best_result.config["l1"], best_result.config["l2"],2)
 
         checkpoint_path = os.path.join(best_result.checkpoint.to_directory(), "checkpoint.pt")
 
         model_state, optimizer_state = torch.load(checkpoint_path)
         best_trained_model.load_state_dict(model_state)
         
         self.model = best_trained_model
         self.trained=True
 
     def predict(self, dadata):
         """Use a trained TabularNN to predict label of dataset.
 
         :param dadata: Dataset to evaluate.
         :type dadata: fetch_data.Dataset
-        :return: Input dataset completed with mia result as a column called "mia".
+        :return: Input dataset completed with hard labels, soft labels and loss.
         :rtype: fetch_data.Dataset
         """
         if not(self.trained):
             raise AssertionError(f"{self} must be trained prioir to predict")
         with torch.no_grad():
             criterion = nn.CrossEntropyLoss()
             data = dadata.load()
-            x = data["loss"].to_numpy().reshape(-1,1)
+            x = data[self.columns].to_numpy()
             x = self.scaler.transform(x)
             x = torch.from_numpy(x).float()
             output = self.model(x)
+            labels = torch.from_numpy(data["PINCP"].to_numpy()).long()
+            loss = criterion(output,labels)
+            ysoft = output
             yhard = np.argmax(output,axis=1)
-        data["mia"] = yhard
+        data["soft0"] = ysoft[:,0]
+        data["soft1"] = ysoft[:,1]
+        data["hard"] = yhard
+        data["loss"] = loss
         dadata.update(data)
         return dadata
 
-
 def _pandas_to_dataset(data):
     """Split pands dataset into training and validation and convert into pytorch dataset.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
     :return: Training and validation dataset (train,validation).
     :rtype: tuple of torch.utils.data.dataset
     """
     skf = StratifiedKFold(shuffle=True,random_state=123)
-    for train,validation in skf.split(data,data["member"]):
+    for train,validation in skf.split(data,data["PINCP"]):
         pass
-    train_dataset = AiaDataset(data.iloc[train])
-    validation_dataset = AiaDataset(data.iloc[validation])
+    train_dataset = AdultDataset(data.iloc[train])
+    validation_dataset = AdultDataset(data.iloc[validation])
     return train_dataset, validation_dataset
 
         
 def _stop_train(trial_id, result):
     """Tell tray tune to stop training after 20 iterations or when overfitting.
 
     :param trial_id:
@@ -217,15 +222,15 @@
     """Train TabularNN with ray_tune hyper parameter tuning.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
     :param stand_alone: (Optional default=False) If True _train does not use ray.tune and return the trained model.
     :type return_model: bool
     """
-    net = TabularNN(1,config["l1"],config["l2"],2)
+    net = TabularNN(len(data.columns)-1,config["l1"],config["l2"],2)
 
     device = "cpu"
     if torch.cuda.is_available():
         device = "cuda:0"
     net.to(device)
 
     criterion = nn.CrossEntropyLoss()
```

### Comparing `synthetic_aia_mia-0.0.8/src/synthetic_aia_mia/predictor/adult.py` & `synthetic_aia_mia-0.0.9/src/synthetic_aia_mia/predictor/utk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,105 @@
-"""Define structures to manage and interface a fully connected neural network for adult."""
+"""Define structures to manage and interface a fully connected neural network for UTKfaces."""
 
 import numpy as np
 from sklearn.model_selection import StratifiedKFold
-from sklearn.preprocessing import StandardScaler
-import pandas as pd
-from functools import partial
-import tempfile
-import os
 
 #Pytorch 
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.utils.data import Dataset
 
 #Ray tune
 from ray import train, tune
 from ray.tune.schedulers import ASHAScheduler
 from ray.tune.search.hyperopt import HyperOptSearch
-from ray.train import Checkpoint
 
-from ..fetch_data import Dataset
+from functools import partial
 
-class AdultDataset(Dataset):
+class UtkDataset(Dataset):
     """Pytorch dataset to handle adult data."""
     def __init__(self, data):
         """Make data conversion for pytorch integration.
 
         :param data: dataset to convert.
-        :type data: pandas.dataframe
+        :type data: dictionary of numpy.ndarray
         """
-        y = data["PINCP"].to_numpy()
-        self.y = torch.from_numpy(y).type(torch.float) 
-        self.x = torch.from_numpy(data.drop("PINCP", axis=1).to_numpy()).type(torch.float)
+        self.y = torch.from_numpy(data["y"]).type(torch.float)
+        self.x = torch.from_numpy(data["x"]).type(torch.float)
 
     def __len__(self):
         """Length of dataset."""
         return len(self.y)
 
     def __getitem__(self, idx):
         """Fetch ith data point.
 
         :param idx: Data index.
         :type idx: int or array of int
         """
         return self.x[idx], self.y[idx]
 
-class TabularNN(nn.Module):
-    """Pytorch neural network for adult."""
-    def __init__(self, input_size, l1, l2, output_size):
+class CNN(nn.Module):
+    """Pytorch convulutional neural network for UTKfaces."""
+    def __init__(self, input_size, c,l1, l2, output_size):
         """Sets layers for a neural network.
 
         :param input_size: Number of features.
         :type input_size: int
-        :param hidden_size: Number of neurons/hidden layer.
-        :type hidden_size: int
+        :param c: Number channels after convolution.
+        :type c: int
         :param l1: Size of the first layer.
         :type l1: int
         :param l2: Size of the second layer.
         :type l2: int
         :param output_size: Number classes in the labels.
         :type output_size: int
         """
 
-        super(TabularNN, self).__init__()
-        self.fc1 = nn.Linear(input_size, l1)
+        super(CNN, self).__init__()
+        self.conv1 = nn.Conv2d(3, c, kernel_size=3, stride=1, padding=1)
+        self.pool = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.fc1 = nn.Linear(c*6*6, l1)
         self.relu = nn.ReLU()
         self.fc2 = nn.Linear(l1, l2)
         self.fc3 = nn.Linear(l2, output_size)
         self.sigmoid = nn.Sigmoid()
 
     def forward(self, x):
         """Forward pass in the neural network.
 
         :param x: Data points.
         :type x: torch.tensor
         :return: Neural network function applied to x.
         :rtype: torch.tensor
         """
-        x = self.fc1(x)
+        x = self.conv1(x)
         x = self.relu(x)
+        x = self.pool(x)
         x = self.fc2(x)
         x = self.relu(x)
         x = self.fc3(x)
         x = self.sigmoid(x)
         return x
 
-class AdultNN:
+class UtkNN:
     """Wrapper arround pytorch neural network. Interfare for hyper parameter optimisation using raytune."""
     def __init__(self):
         self.trained = False
 
-    def fit(self, dadata):
+    def fit(self, data):
         """Train and tune hyper parameters.
         
         :parameter data: Dataset the will be split for training and hyper parameter tuning. Dataset must contain a column called "PINCP" used as training label.
-        :type dadata: fetch_data.Dataset
+        :type data: Dictionary of numpy.ndarray
         """
 
-        data = dadata.load()
-        x = data.drop("PINCP",axis=1).to_numpy()
-        self.columns = data.columns.drop("PINCP")
-        self.scaler = StandardScaler()
-        self.scaler.fit(x)
-        x = self.scaler.transform(x)
-        x = pd.DataFrame(x,columns=data.columns.drop("PINCP"))
-        data.replace(x,inplace=True)
-
         search_space = {
+                "c": tune.choice([2 ** i for i in range(9)]),
                 "l1": tune.choice([2 ** i for i in range(9)]),
                 "l2": tune.choice([2 ** i for i in range(9)]),
                 "lr": tune.loguniform(1e-4, 1e-1),
                 "batch_size": tune.choice([8, 16, 32, 64, 128])
                 }
 
         asha_scheduler = ASHAScheduler(
@@ -130,130 +118,89 @@
                 num_samples=20,
                 scheduler=asha_scheduler,
                 search_alg=hyperopt_search
                 )
 
         tuner = tune.Tuner(
                 partial(_train,data=data,stand_alone=False),
-                tune_config=tune_config,
-                run_config=train.RunConfig(stop=_stop_train)
+                tune_config=tune_config
                 )
 
         results = tuner.fit()
 
         #Real training on full train dataset (no validation)
         #Using best hyper parameters 
-        best_result = results.get_best_result("loss","min")
-        best_trained_model = TabularNN(len(data.columns)-1,best_result.config["l1"], best_result.config["l2"],2)
-
-        checkpoint_path = os.path.join(best_result.checkpoint.to_directory(), "checkpoint.pt")
-
-        model_state, optimizer_state = torch.load(checkpoint_path)
-        best_trained_model.load_state_dict(model_state)
-        
-        self.model = best_trained_model
+        best_trial = results.get_best_result(metric="loss",mode="min")
+        self.model = _train(best_trial.config, data=data, stand_alone=True)
         self.trained=True
 
-    def predict(self, dadata):
-        """Use a trained TabularNN to predict label of dataset.
+    def predict(self, data):
+        """Use a trained CNN to predict label of dataset.
 
-        :param dadata: Dataset to evaluate.
-        :type dadata: fetch_data.Dataset
-        :return: Input dataset completed with hard labels, soft labels and loss.
-        :rtype: fetch_data.Dataset
+        :param data: Dataset without label.
+        :type data: numpy.ndarray
+        :return: Prediction.
+        :rtype: numpy.ndarray
         """
         if not(self.trained):
             raise AssertionError(f"{self} must be trained prioir to predict")
         with torch.no_grad():
-            criterion = nn.CrossEntropyLoss()
-            data = dadata.load()
-            x = data[self.columns].to_numpy()
-            x = self.scaler.transform(x)
-            x = torch.from_numpy(x).float()
-            output = self.model(x)
-            labels = torch.from_numpy(data["PINCP"].to_numpy()).long()
-            loss = criterion(output,labels)
-            ysoft = output
-            yhard = np.argmax(output,axis=1)
-        data["soft0"] = ysoft[:,0]
-        data["soft1"] = ysoft[:,1]
-        data["hard"] = yhard
-        data["loss"] = loss
-        dadata.update(data)
-        return dadata
+           x = torch.from_numpy(x).float()
+           y = np.argmax(self.model(x).cpu().numpy(),axis=1)
+        return y
 
-def _pandas_to_dataset(data):
-    """Split pands dataset into training and validation and convert into pytorch dataset.
+def _images_to_dataset(data):
+    """Split images dataset into training and validation and convert into pytorch dataset.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
     :return: Training and validation dataset (train,validation).
     :rtype: tuple of torch.utils.data.dataset
     """
     skf = StratifiedKFold(shuffle=True,random_state=123)
     for train,validation in skf.split(data,data["PINCP"]):
         pass
-    train_dataset = AdultDataset(data.iloc[train])
-    validation_dataset = AdultDataset(data.iloc[validation])
+    train_dataset = UtkDataset(data.iloc[train])
+    validation_dataset = UtkDataset(data.iloc[validation])
     return train_dataset, validation_dataset
 
-        
-def _stop_train(trial_id, result):
-    """Tell tray tune to stop training after 20 iterations or when overfitting.
-
-    :param trial_id:
-    :type trial_id:
-    :param result:
-    :type result:
-    """
-    over_iter = result["training_iteration"] >= 20
-    val_loss = result["val_loss"]
-    N = len(val_loss)
-    if N<5:
-        overfit = False
-    else:
-        overfit = False
-        for i in range(1,5):
-            overfit = overfit or val_loss[-5]<= val_loss[-i]
-        overfit = overfit
-
-    return overfit or over_iter
-
 def _train(config, data, stand_alone=False):
     """Train TabularNN with ray_tune hyper parameter tuning.
 
     :param data: Dataset that will be split for validation.
     :type data: pandas.dataframe
-    :param stand_alone: (Optional default=False) If True _train does not use ray.tune and return the trained model.
+    :param stand_alone: (Optional default=False) If True _train does not use ray.tune and return the trained model. All the data provided is used in training without validation split.
     :type return_model: bool
     """
-    net = TabularNN(len(data.columns)-1,config["l1"],config["l2"],2)
+    net = CNN(len(data.columns)-1,config["l1"],config["l2"],2)
 
     device = "cpu"
     if torch.cuda.is_available():
         device = "cuda:0"
     net.to(device)
 
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.Adam(net.parameters(), lr=config["lr"])
 
-    train_dataset, validation_dataset = _pandas_to_dataset(data)
+    if stand_alone:
+        train_dataset = AdultDataset(data)
+    else:
+        train_dataset, validation_dataset = _pandas_to_dataset(data)
 
     torch.manual_seed(1234)
     train_loader = torch.utils.data.DataLoader(
         train_dataset, batch_size=int(config["batch_size"]), shuffle=True, num_workers=8
     )
-    torch.manual_seed(1234)
-    validation_loader = torch.utils.data.DataLoader(
-    validation_dataset, batch_size=int(config["batch_size"]), shuffle=True, num_workers=8
-)
-
-    val_loss_hist = []
+    if not(stand_alone):
+        torch.manual_seed(1234)
+        validation_loader = torch.utils.data.DataLoader(
+        validation_dataset, batch_size=int(config["batch_size"]), shuffle=True, num_workers=8
+    )
 
-    for epoch in range(0, 100):  # loop over the dataset multiple times
+    for epoch in range(0, 10):  # loop over the dataset multiple times
         running_loss = 0.0
         epoch_steps = 0
         for i, batch_data in enumerate(train_loader, 0):
             # get the inputs; data is a list of [inputs, labels]
             inputs, labels = batch_data
             inputs, labels = inputs.to(device), labels.to(device)
 
@@ -262,51 +209,32 @@
 
             # forward + backward + optimize
             outputs = net(inputs)
             loss = criterion(outputs, labels.long())
             loss.backward()
             optimizer.step()
 
-        # Validation loss
-        val_loss = 0.0
-        val_steps = 0
-        total = 0
-        correct = 0
-        for i, data in enumerate(validation_loader, 0):
-            with torch.no_grad():
-                inputs, labels = data
-                inputs, labels = inputs.to(device), labels.to(device)
-
-                outputs = net(inputs)
-                _, predicted = torch.max(outputs.data, 1)
-                total += labels.size(0)
-                correct += (predicted == labels).sum().item()
-
-                loss = criterion(outputs, labels.long())
-                val_loss += loss.cpu().numpy()
-                val_steps += 1
-
-        val_loss_hist += [val_loss/val_steps]
-        #Report back to Raytune
         if not(stand_alone):
+            # Validation loss
+            val_loss = 0.0
+            val_steps = 0
+            total = 0
+            correct = 0
+            for i, data in enumerate(validation_loader, 0):
+                with torch.no_grad():
+                    inputs, labels = data
+                    inputs, labels = inputs.to(device), labels.to(device)
+
+                    outputs = net(inputs)
+                    _, predicted = torch.max(outputs.data, 1)
+                    total += labels.size(0)
+                    correct += (predicted == labels).sum().item()
+
+                    loss = criterion(outputs, labels.long())
+                    val_loss += loss.cpu().numpy()
+                    val_steps += 1
 
-           # Here we save a checkpoint. It is automatically registered with
-            # Ray Tune and will potentially be accessed through in ``get_checkpoint()``
-            # in future iterations.
-            # Note to save a file like checkpoint, you still need to put it under a directory
-            # to construct a checkpoint.
-            with tempfile.TemporaryDirectory() as temp_checkpoint_dir:
-                path = os.path.join(temp_checkpoint_dir, "checkpoint.pt")
-                torch.save(
-                    (net.state_dict(), optimizer.state_dict()), path
-                )
-                checkpoint = Checkpoint.from_directory(temp_checkpoint_dir)
-                train.report({"loss":val_loss/val_steps,
-                              "training_iteration":epoch,
-                              "val_loss":val_loss_hist},
-                             checkpoint=checkpoint,
-                             )
-
-
+            #Report back to Raytune
+            train.report({"loss":val_loss/val_steps})
 
     if stand_alone:
         return net
```

### Comparing `synthetic_aia_mia-0.0.8/test/aia_soft.log` & `synthetic_aia_mia-0.0.9/test/aia_soft.log`

 * *Files 26% similar despite different names*

```diff
@@ -2926,7 +2926,862 @@
 INFO:sdv.data_processing.data_processor:Setting the configuration for the ``HyperTransformer`` for table None
 INFO:sdv.data_processing.data_processor:Fitting HyperTransformer for table None
 INFO:rdt.transformers.utils:No rounding scheme detected for column 'victore'. Data will not be rounded.
 DEBUG:sdv.data_processing.data_processor:Transforming constraints for table None
 DEBUG:sdv.data_processing.data_processor:Transforming table None
 INFO:rdt.transformers.null:Guidance: There are no missing values in column cookie. Extra column not created.
 INFO:rdt.transformers.null:Guidance: There are no missing values in column victore. Extra column not created.
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:faker.factory:Not in REPL -> leaving logger event level as is.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.address`.
+DEBUG:faker.factory:Provider `faker.providers.address` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.automotive`.
+DEBUG:faker.factory:Provider `faker.providers.automotive` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.bank`.
+DEBUG:faker.factory:Specified locale `en_US` is not available for provider `faker.providers.bank`. Locale reset to `en_GB` for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.barcode`.
+DEBUG:faker.factory:Provider `faker.providers.barcode` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.color`.
+DEBUG:faker.factory:Provider `faker.providers.color` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.company`.
+DEBUG:faker.factory:Provider `faker.providers.company` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.credit_card`.
+DEBUG:faker.factory:Provider `faker.providers.credit_card` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.currency`.
+DEBUG:faker.factory:Provider `faker.providers.currency` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.date_time`.
+DEBUG:faker.factory:Provider `faker.providers.date_time` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.emoji` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.file` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.geo`.
+DEBUG:faker.factory:Provider `faker.providers.geo` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.internet`.
+DEBUG:faker.factory:Provider `faker.providers.internet` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.isbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.job`.
+DEBUG:faker.factory:Provider `faker.providers.job` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.lorem`.
+DEBUG:faker.factory:Provider `faker.providers.lorem` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.misc`.
+DEBUG:faker.factory:Provider `faker.providers.misc` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.passport`.
+DEBUG:faker.factory:Provider `faker.providers.passport` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.person`.
+DEBUG:faker.factory:Provider `faker.providers.person` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.phone_number`.
+DEBUG:faker.factory:Provider `faker.providers.phone_number` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.profile` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.python` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.sbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.ssn`.
+DEBUG:faker.factory:Provider `faker.providers.ssn` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.user_agent` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.viewing.view(['quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.node(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.saving.Save.save(['directory'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.save(['directory'])
+DEBUG:root:        soft0     soft1  attribute
+0    0.895104  0.731057        2.0
+1    0.050365  0.154452        3.0
+2    0.566542  0.040968        3.0
+3    0.417419  0.036738        0.0
+4    0.935142  0.992139        3.0
+..        ...       ...        ...
+995  0.886498  0.645238        2.0
+996  0.129545  0.982200        1.0
+997  0.472334  0.859319        1.0
+998  0.685519  0.735090        1.0
+999  0.764593  0.590765        1.0
+
+[1000 rows x 3 columns]
+DEBUG:filelock:Attempting to acquire lock 129155904783440 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/node_ip_address.json.lock
+DEBUG:filelock:Lock 129155904783440 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/node_ip_address.json.lock
+DEBUG:filelock:Attempting to release lock 129155904783440 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/node_ip_address.json.lock
+DEBUG:filelock:Lock 129155904783440 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/node_ip_address.json.lock
+DEBUG:filelock:Attempting to acquire lock 129155903357712 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903357712 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 129155903357712 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903357712 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 129155903306512 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903306512 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 129155903306512 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903306512 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 129155903306512 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903306512 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 129155903306512 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155903306512 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 129155919447376 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155919447376 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 129155919447376 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155919447376 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 129155919447376 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155919447376 acquired on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 129155919447376 on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:filelock:Lock 129155919447376 released on /tmp/ray/session_2024-03-11_19-56-54_237658_258182/ports_by_node.json.lock
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        0.0
+3   0.207971  0.846426        1.0
+5   0.936400  0.265451        1.0
+6   0.249495  0.457136        0.0
+7   0.936008  0.857233        1.0
+..       ...       ...        ...
+95  0.181569  0.415081        0.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        1.0
+98  0.736714  0.683980        1.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        1.0
+3   0.207971  0.846426        0.0
+5   0.936400  0.265451        0.0
+6   0.249495  0.457136        1.0
+7   0.936008  0.857233        1.0
+..       ...       ...        ...
+95  0.181569  0.415081        1.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        0.0
+98  0.736714  0.683980        0.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+1   0.329673  0.051351        0.0
+2   0.015210  0.255188        0.0
+4   0.601932  0.705615        1.0
+5   0.936400  0.265451        1.0
+6   0.249495  0.457136        0.0
+..       ...       ...        ...
+93  0.928455  0.799306        0.0
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        0.0
+96  0.098026  0.231006        0.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+1   0.329673  0.051351        1.0
+2   0.015210  0.255188        0.0
+4   0.601932  0.705615        0.0
+5   0.936400  0.265451        0.0
+6   0.249495  0.457136        1.0
+..       ...       ...        ...
+93  0.928455  0.799306        0.0
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        1.0
+96  0.098026  0.231006        0.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        0.0
+1   0.329673  0.051351        0.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        1.0
+4   0.601932  0.705615        1.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        0.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        1.0
+98  0.736714  0.683980        1.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        1.0
+1   0.329673  0.051351        1.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        0.0
+4   0.601932  0.705615        0.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        1.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        0.0
+98  0.736714  0.683980        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        0.0
+1   0.329673  0.051351        0.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        1.0
+4   0.601932  0.705615        1.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        0.0
+97  0.981218  0.082600        1.0
+98  0.736714  0.683980        1.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        1.0
+1   0.329673  0.051351        1.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        0.0
+4   0.601932  0.705615        0.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+95  0.181569  0.415081        1.0
+97  0.981218  0.082600        0.0
+98  0.736714  0.683980        0.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        0.0
+1   0.329673  0.051351        0.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        1.0
+4   0.601932  0.705615        1.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        1.0
+98  0.736714  0.683980        1.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.547851  0.523308        1.0
+1   0.329673  0.051351        1.0
+2   0.015210  0.255188        0.0
+3   0.207971  0.846426        0.0
+4   0.601932  0.705615        0.0
+..       ...       ...        ...
+94  0.211531  0.263821        1.0
+96  0.098026  0.231006        0.0
+97  0.981218  0.082600        0.0
+98  0.736714  0.683980        0.0
+99  0.443571  0.922851        0.0
+
+[80 rows x 3 columns]
+INFO:sdv.metadata.single_table:Detected metadata:
+INFO:sdv.metadata.single_table:{
+    "columns": {
+        "cookie": {
+            "sdtype": "numerical"
+        },
+        "victore": {
+            "sdtype": "numerical"
+        }
+    },
+    "METADATA_SPEC_VERSION": "SINGLE_TABLE_V1"
+}
+INFO:sdv.data_processing.data_processor:Fitting table None metadata
+INFO:sdv.data_processing.data_processor:Fitting formatters for table None
+INFO:sdv.data_processing.numerical_formatter:No rounding scheme detected for column 'victore'. Synthetic data will not be rounded.
+INFO:sdv.data_processing.data_processor:Fitting constraints for table None
+INFO:sdv.data_processing.data_processor:Setting the configuration for the ``HyperTransformer`` for table None
+INFO:sdv.data_processing.data_processor:Fitting HyperTransformer for table None
+INFO:rdt.transformers.utils:No rounding scheme detected for column 'victore'. Data will not be rounded.
+DEBUG:sdv.data_processing.data_processor:Transforming constraints for table None
+DEBUG:sdv.data_processing.data_processor:Transforming table None
+INFO:rdt.transformers.null:Guidance: There are no missing values in column cookie. Extra column not created.
+INFO:rdt.transformers.null:Guidance: There are no missing values in column victore. Extra column not created.
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:faker.factory:Not in REPL -> leaving logger event level as is.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.address`.
+DEBUG:faker.factory:Provider `faker.providers.address` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.automotive`.
+DEBUG:faker.factory:Provider `faker.providers.automotive` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.bank`.
+DEBUG:faker.factory:Specified locale `en_US` is not available for provider `faker.providers.bank`. Locale reset to `en_GB` for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.barcode`.
+DEBUG:faker.factory:Provider `faker.providers.barcode` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.color`.
+DEBUG:faker.factory:Provider `faker.providers.color` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.company`.
+DEBUG:faker.factory:Provider `faker.providers.company` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.credit_card`.
+DEBUG:faker.factory:Provider `faker.providers.credit_card` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.currency`.
+DEBUG:faker.factory:Provider `faker.providers.currency` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.date_time`.
+DEBUG:faker.factory:Provider `faker.providers.date_time` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.emoji` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.file` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.geo`.
+DEBUG:faker.factory:Provider `faker.providers.geo` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.internet`.
+DEBUG:faker.factory:Provider `faker.providers.internet` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.isbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.job`.
+DEBUG:faker.factory:Provider `faker.providers.job` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.lorem`.
+DEBUG:faker.factory:Provider `faker.providers.lorem` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.misc`.
+DEBUG:faker.factory:Provider `faker.providers.misc` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.passport`.
+DEBUG:faker.factory:Provider `faker.providers.passport` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.person`.
+DEBUG:faker.factory:Provider `faker.providers.person` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.phone_number`.
+DEBUG:faker.factory:Provider `faker.providers.phone_number` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.profile` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.python` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.sbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.ssn`.
+DEBUG:faker.factory:Provider `faker.providers.ssn` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.user_agent` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.viewing.view(['quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.node(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.saving.Save.save(['directory'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.save(['directory'])
+DEBUG:root:       soft0     soft1  attribute
+0  -0.259825 -0.645083          2
+1   1.435855 -0.026859          1
+2  -1.326099  1.250802          0
+3  -1.261651 -0.958160          6
+4   0.811319  0.311497          4
+..       ...       ...        ...
+95  0.241474  1.187565          1
+96 -0.255651  1.519576          4
+97  0.175550  0.173391          4
+98 -0.767030  1.481124          4
+99 -0.011900  1.189952          6
+
+[100 rows x 3 columns]
+DEBUG:filelock:Attempting to acquire lock 124551234563088 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/node_ip_address.json.lock
+DEBUG:filelock:Lock 124551234563088 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/node_ip_address.json.lock
+DEBUG:filelock:Attempting to release lock 124551234563088 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/node_ip_address.json.lock
+DEBUG:filelock:Lock 124551234563088 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/node_ip_address.json.lock
+DEBUG:filelock:Attempting to acquire lock 124551284800272 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551284800272 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 124551284800272 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551284800272 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 124551249181776 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551249181776 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 124551249181776 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551249181776 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 124551236094480 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236094480 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 124551236094480 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236094480 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 124551236054672 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236054672 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 124551236054672 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236054672 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 124551236094480 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236094480 acquired on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 124551236094480 on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:filelock:Lock 124551236094480 released on /tmp/ray/session_2024-03-12_11-27-21_426219_159923/ports_by_node.json.lock
+DEBUG:root:       soft0     soft1  attribute
+1   0.173616 -1.241294        1.0
+2  -0.665067 -0.981578        0.0
+3  -0.251436  0.766102        0.0
+4   0.306174  1.185511        0.0
+5  -1.609320  0.067868        1.0
+..       ...       ...        ...
+91       NaN       NaN        NaN
+93       NaN       NaN        NaN
+94       NaN       NaN        NaN
+95       NaN       NaN        NaN
+98       NaN       NaN        NaN
+
+[80 rows x 3 columns]
+INFO:sdv.metadata.single_table:Detected metadata:
+INFO:sdv.metadata.single_table:{
+    "METADATA_SPEC_VERSION": "SINGLE_TABLE_V1",
+    "columns": {
+        "cookie": {
+            "sdtype": "numerical"
+        },
+        "victore": {
+            "sdtype": "numerical"
+        }
+    }
+}
+INFO:sdv.data_processing.data_processor:Fitting table None metadata
+INFO:sdv.data_processing.data_processor:Fitting formatters for table None
+INFO:sdv.data_processing.numerical_formatter:No rounding scheme detected for column 'victore'. Synthetic data will not be rounded.
+INFO:sdv.data_processing.data_processor:Fitting constraints for table None
+INFO:sdv.data_processing.data_processor:Setting the configuration for the ``HyperTransformer`` for table None
+INFO:sdv.data_processing.data_processor:Fitting HyperTransformer for table None
+INFO:rdt.transformers.utils:No rounding scheme detected for column 'victore'. Data will not be rounded.
+DEBUG:sdv.data_processing.data_processor:Transforming constraints for table None
+DEBUG:sdv.data_processing.data_processor:Transforming table None
+INFO:rdt.transformers.null:Guidance: There are no missing values in column cookie. Extra column not created.
+INFO:rdt.transformers.null:Guidance: There are no missing values in column victore. Extra column not created.
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:h5py._conv:Creating converter from 7 to 5
+DEBUG:h5py._conv:Creating converter from 5 to 7
+DEBUG:faker.factory:Not in REPL -> leaving logger event level as is.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.address`.
+DEBUG:faker.factory:Provider `faker.providers.address` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.automotive`.
+DEBUG:faker.factory:Provider `faker.providers.automotive` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.bank`.
+DEBUG:faker.factory:Specified locale `en_US` is not available for provider `faker.providers.bank`. Locale reset to `en_GB` for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.barcode`.
+DEBUG:faker.factory:Provider `faker.providers.barcode` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.color`.
+DEBUG:faker.factory:Provider `faker.providers.color` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.company`.
+DEBUG:faker.factory:Provider `faker.providers.company` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.credit_card`.
+DEBUG:faker.factory:Provider `faker.providers.credit_card` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.currency`.
+DEBUG:faker.factory:Provider `faker.providers.currency` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.date_time`.
+DEBUG:faker.factory:Provider `faker.providers.date_time` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.emoji` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.file` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.geo`.
+DEBUG:faker.factory:Provider `faker.providers.geo` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.internet`.
+DEBUG:faker.factory:Provider `faker.providers.internet` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.isbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.job`.
+DEBUG:faker.factory:Provider `faker.providers.job` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.lorem`.
+DEBUG:faker.factory:Provider `faker.providers.lorem` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.misc`.
+DEBUG:faker.factory:Provider `faker.providers.misc` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.passport`.
+DEBUG:faker.factory:Provider `faker.providers.passport` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.person`.
+DEBUG:faker.factory:Provider `faker.providers.person` has been localized to `en_US`.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.phone_number`.
+DEBUG:faker.factory:Provider `faker.providers.phone_number` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.profile` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.python` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Provider `faker.providers.sbn` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:faker.factory:Looking for locale `en_US` in provider `faker.providers.ssn`.
+DEBUG:faker.factory:Provider `faker.providers.ssn` has been localized to `en_US`.
+DEBUG:faker.factory:Provider `faker.providers.user_agent` does not feature localization. Specified locale `en_US` is not utilized for this provider.
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.backend.viewing.view(['quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.node(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.saving.Save.save(['directory'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])
+DEBUG:graphviz._tools:deprecate positional args: graphviz.sources.Source.save(['directory'])
+DEBUG:root:       soft0     soft1  attribute
+0  -0.881135 -1.023735          0
+1   0.008985 -1.644755          0
+2  -0.357474 -1.410075          0
+3   1.558801  1.410471          1
+4   0.768197  0.396855          0
+..       ...       ...        ...
+95 -1.428118 -1.313604          1
+96  1.535867 -1.228493          0
+97  1.276126  0.743171          1
+98 -0.589241 -1.671259          0
+99  0.462512  0.842239          1
+
+[100 rows x 3 columns]
+DEBUG:filelock:Attempting to acquire lock 132879660347408 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/node_ip_address.json.lock
+DEBUG:filelock:Lock 132879660347408 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/node_ip_address.json.lock
+DEBUG:filelock:Attempting to release lock 132879660347408 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/node_ip_address.json.lock
+DEBUG:filelock:Lock 132879660347408 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/node_ip_address.json.lock
+DEBUG:filelock:Attempting to acquire lock 132879663852176 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879663852176 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 132879663852176 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879663852176 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 132879660344144 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660344144 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 132879660344144 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660344144 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to acquire lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 acquired on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Attempting to release lock 132879660341584 on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:filelock:Lock 132879660341584 released on /tmp/ray/session_2024-03-12_12-58-27_315630_561213/ports_by_node.json.lock
+DEBUG:root:       soft0     soft1  attribute
+0  -0.881135 -1.023735          1
+1   0.008985 -1.644755          1
+2  -0.357474 -1.410075          1
+3   1.558801  1.410471          0
+4   0.768197  0.396855          1
+..       ...       ...        ...
+95 -1.428118 -1.313604          1
+96  1.535867 -1.228493          0
+97  1.276126  0.743171          1
+98 -0.589241 -1.671259          1
+99  0.462512  0.842239          1
+
+[100 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0  -0.690518  0.975712          3
+1  -0.636315 -0.426189          4
+2  -0.840036  0.980672          5
+3  -1.457974  0.846538          5
+4   1.464960  0.279094          4
+..       ...       ...        ...
+95 -0.683939  0.778895          1
+96 -1.182226 -0.044837          1
+97  1.142812  0.272383          0
+98  0.585370 -0.336213          0
+99  1.327292 -1.175947          5
+
+[100 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.310424 -0.855868          1
+1  -1.722555 -0.953759          0
+2  -0.814160 -0.113514          1
+3   0.831458  0.815455          1
+4  -0.404695  0.334187          0
+..       ...       ...        ...
+75  0.982429  0.866405          0
+76 -0.279924 -1.523077          0
+77 -0.089272 -0.232740          1
+78 -1.498091  1.295651          1
+79 -0.473161  0.327736          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.310424 -0.855868          0
+1  -1.722555 -0.953759          1
+2  -0.814160 -0.113514          0
+3   0.831458  0.815455          0
+4  -0.404695  0.334187          1
+..       ...       ...        ...
+75  0.982429  0.866405          0
+76 -0.279924 -1.523077          0
+77 -0.089272 -0.232740          0
+78 -1.498091  1.295651          1
+79 -0.473161  0.327736          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0  -1.705809 -0.934204          0
+1   0.860820  0.933696          1
+2  -0.381439  0.425583          0
+3   0.849855 -1.640715          0
+4  -0.208817  1.592184          0
+..       ...       ...        ...
+75 -0.274857  0.203046          0
+76 -0.064458 -0.172967          1
+77 -1.480236  1.440677          1
+78 -1.558084 -0.201811          1
+79 -0.450244  0.418773          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0  -1.705809 -0.934204          1
+1   0.860820  0.933696          0
+2  -0.381439  0.425583          1
+3   0.849855 -1.640715          1
+4  -0.208817  1.592184          1
+..       ...       ...        ...
+75 -0.274857  0.203046          1
+76 -0.064458 -0.172967          0
+77 -1.480236  1.440677          1
+78 -1.558084 -0.201811          0
+79 -0.450244  0.418773          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.417442 -0.797967          1
+1  -1.700477 -0.897750          0
+2  -0.754128 -0.041260          1
+3   0.948879 -1.579872          0
+4  -0.148604  1.541426          0
+..       ...       ...        ...
+75 -0.197571 -1.478076          0
+76 -0.217066  0.200241          0
+77 -1.466635  1.395149          1
+78 -1.547337 -0.190640          1
+79 -0.398882  0.408521          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.417442 -0.797967          0
+1  -1.700477 -0.897750          1
+2  -0.754128 -0.041260          0
+3   0.948879 -1.579872          1
+4  -0.148604  1.541426          1
+..       ...       ...        ...
+75 -0.197571 -1.478076          0
+76 -0.217066  0.200241          1
+77 -1.466635  1.395149          1
+78 -1.547337 -0.190640          0
+79 -0.398882  0.408521          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.318918 -0.904462          1
+1  -1.839470 -1.008007          0
+2  -0.875038 -0.119227          1
+3   0.872093  0.863401          1
+4  -0.440315  0.354334          0
+..       ...       ...        ...
+75 -0.327715  0.131379          0
+76 -0.105434 -0.245340          1
+77 -1.601159  1.371334          1
+78 -1.683404 -0.274239          1
+79 -0.513005  0.347510          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.318918 -0.904462          0
+1  -1.839470 -1.008007          1
+2  -0.875038 -0.119227          0
+3   0.872093  0.863401          0
+4  -0.440315  0.354334          1
+..       ...       ...        ...
+75 -0.327715  0.131379          1
+76 -0.105434 -0.245340          0
+77 -1.601159  1.371334          1
+78 -1.683404 -0.274239          0
+79 -0.513005  0.347510          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.433994 -0.897377          1
+1  -0.763866 -0.139332          1
+2   0.988977  0.809271          1
+3  -0.327721  0.317831          0
+4  -0.144755  1.446152          0
+..       ...       ...        ...
+75  1.149785  0.861298          0
+76 -0.194820 -1.578687          0
+77 -0.214753  0.102596          0
+78  0.008254 -0.261078          1
+79 -1.574874 -0.288976          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.433994 -0.897377          0
+1  -0.763866 -0.139332          0
+2   0.988977  0.809271          0
+3  -0.327721  0.317831          1
+4  -0.144755  1.446152          1
+..       ...       ...        ...
+75  1.149785  0.861298          0
+76 -0.194820 -1.578687          0
+77 -0.214753  0.102596          1
+78  0.008254 -0.261078          0
+79 -1.574874 -0.288976          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.320542 -0.965011          1
+1  -0.865638 -0.160470          1
+2   0.870114  0.846318          1
+3  -0.252563  1.522263          0
+4   1.549188 -0.379637          0
+..       ...       ...        ...
+75  1.029354  0.901536          0
+76 -0.321879  0.096297          0
+77 -0.101046 -0.289684          1
+78 -1.587030  1.366739          1
+79 -0.505962  0.317743          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.320542 -0.965011          0
+1  -0.865638 -0.160470          0
+2   0.870114  0.846318          0
+3  -0.252563  1.522263          1
+4   1.549188 -0.379637          1
+..       ...       ...        ...
+75  1.029354  0.901536          0
+76 -0.321879  0.096297          1
+77 -0.101046 -0.289684          0
+78 -1.587030  1.366739          1
+79 -0.505962  0.317743          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.360789 -0.810896          1
+1  -1.770130 -0.909965          0
+2  -0.817972 -0.059609          1
+3   0.906924  0.880537          1
+4  -0.388781  0.393478          0
+..       ...       ...        ...
+75 -0.277614  0.180162          0
+76 -0.058162 -0.180270          1
+77 -1.534852  1.366511          1
+78 -1.616050 -0.207919          1
+79 -0.460546  0.386950          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.360789 -0.810896          0
+1  -1.770130 -0.909965          1
+2  -0.817972 -0.059609          0
+3   0.906924  0.880537          0
+4  -0.388781  0.393478          1
+..       ...       ...        ...
+75 -0.277614  0.180162          1
+76 -0.058162 -0.180270          0
+77 -1.534852  1.366511          1
+78 -1.616050 -0.207919          0
+79 -0.460546  0.386950          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.405787 -0.833425          1
+1  -1.771593 -0.933798          0
+2   0.963830  0.880292          1
+3  -0.360126  0.386816          0
+4   0.952145 -1.619956          0
+..       ...       ...        ...
+75 -0.226493 -1.517557          0
+76 -0.246535  0.170690          0
+77 -0.022299 -0.194491          1
+78 -1.614154 -0.222504          1
+79 -0.433455  0.380202          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.405787 -0.833425          0
+1  -1.771593 -0.933798          1
+2   0.963830  0.880292          0
+3  -0.360126  0.386816          1
+4   0.952145 -1.619956          1
+..       ...       ...        ...
+75 -0.226493 -1.517557          0
+76 -0.246535  0.170690          1
+77 -0.022299 -0.194491          0
+78 -1.614154 -0.222504          0
+79 -0.433455  0.380202          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0  -1.614868 -0.989037          0
+1  -0.732493 -0.106458          1
+2  -0.334757  0.363799          0
+3   0.855388 -1.691937          0
+4   1.491356 -0.318874          0
+..       ...       ...        ...
+75  1.012633  0.922832          0
+76 -0.213560 -1.587039          0
+77 -1.396833  1.373704          1
+78 -1.472080 -0.260388          1
+79 -0.401262  0.357023          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0  -1.614868 -0.989037          1
+1  -0.732493 -0.106458          0
+2  -0.334757  0.363799          1
+3   0.855388 -1.691937          1
+4   1.491356 -0.318874          1
+..       ...       ...        ...
+75  1.012633  0.922832          0
+76 -0.213560 -1.587039          0
+77 -1.396833  1.373704          1
+78 -1.472080 -0.260388          0
+79 -0.401262  0.357023          0
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.367059 -0.799615          1
+1  -1.722957 -0.896091          0
+2  -0.789076 -0.067989          1
+3   0.902712  0.847555          1
+4  -0.368123  0.373242          0
+..       ...       ...        ...
+75 -0.239851 -1.457181          0
+76 -0.259089  0.165508          0
+77 -0.043850 -0.185492          1
+78 -1.492195  1.320811          1
+79 -1.571835 -0.212417          1
+
+[80 rows x 3 columns]
+DEBUG:root:       soft0     soft1  attribute
+0   0.367059 -0.799615          0
+1  -1.722957 -0.896091          1
+2  -0.789076 -0.067989          0
+3   0.902712  0.847555          0
+4  -0.368123  0.373242          1
+..       ...       ...        ...
+75 -0.239851 -1.457181          0
+76 -0.259089  0.165508          1
+77 -0.043850 -0.185492          0
+78 -1.492195  1.320811          1
+79 -1.571835 -0.212417          0
+
+[80 rows x 3 columns]
+INFO:sdv.metadata.single_table:Detected metadata:
+INFO:sdv.metadata.single_table:{
+    "columns": {
+        "cookie": {
+            "sdtype": "numerical"
+        },
+        "victore": {
+            "sdtype": "numerical"
+        }
+    },
+    "METADATA_SPEC_VERSION": "SINGLE_TABLE_V1"
+}
+INFO:sdv.data_processing.data_processor:Fitting table None metadata
+INFO:sdv.data_processing.data_processor:Fitting formatters for table None
+INFO:sdv.data_processing.numerical_formatter:No rounding scheme detected for column 'victore'. Synthetic data will not be rounded.
+INFO:sdv.data_processing.data_processor:Fitting constraints for table None
+INFO:sdv.data_processing.data_processor:Setting the configuration for the ``HyperTransformer`` for table None
+INFO:sdv.data_processing.data_processor:Fitting HyperTransformer for table None
+INFO:rdt.transformers.utils:No rounding scheme detected for column 'victore'. Data will not be rounded.
+DEBUG:sdv.data_processing.data_processor:Transforming constraints for table None
+DEBUG:sdv.data_processing.data_processor:Transforming table None
+INFO:rdt.transformers.null:Guidance: There are no missing values in column cookie. Extra column not created.
+INFO:rdt.transformers.null:Guidance: There are no missing values in column victore. Extra column not created.
```

### Comparing `synthetic_aia_mia-0.0.8/test/aia/hard.py` & `synthetic_aia_mia-0.0.9/test/aia/hard.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/aia/soft.py` & `synthetic_aia_mia-0.0.9/test/aia/soft.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Unit tests for neural network for attribute inference attack"""
 
 import unittest
 import pandas as pd
 import numpy as np
 import torch
+import logging
 
 from synthetic_aia_mia.aia import soft
 from synthetic_aia_mia.fetch_data import Dataset
 
 class TestAdultNN(unittest.TestCase):
     """Test for aia"""
 
@@ -18,27 +19,27 @@
         with self.assertRaises(AssertionError) as cm:
             clf.predict(df)
 
     def test_neural_network(self):
         """Test if the pytroch model trains and predicts."""
         N = 100
         x = np.random.uniform(0,1,[N,2])
-        x = np.hstack([x,np.random.randint(0,2,[N,1])])
+        x = np.hstack([x,np.random.randint(0,5,[N,1])])
         df = pd.DataFrame(x, columns=["soft0", "soft1" ,"attribute"])
         config = {"l1":2,"l2":2,"lr":0.001,"batch_size":1}
         clf = soft._train(config,df,stand_alone=True)
         x = torch.tensor(np.random.uniform(0,1,[N,2]),dtype=torch.float)
         y = clf(x)
         self.assertEqual(len(y),N)
 
     def test_predict_trained(self):
         """Test if a trained model in the hyperparameter optimization interface can make a prediction."""
-        N = 1000
+        N = 100
         x = np.random.uniform(0,1,[N,2])
-        y = np.random.randint(0,4,[N,1])
+        y = np.random.randint(2,9,[N,1])
         data = np.hstack([x,y])
         df = pd.DataFrame(data, columns=["soft0", "soft1","sex"])
         dset = Dataset()
         dset.update(df)
 
         clf = soft.AiaNN()
         clf.fit(dset,"sex")
```

### Comparing `synthetic_aia_mia-0.0.8/test/data_management/dataset.py` & `synthetic_aia_mia-0.0.9/test/data_management/dataset.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/data_management/fetch.py` & `synthetic_aia_mia-0.0.9/test/data_management/fetch.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/data_management/split.py` & `synthetic_aia_mia-0.0.9/test/data_management/split.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/experiement/adult.py` & `synthetic_aia_mia-0.0.9/test/experiement/adult.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                 self.assertTrue(lab in metrics[attrib].keys())
                 self.assertTrue("balanced_accuracy" in metrics[attrib][lab].keys())
 
 class TestMia(unittest.TestCase):
     """Test _mia wrapper."""
 
     def test_metric(self):
+        return
         """Test if _mia outputs the right metrics."""
         N = 100
         x = np.random.uniform(0,1,[N,1])
         x = np.hstack([x,np.random.randint(0,2,[N,1])])
         df = pd.DataFrame(x,columns=["loss","member"])
         dset = Dataset()
         dset.update(df)
```

### Comparing `synthetic_aia_mia-0.0.8/test/generator/adult.py` & `synthetic_aia_mia-0.0.9/test/generator/adult.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/metrics/metrics.py` & `synthetic_aia_mia-0.0.9/test/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/mia/ml.py` & `synthetic_aia_mia-0.0.9/test/mia/ml.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/mia/random_fusion.py` & `synthetic_aia_mia-0.0.9/test/mia/random_fusion.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/predictor/adult_nn.py` & `synthetic_aia_mia-0.0.9/test/predictor/adult_nn.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/predictor/stop_train_condition.py` & `synthetic_aia_mia-0.0.9/test/predictor/stop_train_condition.py`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/test/predictor/utk_nn` & `synthetic_aia_mia-0.0.9/test/predictor/utk_nn`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/README.md` & `synthetic_aia_mia-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_aia_mia-0.0.8/pyproject.toml` & `synthetic_aia_mia-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synthetic_aia_mia"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com"} ,
   {name="Thomas Lebrun", email="thomas.lebrun@inria.fr"},
 ]
 description = "AIA and MIA attack versus synthetic and real data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `synthetic_aia_mia-0.0.8/PKG-INFO` & `synthetic_aia_mia-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_aia_mia
-Version: 0.0.8
+Version: 0.0.9
 Summary: AIA and MIA attack versus synthetic and real data.
 Project-URL: Homepage, https://gitlab.inria.fr/jaalmoes/synthetic
 Project-URL: Bug Tracker, https://gitlab.inria.fr/jaalmoes/synthetic
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>, Thomas Lebrun <thomas.lebrun@inria.fr>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

