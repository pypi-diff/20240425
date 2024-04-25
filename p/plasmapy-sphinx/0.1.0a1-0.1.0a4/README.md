# Comparing `tmp/plasmapy_sphinx-0.1.0a1.tar.gz` & `tmp/plasmapy_sphinx-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmapy_sphinx-0.1.0a1.tar", last modified: Sat Apr 13 01:54:27 2024, max compression
+gzip compressed data, was "plasmapy_sphinx-0.1.0a4.tar", last modified: Thu Apr 25 18:04:19 2024, max compression
```

## Comparing `plasmapy_sphinx-0.1.0a1.tar` & `plasmapy_sphinx-0.1.0a4.tar`

### file list

```diff
@@ -1,89 +1,95 @@
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.964743 plasmapy_sphinx-0.1.0a1/
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/.github/
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/.github/workflows/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1377 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/.github/workflows/mint-release.yml
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      651 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/.github/workflows/publish-to-pypi.yml
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1745 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/.gitignore
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     2376 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/.pre-commit-config.yaml
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      342 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/.readthedocs.yml
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1331 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/LICENSE.md
--rw-r--r--   0 namurphy (10742) namurphy  (1001)     4342 2024-04-13 01:54:27.964743 plasmapy_sphinx-0.1.0a1/PKG-INFO
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       18 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/README.md
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/docs/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1028 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/Makefile
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/docs/api_static/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      324 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.autodoc.automodapi.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      248 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.autodoc.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      315 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.automodsumm.core.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      199 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.automodsumm.generate.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      268 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.automodsumm.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      303 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.directives.confval.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      293 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.directives.event.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      263 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.directives.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      163 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.ext.autodoc.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      179 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.ext.automodsumm.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      147 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.ext.css.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      175 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.ext.directives.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      131 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.ext.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      316 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      139 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/api_static/plasmapy_sphinx.utils.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      155 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/common_links.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)    13703 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/docs/conf.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/docs/first_steps/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       60 2024-04-13 00:08:26.000000 plasmapy_sphinx-0.1.0a1/docs/first_steps/configure.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       64 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/first_steps/install.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1382 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/index.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      770 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/docs/make.bat
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     4572 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/__init__.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/autodoc/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     3194 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/autodoc/__init__.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)    30418 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/autodoc/automodapi.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     3913 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/__init__.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)    23883 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/core.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)    18359 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/generate.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1402 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/__init__.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     3245 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/confval.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     4525 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/event.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      119 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/__init__.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      470 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/autodoc.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      260 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/automodsumm.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      631 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/css.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      305 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/ext/directives.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      528 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/__init__.py
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       98 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/breadcrumbs.html
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1832 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/footer.html
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      513 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/layout.html
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/css/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     6404 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     4545 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/css/plasmapy.css
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/automodsumm/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      105 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/automodsumm/base.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     1096 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      181 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/automodsumm/module.rst
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       87 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/theme.conf
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)    11403 2024-04-13 00:27:15.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/utils.py
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.964743 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/
--rw-r--r--   0 namurphy (10742) namurphy  (1001)     4342 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/PKG-INFO
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     2412 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/SOURCES.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)        1 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/dependency_links.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       60 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/entry_points.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      514 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/requires.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       16 2024-04-13 01:54:27.000000 plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/top_level.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)     3905 2024-04-13 01:52:33.000000 plasmapy_sphinx-0.1.0a1/pyproject.toml
-drwxrwxr-x   0 namurphy (10742) namurphy  (1001)        0 2024-04-13 01:54:27.960744 plasmapy_sphinx-0.1.0a1/requirements/
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      201 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/build.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      469 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/docs.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       84 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/environment.yml
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      278 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/extras.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      210 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/install.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      459 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements/tests.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      348 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/requirements.txt
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)       38 2024-04-13 01:54:27.964743 plasmapy_sphinx-0.1.0a1/setup.cfg
--rw-rw-r--   0 namurphy (10742) namurphy  (1001)      367 2024-04-12 21:59:14.000000 plasmapy_sphinx-0.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/mint-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.411573 plasmapy_sphinx-0.1.0a4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    90022 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/_static/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/_static/with-text-light-190px.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/docs/api_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.autodoc.automodapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.autodoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.generate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.automodsumm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.confval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.event.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.directives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.autodoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.automodsumm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.css.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.directives.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.theme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/api_static/plasmapy_sphinx.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/common_links.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/docs/first_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/first_steps/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/first_steps/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30418 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/automodapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/confval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.415573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/automodsumm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/ext/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/plasmapy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.407573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 18:04:19.000000 plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:04:19.419573 plasmapy_sphinx-0.1.0a4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:04:19.423573 plasmapy_sphinx-0.1.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 18:04:14.000000 plasmapy_sphinx-0.1.0a4/setup.py
```

### Comparing `plasmapy_sphinx-0.1.0a1/.github/workflows/mint-release.yml` & `plasmapy_sphinx-0.1.0a4/.github/workflows/mint-release.yml`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/.github/workflows/publish-to-pypi.yml` & `plasmapy_sphinx-0.1.0a4/.github/workflows/publish-to-pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,21 @@
   contents: read
 
 jobs:
 
   deploy:
     runs-on: ubuntu-latest
 
+    environment:
+      name: pypi
+      url: https://pypi.org/p/plasmapy-sphinx
+
+    permissions:
+      id-token: write
+
     steps:
 
     - name: Checkout code
       uses: actions/checkout@v4
 
     - name: Set up Python
       uses: actions/setup-python@v5
@@ -27,11 +34,8 @@
         python -m pip install --upgrade pip
         pip install build
 
     - name: Build package
       run: python -m build
 
     - name: Upload package to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.8.14
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `plasmapy_sphinx-0.1.0a1/.gitignore` & `plasmapy_sphinx-0.1.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/.pre-commit-config.yaml` & `plasmapy_sphinx-0.1.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/LICENSE.md` & `plasmapy_sphinx-0.1.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/PKG-INFO` & `plasmapy_sphinx-0.1.0a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmapy_sphinx
-Version: 0.1.0a1
+Version: 0.1.0a4
 Summary: Sphinx extensions for the PlasmaPy Project
 Maintainer-email: "Erik T. Everson" <eeverson@plasmapy.org>, "Nicholas A. Murphy" <namurphy@cfa.harvard.edu>
 License: # BSD 2-Clause License
         
         Copyright (c) 2021, PlasmaPy Developers.
         All rights reserved.
         
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: docutils
+Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: jinja2!=3.1
 Requires-Dist: sphinx>=4.4
 Requires-Dist: sphinx-gallery
 Requires-Dist: sphinx_rtd_theme>=1.0.0
 Provides-Extra: tests
 Requires-Dist: codespell; extra == "tests"
 Requires-Dist: dlint; extra == "tests"
@@ -70,14 +71,15 @@
 Requires-Dist: pydocstyle; extra == "tests"
 Requires-Dist: pytest>=5.4.0; extra == "tests"
 Requires-Dist: pytest-regressions; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: packaging; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 Requires-Dist: pygments>=2.11.0; extra == "docs"
 Requires-Dist: sphinx-changelog; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-hoverxref>=1.1.1; extra == "docs"
 Requires-Dist: sphinx-issues>=3.0.1; extra == "docs"
 Requires-Dist: sphinx-notfound-page>=0.8; extra == "docs"
```

### Comparing `plasmapy_sphinx-0.1.0a1/docs/Makefile` & `plasmapy_sphinx-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/docs/conf.py` & `plasmapy_sphinx-0.1.0a4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 import os
 import sys
 
 from datetime import datetime
-from pkg_resources import parse_version
+from packaging.version import Version
 
 sys.path.insert(0, os.path.abspath(".."))
 sys.path.insert(0, os.path.abspath("."))
 
 from plasmapy_sphinx import __version__ as release
 
 if False:
@@ -101,14 +101,15 @@
     "python": ("https://docs.python.org/3/", None),
     "pytest": ("https://docs.pytest.org/en/stable/", None),
     "sphinx_automodapi": (
         "https://sphinx-automodapi.readthedocs.io/en/latest/",
         None,
     ),
     "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
+    "plasmapy": ("https://docs.plasmapy.org/en/latest/", None),
 }
 
 hoverxref_intersphinx = [
     "readthedocs",
     "python",
     "numpy",
     "scipy",
@@ -150,18 +151,20 @@
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
 #  Note: If plasmapy.__version__ can not be defined then it is set to 'unknown'.
 #        However, release needs to be a semantic style version number, so set
 #        the 'unknown' case to ''.
 release = "" if release == "unknown" else release
-pv = parse_version(release)
-release = pv.public
+revision = ""
+if release != "":
+    pv = Version(release)
+    release = pv.public
+    revision = "" if pv.local is None else pv.local[1:]
 version = ".".join(release.split(".")[:2])  # short X.Y version
-revision = pv.local[1:] if pv.local is not None else ""
 
 # This is added to the end of RST files — a good place to put substitutions to
 # be used globally.
 rst_epilog = ""
 with open("common_links.rst") as cl:
     rst_epilog += cl.read()
 
@@ -325,14 +328,16 @@
     (python_role, "Builder"),
     (python_role, "docutils.*"),
     (python_role, "level"),
     (python_role, ".*member.*"),
     (python_role, "OptionSpec"),
     (python_role, "py"),
     (python_role, "[Ss]phinx.*"),  # also for reST workarounds in docs/common_links.rst
+    (python_role, "Documenter"),
+    (python_role, "Node"),
     # The following patterns still need to be fixed.
     (python_role, "json.decoder.JSONDecoder"),
     (python_role, "plasmapy.analysis.swept_langmuir.find_floating_potential"),
     (python_role, "plasmapy.particles.particle_collections"),
     (python_role, "plasmapy.utils.decorators.lite_func"),
 ]
 
@@ -348,19 +353,15 @@
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_logo = "./_static/with-text-light-190px.png"
 html_theme_options = {
-    "logo_only": True,
-    #
-    # TOC options
-    #   https://sphinx-rtd-theme.readthedocs.io/en/stable/configuring.html#theme-options
-    "includehidden": False,
+    "logo_only": False,
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `plasmapy_sphinx-0.1.0a1/docs/index.rst` & `plasmapy_sphinx-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/docs/make.bat` & `plasmapy_sphinx-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/__init__.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,36 +69,34 @@
 # Enforce Python version check during package import.
 # This is the same check as the one at the top of setup.py
 import sys
 
 if sys.version_info < (3, 6):  # coverage: ignore
     raise ImportError("plasmapy_sphinx does not support Python < 3.6")
 
-# Packages may add whatever they like to this file, but
-# should keep this content at the top.
-# ----------------------------------------------------------------------------
-import pkg_resources
+if sys.version_info >= (3, 8):
+    from importlib.metadata import version, PackageNotFoundError
+else:
+    from importlib_metadata import version, PackageNotFoundError
 
 from plasmapy_sphinx import autodoc, automodsumm, directives, utils
 
 
 # define version
 try:
-    # this places a runtime dependency on setuptools
-    #
     # note: if there's any distribution metadata in your source files, then this
     #       will find a version based on those files.  Keep distribution metadata
     #       out of your repository unless you've intentionally installed the package
-    #       as editable (e.g. `pip install -e {plasmapy_directory_root}`),
+    #       as editable (e.g. `pip install -e {root_directory}`),
     #       but then __version__ will not be updated with each commit, it is
     #       frozen to the version at time of install.
     #
     #: `plasmapy_sphinx` version string
-    __version__ = pkg_resources.get_distribution("plasmapy_sphinx").version
-except pkg_resources.DistributionNotFound:
+    __version__ = version("plasmapy_sphinx")
+except PackageNotFoundError:
     # package is not installed
     fallback_version = "unknown"
     try:
         # code most likely being used from source
         # if setuptools_scm is installed then generate a version
         from setuptools_scm import get_version
 
@@ -120,8 +118,8 @@
             f"plasmapy_sphinx is not an installed package and {warn_add}.",
             RuntimeWarning,
         )
 
         del warn
     del fallback_version, warn_add
 
-del pkg_resources, sys
+del sys
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/autodoc/__init__.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/autodoc/automodapi.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/autodoc/automodapi.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/__init__.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/core.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/core.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/automodsumm/generate.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/automodsumm/generate.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/__init__.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/confval.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/confval.py`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/directives/event.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/directives/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     Parameters
     ----------
     env : sphinx.environment.BuildEnvironment
         Instance of the Sphinx's build environment.
 
     sig : str
-        The "signature" given the the event directive or role.  For example,
+        The "signature" given the event directive or role.  For example,
 
         .. code-block:: rst
 
             .. event:: foo(bar)
 
             :event:`foo`
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/footer.html` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/footer.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- extends "!sphinx_rtd_theme/footer.html" %}
+{% extends "sphinx_rtd_theme/footer.html" %}
 
 {% if page_source_suffix %}
 {% set suffix = page_source_suffix %}
 {% else %}
 {% set suffix = source_suffix %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-{%- extends "!sphinx_rtd_theme/footer.html" %} {% if page_source_suffix %} {%
-set suffix = page_source_suffix %} {% else %} {% set suffix = source_suffix %}
-{% endif %} {% if meta is defined and meta is not none %} {% set check_meta =
-True %} {% else %} {% set check_meta = False %} {% endif %} {% if check_meta
-and 'github_url' in meta %} {% set display_github = True %} {% endif %} {% set
+{% extends "sphinx_rtd_theme/footer.html" %} {% if page_source_suffix %} {% set
+suffix = page_source_suffix %} {% else %} {% set suffix = source_suffix %} {%
+endif %} {% if meta is defined and meta is not none %} {% set check_meta = True
+%} {% else %} {% set check_meta = False %} {% endif %} {% if check_meta and
+'github_url' in meta %} {% set display_github = True %} {% endif %} {% set
 display_vcs_links = display_vcs_links if display_vcs_links is defined else True
 %} {% block extrafooter %}
 {% if hasdoc(pagename) and display_vcs_links %} {% if display_github %} {% if
 check_meta and 'github_url' in meta %} _{_{_ ___(_'_E_d_i_t_ _o_n_ _G_i_t_H_u_b_'_)_ _}_}_{_{_ _r_e_l_d_e_l_i_m_2_ _}_}
 {% else %} _{_{_ ___(_'_E_d_i_t_ _o_n_ _G_i_t_H_u_b_'_)_ _}_}_{_{_ _r_e_l_d_e_l_i_m_2_ _}_}_ {% endif %} {% elif
 show_source and source_url_prefix %} _{_{_ ___(_'_P_a_g_e_ _S_o_u_r_c_e_'_)_ _}_}_{_{_ _r_e_l_d_e_l_i_m_2_ _}_}_ {%
 elif show_source and has_source and sourcename %} _{_{_ ___(_'_P_a_g_e_ _S_o_u_r_c_e_'_)_ _}_}_{
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/admonition_color_contrast.css`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/css/plasmapy.css` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/css/plasmapy.css`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
   difficult. Use relative units like rem (root font size) to help with
   accessibility and scaling. Please add descriptive comments for new
   rules that are understandable to someone who is unfamiliar with CSS.
 
   CSS files can be validated at: https://jigsaw.w3.org/css-validator
 */
 
+@import "theme.css"; /* From sphinx_rtd_theme */
+@import "admonition_color_contrast.css";
+
 /* -----------------------------------------------------------------------------
  * RTD Overrides
  */
 
 /* Style for toctree in a table */
 td .toctree-wrapper ul {
     font-size: 16px;
@@ -63,14 +66,22 @@
  */
 .rst-content dl.rst table p,
 .rst-content dl.std table p,
 .rst-content dl.py table p {
     margin-bottom: 0 !important;
 }
 
+/*
+ * Patch for overflow wrapping caused by sphinx_rtd_theme==1.1.0
+ * See https://github.com/PlasmaPy/PlasmaPy/issues/1784
+ */
+.rst-content p a code {
+    overflow-wrap: normal;
+}
+
 /* Remove excess bottom margin for table headings */
 .rst-content table.docutils thead p {
     margin-bottom: 0;
 }
 
 /* Remove excess bottom margin for for multiline table entries when using line-block */
 .rst-content table.docutils div.line-block {
@@ -122,35 +133,35 @@
 }
 div.wy-nav-content a:hover {
     text-decoration:underline;
 }
 
 /*
   The style for generic code literals, in particular text that is
-  enclosed in double back ticks in reST (e.g., ``make -j 32``).
+  enclosed in double back ticks in reStructuredText (e.g., ``make -j 32``).
 */
 
 div.wy-nav-content .rst-content code.literal {
     background-color: #f6f6f6;
     color: #db2424;
 }
 
 /*
   The style for links to Python objects, in particular text enclosed in
-  single back ticks in reST (e.g., `~plasmapy.particles`).
+  single back ticks in reStructuredText (e.g., `~plasmapy.particles`).
 */
 
 div.wy-nav-content .rst-content code.literal.xref {
     color: #0069d6;
     font-weight: bold;
 }
 
 /*
   The style for literal text that shows the location of a file, in
-  particular when used by the reST role :file: (e.g.,
+  particular when used by the reStructuredText role :file: (e.g.,
   :file:`docs/_static/css/plasmapy.css`).
 */
 div.wy-nav-content .rst-content code.literal.file {
     color: #b84d00;
     background-color: #F9F1F0;
 }
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/theme/static/templates/automodsumm/class.rst`

 * *Files identical despite different names*

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx/utils.py` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 """
 __all__ = [
     "default_grouping_info",
     "find_mod_objs",
     "get_custom_grouping_info",
     "package_dir",
     "templates_dir",
+    "theme_dir",
+    "css_dir",
+    "static_dir",
 ]
 
 import inspect
 
 from collections import OrderedDict
 from importlib import import_module
 from sphinx.application import Sphinx
@@ -19,18 +22,21 @@
 from typing import Any, Dict
 
 package_dir = Path(__file__).parent.absolute()
 """Absolute path to the `plasmapy_sphinx` package directory."""
 
 theme_dir = (package_dir / "theme").resolve()
 
-css_dir = (theme_dir / "static" / "css").resolve()
+static_dir = (theme_dir / "static").resolve().absolute()
+"""Absolute path to the `plasmapy_sphinx` static directory."""
+
+css_dir = (static_dir / "css").resolve()
 """Absolute path to the `plasmapy_sphinx` CSS directory."""
 
-templates_dir = (theme_dir / "static" / "templates").resolve()
+templates_dir = (static_dir / "templates").resolve()
 """Absolute path to the `plasmapy_sphinx` templates directory."""
 
 default_grouping_info = OrderedDict(
     {
         "modules": {"title": "Sub-Packages & Modules"},
         "classes": {"title": "Classes"},
         "exceptions": {"title": "Exceptions"},
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/PKG-INFO` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmapy_sphinx
-Version: 0.1.0a1
+Version: 0.1.0a4
 Summary: Sphinx extensions for the PlasmaPy Project
 Maintainer-email: "Erik T. Everson" <eeverson@plasmapy.org>, "Nicholas A. Murphy" <namurphy@cfa.harvard.edu>
 License: # BSD 2-Clause License
         
         Copyright (c) 2021, PlasmaPy Developers.
         All rights reserved.
         
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: docutils
+Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: jinja2!=3.1
 Requires-Dist: sphinx>=4.4
 Requires-Dist: sphinx-gallery
 Requires-Dist: sphinx_rtd_theme>=1.0.0
 Provides-Extra: tests
 Requires-Dist: codespell; extra == "tests"
 Requires-Dist: dlint; extra == "tests"
@@ -70,14 +71,15 @@
 Requires-Dist: pydocstyle; extra == "tests"
 Requires-Dist: pytest>=5.4.0; extra == "tests"
 Requires-Dist: pytest-regressions; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: packaging; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 Requires-Dist: pygments>=2.11.0; extra == "docs"
 Requires-Dist: sphinx-changelog; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-hoverxref>=1.1.1; extra == "docs"
 Requires-Dist: sphinx-issues>=3.0.1; extra == "docs"
 Requires-Dist: sphinx-notfound-page>=0.8; extra == "docs"
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/SOURCES.txt` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE.md
 README.md
 pyproject.toml
 requirements.txt
 setup.py
+.github/workflows/documentation.yml
 .github/workflows/mint-release.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/common_links.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
+docs/robots.txt
+docs/_static/icon.ico
+docs/_static/with-text-light-190px.png
 docs/api_static/plasmapy_sphinx.autodoc.automodapi.rst
 docs/api_static/plasmapy_sphinx.autodoc.rst
 docs/api_static/plasmapy_sphinx.automodsumm.core.rst
 docs/api_static/plasmapy_sphinx.automodsumm.generate.rst
 docs/api_static/plasmapy_sphinx.automodsumm.rst
 docs/api_static/plasmapy_sphinx.directives.confval.rst
 docs/api_static/plasmapy_sphinx.directives.event.rst
 docs/api_static/plasmapy_sphinx.directives.rst
 docs/api_static/plasmapy_sphinx.ext.autodoc.rst
 docs/api_static/plasmapy_sphinx.ext.automodsumm.rst
 docs/api_static/plasmapy_sphinx.ext.css.rst
 docs/api_static/plasmapy_sphinx.ext.directives.rst
 docs/api_static/plasmapy_sphinx.ext.rst
 docs/api_static/plasmapy_sphinx.rst
+docs/api_static/plasmapy_sphinx.theme.rst
 docs/api_static/plasmapy_sphinx.utils.rst
 docs/first_steps/configure.rst
 docs/first_steps/install.rst
 plasmapy_sphinx/__init__.py
 plasmapy_sphinx/utils.py
 plasmapy_sphinx.egg-info/PKG-INFO
 plasmapy_sphinx.egg-info/SOURCES.txt
```

### Comparing `plasmapy_sphinx-0.1.0a1/plasmapy_sphinx.egg-info/requires.txt` & `plasmapy_sphinx-0.1.0a4/plasmapy_sphinx.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 docutils
 jinja2!=3.1
 sphinx>=4.4
 sphinx-gallery
 sphinx_rtd_theme>=1.0.0
 
+[:python_version < "3.8"]
+importlib_metadata
+
 [docs]
 numpydoc
+packaging
 pillow
 pygments>=2.11.0
 sphinx-changelog
 sphinx-copybutton
 sphinx-hoverxref>=1.1.1
 sphinx-issues>=3.0.1
 sphinx-notfound-page>=0.8
```

### Comparing `plasmapy_sphinx-0.1.0a1/pyproject.toml` & `plasmapy_sphinx-0.1.0a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "docutils",
+  "importlib_metadata; python_version < '3.8'",
   "jinja2 != 3.1",
   "sphinx >= 4.4",
   "sphinx-gallery",
   "sphinx_rtd_theme >= 1.0.0",
 ]
 
 [project.optional-dependencies]
@@ -56,14 +57,15 @@
   "pytest >= 5.4.0",
   "pytest-regressions",
   "pytest-xdist",
   "tox",
 ]
 docs = [
     "numpydoc",
+    "packaging",
     "pillow",
     "pygments >= 2.11.0",
     "sphinx-changelog",
     "sphinx-copybutton",
     "sphinx-hoverxref >= 1.1.1",
     "sphinx-issues >= 3.0.1",
     "sphinx-notfound-page >= 0.8",
@@ -83,16 +85,20 @@
 website = "https://www.plasmapy.org"
 
 [tool]
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-"plasmapy_sphinx.templates" = ["*"]
-
+plasmapy_sphinx = [
+    "theme/theme.conf",
+    "theme/*.html",
+    "theme/static/css/*.css",
+    "theme/static/templates/automodsumm/*.rst",
+]
 
 [tool.isort]
 line_length = 88
 wrap_length = 80
 sections = ["FUTURE", "STDLIB", "FIRSTPARTY", "LOCALFOLDER"]
 known_first_party = ["plasmapy", ]
 default_section = "STDLIB"
```

