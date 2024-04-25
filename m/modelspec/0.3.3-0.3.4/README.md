# Comparing `tmp/modelspec-0.3.3.tar.gz` & `tmp/modelspec-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelspec-0.3.3.tar", last modified: Thu Dec 14 10:46:28 2023, max compression
+gzip compressed data, was "modelspec-0.3.4.tar", last modified: Thu Apr 25 12:59:44 2024, max compression
```

## Comparing `modelspec-0.3.3.tar` & `modelspec-0.3.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.812814 modelspec-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.792814 modelspec-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-12-14 10:46:19.000000 modelspec-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-14 10:46:19.000000 modelspec-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-12-14 10:46:19.000000 modelspec-0.3.3/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2023-12-14 10:46:19.000000 modelspec-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-14 10:46:19.000000 modelspec-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-14 10:46:19.000000 modelspec-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-12-14 10:46:28.812814 modelspec-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-14 10:46:19.000000 modelspec-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/contributors.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/sphinx/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/sphinx/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/_static/pydata-custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/_static/rtd-custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/sphinx/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/_templates/custom-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.796814 modelspec-0.3.3/docs/sphinx/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/Contributors.md
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/Installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/Introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/Quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.800814 modelspec-0.3.3/docs/sphinx/source/api/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.bson
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.json
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.rst
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.bson
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.xml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/examples/document.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-12-14 10:46:19.000000 modelspec-0.3.3/docs/sphinx/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.800814 modelspec-0.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/COMBINE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.bson
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.json
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.specification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.xml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/document.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.800814 modelspec-0.3.3/examples/images/
--rw-r--r--   0 runner    (1001) docker     (127)   168517 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/images/combine.png
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/images/neuroml.png
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/images/sbml.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.804814 modelspec-0.3.3/examples/neuroml2/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/neuroml2/.test.validate.omt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/neuroml2/LEMS_hello_world.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/neuroml2/NeuroML2.md
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-14 10:46:19.000000 modelspec-0.3.3/examples/neuroml2/NeuroML2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/NeuroML2.specification.json
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/NeuroML2.specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/TestNeuroML.bson
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/TestNeuroML.json
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/TestNeuroML.xml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/TestNeuroML.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/hello_world_neuroml.net.nml
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/neuroml2/neuroml2_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.804814 modelspec-0.3.3/examples/sbml/
--rw-r--r--   0 runner    (1001) docker     (127)    32856 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/SBML.md
--rw-r--r--   0 runner    (1001) docker     (127)    40472 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/SBML.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29862 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/SBML.specification.json
--rw-r--r--   0 runner    (1001) docker     (127)    20363 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/SBML.specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/example_sbml_minimal.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      145 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/regenerateAndTest.sh
--rw-r--r--   0 runner    (1001) docker     (127)    13027 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/sbml32spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/sbml_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/test_minimal_example.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/test_minimal_example.xml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/test_minimal_example.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2005 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/sbml/test_sbml3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.808814 modelspec-0.3.3/examples/test/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test.md
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test.specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test_instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-14 10:46:20.000000 modelspec-0.3.3/examples/test/test_instance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-14 10:46:20.000000 modelspec-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2023-12-14 10:46:28.812814 modelspec-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.792814 modelspec-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.808814 modelspec-0.3.3/src/modelspec/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-14 10:46:20.000000 modelspec-0.3.3/src/modelspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40488 2023-12-14 10:46:20.000000 modelspec-0.3.3/src/modelspec/base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    19227 2023-12-14 10:46:20.000000 modelspec-0.3.3/src/modelspec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.808814 modelspec-0.3.3/src/modelspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-12-14 10:46:28.000000 modelspec-0.3.3/src/modelspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-12-14 10:46:28.000000 modelspec-0.3.3/src/modelspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 10:46:28.000000 modelspec-0.3.3/src/modelspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-14 10:46:28.000000 modelspec-0.3.3/src/modelspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-14 10:46:28.000000 modelspec-0.3.3/src/modelspec.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      654 2023-12-14 10:46:20.000000 modelspec-0.3.3/test_all.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.808814 modelspec-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 10:46:28.808814 modelspec-0.3.3/tests/temp/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-14 10:46:20.000000 modelspec-0.3.3/tests/temp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2023-12-14 10:46:20.000000 modelspec-0.3.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-14 10:46:20.000000 modelspec-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.821573 modelspec-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.801573 modelspec-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-25 12:59:39.000000 modelspec-0.3.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-25 12:59:39.000000 modelspec-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-25 12:59:39.000000 modelspec-0.3.4/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 12:59:39.000000 modelspec-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 12:59:39.000000 modelspec-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 12:59:39.000000 modelspec-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-25 12:59:44.821573 modelspec-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 12:59:39.000000 modelspec-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/docs/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/docs/sphinx/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/docs/sphinx/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/_static/pydata-custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/_static/rtd-custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.805573 modelspec-0.3.4/docs/sphinx/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/_templates/custom-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.809573 modelspec-0.3.4/docs/sphinx/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/Contributors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/Installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/Introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/Quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.809573 modelspec-0.3.4/docs/sphinx/source/api/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.bson
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.bson
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/examples/document.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-25 12:59:39.000000 modelspec-0.3.4/docs/sphinx/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.809573 modelspec-0.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/COMBINE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.bson
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.specification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/document.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.813573 modelspec-0.3.4/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   168517 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/images/combine.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/images/neuroml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/images/sbml.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.813573 modelspec-0.3.4/examples/neuroml2/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/.test.validate.omt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/LEMS_hello_world.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/NeuroML2.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/NeuroML2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/NeuroML2.specification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/NeuroML2.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/TestNeuroML.bson
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/TestNeuroML.json
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/TestNeuroML.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/TestNeuroML.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/hello_world_neuroml.net.nml
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/neuroml2/neuroml2_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/examples/sbml/
+-rw-r--r--   0 runner    (1001) docker     (127)    32856 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/SBML.md
+-rw-r--r--   0 runner    (1001) docker     (127)    40472 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/SBML.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29862 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/SBML.specification.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/SBML.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/example_sbml_minimal.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/regenerateAndTest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/sbml32spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/sbml_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/test_minimal_example.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/test_minimal_example.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/test_minimal_example.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1995 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/sbml/test_sbml3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/examples/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test.specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test_instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 12:59:39.000000 modelspec-0.3.4/examples/test/test_instance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 12:59:39.000000 modelspec-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-25 12:59:44.821573 modelspec-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.801573 modelspec-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/src/modelspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 12:59:39.000000 modelspec-0.3.4/src/modelspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40010 2024-04-25 12:59:39.000000 modelspec-0.3.4/src/modelspec/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19348 2024-04-25 12:59:39.000000 modelspec-0.3.4/src/modelspec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/src/modelspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-25 12:59:44.000000 modelspec-0.3.4/src/modelspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-25 12:59:44.000000 modelspec-0.3.4/src/modelspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:59:44.000000 modelspec-0.3.4/src/modelspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 12:59:44.000000 modelspec-0.3.4/src/modelspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 12:59:44.000000 modelspec-0.3.4/src/modelspec.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-04-25 12:59:39.000000 modelspec-0.3.4/test_all.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:44.817573 modelspec-0.3.4/tests/temp/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 12:59:39.000000 modelspec-0.3.4/tests/temp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-04-25 12:59:39.000000 modelspec-0.3.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-25 12:59:39.000000 modelspec-0.3.4/tests/test_utils.py
```

### Comparing `modelspec-0.3.3/.github/workflows/python-publish.yml` & `modelspec-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/.github/workflows/static.yml` & `modelspec-0.3.4/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/.gitignore` & `modelspec-0.3.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -160,7 +160,8 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 /examples/document.specification.bson
 /examples/neuroml2/hello_world.v.dat
 /examples/sbml/example_sbml_test.xml
+/updatelibs.sh
```

### Comparing `modelspec-0.3.3/.pre-commit-config.yaml` & `modelspec-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/LICENSE` & `modelspec-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/PKG-INFO` & `modelspec-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelspec
-Version: 0.3.3
+Version: 0.3.4
 Summary: A common JSON/YAML based format for compact model specification
 Home-page: https://github.com/ModECI/modelspec
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: Padraig Gleeson, David Turner
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
```

### Comparing `modelspec-0.3.3/README.md` & `modelspec-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/contributors.py` & `modelspec-0.3.4/docs/contributors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import requests
 import pandas as pd
-import json
 import textwrap
 from datetime import date
 
 
 url = "https://api.github.com/repos/modeci/modelspec/contributors"
 
 response = requests.get(url=url, auth=("<github_username>", "<github_token>"))
```

### Comparing `modelspec-0.3.3/docs/sphinx/Makefile` & `modelspec-0.3.4/docs/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/make.bat` & `modelspec-0.3.4/docs/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/_static/rtd-custom.css` & `modelspec-0.3.4/docs/sphinx/source/_static/rtd-custom.css`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/_templates/custom-class-template.rst` & `modelspec-0.3.4/docs/sphinx/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/_templates/custom-module-template.rst` & `modelspec-0.3.4/docs/sphinx/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/Contributors.md` & `modelspec-0.3.4/docs/sphinx/source/api/Contributors.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 (Modelspec:contributors)=
 
 # Modelspec contributors
 
 This page list names and Github profiles of contributors to Modelspec, listed in no particular order.
-This page is generated periodically, most recently on 2023-12-13.
+This page is generated periodically, most recently on 2024-04-25.
 
 - Padraig Gleeson ([@pgleeson](https://github.com/pgleeson))
 - Manifest Chakalov  ([@mqnifestkelvin](https://github.com/mqnifestkelvin))
 - David Turner ([@davidt0x](https://github.com/davidt0x))
 - Peace Ododo ([@Onoyiza](https://github.com/Onoyiza))
 - Parikshit Singh Rathore ([@parikshit14](https://github.com/parikshit14))
 - Ankur Sinha ([@sanjayankur31](https://github.com/sanjayankur31))
 - kmantel ([@kmantel](https://github.com/kmantel))
+- Robert Vickerstaff ([@robertvi](https://github.com/robertvi))
```

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/Installation.md` & `modelspec-0.3.4/docs/sphinx/source/api/Installation.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/Introduction.md` & `modelspec-0.3.4/docs/sphinx/source/api/Introduction.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/Quickstart.md` & `modelspec-0.3.4/docs/sphinx/source/api/Quickstart.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/README.md` & `modelspec-0.3.4/docs/sphinx/source/api/examples/README.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.json` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.md` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.py` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import modelspec
 from modelspec import field, instance_of, optional
 from modelspec.base_types import Base
 from typing import List
 import sys
+import json
+import yaml
+import bson
 
 # Example showing how to create a model of a document and use it to create/serialize instances
 
 
 @modelspec.define
 class Paragraph(Base):
     """
@@ -92,17 +95,14 @@
 with open("document.rst", "w") as d:
     d.write(doc_rst)
 
 
 print("\n  >> Generating specification in dict form...")
 doc_dict = doc.generate_documentation(format="dict")
 
-import json
-import yaml
-import bson
 
 with open("document.specification.json", "w") as d:
     d.write(json.dumps(doc_dict, indent=4))
 
 print("  >> Generating specification in YAML...\n")
 
 with open("document.specification.yaml", "w") as d:
```

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.rst` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.bson` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.bson`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.json` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/api/examples/document.specification.yaml` & `modelspec-0.3.4/docs/sphinx/source/api/examples/document.specification.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/conf.py` & `modelspec-0.3.4/docs/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/docs/sphinx/source/index.rst` & `modelspec-0.3.4/docs/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/COMBINE.md` & `modelspec-0.3.4/examples/COMBINE.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/README.md` & `modelspec-0.3.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/document.json` & `modelspec-0.3.4/examples/document.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/document.md` & `modelspec-0.3.4/examples/document.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/document.py` & `modelspec-0.3.4/examples/document.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import modelspec
 from modelspec import field, instance_of, optional
 from modelspec.base_types import Base
 from typing import List
 import sys
+import json
+import yaml
+import bson
 
 # Example showing how to create a model of a document and use it to create/serialize instances
 
 
 @modelspec.define
 class Paragraph(Base):
     """
@@ -92,17 +95,14 @@
 with open("document.rst", "w") as d:
     d.write(doc_rst)
 
 
 print("\n  >> Generating specification in dict form...")
 doc_dict = doc.generate_documentation(format="dict")
 
-import json
-import yaml
-import bson
 
 with open("document.specification.json", "w") as d:
     d.write(json.dumps(doc_dict, indent=4))
 
 print("  >> Generating specification in YAML...\n")
 
 with open("document.specification.yaml", "w") as d:
```

### Comparing `modelspec-0.3.3/examples/document.rst` & `modelspec-0.3.4/examples/document.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/document.specification.json` & `modelspec-0.3.4/examples/document.specification.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/document.specification.yaml` & `modelspec-0.3.4/examples/document.specification.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/images/combine.png` & `modelspec-0.3.4/examples/images/combine.png`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/images/neuroml.png` & `modelspec-0.3.4/examples/images/neuroml.png`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/images/sbml.png` & `modelspec-0.3.4/examples/images/sbml.png`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/LEMS_hello_world.xml` & `modelspec-0.3.4/examples/neuroml2/LEMS_hello_world.xml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/NeuroML2.md` & `modelspec-0.3.4/examples/neuroml2/NeuroML2.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/NeuroML2.rst` & `modelspec-0.3.4/examples/neuroml2/NeuroML2.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/NeuroML2.specification.json` & `modelspec-0.3.4/examples/neuroml2/NeuroML2.specification.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/NeuroML2.specification.yaml` & `modelspec-0.3.4/examples/neuroml2/NeuroML2.specification.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/TestNeuroML.json` & `modelspec-0.3.4/examples/neuroml2/TestNeuroML.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/TestNeuroML.xml` & `modelspec-0.3.4/examples/neuroml2/TestNeuroML.xml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/TestNeuroML.yaml` & `modelspec-0.3.4/examples/neuroml2/TestNeuroML.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/hello_world_neuroml.net.nml` & `modelspec-0.3.4/examples/neuroml2/hello_world_neuroml.net.nml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/neuroml2/neuroml2_spec.py` & `modelspec-0.3.4/examples/neuroml2/neuroml2_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 
     izhikevich2007Cells: List[izhikevich2007Cell] = field(factory=list)
     pulseGenerators: List[pulseGenerator] = field(factory=list)
     networks: List[network] = field(factory=list)
 
 
 if __name__ == "__main__":
-
     nml_doc = neuroml(id="TestNeuroML")
 
     izh = izhikevich2007Cell(
         id="izh2007RS0",
         C="100pF",
         v0="-60mV",
         k="0.7nS_per_mV",
```

### Comparing `modelspec-0.3.3/examples/sbml/SBML.md` & `modelspec-0.3.4/examples/sbml/SBML.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/SBML.rst` & `modelspec-0.3.4/examples/sbml/SBML.rst`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/SBML.specification.json` & `modelspec-0.3.4/examples/sbml/SBML.specification.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/SBML.specification.yaml` & `modelspec-0.3.4/examples/sbml/SBML.specification.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/sbml32spec.py` & `modelspec-0.3.4/examples/sbml/sbml32spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     annotation: str = field(
         default=None, validator=optional([instance_of(str), valid_xml_content])
     )
 
 
 @modelspec.define
 class SBaseWithId(SBase):
-
     id: str = field(default=None, validator=optional([instance_of(str), valid_sid]))
 
 
 @modelspec.define
 class Trigger(SBase):
     initialValue: bool = field(default=None, validator=instance_of(bool))
     persistent: bool = field(default=None, validator=instance_of(bool))
```

### Comparing `modelspec-0.3.3/examples/sbml/sbml_validators.py` & `modelspec-0.3.4/examples/sbml/sbml_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """.split()
 
 SBML_VERSION = "2"
 SBML_LEVEL = "3"
 
 
 def valid_kind(instance, attribute, value):
-    if not value in sbml_si_units:
+    if value not in sbml_si_units:
         raise ValueError(
             f"kind {value} must be one of the standard SI units: {sbml_si_units}"
         )
 
 
 def valid_mathml(instance, attribute, value):
     "http://www.w3.org/1998/Math/MathML"
@@ -164,15 +164,14 @@
             )
     print("-" * 80)
 
     return len(warnings) + len(errors)
 
 
 if __name__ == "__main__":
-
     import libsbml
 
     sbml_file = sys.argv[1]
 
     print("Going to validate SBML file: %s" % sbml_file)
     reader = libsbml.SBMLReader()
     document = reader.readSBML(sbml_file)
```

### Comparing `modelspec-0.3.3/examples/sbml/test_minimal_example.json` & `modelspec-0.3.4/examples/sbml/test_minimal_example.json`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/test_minimal_example.xml` & `modelspec-0.3.4/examples/sbml/test_minimal_example.xml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/sbml/test_sbml3.py` & `modelspec-0.3.4/examples/sbml/test_sbml3.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 derived from https://github.com/combine-org/draft-modelspec-sbml-api/blob/main/test_sbml32.py
 a minimalish sbml to xml example
 """
 
 import json
 import yaml
-import os
 
 from sbml32spec import *
 
 
 def test_example_sbml_minimal():
     "aiming to match the xml file example_sbml_minimal.xml"
```

### Comparing `modelspec-0.3.3/examples/test/test.md` & `modelspec-0.3.4/examples/test/test.md`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/examples/test/test.py` & `modelspec-0.3.4/examples/test/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import modelspec
 from modelspec import field, instance_of, optional
 from modelspec.base_types import Base
-from modelspec.utils import load_json
-from typing import List
 from typing import Any
 import sys
+import yaml
 
 
 # Example testing multiple options...
 
 
 def convert2float(x: Any) -> float:
     print("convert2float {} ({})".format(x, type(x)))
@@ -100,12 +99,11 @@
 with open("test.md", "w") as d:
     d.write(doc_md)
 
 
 print("\nGenerating specification in dict form")
 doc_dict = tc.generate_documentation(format="dict")
 
-import yaml
 
 print("Generating specification in YAML")
 with open("test.specification.yaml", "w") as d:
     d.write(yaml.dump(doc_dict, indent=4, sort_keys=False))
```

### Comparing `modelspec-0.3.3/examples/test/test.specification.yaml` & `modelspec-0.3.4/examples/test/test.specification.yaml`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/setup.cfg` & `modelspec-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/src/modelspec/base_types.py` & `modelspec-0.3.4/src/modelspec/base_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
     @classmethod
     def from_dict(cls, d: Dict[str, Any]) -> "Base":
         """Instantiate an Base object from a dictionary"""
 
         # If this object has an id attribute, it may have been serialized within a dict with the id as the key, even if
         # it is a single object.
         if "id" in [f.name for f in attr.fields(cls)] and "id" not in d.keys():
-
             keys = list(d.keys())
             if len(keys) == 0:
                 raise ValueError(
                     f"Cannot deserialize Base modelspec object ({cls}) because it is empty."
                 )
 
             # Get the first key, this should be the id
@@ -163,29 +162,19 @@
 
     @classmethod
     def from_yaml(cls, yaml_str: str) -> "Base":
         """Instantiate an modelspec object from a YAML string"""
         return cls.from_dict(yaml.load(yaml_str, Loader=yaml.SafeLoader))
 
     @classmethod
-    def from_yaml_file(cls, yaml_file: str) -> "Base":
-        """Instantiate an modelspec object from a file containing YAML"""
-        return cls.from_dict(yaml.load(yaml_str, Loader=yaml.SafeLoader))
-
-    @classmethod
     def from_json(cls, json_str: str) -> "Base":
         """Instantiate an modelspec object from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     @classmethod
-    def from_json_file(cls, json_file: str) -> "Base":
-        """Instantiate an modelspec object from a file containing JSON"""
-        return cls.from_dict(json.load(json_file))
-
-    @classmethod
     def from_bson(cls, bson_str: str) -> "Base":
         """Instantiate an modelspec object from a BSON string"""
         return cls.from_dict(bson.decode(bson_str))
 
     @classmethod
     def from_xml(cls, xml_str: str) -> "Base":
         """Instantiate a Base object from an XML string"""
@@ -298,15 +287,14 @@
             The name of the generated yaml file
         """
 
         if filename is None:
             filename = f"{self.id}.yaml"
 
         with open(filename, "w") as outfile:
-
             # We need to setup another
             yaml.dump(
                 yaml_converter.unstructure(self.to_dict()),
                 outfile,
                 sort_keys=False,
                 indent=4,
             )
@@ -314,16 +302,14 @@
         return filename
 
     def to_xml_file(
         self,
         filename: Optional[str] = None,
         include_metadata: bool = True,
     ) -> str:
-        from modelspec.utils import build_xml_element
-
         if filename is None:
             filename = f"{self.id}.xml"
 
         pretty_xml_str = self.to_xml()
 
         # Write the XML data to the file
         with open(filename, "w", encoding="utf-8") as file:
@@ -638,15 +624,14 @@
         value,
         can_be_list=False,
         can_be_dict=False,
         can_be_ndarray=False,
         can_be_none=False,
         can_be_eval_expr=False,
     ):
-
         import numpy
 
         if verbose:
             print_v(
                 " > Checking type of %s, ee: %s"
                 % (value, cls._is_evaluable_expression(value))
             )
@@ -732,15 +717,14 @@
         allowed_children = cls._parse_allowed_children()
 
         # print(f" - {cls.__name__} ({definition})")
 
         rst_url_format = "`%s <%s>`__"
 
         def insert_links(text, format=MARKDOWN_FORMAT):
-
             code_ref = ":code:`"
             # print("    > Converting: %s" % text)
             text2 = text
             while code_ref in text2:
                 ind = text2.index(code_ref)
                 ind2 = text2.index("`", ind + len(code_ref) + 1)
                 pre = text2[0:ind]
```

### Comparing `modelspec-0.3.3/src/modelspec/utils.py` & `modelspec-0.3.4/src/modelspec/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import attr
 
 
 from modelspec.base_types import print_
 from modelspec.base_types import EvaluableExpression
 
 from random import Random
-from typing import Union, Dict
+from typing import Union
 
 verbose = False
 
 
 def load_json(filename: str):
     """
     Load a generic JSON file
@@ -188,22 +188,20 @@
     elif isinstance(value, list):
         return [convert_xml_dict_values(item) for item in value]
 
     return value
 
 
 def save_to_json_file(info_dict, filename, indent=4):
-
     strj = json.dumps(info_dict, indent=indent)
     with open(filename, "w") as fp:
         fp.write(strj)
 
 
 def save_to_yaml_file(info_dict, filename, indent=4):
-
     if sys.version_info[0] == 2:
         stry = yaml.dump(info_dict, indent=indent, default_flow_style=False)
     else:
         stry = yaml.dump(info_dict, indent=indent, sort_keys=False)
     with open(filename, "w") as fp:
         fp.write(stry)
 
@@ -247,15 +245,14 @@
     if parent is None:
         parent = ET.Element(data.__class__.__name__)
 
     print_(" == Converting to XML: %s" % data, verbose)
 
     attrs = attr.fields(data.__class__)
     for aattr in attrs:
-
         print_("     == Looking at: {} ({})".format(aattr, type(aattr)), verbose)
         if isinstance(aattr.default, attr.Factory):
             children = data.__getattribute__(aattr.name)
             if not isinstance(children, (list, tuple)):
                 children = [children]
 
             for child in children:
@@ -268,23 +265,22 @@
             attribute_value = data.__getattribute__(aattr.name)
             print_(
                 f"     --   {attribute_name} = {attribute_value} (is type: {type(attribute_value)}, should be type:{aattr.type}))",
                 verbose,
             )
             if attribute_value is not None:
                 if (
-                    type(attribute_value) == int
-                    or type(attribute_value) == float
-                    or type(attribute_value) == str
-                    or type(attribute_value) == bool
-                    or type(attribute_value) == list
+                    isinstance(attribute_value, int)
+                    or isinstance(attribute_value, float)
+                    or isinstance(attribute_value, str)
+                    or isinstance(attribute_value, bool)
+                    or isinstance(attribute_value, list)
                 ):
                     parent.set(attribute_name, str(attribute_value))
-                elif type(attribute_value) == dict:
-
+                elif isinstance(attribute_value, dict):
                     """for k, v in attribute_value.items():
                     child_element = build_xml_element(v)"""
                 else:
                     child_element = build_xml_element(attribute_value)
                     child_element.tag = attribute_name
                     #
                     parent.append(child_element)
@@ -305,55 +301,53 @@
         if (sys.version_info[0] == 2 and isinstance(x, unicode))
         else x
     )
     return dict(map(ascii_encode, pair) for pair in data.items())
 
 
 def _parse_element(dict_format, to_build):
-
     print_("Parse for element: [%s]" % dict_format, verbose)
     for k in dict_format.keys():
         print_(
             "  Setting id: {} in {} ({})".format(k, type.__name__, type(to_build)),
             verbose,
         )
         to_build.id = k
         to_build = _parse_attributes(dict_format[k], to_build)
 
     return to_build
 
 
 def _parse_attributes(dict_format, to_build):
-
     for key in dict_format:
         value = dict_format[key]
         new_format = True
         print_(
             "  Setting {}={} ({}) in {}".format(key, value, type(value), to_build),
             verbose,
         )
 
         if new_format:
-            if type(to_build) == dict:
+            if isinstance(to_build, dict):
                 to_build[key] = value
 
             elif key in to_build.allowed_children:
                 type_to_use = to_build.allowed_children[key][1]
                 for v in value:
                     ff = type_to_use()
                     print_(f"    Type for {key}: {type_to_use} ({ff})", verbose)
                     ff = _parse_element({v: value[v]}, ff)
                     exec("to_build.%s.append(ff)" % key)
             else:
                 if (
-                    type(value) == str
-                    or type(value) == int
-                    or type(value) == float
-                    or type(value) == bool
-                    or type(value) == list
+                    isinstance(value, str)
+                    or isinstance(value, int)
+                    or isinstance(value, float)
+                    or isinstance(value, bool)
+                    or isinstance(value, list)
                     or value is None
                 ):
                     to_build.__setattr__(key, value)
                 else:
                     type_to_use = to_build.allowed_fields[key][1]
                     print_(
                         "type_to_use: {} ({})".format(type_to_use, type(type_to_use)),
@@ -366,19 +360,23 @@
                         to_build.__setattr__(key, vv)
                     else:
                         ff = type_to_use()
                         ff = _parse_attributes(value, ff)
                         exec("to_build.%s = ff" % key)
 
         else:
-            if type(to_build) == dict:
+            if isinstance(to_build, dict):
                 to_build[key] = value
-            elif type(value) == str or type(value) == int or type(value) == float:
+            elif (
+                isinstance(value, str)
+                or isinstance(value, int)
+                or isinstance(value, float)
+            ):
                 to_build.__setattr__(key, value)
-            elif type(value) == list:
+            elif isinstance(value, list):
                 type_to_use = to_build.allowed_children[key][1]
 
                 for vl in value:
                     ff = type_to_use()
                     ff = _parse_element(vl, ff)
                     exec("to_build.%s.append(ff)" % key)
             else:
@@ -399,31 +397,31 @@
     file_name = os.path.join(base_dir, f)
     real = os.path.realpath(file_name)
     # print_v('- Located %s at %s'%(f,real))
     return real
 
 
 def _val_info(param_val):
-    if type(param_val) == np.ndarray:
+    if isinstance(param_val, np.ndarray):
         pp = "%s" % (np.array2string(param_val, threshold=4, edgeitems=1))
         pp = pp.replace("\n", "")
         pp += f" (NP {param_val.shape} {param_val.dtype})"
     elif type(param_val).__name__ == "EagerTensor":
         pp = "%s" % param_val
         pp = pp.replace("\n", "")
         # pp+=' (TF %s %s)'%(param_val.shape,param_val.dtype)
-    elif type(param_val) == tuple:
+    elif type(param_val) is tuple:
         # If param_val is a tuple, recursively print its elements
         # separated by commas and wrapped in parentheses
         pp = "(" + ", ".join([_val_info(el) for el in param_val]) + ")"
     else:
         pp = "%s" % param_val
         t = type(param_val)
-        if not (t == int or t == float):
-            pp += "(%s)" % (t if type(t) == str else t.__name__)
+        if not (t is int or t is float):
+            pp += "(%s)" % (t if type(t) is str else t.__name__)
     return pp
 
 
 def _params_info(parameters, multiline=False):
     """
     Short info on names, values and types in parameter list
     """
@@ -472,44 +470,43 @@
 
     print_(
         " > Evaluating: [%s] which is a: %s, vs parameters: %s (using %s arrays)..."
         % (expr, type(expr).__name__, _params_info(parameters), array_format),
         verbose,
     )
     try:
-        if type(expr) == str and expr in parameters:
+        if type(expr) is str and expr in parameters:
             expr = parameters[
                 expr
             ]  # replace with the value in parameters & check whether it's float/int...
             print_("   Using for that param: %s" % _val_info(expr), verbose)
 
-        if type(expr) == str:
+        if type(expr) is str:
             try:
                 if array_format == FORMAT_TENSORFLOW:
                     expr = tf.constant(int(expr))
                 else:
                     expr = int(expr)
             except:
-
                 try:
                     if array_format == FORMAT_TENSORFLOW:
                         expr = tf.constant(float(expr))
                     else:
                         expr = float(expr)
                 except:
                     pass
 
-        if type(expr) == list:
+        if type(expr) is list:
             print_("   Returning a list in format: %s" % array_format, verbose)
             if array_format == FORMAT_TENSORFLOW:
                 return tf.constant(expr, dtype=tf.float64)
             else:
                 return np.array(expr)
 
-        if type(expr) == np.ndarray:
+        if type(expr) is np.ndarray:
             print_("   Returning a numpy array in format: %s" % array_format, verbose)
             if array_format == FORMAT_TENSORFLOW:
                 return tf.convert_to_tensor(expr, dtype=tf.float64)
             else:
                 return np.array(expr)
 
         if "Tensor" in type(expr).__name__:
@@ -534,17 +531,17 @@
                 expr = expr.replace("random()", "rng.random()")
                 parameters["rng"] = rng
             elif "random()" in expr:
                 raise Exception(
                     "The expression [%s] contains a random() call, but a random number generator (rng) must be supplied to the evaluate() call when this expression string is to be evaluated"
                 )
 
-            if type(expr) == str and "math." in expr:
+            if type(expr) is str and "math." in expr:
                 parameters["math"] = math
-            if type(expr) == str and "numpy." in expr:
+            if type(expr) is str and "numpy." in expr:
                 parameters["numpy"] = np
 
             print_(
                 "   Trying to eval [%s] with Python using %s..."
                 % (expr, parameters.keys()),
                 verbose,
             )
@@ -552,16 +549,15 @@
             v = eval(expr, parameters)
 
             print_(
                 "   Evaluated with Python: {} = {}".format(expr, _val_info(v)),
                 verbose,
             )
 
-            if (type(v) == float or type(v) == str) and int(v) == v:
-
+            if (type(v) is float or type(v) is str) and int(v) == v:
                 print_("   Returning int: %s" % int(v), verbose)
 
                 if array_format == FORMAT_TENSORFLOW:
                     return tf.constant(int(v))
                 else:
                     return int(v)
             return v
@@ -572,22 +568,21 @@
 
 """
     Translates a string like '3', '[0,2]' to a list
 """
 
 
 def parse_list_like(list_str):
-
     if isinstance(list_str, int):
         return [list_str]
     elif isinstance(list_str, float):
         return [list_str]
     elif isinstance(list_str, list):
         return list_str
-    elif type(list_str) == str:
+    elif type(list_str) is str:
         try:
             expr = int(list_str)
             return [expr]
         except:
             pass
         try:
             expr = float(list_str)
```

### Comparing `modelspec-0.3.3/src/modelspec.egg-info/PKG-INFO` & `modelspec-0.3.4/src/modelspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelspec
-Version: 0.3.3
+Version: 0.3.4
 Summary: A common JSON/YAML based format for compact model specification
 Home-page: https://github.com/ModECI/modelspec
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: Padraig Gleeson, David Turner
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
```

### Comparing `modelspec-0.3.3/src/modelspec.egg-info/SOURCES.txt` & `modelspec-0.3.4/src/modelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/src/modelspec.egg-info/requires.txt` & `modelspec-0.3.4/src/modelspec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `modelspec-0.3.3/tests/test_base.py` & `modelspec-0.3.4/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,16 +188,17 @@
 
     nety2 = NewNetwork.from_yaml(net.to_yaml() + " ")
     str_nety2 = str(nety2)
 
     nety3 = NewNetwork.from_yaml_file(filenamey)
     str_nety3 = str(nety3)
 
-    # datax = load_xml(filenamex)
-    # print_v("Loaded network specification from %s" % filenamex)
+    datax = load_xml(filenamex)
+    assert len(datax) > 0
+    print_v("Loaded network specification from %s" % filenamex)
 
     # netx = NewNetwork.from_dict(datax)
     # str_netx = str(netx)
 
     print("----- Before -----")
     print(str_orig)
     print("----- After via %s -----" % filenamej)
```

### Comparing `modelspec-0.3.3/tests/test_utils.py` & `modelspec-0.3.4/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 
 class TestUtils(unittest.TestCase):
     def test_evaluate(self):
-
         assert evaluate("33") == 33.0
         assert evaluate("33") == 33
         assert evaluate(33) == 33
         params = {"p": 33}
         assert evaluate("p+p", params, verbose=True) == 66
 
         print("======")
```

