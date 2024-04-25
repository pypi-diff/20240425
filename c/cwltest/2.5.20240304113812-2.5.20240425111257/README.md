# Comparing `tmp/cwltest-2.5.20240304113812.tar.gz` & `tmp/cwltest-2.5.20240425111257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltest-2.5.20240304113812.tar", last modified: Mon Mar  4 11:42:22 2024, max compression
+gzip compressed data, was "cwltest-2.5.20240425111257.tar", last modified: Thu Apr 25 11:24:38 2024, max compression
```

## Comparing `cwltest-2.5.20240304113812.tar` & `cwltest-2.5.20240425111257.tar`

### file list

```diff
@@ -1,152 +1,157 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.736727 cwltest-2.5.20240304113812/
--rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      198 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.flake8
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.720727 cwltest-2.5.20240304113812/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.720727 cwltest-2.5.20240304113812/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3367 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1010 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       66 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      422 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     6428 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)     4334 2024-03-04 11:42:22.736727 cwltest-2.5.20240304113812/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3031 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.720727 cwltest-2.5.20240304113812/cwltest/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      334 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest/_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3646 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/argparser.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8920 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/compare.py
--rw-r--r--   0 michael   (1000) michael   (1000)      548 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/cwltest-schema-strict.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      585 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      738 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/hooks.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7451 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12691 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/plugin.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    15548 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/cwltest/utils.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.732727 cwltest-2.5.20240304113812/cwltest.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     4334 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3819 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      151 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-03-04 11:42:22.000000 cwltest-2.5.20240304113812/cwltest.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-04 11:39:40.000000 cwltest-2.5.20240304113812/cwltest.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)     3518 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      327 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     6358 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/pytest.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      135 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/docs/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/mypy-stubs/defusedxml/
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/defusedxml/ElementTree.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/defusedxml/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2521 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/junit_xml.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.724727 cwltest-2.5.20240304113812/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8351 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.728727 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      288 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.728727 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.728727 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1398 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/rdflib/term.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.728727 cwltest-2.5.20240304113812/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy-stubs/ruamel/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      568 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)     1839 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3496 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-03-04 11:42:22.736727 cwltest-2.5.20240304113812/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)       63 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.732727 cwltest-2.5.20240304113812/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.732727 cwltest-2.5.20240304113812/tests/test-data/
--rw-r--r--   0 michael   (1000) michael   (1000)      462 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/conformance_test_v1.0.cwltest.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      440 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/conformance_test_v1.2.cwltest.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/cores.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1077 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/cwltool-conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)      424 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/exclude-tags.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/integer-id.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      999 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/mock_cwl_runner.py
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/multi-lined-doc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      292 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/optional-error.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/optional-unsupported.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      537 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/required-unsupported.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/return-0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/return-1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/return-unsupported.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/short-names.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/string-id.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/timeout.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      240 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/timeout.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-04 11:42:22.732727 cwltest-2.5.20240304113812/tests/test-data/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/args.py
--rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/cat-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/cat-n-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/cat1-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1048 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/cat1-testcli.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/cat2-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)        3 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/empty.json
--rw-r--r--   0 michael   (1000) michael   (1000)       12 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/v1.0/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test-data/with-and-without-short-names.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      372 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_argparse.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3023 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_categories.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16651 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_compare.py
--rw-r--r--   0 michael   (1000) michael   (1000)      883 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_exclude_tags.py
--rw-r--r--   0 michael   (1000) michael   (1000)      387 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_integer_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)      721 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_multi_lined_doc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4511 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_plugin.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_prepare.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1669 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_short_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)      316 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_string_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1516 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/test_timeout.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tests/util.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2275 2024-03-04 11:39:38.000000 cwltest-2.5.20240304113812/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.932898 cwltest-2.5.20240425111257/
+-rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      198 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.flake8
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.904898 cwltest-2.5.20240425111257/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.908898 cwltest-2.5.20240425111257/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3367 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1010 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      422 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     6428 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     4334 2024-04-25 11:24:38.932898 cwltest-2.5.20240425111257/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3031 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.908898 cwltest-2.5.20240425111257/cwltest/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      334 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest/_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3646 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8920 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/compare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      548 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/cwltest-schema-strict.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      738 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/hooks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7465 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12691 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/plugin.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    16097 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/cwltest/utils.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.932898 cwltest-2.5.20240425111257/cwltest.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     4334 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3962 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      151 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-25 11:24:38.000000 cwltest-2.5.20240425111257/cwltest.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-25 11:20:44.000000 cwltest-2.5.20240425111257/cwltest.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)     3518 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      327 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     6358 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/pytest.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      135 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/docs/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.912898 cwltest-2.5.20240425111257/mypy-stubs/defusedxml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/defusedxml/ElementTree.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/defusedxml/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2521 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/junit_xml.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.916898 cwltest-2.5.20240425111257/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8351 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.920898 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      288 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.920898 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.920898 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.920898 cwltest-2.5.20240425111257/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy-stubs/ruamel/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)     1839 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3496 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-25 11:24:38.932898 cwltest-2.5.20240425111257/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)       63 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.924898 cwltest-2.5.20240425111257/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.928898 cwltest-2.5.20240425111257/tests/test-data/
+-rw-r--r--   0 michael   (1000) michael   (1000)      462 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/conformance_test_v1.0.cwltest.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      440 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/conformance_test_v1.2.cwltest.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/cores.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1077 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/cwltool-conftest.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       41 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/dummy-executor.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)        3 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/empty.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      424 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/exclude-tags.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/integer-id.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      999 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/mock_cwl_runner.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/multi-lined-doc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      198 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/nothing.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      292 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/optional-error.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/optional-unsupported.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/required-unsupported.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/return-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/return-1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/return-unsupported.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/short-names.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/string-id.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/timeout.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      240 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/timeout.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       85 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/true.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-25 11:24:38.932898 cwltest-2.5.20240425111257/tests/test-data/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/cat-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/cat-n-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/cat1-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1048 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/cat1-testcli.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/cat2-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)        3 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/empty.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/v1.0/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test-data/with-and-without-short-names.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      372 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_argparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3023 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_categories.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16651 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_compare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      883 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_exclude_tags.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      387 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_integer_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      513 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_invalid_outputs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_multi_lined_doc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4511 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_plugin.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_prepare.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1669 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_short_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      316 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_string_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1516 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/test_timeout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tests/util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2275 2024-04-25 11:20:40.000000 cwltest-2.5.20240425111257/tox.ini
```

### Comparing `cwltest-2.5.20240304113812/.github/dependabot.yml` & `cwltest-2.5.20240425111257/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/.github/workflows/ci-tests.yml` & `cwltest-2.5.20240425111257/.github/workflows/ci-tests.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/.github/workflows/codeql-analysis.yml` & `cwltest-2.5.20240425111257/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/.readthedocs.yml` & `cwltest-2.5.20240425111257/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/LICENSE` & `cwltest-2.5.20240425111257/LICENSE`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/Makefile` & `cwltest-2.5.20240425111257/Makefile`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/PKG-INFO` & `cwltest-2.5.20240425111257/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltest
-Version: 2.5.20240304113812
+Version: 2.5.20240425111257
 Summary: Common Workflow Language testing framework
 Author-email: Common workflow language working group <common-workflow-language@googlegroups.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/common-workflow-language/cwltest
 Project-URL: Download, https://github.com/common-workflow-language/cwltest
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
```

### Comparing `cwltest-2.5.20240304113812/README.rst` & `cwltest-2.5.20240425111257/README.rst`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/argparser.py` & `cwltest-2.5.20240425111257/cwltest/argparser.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/compare.py` & `cwltest-2.5.20240425111257/cwltest/compare.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/cwltest-schema-strict.yml` & `cwltest-2.5.20240425111257/cwltest/cwltest-schema-strict.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/cwltest-schema.yml` & `cwltest-2.5.20240425111257/cwltest/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/hooks.py` & `cwltest-2.5.20240425111257/cwltest/hooks.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/main.py` & `cwltest-2.5.20240425111257/cwltest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     if args.exclude_tags:
         tags = set(args.exclude_tags.split(","))
         tests = [t for t in tests if not tags.intersection(t.get("tags", []))]
 
     for t in tests:
         if t.get("label"):
             logger.warning("The `label` field is deprecated. Use `id` field instead.")
-            t["short_name"] = t["label"]
+            t["short_name"] = t["label"]  # noqa: B909
         elif t.get("id"):
             if isinstance(t.get("id"), str):
                 t["short_name"] = utils.shortname(t["id"])
             else:
                 logger.warning(
                     "The `id` field with integer is deprecated. Use string identifier instead."
                 )
```

### Comparing `cwltest-2.5.20240304113812/cwltest/plugin.py` & `cwltest-2.5.20240425111257/cwltest/plugin.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/cwltest/utils.py` & `cwltest-2.5.20240425111257/cwltest/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,14 +418,31 @@
     except KeyboardInterrupt:
         logger.error(
             """Test %s interrupted: %s""",
             number,
             " ".join([shlex.quote(tc) for tc in test_command]),
         )
         raise
+    except json.JSONDecodeError:
+        logger.error(
+            """Test %s failed: %s""",
+            number,
+            " ".join([shlex.quote(tc) for tc in test_command]),
+        )
+        logger.error(test.get("doc", "").replace("\n", " ").strip())
+        invalid_json_msg = "Output is not a valid JSON document: '%s'" % outstr
+        logger.error(invalid_json_msg)
+        return TestResult(
+            1,
+            outstr,
+            outerr,
+            duration,
+            config.classname,
+            invalid_json_msg,
+        )
     except subprocess.TimeoutExpired:
         logger.error(
             """Test %s timed out: %s""",
             number,
             " ".join([shlex.quote(tc) for tc in test_command]),
         )
         logger.error(test.get("doc", "").replace("\n", " ").strip())
```

### Comparing `cwltest-2.5.20240304113812/cwltest.egg-info/PKG-INFO` & `cwltest-2.5.20240425111257/cwltest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltest
-Version: 2.5.20240304113812
+Version: 2.5.20240425111257
 Summary: Common Workflow Language testing framework
 Author-email: Common workflow language working group <common-workflow-language@googlegroups.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/common-workflow-language/cwltest
 Project-URL: Download, https://github.com/common-workflow-language/cwltest
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
```

### Comparing `cwltest-2.5.20240304113812/cwltest.egg-info/SOURCES.txt` & `cwltest-2.5.20240425111257/cwltest.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -91,39 +91,44 @@
 mypy-stubs/ruamel/__init__.pyi
 tests/__init__.py
 tests/test_argparse.py
 tests/test_categories.py
 tests/test_compare.py
 tests/test_exclude_tags.py
 tests/test_integer_id.py
+tests/test_invalid_outputs.py
 tests/test_multi_lined_doc.py
 tests/test_plugin.py
 tests/test_prepare.py
 tests/test_short_names.py
 tests/test_string_id.py
 tests/test_timeout.py
 tests/util.py
 tests/test-data/conformance_test_v1.0.cwltest.yml
 tests/test-data/conformance_test_v1.2.cwltest.yaml
 tests/test-data/cores.txt
 tests/test-data/cwltool-conftest.py
+tests/test-data/dummy-executor.sh
+tests/test-data/empty.yml
 tests/test-data/exclude-tags.yml
 tests/test-data/integer-id.yml
 tests/test-data/mock_cwl_runner.py
 tests/test-data/multi-lined-doc.yml
+tests/test-data/nothing.yml
 tests/test-data/optional-error.yml
 tests/test-data/optional-unsupported.yml
 tests/test-data/required-unsupported.yml
 tests/test-data/return-0.cwl
 tests/test-data/return-1.cwl
 tests/test-data/return-unsupported.cwl
 tests/test-data/short-names.yml
 tests/test-data/string-id.yml
 tests/test-data/timeout.cwl
 tests/test-data/timeout.yml
+tests/test-data/true.cwl
 tests/test-data/with-and-without-short-names.yml
 tests/test-data/v1.0/args.py
 tests/test-data/v1.0/cat-job.json
 tests/test-data/v1.0/cat-n-job.json
 tests/test-data/v1.0/cat1-job.json
 tests/test-data/v1.0/cat1-testcli.cwl
 tests/test-data/v1.0/cat2-job.json
```

### Comparing `cwltest-2.5.20240304113812/docs/Makefile` & `cwltest-2.5.20240425111257/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/docs/_static/favicon.ico` & `cwltest-2.5.20240425111257/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/docs/conf.py` & `cwltest-2.5.20240425111257/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/docs/pytest.rst` & `cwltest-2.5.20240425111257/docs/pytest.rst`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/cachecontrol/wrapper.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/junit_xml.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/junit_xml.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/__init__.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/collection.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/graph.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/paths.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/query.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/resource.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/mypy-stubs/rdflib/term.pyi` & `cwltest-2.5.20240425111257/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/pyproject.toml` & `cwltest-2.5.20240425111257/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/release-test.sh` & `cwltest-2.5.20240425111257/release-test.sh`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test-data/cwltool-conftest.py` & `cwltest-2.5.20240425111257/tests/test-data/cwltool-conftest.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test-data/mock_cwl_runner.py` & `cwltest-2.5.20240425111257/tests/test-data/mock_cwl_runner.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test-data/required-unsupported.yml` & `cwltest-2.5.20240425111257/tests/test-data/required-unsupported.yml`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test-data/v1.0/cat1-testcli.cwl` & `cwltest-2.5.20240425111257/tests/test-data/v1.0/cat1-testcli.cwl`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_categories.py` & `cwltest-2.5.20240425111257/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_compare.py` & `cwltest-2.5.20240425111257/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_exclude_tags.py` & `cwltest-2.5.20240425111257/tests/test_exclude_tags.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_multi_lined_doc.py` & `cwltest-2.5.20240425111257/tests/test_multi_lined_doc.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_plugin.py` & `cwltest-2.5.20240425111257/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_prepare.py` & `cwltest-2.5.20240425111257/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_short_names.py` & `cwltest-2.5.20240425111257/tests/test_short_names.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/test_timeout.py` & `cwltest-2.5.20240425111257/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `cwltest-2.5.20240304113812/tests/util.py` & `cwltest-2.5.20240425111257/tests/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test functions."""
 
 import atexit
 import os
 import subprocess  # nosec
 from contextlib import ExitStack
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from cwltest.utils import as_file, files
 
 
 def get_data(filename: str) -> str:
     """Return the absolute path starting from a file name."""
     filename = os.path.normpath(filename)
@@ -24,17 +24,20 @@
     except ModuleNotFoundError:
         pass
     if not filepath or not os.path.isfile(filepath):
         filepath = Path(os.path.dirname(__file__)) / ".." / filename
     return str(filepath.resolve())
 
 
-def run_with_mock_cwl_runner(args: List[str]) -> Tuple[int, str, str]:
+def run_with_mock_cwl_runner(
+    args: List[str], cwl_runner: Optional[str] = None
+) -> Tuple[int, str, str]:
     """Bind a mock cwlref-runner implementation to cwltest."""
-    cwl_runner = get_data("tests/test-data/mock_cwl_runner.py")
+    if cwl_runner is None:
+        cwl_runner = get_data("tests/test-data/mock_cwl_runner.py")
     process = subprocess.Popen(  # nosec
         ["cwltest", "--tool", cwl_runner] + args,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
 
     stdout, stderr = process.communicate()
```

### Comparing `cwltest-2.5.20240304113812/tox.ini` & `cwltest-2.5.20240425111257/tox.ini`

 * *Files identical despite different names*

