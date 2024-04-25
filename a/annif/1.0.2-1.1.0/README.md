# Comparing `tmp/annif-1.0.2.tar.gz` & `tmp/annif-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annif-1.0.2.tar", max compression
+gzip compressed data, was "annif-1.1.0.tar", max compression
```

## Comparing `annif-1.0.2.tar` & `annif-1.1.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      606 2024-02-02 09:34:31.670576 annif-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     8845 2024-02-02 09:34:31.670576 annif-1.0.2/README.md
--rw-r--r--   0        0        0     2962 2024-02-02 09:34:31.670576 annif-1.0.2/annif/__init__.py
--rw-r--r--   0        0        0     1398 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/__init__.py
--rw-r--r--   0        0        0     1871 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/analyzer.py
--rw-r--r--   0        0        0      383 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/simple.py
--rw-r--r--   0        0        0      436 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/simplemma.py
--rw-r--r--   0        0        0      566 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/snowball.py
--rw-r--r--   0        0        0     1248 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/spacy.py
--rw-r--r--   0        0        0      991 2024-02-02 09:34:31.670576 annif-1.0.2/annif/analyzer/voikko.py
--rw-r--r--   0        0        0     2580 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/__init__.py
--rw-r--r--   0        0        0     5939 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/backend.py
--rw-r--r--   0        0        0     1611 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/dummy.py
--rw-r--r--   0        0        0     6194 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/ensemble.py
--rw-r--r--   0        0        0     6205 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/fasttext.py
--rw-r--r--   0        0        0     3092 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/http.py
--rw-r--r--   0        0        0     4009 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/hyperopt.py
--rw-r--r--   0        0        0     3026 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/mixins.py
--rw-r--r--   0        0        0     6084 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/mllm.py
--rw-r--r--   0        0        0    10037 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/nn_ensemble.py
--rw-r--r--   0        0        0     5575 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/omikuji.py
--rw-r--r--   0        0        0     6410 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/pav.py
--rw-r--r--   0        0        0     5074 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/stwfsa.py
--rw-r--r--   0        0        0     4216 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/svc.py
--rw-r--r--   0        0        0     4778 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/tfidf.py
--rw-r--r--   0        0        0     6960 2024-02-02 09:34:31.670576 annif-1.0.2/annif/backend/yake.py
--rw-r--r--   0        0        0    20985 2024-02-02 09:34:31.674576 annif-1.0.2/annif/cli.py
--rw-r--r--   0        0        0     8415 2024-02-02 09:34:31.674576 annif-1.0.2/annif/cli_util.py
--rw-r--r--   0        0        0     4707 2024-02-02 09:34:31.674576 annif-1.0.2/annif/config.py
--rw-r--r--   0        0        0      664 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/__init__.py
--rw-r--r--   0        0        0      665 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/combine.py
--rw-r--r--   0        0        0     4579 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/document.py
--rw-r--r--   0        0        0     5128 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/skos.py
--rw-r--r--   0        0        0     9631 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/subject.py
--rw-r--r--   0        0        0     1843 2024-02-02 09:34:31.674576 annif-1.0.2/annif/corpus/types.py
--rw-r--r--   0        0        0      691 2024-02-02 09:34:31.674576 annif-1.0.2/annif/datadir.py
--rw-r--r--   0        0        0     1135 2024-02-02 09:34:31.674576 annif-1.0.2/annif/default_config.py
--rw-r--r--   0        0        0    10071 2024-02-02 09:34:31.674576 annif-1.0.2/annif/eval.py
--rw-r--r--   0        0        0     1987 2024-02-02 09:34:31.674576 annif-1.0.2/annif/exception.py
--rw-r--r--   0        0        0        0 2024-02-02 09:34:31.674576 annif-1.0.2/annif/lexical/__init__.py
--rw-r--r--   0        0        0    13406 2024-02-02 09:34:31.674576 annif-1.0.2/annif/lexical/mllm.py
--rw-r--r--   0        0        0     3117 2024-02-02 09:34:31.674576 annif-1.0.2/annif/lexical/tokenset.py
--rw-r--r--   0        0        0     1773 2024-02-02 09:34:31.674576 annif-1.0.2/annif/lexical/util.py
--rw-r--r--   0        0        0        0 2024-02-02 09:34:31.674576 annif-1.0.2/annif/openapi/__init__.py
--rw-r--r--   0        0        0    10845 2024-02-02 09:34:31.674576 annif-1.0.2/annif/openapi/annif.yaml
--rw-r--r--   0        0        0     1652 2024-02-02 09:34:31.674576 annif-1.0.2/annif/openapi/validation.py
--rw-r--r--   0        0        0     3400 2024-02-02 09:34:31.674576 annif-1.0.2/annif/parallel.py
--rw-r--r--   0        0        0    10976 2024-02-02 09:34:31.674576 annif-1.0.2/annif/project.py
--rw-r--r--   0        0        0     5869 2024-02-02 09:34:31.674576 annif-1.0.2/annif/registry.py
--rw-r--r--   0        0        0     6370 2024-02-02 09:34:31.674576 annif-1.0.2/annif/rest.py
--rw-r--r--   0        0        0   194901 2024-02-02 09:34:31.674576 annif-1.0.2/annif/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   522721 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0      590 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/css/fonts.css
--rw-r--r--   0        0        0     2862 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/css/style.css
--rw-r--r--   0        0        0    15086 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/favicon.ico
--rw-r--r--   0        0        0    35776 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/fonts/Jost-400-Book.otf
--rw-r--r--   0        0        0    98228 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/fonts/Jost-400-Book.ttf
--rw-r--r--   0        0        0    39056 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/fonts/Jost-500-Medium.otf
--rw-r--r--   0        0        0   109760 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/fonts/Jost-500-Medium.ttf
--rw-r--r--   0        0        0     2663 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/img/annif-RGB.svg
--rw-r--r--   0        0        0      530 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/img/arrow-white.svg
--rw-r--r--   0        0        0    26580 2024-02-02 09:34:31.678576 annif-1.0.2/annif/static/js/axios.min.js
--rw-r--r--   0        0        0   124862 2024-02-02 09:34:31.682576 annif-1.0.2/annif/static/js/axios.min.js.map
--rw-r--r--   0        0        0    60480 2024-02-02 09:34:31.682576 annif-1.0.2/annif/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   217134 2024-02-02 09:34:31.682576 annif-1.0.2/annif/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    87533 2024-02-02 09:34:31.682576 annif-1.0.2/annif/static/js/vue.min.js
--rw-r--r--   0        0        0     5531 2024-02-02 09:34:31.682576 annif-1.0.2/annif/suggestion.py
--rw-r--r--   0        0        0    11156 2024-02-02 09:34:31.682576 annif-1.0.2/annif/templates/home.html
--rw-r--r--   0        0        0     1992 2024-02-02 09:34:31.682576 annif-1.0.2/annif/transform/__init__.py
--rw-r--r--   0        0        0      938 2024-02-02 09:34:31.682576 annif-1.0.2/annif/transform/inputlimiter.py
--rw-r--r--   0        0        0     1381 2024-02-02 09:34:31.682576 annif-1.0.2/annif/transform/langfilter.py
--rw-r--r--   0        0        0     2356 2024-02-02 09:34:31.682576 annif-1.0.2/annif/transform/transform.py
--rw-r--r--   0        0        0     3481 2024-02-02 09:34:31.682576 annif-1.0.2/annif/util.py
--rw-r--r--   0        0        0      147 2024-02-02 09:34:31.682576 annif-1.0.2/annif/views.py
--rw-r--r--   0        0        0     5183 2024-02-02 09:34:31.682576 annif-1.0.2/annif/vocab.py
--rw-r--r--   0        0        0     2501 2024-02-02 09:34:31.682576 annif-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 annif-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      606 2024-04-25 13:03:25.754919 annif-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     9146 2024-04-25 13:03:25.754919 annif-1.1.0/README.md
+-rw-r--r--   0        0        0     3542 2024-04-25 13:03:25.754919 annif-1.1.0/annif/__init__.py
+-rw-r--r--   0        0        0     1399 2024-04-25 13:03:25.754919 annif-1.1.0/annif/analyzer/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-25 13:03:25.754919 annif-1.1.0/annif/analyzer/analyzer.py
+-rw-r--r--   0        0        0      384 2024-04-25 13:03:25.754919 annif-1.1.0/annif/analyzer/simple.py
+-rw-r--r--   0        0        0      437 2024-04-25 13:03:25.754919 annif-1.1.0/annif/analyzer/simplemma.py
+-rw-r--r--   0        0        0      567 2024-04-25 13:03:25.754919 annif-1.1.0/annif/analyzer/snowball.py
+-rw-r--r--   0        0        0     1249 2024-04-25 13:03:25.758919 annif-1.1.0/annif/analyzer/spacy.py
+-rw-r--r--   0        0        0      992 2024-04-25 13:03:25.758919 annif-1.1.0/annif/analyzer/voikko.py
+-rw-r--r--   0        0        0     2581 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/__init__.py
+-rw-r--r--   0        0        0     6023 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/backend.py
+-rw-r--r--   0        0        0     1612 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/dummy.py
+-rw-r--r--   0        0        0     6195 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/ensemble.py
+-rw-r--r--   0        0        0     6206 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/fasttext.py
+-rw-r--r--   0        0        0     3093 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/http.py
+-rw-r--r--   0        0        0     4010 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/hyperopt.py
+-rw-r--r--   0        0        0     3027 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/mixins.py
+-rw-r--r--   0        0        0     6085 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/mllm.py
+-rw-r--r--   0        0        0    11226 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/nn_ensemble.py
+-rw-r--r--   0        0        0     5576 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/omikuji.py
+-rw-r--r--   0        0        0     6487 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/pav.py
+-rw-r--r--   0        0        0     5074 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/stwfsa.py
+-rw-r--r--   0        0        0     4217 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/svc.py
+-rw-r--r--   0        0        0     4779 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/tfidf.py
+-rw-r--r--   0        0        0     6965 2024-04-25 13:03:25.758919 annif-1.1.0/annif/backend/yake.py
+-rw-r--r--   0        0        0    25489 2024-04-25 13:03:25.758919 annif-1.1.0/annif/cli.py
+-rw-r--r--   0        0        0     8425 2024-04-25 13:03:25.758919 annif-1.1.0/annif/cli_util.py
+-rw-r--r--   0        0        0     4708 2024-04-25 13:03:25.758919 annif-1.1.0/annif/config.py
+-rw-r--r--   0        0        0      663 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/combine.py
+-rw-r--r--   0        0        0     4580 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/document.py
+-rw-r--r--   0        0        0     5225 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/skos.py
+-rw-r--r--   0        0        0     9632 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/subject.py
+-rw-r--r--   0        0        0     1844 2024-04-25 13:03:25.758919 annif-1.1.0/annif/corpus/types.py
+-rw-r--r--   0        0        0      692 2024-04-25 13:03:25.758919 annif-1.1.0/annif/datadir.py
+-rw-r--r--   0        0        0     1135 2024-04-25 13:03:25.758919 annif-1.1.0/annif/default_config.py
+-rw-r--r--   0        0        0    10070 2024-04-25 13:03:25.758919 annif-1.1.0/annif/eval.py
+-rw-r--r--   0        0        0     1988 2024-04-25 13:03:25.758919 annif-1.1.0/annif/exception.py
+-rw-r--r--   0        0        0     7867 2024-04-25 13:03:25.758919 annif-1.1.0/annif/hfh_util.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:03:25.758919 annif-1.1.0/annif/lexical/__init__.py
+-rw-r--r--   0        0        0    13407 2024-04-25 13:03:25.758919 annif-1.1.0/annif/lexical/mllm.py
+-rw-r--r--   0        0        0     3118 2024-04-25 13:03:25.758919 annif-1.1.0/annif/lexical/tokenset.py
+-rw-r--r--   0        0        0     1774 2024-04-25 13:03:25.758919 annif-1.1.0/annif/lexical/util.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:03:25.758919 annif-1.1.0/annif/openapi/__init__.py
+-rw-r--r--   0        0        0    10889 2024-04-25 13:03:25.758919 annif-1.1.0/annif/openapi/annif.yaml
+-rw-r--r--   0        0        0     1469 2024-04-25 13:03:25.758919 annif-1.1.0/annif/openapi/validation.py
+-rw-r--r--   0        0        0     3401 2024-04-25 13:03:25.758919 annif-1.1.0/annif/parallel.py
+-rw-r--r--   0        0        0    10977 2024-04-25 13:03:25.758919 annif-1.1.0/annif/project.py
+-rw-r--r--   0        0        0     5956 2024-04-25 13:03:25.758919 annif-1.1.0/annif/registry.py
+-rw-r--r--   0        0        0     6562 2024-04-25 13:03:25.758919 annif-1.1.0/annif/rest.py
+-rw-r--r--   0        0        0   194901 2024-04-25 13:03:25.758919 annif-1.1.0/annif/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   522721 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0      590 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/css/fonts.css
+-rw-r--r--   0        0        0     2938 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/css/style.css
+-rw-r--r--   0        0        0    15086 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/favicon.ico
+-rw-r--r--   0        0        0    35776 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/fonts/Jost-400-Book.otf
+-rw-r--r--   0        0        0    98228 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/fonts/Jost-400-Book.ttf
+-rw-r--r--   0        0        0    39056 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/fonts/Jost-500-Medium.otf
+-rw-r--r--   0        0        0   109760 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/fonts/Jost-500-Medium.ttf
+-rw-r--r--   0        0        0     2663 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/img/annif-RGB.svg
+-rw-r--r--   0        0        0      530 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/img/arrow-white.svg
+-rw-r--r--   0        0        0    26580 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/js/axios.min.js
+-rw-r--r--   0        0        0   124862 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/js/axios.min.js.map
+-rw-r--r--   0        0        0    60480 2024-04-25 13:03:25.762919 annif-1.1.0/annif/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   217134 2024-04-25 13:03:25.766919 annif-1.1.0/annif/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    87533 2024-04-25 13:03:25.766919 annif-1.1.0/annif/static/js/vue.min.js
+-rw-r--r--   0        0        0     5527 2024-04-25 13:03:25.766919 annif-1.1.0/annif/suggestion.py
+-rw-r--r--   0        0        0    11448 2024-04-25 13:03:25.766919 annif-1.1.0/annif/templates/home.html
+-rw-r--r--   0        0        0     1993 2024-04-25 13:03:25.766919 annif-1.1.0/annif/transform/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-25 13:03:25.766919 annif-1.1.0/annif/transform/inputlimiter.py
+-rw-r--r--   0        0        0     1382 2024-04-25 13:03:25.766919 annif-1.1.0/annif/transform/langfilter.py
+-rw-r--r--   0        0        0     2357 2024-04-25 13:03:25.766919 annif-1.1.0/annif/transform/transform.py
+-rw-r--r--   0        0        0     3482 2024-04-25 13:03:25.766919 annif-1.1.0/annif/util.py
+-rw-r--r--   0        0        0      147 2024-04-25 13:03:25.766919 annif-1.1.0/annif/views.py
+-rw-r--r--   0        0        0     5184 2024-04-25 13:03:25.766919 annif-1.1.0/annif/vocab.py
+-rw-r--r--   0        0        0     2450 2024-04-25 13:03:25.766919 annif-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11408 1970-01-01 00:00:00.000000 annif-1.1.0/PKG-INFO
```

### Comparing `annif-1.0.2/LICENSE.txt` & `annif-1.1.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2022 University Of Helsinki (The National Library Of Finland)
+Copyright (c) 2017-2024 University Of Helsinki (The National Library Of Finland)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `annif-1.0.2/README.md` & `annif-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 <img src="https://annif.org/static/img/annif-RGB.svg" width="150">
 
 [![DOI](https://zenodo.org/badge/100936800.svg)](https://zenodo.org/badge/latestdoi/100936800)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Container image](https://img.shields.io/badge/container_image-quay.io-blue.svg)](https://quay.io/repository/natlibfi/annif)
 [![CI/CD](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml)
 [![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/main/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)
-[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
 [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=main)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=main)
+[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/NatLibFi/Annif/badge)](https://securityscorecards.dev/viewer/?uri=github.com/NatLibFi/Annif)
 [![codebeat badge](https://codebeat.co/badges/7a8ef539-0094-48b8-84c2-c413b4a50d57)](https://codebeat.co/projects/github-com-natlibfi-annif-main)
 [![CodeQL](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NatLibFi_Annif&metric=alert_status)](https://sonarcloud.io/dashboard?id=NatLibFi_Annif)
 [![docs](https://readthedocs.org/projects/annif/badge/?version=latest)](https://annif.readthedocs.io/en/latest/index.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Annif is an automated subject indexing toolkit. It was originally created as
@@ -22,15 +24,15 @@
 
 [Finto AI](https://ai.finto.fi/) is a service based on Annif; see the [source code for Finto AI](https://github.com/NatLibFi/FintoAI).
 
 # Basic install
 
 Annif is developed and tested on Linux. If you want to run Annif on Windows or Mac OS, the recommended way is to use Docker (see below) or a Linux virtual machine.
 
-You will need Python 3.8+ to install Annif.
+You will need Python 3.9-3.12 to install Annif.
 
 The recommended way is to install Annif from
 [PyPI](https://pypi.org/project/annif/) into a virtual environment.
 
     python3 -m venv annif-venv
     source annif-venv/bin/activate
     pip install annif
```

### Comparing `annif-1.0.2/annif/__init__.py` & `annif-1.1.0/annif/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,73 +3,89 @@
 from __future__ import annotations
 
 import logging
 import os
 import os.path
 from typing import TYPE_CHECKING
 
+from flask import Flask
+
 logging.basicConfig()
 logger = logging.getLogger("annif")
 logger.setLevel(level=logging.INFO)
 
 import annif.backend  # noqa
 
 if TYPE_CHECKING:
-    from flask.app import Flask
+    from connexion.apps.flask import FlaskApp
 
 
 def create_flask_app(config_name: str | None = None) -> Flask:
     """Create a Flask app to be used by the CLI."""
-    from flask import Flask
 
     _set_tensorflow_loglevel()
 
     app = Flask(__name__)
     config_name = _get_config_name(config_name)
     logger.debug(f"creating flask app with configuration {config_name}")
     app.config.from_object(config_name)
     app.config.from_envvar("ANNIF_SETTINGS", silent=True)
     return app
 
 
-def create_app(config_name: str | None = None) -> Flask:
+def create_cx_app(config_name: str | None = None) -> FlaskApp:
     """Create a Connexion app to be used for the API."""
-    # 'cxapp' here is the Connexion application that has a normal Flask app
-    # as a property (cxapp.app)
     import connexion
-    from flask_cors import CORS
+    from connexion.datastructures import MediaTypeDict
+    from connexion.middleware import MiddlewarePosition
+    from connexion.validators import FormDataValidator, MultiPartFormDataValidator
+    from starlette.middleware.cors import CORSMiddleware
 
+    import annif.registry
     from annif.openapi.validation import CustomRequestBodyValidator
 
     specdir = os.path.join(os.path.dirname(__file__), "openapi")
-    cxapp = connexion.App(__name__, specification_dir=specdir)
+    cxapp = connexion.FlaskApp(__name__, specification_dir=specdir)
     config_name = _get_config_name(config_name)
     logger.debug(f"creating connexion app with configuration {config_name}")
     cxapp.app.config.from_object(config_name)
     cxapp.app.config.from_envvar("ANNIF_SETTINGS", silent=True)
 
     validator_map = {
-        "body": CustomRequestBodyValidator,
+        "body": MediaTypeDict(
+            {
+                "*/*json": CustomRequestBodyValidator,
+                "application/x-www-form-urlencoded": FormDataValidator,
+                "multipart/form-data": MultiPartFormDataValidator,
+            }
+        ),
     }
     cxapp.add_api("annif.yaml", validator_map=validator_map)
 
     # add CORS support
-    CORS(cxapp.app)
+    cxapp.add_middleware(
+        CORSMiddleware,
+        position=MiddlewarePosition.BEFORE_EXCEPTION,
+        allow_origins=["*"],
+    )
 
     if cxapp.app.config["INITIALIZE_PROJECTS"]:
         annif.registry.initialize_projects(cxapp.app)
         logger.info("finished initializing projects")
 
     # register the views via blueprints
     from annif.views import bp
 
     cxapp.app.register_blueprint(bp)
 
-    # return the Flask app
-    return cxapp.app
+    # return the Connexion app
+    return cxapp
+
+
+create_app = create_cx_app  # Alias to allow starting directly with uvicorn run
 
 
 def _get_config_name(config_name: str | None) -> str:
     if config_name is None:
         config_name = os.environ.get("ANNIF_CONFIG")
     if config_name is None:
         if os.environ.get("FLASK_RUN_FROM_CLI") == "true":  # pragma: no cover
```

### Comparing `annif-1.0.2/annif/analyzer/__init__.py` & `annif-1.1.0/annif/analyzer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Collection of language-specific analyzers and analyzer registry for Annif"""
+
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
 import annif
 from annif.util import parse_args
```

### Comparing `annif-1.0.2/annif/analyzer/analyzer.py` & `annif-1.1.0/annif/analyzer/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common functionality for analyzers."""
+
 from __future__ import annotations
 
 import abc
 import functools
 import unicodedata
 
 _KEY_TOKEN_MIN_LENGTH = "token_min_length"
```

### Comparing `annif-1.0.2/annif/analyzer/snowball.py` & `annif-1.1.0/annif/analyzer/snowball.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Snowball analyzer for Annif, based on nltk Snowball stemmer."""
+
 from __future__ import annotations
 
 import functools
 
 from . import analyzer
```

### Comparing `annif-1.0.2/annif/analyzer/spacy.py` & `annif-1.1.0/annif/analyzer/spacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """spaCy analyzer for Annif which uses spaCy for lemmatization"""
+
 from __future__ import annotations
 
 import annif.util
 from annif.exception import OperationFailedException
 
 from . import analyzer
```

### Comparing `annif-1.0.2/annif/analyzer/voikko.py` & `annif-1.1.0/annif/analyzer/voikko.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Voikko analyzer for Annif, based on libvoikko library."""
+
 from __future__ import annotations
 
 import functools
 
 import voikko.libvoikko
 
 from . import analyzer
```

### Comparing `annif-1.0.2/annif/backend/__init__.py` & `annif-1.1.0/annif/backend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Registry of backend types for Annif"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Type
 
 if TYPE_CHECKING:
     from annif.backend.backend import AnnifBackend
```

### Comparing `annif-1.0.2/annif/backend/backend.py` & `annif-1.1.0/annif/backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common functionality for backends."""
+
 from __future__ import annotations
 
 import abc
 import os.path
 from datetime import datetime, timezone
 from glob import glob
 from typing import TYPE_CHECKING, Any
@@ -49,22 +50,23 @@
         params = {}
         params.update(self.default_params())
         params.update(self.config_params)
         return params
 
     @property
     def _model_file_paths(self) -> list:
-        all_paths = glob(os.path.join(self.datadir, "*"))
+        all_paths = glob(os.path.join(self.datadir, "**"), recursive=True)
+        file_paths = [p for p in all_paths if os.path.isfile(p)]
         ignore_patterns = ("*-train*", "tmp-*", "vectorizer")
         ignore_paths = [
             path
             for igp in ignore_patterns
             for path in glob(os.path.join(self.datadir, igp))
         ]
-        return list(set(all_paths) - set(ignore_paths))
+        return list(set(file_paths) - set(ignore_paths))
 
     @property
     def is_trained(self) -> bool:
         return bool(self._model_file_paths)
 
     @property
     def modification_time(self) -> datetime | None:
```

### Comparing `annif-1.0.2/annif/backend/dummy.py` & `annif-1.1.0/annif/backend/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dummy backend for testing basic interaction of projects and backends"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from annif.suggestion import SubjectSuggestion
 
 from . import backend
```

### Comparing `annif-1.0.2/annif/backend/ensemble.py` & `annif-1.1.0/annif/backend/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Ensemble backend that combines results from multiple projects"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import annif.eval
 import annif.parallel
 import annif.util
```

### Comparing `annif-1.0.2/annif/backend/fasttext.py` & `annif-1.1.0/annif/backend/fasttext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annif backend using the fastText classifier"""
+
 from __future__ import annotations
 
 import collections
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import fasttext
```

### Comparing `annif-1.0.2/annif/backend/http.py` & `annif-1.1.0/annif/backend/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """HTTP/REST client backend that makes calls to a web service
 and returns the results"""
+
 from __future__ import annotations
 
 import importlib
 from typing import TYPE_CHECKING, Any
 
 import dateutil.parser
 import requests
```

### Comparing `annif-1.0.2/annif/backend/hyperopt.py` & `annif-1.1.0/annif/backend/hyperopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hyperparameter optimization functionality for backends"""
+
 from __future__ import annotations
 
 import abc
 import collections
 import warnings
 from typing import TYPE_CHECKING, Callable
```

### Comparing `annif-1.0.2/annif/backend/mixins.py` & `annif-1.1.0/annif/backend/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annif backend mixins that can be used to implement features"""
+
 from __future__ import annotations
 
 import abc
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import joblib
```

### Comparing `annif-1.0.2/annif/backend/mllm.py` & `annif-1.1.0/annif/backend/mllm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Maui-like Lexical Matching backend"""
+
 from __future__ import annotations
 
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import joblib
 import numpy as np
```

### Comparing `annif-1.0.2/annif/backend/nn_ensemble.py` & `annif-1.1.0/annif/backend/nn_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Neural network based ensemble backend that combines results from multiple
 projects."""
+
 from __future__ import annotations
 
+import importlib
+import json
 import os.path
 import shutil
+import zipfile
 from io import BytesIO
 from typing import TYPE_CHECKING, Any
 
 import joblib
 import keras.backend as K
 import lmdb
 import numpy as np
@@ -16,24 +20,30 @@
 from keras.saving import load_model
 from keras.utils import Sequence
 from scipy.sparse import csc_matrix, csr_matrix
 
 import annif.corpus
 import annif.parallel
 import annif.util
-from annif.exception import NotInitializedException, NotSupportedException
+from annif.exception import (
+    NotInitializedException,
+    NotSupportedException,
+    OperationFailedException,
+)
 from annif.suggestion import SuggestionBatch, vector_to_suggestions
 
 from . import backend, ensemble
 
 if TYPE_CHECKING:
     from tensorflow.python.framework.ops import EagerTensor
 
     from annif.corpus.document import DocumentCorpus
 
+logger = annif.logger
+
 
 def idx_to_key(idx: int) -> bytes:
     """convert an integer index to a binary key for use in LMDB"""
     return b"%08d" % idx
 
 
 def key_to_idx(key: memoryview | bytes) -> int:
@@ -124,17 +134,28 @@
         model_filename = os.path.join(self.datadir, self.MODEL_FILE)
         if not os.path.exists(model_filename):
             raise NotInitializedException(
                 "model file {} not found".format(model_filename),
                 backend_id=self.backend_id,
             )
         self.debug("loading Keras model from {}".format(model_filename))
-        self._model = load_model(
-            model_filename, custom_objects={"MeanLayer": MeanLayer}
-        )
+        try:
+            self._model = load_model(
+                model_filename, custom_objects={"MeanLayer": MeanLayer}
+            )
+        except Exception as err:
+            metadata = self.get_model_metadata(model_filename)
+            keras_version = importlib.metadata.version("keras")
+            message = (
+                f"loading Keras model from {model_filename}; "
+                f"model metadata: {metadata}; "
+                f"you have Keras version {keras_version}. "
+                f'Original error message: "{err}"'
+            )
+            raise OperationFailedException(message, backend_id=self.backend_id)
 
     def _merge_source_batches(
         self,
         batch_by_source: dict[str, SuggestionBatch],
         sources: list[tuple[str, float]],
         params: dict[str, Any],
     ) -> SuggestionBatch:
@@ -284,7 +305,20 @@
         corpus: DocumentCorpus,
         params: dict[str, Any],
     ) -> None:
         self.initialize()
         self._fit_model(
             corpus, int(params["learn-epochs"]), int(params["lmdb_map_size"])
         )
+
+    def get_model_metadata(self, model_filename: str) -> dict | None:
+        """Read metadata from Keras model files."""
+
+        try:
+            with zipfile.ZipFile(model_filename, "r") as zip:
+                with zip.open("metadata.json") as metadata_file:
+                    metadata_str = metadata_file.read().decode("utf-8")
+                    metadata = json.loads(metadata_str)
+                    return metadata
+        except Exception:
+            self.warning(f"Failed to read metadata from {model_filename}")
+            return None
```

### Comparing `annif-1.0.2/annif/backend/omikuji.py` & `annif-1.1.0/annif/backend/omikuji.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annif backend using the Omikuji classifier"""
+
 from __future__ import annotations
 
 import os.path
 import shutil
 from typing import TYPE_CHECKING, Any
 
 import omikuji
```

### Comparing `annif-1.0.2/annif/backend/pav.py` & `annif-1.1.0/annif/backend/pav.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """PAV ensemble backend that combines results from multiple projects and
 learns which concept suggestions from each backend are trustworthy using the
 PAV algorithm, a.k.a. isotonic regression, to turn raw scores returned by
 individual backends into probabilities."""
+
 from __future__ import annotations
 
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import joblib
 import numpy as np
@@ -65,21 +66,23 @@
         params: dict[str, Any],
     ) -> SuggestionBatch:
         reg_batch_by_source = {}
         for project_id, batch in batch_by_source.items():
             reg_models = self._get_model(project_id)
             pav_batch = [
                 [
-                    SubjectSuggestion(
-                        subject_id=sugg.subject_id,
-                        score=reg_models[sugg.subject_id].predict([sugg.score])[0],
-                    )
-                    if sugg.subject_id in reg_models
-                    else SubjectSuggestion(
-                        subject_id=sugg.subject_id, score=sugg.score
+                    (
+                        SubjectSuggestion(
+                            subject_id=sugg.subject_id,
+                            score=reg_models[sugg.subject_id].predict([sugg.score])[0],
+                        )
+                        if sugg.subject_id in reg_models
+                        else SubjectSuggestion(
+                            subject_id=sugg.subject_id, score=sugg.score
+                        )
                     )  # default to raw score
                     for sugg in result
                 ]
                 for result in batch
             ]
             reg_batch_by_source[project_id] = SuggestionBatch.from_sequence(
                 pav_batch, self.project.subjects
```

### Comparing `annif-1.0.2/annif/backend/stwfsa.py` & `annif-1.1.0/annif/backend/stwfsa.py`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/backend/svc.py` & `annif-1.1.0/annif/backend/svc.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annif backend using a SVM classifier"""
+
 from __future__ import annotations
 
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import joblib
 import numpy as np
```

### Comparing `annif-1.0.2/annif/backend/tfidf.py` & `annif-1.1.0/annif/backend/tfidf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Backend that returns most similar subjects based on similarity in sparse
 TF-IDF normalized bag-of-words vector space"""
+
 from __future__ import annotations
 
 import os.path
 import tempfile
 from typing import TYPE_CHECKING, Any
 
 import gensim.similarities
```

### Comparing `annif-1.0.2/annif/backend/yake.py` & `annif-1.1.0/annif/backend/yake.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Annif backend using Yake keyword extraction"""
+
 # For license remarks of this backend see README.md:
 # https://github.com/NatLibFi/Annif#license.
 from __future__ import annotations
 
 import os.path
 import re
 from collections import defaultdict
@@ -47,15 +48,15 @@
 
     @property
     def is_trained(self):
         return True
 
     @property
     def label_types(self) -> list[URIRef]:
-        if type(self.params["label_types"]) == str:  # Label types set by user
+        if isinstance(self.params["label_types"], str):  # Label types set by user
             label_types = [lt.strip() for lt in self.params["label_types"].split(",")]
             self._validate_label_types(label_types)
         else:
             label_types = self.params["label_types"]  # The defaults
         return [getattr(SKOS, lt) for lt in label_types]
 
     def _validate_label_types(self, label_types: list[str]) -> None:
```

### Comparing `annif-1.0.2/annif/cli.py` & `annif-1.1.0/annif/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Definitions for command-line (Click) commands for invoking Annif
 operations and printing the results to console."""
 
-
 import collections
 import importlib
 import json
 import os.path
 import re
 import sys
 
@@ -14,31 +13,32 @@
 from flask.cli import FlaskGroup
 
 import annif
 import annif.corpus
 import annif.parallel
 import annif.project
 import annif.registry
-from annif import cli_util
-from annif.exception import NotInitializedException, NotSupportedException
+from annif import cli_util, hfh_util
+from annif.exception import (
+    NotInitializedException,
+    NotSupportedException,
+    OperationFailedException,
+)
 from annif.project import Access
 from annif.util import metric_code
 
 logger = annif.logger
 click_log.basic_config(logger)
 
-
-if len(sys.argv) > 1 and sys.argv[1] in ("run", "routes"):
-    create_app = annif.create_app  # Use Flask with Connexion
-else:
-    # Connexion is not needed for most CLI commands, use plain Flask
-    create_app = annif.create_flask_app
-
-cli = FlaskGroup(create_app=create_app, add_version_option=False)
+create_app = annif.create_flask_app
+cli = FlaskGroup(
+    create_app=create_app, add_default_commands=False, add_version_option=False
+)
 cli = click.version_option(message="%(version)s")(cli)
+cli.params = [opt for opt in cli.params if opt.name not in ("env_file", "app")]
 
 
 @cli.command("list-projects")
 @cli_util.common_options
 @click_log.simple_verbosity_option(logger, default="ERROR")
 def run_list_projects():
     """
@@ -439,14 +439,29 @@
         json.dump(
             {metric_code(mname): val for mname, val in metrics.items()},
             metrics_file,
             indent=2,
         )
 
 
+@cli.command("run")
+@click.option("--port", type=int, default=5000)
+@click.option("--log-level")
+@click_log.simple_verbosity_option(logger, default="ERROR")
+def run_app(**kwargs):
+    """
+    Run Annif in server mode for development.
+    \f
+    The server is for development purposes only.
+    """
+    kwargs = {k: v for k, v in kwargs.items() if v is not None}
+    cxapp = annif.create_cx_app()
+    cxapp.run(**kwargs)
+
+
 FILTER_BATCH_MAX_LIMIT = 15
 OPTIMIZE_METRICS = ["Precision (doc avg)", "Recall (doc avg)", "F1 score (doc avg)"]
 
 
 @cli.command("optimize")
 @cli_util.project_id
 @click.argument("paths", type=click.Path(exists=True), nargs=-1)
@@ -579,19 +594,137 @@
     click.echo(f"Got best {metric} score {rec.score:.4f} with:")
     click.echo("---")
     for line in rec.lines:
         click.echo(line)
     click.echo("---")
 
 
+@cli.command("upload")
+@click.argument("project_ids_pattern", shell_complete=cli_util.complete_param)
+@click.argument("repo_id")
+@click.option(
+    "--token",
+    help="""Authentication token, obtained from the Hugging Face Hub.
+    Will default to the stored token.""",
+)
+@click.option(
+    "--revision",
+    help="""An optional git revision to commit from. Defaults to the head of the "main"
+    branch.""",
+)
+@click.option(
+    "--commit-message",
+    help="""The summary / title / first line of the generated commit.""",
+)
+@cli_util.common_options
+def run_upload(project_ids_pattern, repo_id, token, revision, commit_message):
+    """
+    Upload selected projects and their vocabularies to a Hugging Face Hub repository.
+    \f
+    This command zips the project directories and vocabularies of the projects
+    that match the given `project_ids_pattern` to archive files, and uploads the
+    archives along with the project configurations to the specified Hugging Face
+    Hub repository. An authentication token and commit message can be given with
+    options.
+    """
+    from huggingface_hub import HfApi
+    from huggingface_hub.utils import HfHubHTTPError, HFValidationError
+
+    projects = hfh_util.get_matching_projects(project_ids_pattern)
+    click.echo(f"Uploading project(s): {', '.join([p.project_id for p in projects])}")
+
+    commit_message = (
+        commit_message
+        if commit_message is not None
+        else f"Upload project(s) {project_ids_pattern} with Annif"
+    )
+
+    fobjs, operations = [], []
+    try:
+        fobjs, operations = hfh_util.prepare_commits(projects, repo_id)
+        api = HfApi()
+        api.create_commit(
+            repo_id=repo_id,
+            operations=operations,
+            commit_message=commit_message,
+            revision=revision,
+            token=token,
+        )
+    except (HfHubHTTPError, HFValidationError) as err:
+        raise OperationFailedException(str(err))
+    finally:
+        for fobj in fobjs:
+            fobj.close()
+
+
+@cli.command("download")
+@click.argument("project_ids_pattern")
+@click.argument("repo_id")
+@click.option(
+    "--token",
+    help="""Authentication token, obtained from the Hugging Face Hub.
+    Will default to the stored token.""",
+)
+@click.option(
+    "--revision",
+    help="""
+    An optional Git revision id which can be a branch name, a tag, or a commit
+    hash.
+    """,
+)
+@click.option(
+    "--force",
+    "-f",
+    default=False,
+    is_flag=True,
+    help="Replace an existing project/vocabulary/config with the downloaded one",
+)
+@cli_util.common_options
+def run_download(project_ids_pattern, repo_id, token, revision, force):
+    """
+    Download selected projects and their vocabularies from a Hugging Face Hub
+    repository.
+    \f
+    This command downloads the project and vocabulary archives and the
+    configuration files of the projects that match the given
+    `project_ids_pattern` from the specified Hugging Face Hub repository and
+    unzips the archives to `data/` directory and places the configuration files
+    to `projects.d/` directory. An authentication token and revision can
+    be given with options.
+    """
+
+    project_ids = hfh_util.get_matching_project_ids_from_hf_hub(
+        project_ids_pattern, repo_id, token, revision
+    )
+    click.echo(f"Downloading project(s): {', '.join(project_ids)}")
+
+    vocab_ids = set()
+    for project_id in project_ids:
+        project_zip_cache_path = hfh_util.download_from_hf_hub(
+            f"projects/{project_id}.zip", repo_id, token, revision
+        )
+        hfh_util.unzip_archive(project_zip_cache_path, force)
+        config_file_cache_path = hfh_util.download_from_hf_hub(
+            f"{project_id}.cfg", repo_id, token, revision
+        )
+        vocab_ids.add(hfh_util.get_vocab_id_from_config(config_file_cache_path))
+        hfh_util.copy_project_config(config_file_cache_path, force)
+
+    for vocab_id in vocab_ids:
+        vocab_zip_cache_path = hfh_util.download_from_hf_hub(
+            f"vocabs/{vocab_id}.zip", repo_id, token, revision
+        )
+        hfh_util.unzip_archive(vocab_zip_cache_path, force)
+
+
 @cli.command("completion")
 @click.option("--bash", "shell", flag_value="bash")
 @click.option("--zsh", "shell", flag_value="zsh")
 @click.option("--fish", "shell", flag_value="fish")
-def completion(shell):
+def run_completion(shell):
     """Generate the script for tab-key autocompletion for the given shell. To enable the
     completion support in your current bash terminal session run\n
         source <(annif completion --bash)
     """
 
     if shell is None:
         raise click.UsageError("Shell not given, try --bash, --zsh or --fish")
```

### Comparing `annif-1.0.2/annif/cli_util.py` & `annif-1.1.0/annif/cli_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for Annif CLI commands"""
+
 from __future__ import annotations
 
 import collections
 import itertools
 import os
 import sys
 from typing import TYPE_CHECKING
@@ -12,16 +13,16 @@
 from flask import current_app
 
 import annif
 from annif.exception import ConfigurationException
 from annif.project import Access
 
 if TYPE_CHECKING:
+    import io
     from datetime import datetime
-    from io import TextIOWrapper
 
     from click.core import Argument, Context, Option
 
     from annif.corpus.document import DocumentCorpus, DocumentList
     from annif.corpus.subject import SubjectIndex
     from annif.project import AnnifProject
     from annif.suggestion import SuggestionResult
@@ -180,15 +181,15 @@
     return annif.corpus.DocumentList(_docs(paths[:docs_limit]))
 
 
 def show_hits(
     hits: SuggestionResult,
     project: AnnifProject,
     lang: str,
-    file: TextIOWrapper | None = None,
+    file: io.TextIOWrapper | None = None,
 ) -> None:
     """
     Print subject suggestions to the console or a file. The suggestions are displayed as
     a table, with one row per hit. Each row contains the URI, label, possible notation,
     and score of the suggestion. The label is given in the specified language.
     """
     template = "<{}>\t{}\t{:.04f}"
@@ -229,15 +230,15 @@
     thresholds = [i * 0.05 for i in range(20)]
     return list(itertools.product(limits, thresholds))
 
 
 def _get_completion_choices(
     param: Argument,
 ) -> dict[str, AnnifVocabulary] | dict[str, AnnifProject] | list:
-    if param.name == "project_id":
+    if param.name in ("project_id", "project_ids_pattern"):
         return annif.registry.get_projects()
     elif param.name == "vocab_id":
         return annif.registry.get_vocabs()
     else:
         return []
```

### Comparing `annif-1.0.2/annif/config.py` & `annif-1.1.0/annif/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration file handling"""
+
 from __future__ import annotations
 
 import configparser
 import os.path
 from glob import glob
 
 try:
```

### Comparing `annif-1.0.2/annif/corpus/__init__.py` & `annif-1.1.0/annif/corpus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Annif corpus operations"""
 
-
 from .combine import CombinedCorpus
 from .document import (
     DocumentDirectory,
     DocumentFile,
     DocumentList,
     LimitingDocumentCorpus,
     TransformingDocumentCorpus,
```

### Comparing `annif-1.0.2/annif/corpus/combine.py` & `annif-1.1.0/annif/corpus/combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for combining multiple corpora so they behave like a single corpus"""
+
 from __future__ import annotations
 
 import itertools
 from typing import TYPE_CHECKING
 
 from .types import DocumentCorpus
```

### Comparing `annif-1.0.2/annif/corpus/document.py` & `annif-1.1.0/annif/corpus/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Clases for supporting document corpora"""
+
 from __future__ import annotations
 
 import glob
 import gzip
 import os.path
 import re
 from itertools import islice
```

### Comparing `annif-1.0.2/annif/corpus/skos.py` & `annif-1.1.0/annif/corpus/skos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Support for subjects loaded from a SKOS/RDF file"""
+
 from __future__ import annotations
 
 import collections
 import os.path
 import shutil
 from typing import TYPE_CHECKING
 
@@ -79,19 +80,23 @@
                 if label.language is not None
             }
         return self._languages
 
     def _concept_labels(self, concept: URIRef) -> dict[str, str]:
         by_lang = self.get_concept_labels(concept, self.PREF_LABEL_PROPERTIES)
         return {
-            lang: by_lang[lang][0]
-            if by_lang[lang]  # correct lang
-            else by_lang[None][0]
-            if by_lang[None]  # no language
-            else self.graph.namespace_manager.qname(concept)
+            lang: (
+                by_lang[lang][0]
+                if by_lang[lang]  # correct lang
+                else (
+                    by_lang[None][0]
+                    if by_lang[None]  # no language
+                    else self.graph.namespace_manager.qname(concept)
+                )
+            )
             for lang in self.languages
         }
 
     @property
     def subjects(self) -> Iterator[Subject]:
         for concept in self.concepts:
             labels = self._concept_labels(concept)
```

### Comparing `annif-1.0.2/annif/corpus/subject.py` & `annif-1.1.0/annif/corpus/subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes for supporting subject corpora expressed as directories or files"""
+
 from __future__ import annotations
 
 import csv
 import os.path
 from typing import TYPE_CHECKING, Any
 
 import annif
```

### Comparing `annif-1.0.2/annif/corpus/types.py` & `annif-1.1.0/annif/corpus/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basic types for document and subject corpora"""
+
 from __future__ import annotations
 
 import abc
 import collections
 from itertools import islice
 
 Document = collections.namedtuple("Document", "text subject_set")
```

### Comparing `annif-1.0.2/annif/datadir.py` & `annif-1.1.0/annif/datadir.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mixin class for types that need a data directory"""
+
 from __future__ import annotations
 
 import os
 import os.path
 
 
 class DatadirMixin:
```

### Comparing `annif-1.0.2/annif/default_config.py` & `annif-1.1.0/annif/default_config.py`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/eval.py` & `annif-1.1.0/annif/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Evaluation metrics for Annif"""
+
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING
 
 import numpy as np
 import scipy.sparse
@@ -59,18 +60,18 @@
 
 def ndcg_score(y_true: csr_array, y_pred: csr_array, limit: int | None = None) -> float:
     """return the normalized discounted cumulative gain (nDCG) score for the
     selected labels vs. relevant labels"""
 
     scores = np.ones(y_true.shape[0], dtype=np.float32)
     for i in range(y_true.shape[0]):
-        true = y_true.getrow(i)
+        true = y_true[[i]]
         idcg = dcg_score(true, true, limit)
         if idcg > 0:
-            pred = y_pred.getrow(i)
+            pred = y_pred[[i]]
             dcg = dcg_score(true, pred, limit)
             scores[i] = dcg / idcg
 
     return float(scores.mean())
 
 
 class EvaluationBatch:
@@ -82,17 +83,17 @@
     def __init__(self, subject_index: SubjectIndex) -> None:
         self._subject_index = subject_index
         self._suggestion_arrays = []
         self._gold_subject_arrays = []
 
     def evaluate_many(
         self,
-        suggestion_batch: list[list[SubjectSuggestion]]
-        | SuggestionBatch
-        | list[Iterator],
+        suggestion_batch: (
+            list[list[SubjectSuggestion]] | SuggestionBatch | list[Iterator]
+        ),
         gold_subject_batch: Sequence[SubjectSet],
     ) -> None:
         if not isinstance(suggestion_batch, SuggestionBatch):
             suggestion_batch = SuggestionBatch.from_sequence(
                 suggestion_batch, self._subject_index
             )
         self._suggestion_arrays.append(suggestion_batch.array)
```

### Comparing `annif-1.0.2/annif/exception.py` & `annif-1.1.0/annif/exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom exceptions used by Annif"""
+
 from __future__ import annotations
 
 from click import ClickException
 
 
 class AnnifException(ClickException):
     """Base Annif exception. We define this as a subclass of ClickException so
```

### Comparing `annif-1.0.2/annif/lexical/mllm.py` & `annif-1.1.0/annif/lexical/mllm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MLLM (Maui-like Lexical Matchin) model for Annif"""
+
 from __future__ import annotations
 
 import collections
 import math
 from enum import IntEnum
 from statistics import mean
 from typing import TYPE_CHECKING, Any
```

### Comparing `annif-1.0.2/annif/lexical/tokenset.py` & `annif-1.1.0/annif/lexical/tokenset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Index for fast matching of token sets."""
+
 from __future__ import annotations
 
 import collections
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from numpy import ndarray
```

### Comparing `annif-1.0.2/annif/lexical/util.py` & `annif-1.1.0/annif/lexical/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility methods for lexical algorithms"""
+
 from __future__ import annotations
 
 import collections
 from typing import TYPE_CHECKING
 
 from rdflib import URIRef
 from rdflib.namespace import SKOS
```

### Comparing `annif-1.0.2/annif/openapi/annif.yaml` & `annif-1.1.0/annif/openapi/annif.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,17 @@
               type: array
               items:
                 $ref: '#/components/schemas/IndexedDocument'
         required: true
       responses:
         "204":
           description: successful operation
-          content: {}
+          content:
+            application/json:
+              {}
         "404":
           $ref: '#/components/responses/NotFound'
         "503":
           $ref: '#/components/responses/ServiceUnavailable'
       x-codegen-request-body-name: documents
 components:
   schemas:
```

### Comparing `annif-1.0.2/annif/openapi/validation.py` & `annif-1.1.0/annif/openapi/validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 """Custom validator for the Annif API."""
+
 from __future__ import annotations
 
 import logging
+from typing import Any
 
-import jsonschema
-from connexion import decorators
 from connexion.exceptions import BadRequestProblem
-from connexion.utils import is_null
+from connexion.json_schema import format_error_with_path
+from connexion.validators import JSONRequestBodyValidator
+from jsonschema.exceptions import ValidationError
 
 logger = logging.getLogger("openapi.validation")
 
 
-class CustomRequestBodyValidator(decorators.validation.RequestBodyValidator):
+class CustomRequestBodyValidator(JSONRequestBodyValidator):
     """Custom request body validator that overrides the default error message for the
-    'maxItems' validator for the 'documents' property."""
+    'maxItems' validator for the 'documents' property to prevent logging request body
+    with the contents of all documents."""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-    def validate_schema(
-        self,
-        data: list | dict,
-        url: str,
-    ) -> None:
-        """Validate the request body against the schema."""
-
-        if self.is_null_value_valid and is_null(data):
-            return None  # pragma: no cover
-
+    def _validate(self, body: Any) -> dict | None:
         try:
-            self.validator.validate(data)
-        except jsonschema.ValidationError as exception:
+            return self._validator.validate(body)
+        except ValidationError as exception:
             if exception.validator == "maxItems" and list(exception.schema_path) == [
                 "properties",
                 "documents",
                 "maxItems",
             ]:
                 exception.message = "too many items"
-
-            error_path_msg = self._error_path_message(exception=exception)
+            error_path_msg = format_error_with_path(exception=exception)
             logger.error(
-                "{url} validation error: {error}{error_path_msg}".format(
-                    url=url, error=exception.message, error_path_msg=error_path_msg
-                ),
+                f"Validation error: {exception.message}{error_path_msg}",
                 extra={"validator": "body"},
             )
             raise BadRequestProblem(detail=f"{exception.message}{error_path_msg}")
-        return None
```

### Comparing `annif-1.0.2/annif/parallel.py` & `annif-1.1.0/annif/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parallel processing functionality for Annif"""
+
 from __future__ import annotations
 
 import multiprocessing
 import multiprocessing.dummy
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
```

### Comparing `annif-1.0.2/annif/project.py` & `annif-1.1.0/annif/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Project management functionality for Annif"""
+
 from __future__ import annotations
 
 import enum
 import os.path
 from shutil import rmtree
 from typing import TYPE_CHECKING
```

### Comparing `annif-1.0.2/annif/registry.py` & `annif-1.1.0/annif/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Registry that keeps track of Annif projects"""
+
 from __future__ import annotations
 
+import os
 import re
 
 from flask import Flask, current_app
 
 import annif
 from annif.config import parse_config
 from annif.exception import ConfigurationException
@@ -31,17 +33,19 @@
     def __init__(
         self, projects_config_path: str, datadir: str, init_projects: bool
     ) -> None:
         self._rid = id(self)
         self._projects_config_path = projects_config_path
         self._datadir = datadir
         self._init_vars()
+        projects_pattern = os.getenv("ANNIF_PROJECTS_INIT", ".*")
         if init_projects:
             for project in self._projects[self._rid].values():
-                project.initialize()
+                if re.search(projects_pattern, project.project_id) is not None:
+                    project.initialize()
 
     def _init_vars(self) -> None:
         # initialize the static variables, if necessary
         if self._rid not in self._projects:
             self._projects[self._rid] = self._create_projects()
             self._vocabs[self._rid] = {}
 
@@ -95,22 +99,19 @@
 
         match = re.match(r"([\w-]+)(\((.*)\))?$", vocab_spec)
         if match is None:
             raise ValueError(f"Invalid vocabulary specification: {vocab_spec}")
         vocab_id = match.group(1)
         posargs, kwargs = parse_args(match.group(3))
         language = posargs[0] if posargs else default_language
-        vocab_key = (vocab_id, language)
 
         self._init_vars()
-        if vocab_key not in self._vocabs[self._rid]:
-            self._vocabs[self._rid][vocab_key] = AnnifVocabulary(
-                vocab_id, self._datadir
-            )
-        return self._vocabs[self._rid][vocab_key], language
+        if vocab_id not in self._vocabs[self._rid]:
+            self._vocabs[self._rid][vocab_id] = AnnifVocabulary(vocab_id, self._datadir)
+        return self._vocabs[self._rid][vocab_id], language
 
 
 def initialize_projects(app: Flask) -> None:
     projects_config_path = app.config["PROJECTS_CONFIG_PATH"]
     datadir = app.config["DATADIR"]
     init_projects = app.config["INITIALIZE_PROJECTS"]
     app.annif_registry = AnnifRegistry(projects_config_path, datadir, init_projects)
```

### Comparing `annif-1.0.2/annif/rest.py` & `annif-1.1.0/annif/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Definitions for REST API operations. These are wired via Connexion to
 methods defined in the OpenAPI specification."""
+
 from __future__ import annotations
 
 import importlib
 from typing import TYPE_CHECKING, Any
 
 import connexion
 
 import annif.registry
 from annif.corpus import Document, DocumentList, SubjectSet
 from annif.exception import AnnifException
 from annif.project import Access
 
 if TYPE_CHECKING:
-    from datetime import datetime
-
     from connexion.lifecycle import ConnexionResponse
 
     from annif.corpus.subject import SubjectIndex
     from annif.suggestion import SubjectSuggestion, SuggestionResults
 
 
 def project_not_found_error(project_id: str) -> ConnexionResponse:
@@ -38,51 +37,53 @@
     or backend problem)"""
 
     return connexion.problem(
         status=503, title="Service unavailable", detail=err.format_message()
     )
 
 
-def show_info() -> dict[str, str]:
+def show_info() -> tuple:
     """return version of annif and a title for the api according to OpenAPI spec"""
 
-    return {"title": "Annif REST API", "version": importlib.metadata.version("annif")}
+    result = {"title": "Annif REST API", "version": importlib.metadata.version("annif")}
+    return result, 200, {"Content-Type": "application/json"}
 
 
 def language_not_supported_error(lang: str) -> ConnexionResponse:
     """return a Connexion error object when attempting to use unsupported language"""
 
     return connexion.problem(
         status=400,
         title="Bad Request",
         detail=f'language "{lang}" not supported by vocabulary',
     )
 
 
-def list_projects() -> dict[str, list[dict[str, str | dict | bool | datetime | None]]]:
+def list_projects() -> tuple:
     """return a dict with projects formatted according to OpenAPI spec"""
 
-    return {
+    result = {
         "projects": [
             proj.dump()
             for proj in annif.registry.get_projects(min_access=Access.public).values()
         ]
     }
+    return result, 200, {"Content-Type": "application/json"}
 
 
 def show_project(
     project_id: str,
 ) -> dict | ConnexionResponse:
     """return a single project formatted according to OpenAPI spec"""
 
     try:
         project = annif.registry.get_project(project_id, min_access=Access.hidden)
     except ValueError:
         return project_not_found_error(project_id)
-    return project.dump()
+    return project.dump(), 200, {"Content-Type": "application/json"}
 
 
 def _suggestion_to_dict(
     suggestion: SubjectSuggestion, subject_index: SubjectIndex, language: str
 ) -> dict[str, str | float | None]:
     subject = subject_index[suggestion.subject_id]
     return {
@@ -119,15 +120,15 @@
         (key, body[key]) for key in ["language", "limit", "threshold"] if key in body
     )
     documents = [{"text": body["text"]}]
     result = _suggest(project_id, documents, parameters)
 
     if _is_error(result):
         return result
-    return result[0]
+    return result[0], 200, {"Content-Type": "application/json"}
 
 
 def suggest_batch(
     project_id: str,
     body: dict[str, list],
     **query_parameters,
 ) -> list[dict[str, Any]] | ConnexionResponse:
@@ -137,15 +138,15 @@
     documents = body["documents"]
     result = _suggest(project_id, documents, query_parameters)
 
     if _is_error(result):
         return result
     for document_results, document in zip(result, documents):
         document_results["document_id"] = document.get("document_id")
-    return result
+    return result, 200, {"Content-Type": "application/json"}
 
 
 def _suggest(
     project_id: str,
     documents: list[dict[str, str]],
     parameters: dict[str, Any],
 ) -> list[dict[str, list]] | ConnexionResponse:
@@ -209,8 +210,8 @@
 
     try:
         corpus = _documents_to_corpus(body, project.subjects)
         project.learn(corpus)
     except AnnifException as err:
         return server_error(err)
 
-    return None, 204
+    return None, 204, {"Content-Type": "application/json"}
```

### Comparing `annif-1.0.2/annif/static/css/bootstrap.min.css` & `annif-1.1.0/annif/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/css/bootstrap.min.css.map` & `annif-1.1.0/annif/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/css/fonts.css` & `annif-1.1.0/annif/static/css/fonts.css`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/css/style.css` & `annif-1.1.0/annif/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
   right: 10px;
   background-color: #ff9182;
   color: black;
   border: none;
   border-radius: 0px;
   padding: 2px 7px;
 }
+#annif-version {
+  float: right;
+  margin-top: 0.5rem;
+  font-size: 1rem;
+}
 label, #suggestions {
   border-top: 1px solid #343260;
   margin-bottom: 0.5rem;
   padding-top: 0.5rem;
   text-transform: uppercase;
   font-size: 1.1rem;
   display: block;
```

### Comparing `annif-1.0.2/annif/static/favicon.ico` & `annif-1.1.0/annif/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/fonts/Jost-400-Book.otf` & `annif-1.1.0/annif/static/fonts/Jost-400-Book.otf`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/fonts/Jost-400-Book.ttf` & `annif-1.1.0/annif/static/fonts/Jost-400-Book.ttf`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/fonts/Jost-500-Medium.otf` & `annif-1.1.0/annif/static/fonts/Jost-500-Medium.otf`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/fonts/Jost-500-Medium.ttf` & `annif-1.1.0/annif/static/fonts/Jost-500-Medium.ttf`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/img/annif-RGB.svg` & `annif-1.1.0/annif/static/img/annif-RGB.svg`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/img/arrow-white.svg` & `annif-1.1.0/annif/static/img/arrow-white.svg`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/js/axios.min.js` & `annif-1.1.0/annif/static/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/js/axios.min.js.map` & `annif-1.1.0/annif/static/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/js/bootstrap.min.js` & `annif-1.1.0/annif/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/js/bootstrap.min.js.map` & `annif-1.1.0/annif/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/static/js/vue.min.js` & `annif-1.1.0/annif/static/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `annif-1.0.2/annif/suggestion.py` & `annif-1.1.0/annif/suggestion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Representing suggested subjects."""
+
 from __future__ import annotations
 
 import collections
 import itertools
 from typing import TYPE_CHECKING
 
 import numpy as np
@@ -34,15 +35,15 @@
     individual prediction; the rest will be left as zeros"""
 
     if limit == 0:
         return csr_array(preds.shape, dtype=np.float32)  # empty
 
     data, rows, cols = [], [], []
     for row in range(preds.shape[0]):
-        arow = preds.getrow(row)
+        arow = preds[[row]]
         if limit is not None and limit < len(arow.data):
             topk_idx = arow.data.argpartition(-limit)[-limit:]
         else:
             topk_idx = range(len(arow.data))
         for idx in topk_idx:
             if arow.data[idx] >= threshold:
                 data.append(arow.data[idx])
```

### Comparing `annif-1.0.2/annif/templates/home.html` & `annif-1.1.0/annif/templates/home.html`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,15 @@
           <h2 v-if="problem.hasTitle()"><% problem.title %></h2>
           <span v-if="problem.hasDetail()"><% problem.detail %></span>
         </div>
       </template>
       <div class="row mb-5">
         <div class="col-md-8">
           <annif-textarea @text-changed="onTextChanged" @text-cleared="onTextCleared"></annif-textarea>
+          <span id="annif-version">Annif v<% annif_version %></span>
         </div>
         <div class="col-md-4">
           <div id="project-selection-wrapper">
             <annif-projects :projects="projects" @project-selected="onProjectSelected"></annif-projects>
             <annif-project-info :projects="projects" :project="project"></annif-project-info>
           </div>
           <annif-limit :limit="limit" @limit-selected="onLimitSelected"></annif-limit>
@@ -229,24 +230,26 @@
 
 // Application, which uses the components above
 new Vue({
   delimiters: ["<%","%>"],
   el: '#app',
   data: {
     text: '',
+    annif_version: '',
     project: '',
     limit: 10,
     projects: [],
     results: [],
     problems: [],
     loading: false
   },
   mounted: function() {
     // TBD: we can add a button to reload the list of projects later
     this.loadProjects();
+    this.loadVersion();
   },
   methods: {
     clearResults: function() {
       while (this.results.length > 0) {
         this.results.pop();
       }
     },
@@ -278,29 +281,36 @@
           } else {
             var title = error.response.data.title || '';
             var detail = error.response.data.detail || '';
             this_.problems.push(new Problem(title, detail, true));
           }
         });
     },
+    loadVersion: function() {
+      var this_ = this;
+      axios.get('/v1/')
+        .then(res => {
+          this_.annif_version = res.data.version;
+        })
+    },
     suggest: function(event) {
       this.problems = [];
       if (this.text.trim() === '') {
         this.problems.push(new Problem('', 'You need to enter the text to get suggestions for', false));
       }
       if (this.project.trim() === '') {
         this.problems.push(new Problem('', 'You need to select one project', false));
       }
       this.clearResults();
       if (this.problems.length) {
         event.preventDefault();
         return;
       }
       var this_ = this;
-      var formData = new FormData();
+      var formData = new URLSearchParams();
       formData.append('text', this_.text);
       formData.append('limit', this_.limit);
       this_.loading = true;
       axios.post('/v1/projects/'+ this_.project + '/suggest', formData)
         .then(function(res) {
           if (res.data.results.length === 0) {
             this_.problems.push(new Problem('No results returned', '', false));
```

#### html2text {}

```diff
@@ -7,13 +7,14 @@
 Welcome!
 See the _O_p_e_n_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n for an interactive REST API specification.
 PPlleeaassee ccoorrrreecctt tthhee ffoolllloowwiinngg eerrrroorr((ss))::
 class="['alert', (problem.isError ? 'alert-danger' : 'alert-warning')]"
 role="alert" v-for="problem in problems">
 ********** <<%% pprroobblleemm..ttiittllee %%>> **********
 <% problem.detail %>
-text-changed="onTextChanged" @text-cleared="onTextCleared">
+text-changed="onTextChanged" @text-cleared="onTextCleared"> Annif v<%
+annif_version %>
 projects="projects" @project-selected="onProjectSelected">
 projects="projects" :project="project">
 limit="limit" @limit-selected="onLimitSelected">
 click="suggest" :disabled="loading"> Get suggestions Loading...
 results="results">
```

### Comparing `annif-1.0.2/annif/transform/__init__.py` & `annif-1.1.0/annif/transform/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for obtaining text transformation from string specification"""
+
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
 import annif
 from annif.exception import ConfigurationException
```

### Comparing `annif-1.0.2/annif/transform/inputlimiter.py` & `annif-1.1.0/annif/transform/inputlimiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A simple transformation that truncates the text of input documents to a
 given character length."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from annif.exception import ConfigurationException
 
 from . import transform
```

### Comparing `annif-1.0.2/annif/transform/langfilter.py` & `annif-1.1.0/annif/transform/langfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Transformation filtering out parts of a text that are in a language
 different from the language of the project."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from simplemma.langdetect import in_target_language
 
 import annif
```

### Comparing `annif-1.0.2/annif/transform/transform.py` & `annif-1.1.0/annif/transform/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common functionality for transforming text of input documents."""
+
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Type
 
 from annif.corpus import TransformingDocumentCorpus
 from annif.exception import ConfigurationException
```

### Comparing `annif-1.0.2/annif/util.py` & `annif-1.1.0/annif/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for Annif"""
+
 from __future__ import annotations
 
 import glob
 import logging
 import os
 import os.path
 import tempfile
```

### Comparing `annif-1.0.2/annif/vocab.py` & `annif-1.1.0/annif/vocab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Vocabulary management functionality for Annif"""
+
 from __future__ import annotations
 
 import os.path
 from typing import TYPE_CHECKING
 
 import annif
 import annif.corpus
```

### Comparing `annif-1.0.2/pyproject.toml` & `annif-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "annif"
-version = "1.0.2"
+version = "1.1.0"
 description = "Automated subject indexing and classification tool"
 authors = ["National Library of Finland <finto-posti@helsinki.fi>"]
 maintainers = [
     "Osma Suominen <osma.suominen@helsinki.fi>",
     "Juho Inkinen <juho.inkinen@helsinki.fi>",
     "Mona Lehtinen <mona.lehtinen@helsinki.fi>",
 ]
@@ -14,72 +14,70 @@
 repository = "https://github.com/NatLibFi/Annif"
 documentation = "https://github.com/NatLibFi/Annif/wiki"
 keywords = [
     "machine-learning",
     "text-classification",
     "rest-api",
     "code4lib",
-    "subject-indexing"
+    "subject-indexing",
 ]
 
-classifiers=[
+classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent"
+    "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 
-connexion = {version = "2.14.2", extras = ["swagger-ui"]}
-flask = "2.2.*"
-flask-cors = "4.0.*"
+connexion = { version = "~3.0.5", extras = ["flask", "uvicorn", "swagger-ui"] }
 click = "8.1.*"
 click-log = "0.4.*"
-joblib = "1.3.*"
+joblib = "1.4.*"
 nltk = "3.8.*"
 gensim = "4.3.*"
-scikit-learn = "1.3.*"
-scipy = "1.10.*"
-rdflib = "6.3.*"
-gunicorn = "21.2.*"
-numpy = "1.24.*"
-optuna = "3.3.*"
-python-dateutil = "2.8.*"
+scikit-learn = "1.4.*"
+scipy = "1.12.*"
+rdflib = "7.0.*"
+requests = "2.31.*"
+gunicorn = "22.0.*"
+numpy = "1.26.*"
+optuna = "3.6.*"
+python-dateutil = "2.9.*"
 tomli = { version = "2.0.*", python = "<3.11" }
 simplemma = "0.9.*"
-jsonschema = "4.17.*"
+jsonschema = "4.21.*"
+huggingface-hub = "0.22.*"
 
-fasttext-wheel = {version = "0.9.2", optional = true}
-voikko = {version = "0.5.*", optional = true}
-tensorflow-cpu = {version = "2.13.*", optional = true}
-tensorflow-io-gcs-filesystem = {version = "<=0.34.*", optional = true, python = "3.8"}
-lmdb = {version = "1.4.1", optional = true}
-omikuji = {version = "0.5.*", optional = true}
-yake = {version = "0.4.5", optional = true}
-spacy = {version = "3.6.*", optional = true}
-stwfsapy = {version="0.3.*", optional = true}
+fasttext-wheel = { version = "0.9.2", optional = true }
+voikko = { version = "0.5.*", optional = true }
+tensorflow-cpu = { version = "2.15.*", optional = true, python = "<3.12" }
+lmdb = { version = "1.4.1", optional = true }
+omikuji = { version = "0.5.*", optional = true }
+yake = { version = "0.4.8", optional = true }
+spacy = { version = "3.7.*", optional = true }
+stwfsapy = { version = "0.4.*", optional = true, python = "<3.12" }
 
 [tool.poetry.dev-dependencies]
 py = "*"
-pytest = "7.*"
-requests = "*"
+pytest = "8.*"
 pytest-cov = "*"
 pytest-watch = "*"
 pytest-flask = "*"
 flake8 = "*"
 bumpversion = "*"
-black = "23.*"
+black = "24.*"
 isort = "*"
 schemathesis = "3.*.*"
 
 [tool.poetry.extras]
 fasttext = ["fasttext-wheel"]
 voikko = ["voikko"]
-nn = ["tensorflow-cpu", "tensorflow-io-gcs-filesystem", "lmdb"]
+nn = ["tensorflow-cpu", "lmdb"]
 omikuji = ["omikuji"]
 yake = ["yake"]
 spacy = ["spacy"]
 stwfsa = ["stwfsapy"]
 
 [tool.poetry.scripts]
 annif = "annif.cli:cli"
@@ -90,11 +88,9 @@
 
 [tool.isort]
 profile = "black"
 line_length = "88"
 skip_gitignore = true
 
 [tool.pytest.ini_options]
-markers = [
-    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
-]
+markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
 addopts = "-m 'not slow'"
```

### Comparing `annif-1.0.2/PKG-INFO` & `annif-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 Metadata-Version: 2.1
 Name: annif
-Version: 1.0.2
+Version: 1.1.0
 Summary: Automated subject indexing and classification tool
 Home-page: https://annif.org
 License: Apache-2.0
 Keywords: machine-learning,text-classification,rest-api,code4lib,subject-indexing
 Author: National Library of Finland
 Author-email: finto-posti@helsinki.fi
 Maintainer: Osma Suominen
 Maintainer-email: osma.suominen@helsinki.fi
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fasttext
 Provides-Extra: nn
 Provides-Extra: omikuji
 Provides-Extra: spacy
 Provides-Extra: stwfsa
 Provides-Extra: voikko
 Provides-Extra: yake
 Requires-Dist: click (==8.1.*)
 Requires-Dist: click-log (==0.4.*)
-Requires-Dist: connexion[swagger-ui] (==2.14.2)
+Requires-Dist: connexion[flask,swagger-ui,uvicorn] (>=3.0.5,<3.1.0)
 Requires-Dist: fasttext-wheel (==0.9.2) ; extra == "fasttext"
-Requires-Dist: flask (==2.2.*)
-Requires-Dist: flask-cors (==4.0.*)
 Requires-Dist: gensim (==4.3.*)
-Requires-Dist: gunicorn (==21.2.*)
-Requires-Dist: joblib (==1.3.*)
-Requires-Dist: jsonschema (==4.17.*)
+Requires-Dist: gunicorn (==22.0.*)
+Requires-Dist: huggingface-hub (==0.22.*)
+Requires-Dist: joblib (==1.4.*)
+Requires-Dist: jsonschema (==4.21.*)
 Requires-Dist: lmdb (==1.4.1) ; extra == "nn"
 Requires-Dist: nltk (==3.8.*)
-Requires-Dist: numpy (==1.24.*)
+Requires-Dist: numpy (==1.26.*)
 Requires-Dist: omikuji (==0.5.*) ; extra == "omikuji"
-Requires-Dist: optuna (==3.3.*)
-Requires-Dist: python-dateutil (==2.8.*)
-Requires-Dist: rdflib (==6.3.*)
-Requires-Dist: scikit-learn (==1.3.*)
-Requires-Dist: scipy (==1.10.*)
+Requires-Dist: optuna (==3.6.*)
+Requires-Dist: python-dateutil (==2.9.*)
+Requires-Dist: rdflib (==7.0.*)
+Requires-Dist: requests (==2.31.*)
+Requires-Dist: scikit-learn (==1.4.*)
+Requires-Dist: scipy (==1.12.*)
 Requires-Dist: simplemma (==0.9.*)
-Requires-Dist: spacy (==3.6.*) ; extra == "spacy"
-Requires-Dist: stwfsapy (==0.3.*) ; extra == "stwfsa"
-Requires-Dist: tensorflow-cpu (==2.13.*) ; extra == "nn"
-Requires-Dist: tensorflow-io-gcs-filesystem (<=0.34) ; (python_version == "3.8") and (extra == "nn")
+Requires-Dist: spacy (==3.7.*) ; extra == "spacy"
+Requires-Dist: stwfsapy (==0.4.*) ; (python_version < "3.12") and (extra == "stwfsa")
+Requires-Dist: tensorflow-cpu (==2.15.*) ; (python_version < "3.12") and (extra == "nn")
 Requires-Dist: tomli (==2.0.*) ; python_version < "3.11"
 Requires-Dist: voikko (==0.5.*) ; extra == "voikko"
-Requires-Dist: yake (==0.4.5) ; extra == "yake"
+Requires-Dist: yake (==0.4.8) ; extra == "yake"
 Project-URL: Documentation, https://github.com/NatLibFi/Annif/wiki
 Project-URL: Repository, https://github.com/NatLibFi/Annif
 Description-Content-Type: text/markdown
 
 <img src="https://annif.org/static/img/annif-RGB.svg" width="150">
 
 [![DOI](https://zenodo.org/badge/100936800.svg)](https://zenodo.org/badge/latestdoi/100936800)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Container image](https://img.shields.io/badge/container_image-quay.io-blue.svg)](https://quay.io/repository/natlibfi/annif)
 [![CI/CD](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml)
 [![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/main/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)
-[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
 [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=main)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=main)
+[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/NatLibFi/Annif/badge)](https://securityscorecards.dev/viewer/?uri=github.com/NatLibFi/Annif)
 [![codebeat badge](https://codebeat.co/badges/7a8ef539-0094-48b8-84c2-c413b4a50d57)](https://codebeat.co/projects/github-com-natlibfi-annif-main)
 [![CodeQL](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NatLibFi_Annif&metric=alert_status)](https://sonarcloud.io/dashboard?id=NatLibFi_Annif)
 [![docs](https://readthedocs.org/projects/annif/badge/?version=latest)](https://annif.readthedocs.io/en/latest/index.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Annif is an automated subject indexing toolkit. It was originally created as
@@ -79,15 +80,15 @@
 
 [Finto AI](https://ai.finto.fi/) is a service based on Annif; see the [source code for Finto AI](https://github.com/NatLibFi/FintoAI).
 
 # Basic install
 
 Annif is developed and tested on Linux. If you want to run Annif on Windows or Mac OS, the recommended way is to use Docker (see below) or a Linux virtual machine.
 
-You will need Python 3.8+ to install Annif.
+You will need Python 3.9-3.12 to install Annif.
 
 The recommended way is to install Annif from
 [PyPI](https://pypi.org/project/annif/) into a virtual environment.
 
     python3 -m venv annif-venv
     source annif-venv/bin/activate
     pip install annif
```

