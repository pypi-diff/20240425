# Comparing `tmp/trio-parallel-1.2.1.tar.gz` & `tmp/trio_parallel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio-parallel-1.2.1.tar", last modified: Sun Nov  5 01:15:45 2023, max compression
+gzip compressed data, was "trio_parallel-1.2.2.tar", last modified: Wed Apr 24 22:38:06 2024, max compression
```

## Comparing `trio-parallel-1.2.1.tar` & `trio_parallel-1.2.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.984587 trio-parallel-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/CHEATSHEET.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2023-11-05 01:15:45.984587 trio-parallel-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/_trio_parallel_workers/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/_trio_parallel_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/_trio_parallel_workers/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.976587 trio-parallel-1.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.980587 trio-parallel-1.2.1/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/async_parallel_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/cache_warmup.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/cancellation.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/parallel_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/parallel_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples/single_use_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/docs/source/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.980587 trio-parallel-1.2.1/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/newsfragments/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/newsfragments/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.980587 trio-parallel-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/build.in
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/coverage.in
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/coverage.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/install.in
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/lint.in
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-11-05 01:15:45.984587 trio-parallel-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.980587 trio-parallel-1.2.1/trio_parallel/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17606 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_posix_pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_proc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.984587 trio-parallel-1.2.1/trio_parallel/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/test_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/test_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_windows_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-11-05 01:15:37.000000 trio-parallel-1.2.1/trio_parallel/_windows_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 01:15:45.984587 trio-parallel-1.2.1/trio_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2023-11-05 01:15:45.000000 trio-parallel-1.2.1/trio_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-11-05 01:15:45.000000 trio-parallel-1.2.1/trio_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 01:15:45.000000 trio-parallel-1.2.1/trio_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-05 01:15:45.000000 trio-parallel-1.2.1/trio_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-05 01:15:45.000000 trio-parallel-1.2.1/trio_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.132463 trio_parallel-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.120463 trio_parallel-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.120463 trio_parallel-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/CHEATSHEET.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-24 22:38:06.132463 trio_parallel-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.120463 trio_parallel-1.2.2/_trio_parallel_workers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/_trio_parallel_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/_trio_parallel_workers/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.124463 trio_parallel-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.124463 trio_parallel-1.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.124463 trio_parallel-1.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.124463 trio_parallel-1.2.2/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/async_parallel_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/cache_warmup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/parallel_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/parallel_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples/single_use_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/docs/source/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.124463 trio_parallel-1.2.2/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/newsfragments/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/newsfragments/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.128463 trio_parallel-1.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/build.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/coverage.in
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/coverage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/install.in
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/lint.in
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-24 22:38:06.132463 trio_parallel-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.128463 trio_parallel-1.2.2/trio_parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17615 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_posix_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_proc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.128463 trio_parallel-1.2.2/trio_parallel/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/test_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/test_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_windows_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-24 22:37:57.000000 trio_parallel-1.2.2/trio_parallel/_windows_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:06.132463 trio_parallel-1.2.2/trio_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-24 22:38:06.000000 trio_parallel-1.2.2/trio_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 22:38:06.000000 trio_parallel-1.2.2/trio_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:38:06.000000 trio_parallel-1.2.2/trio_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 22:38:06.000000 trio_parallel-1.2.2/trio_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 22:38:06.000000 trio_parallel-1.2.2/trio_parallel.egg-info/top_level.txt
```

### Comparing `trio-parallel-1.2.1/.github/workflows/ci.yml` & `trio_parallel-1.2.2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     if: github.event_name == 'pull_request'
     timeout-minutes: 1
     runs-on: ubuntu-latest
     permissions:
       pull-requests: write
       contents: write
     steps:
-      - uses: fastify/github-action-merge-dependabot@v3.9.1
+      - uses: fastify/github-action-merge-dependabot@v3.10.1
         with:
           merge-method: merge
           use-github-auto-merge: true
 
   Verify:
     name: 'Verify requirement pinning'
     timeout-minutes: 2
     runs-on: 'ubuntu-latest'
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: "3.12"
       - name: Install requirements
         run: |
           python -m pip install -U pip
           # Optimistically assume SHA checks won't change much
           python -m pip install pip-compile-multi
@@ -43,17 +43,17 @@
 
   Blacken:
     name: 'Formatting and linting'
     timeout-minutes: 2
     runs-on: 'ubuntu-latest'
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           cache: pip
           cache-dependency-path: requirements/lint.txt
           python-version: "3.12"
       - name: Install requirements
         run: |
           python -m pip install -U pip
@@ -61,182 +61,140 @@
       - name: Run Black
         id: black
         run: black --check --diff trio_parallel _trio_parallel_workers
         continue-on-error: true
       - name: Run flake8
         id: flake8
         run: |
-          flake8 --extend-ignore=D,E,W,F401,F403,F405,F821,F822,TRIO114 \
-          --extend-select=TRIO900,TRIO910,TRIO911
+          flake8 --extend-ignore=D,E,W,F401,F403,F405,F821,F822,ASYNC114 \
+          --extend-select=ASYNC900,ASYNC910,ASYNC911
         continue-on-error: true
       - name: Fail on error
         if: steps.black.outcome != 'success' || steps.flake8.outcome != 'success'
         run: exit 1
 
   Build:
     name: Build
     timeout-minutes: 5
     runs-on: ubuntu-latest
     outputs:
-      wheelname: ${{ steps.outputs.outputs.wheelname }}
+      python-versions: ${{ steps.baipp.outputs.supported_python_classifiers_json_array }}
       settings: ${{ steps.outputs.outputs.settings }}
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
         with:
           fetch-depth: 0
-      - name: Setup python
-        uses: actions/setup-python@v4.7.1
-        with:
-          cache: pip
-          cache-dependency-path: requirements/build.txt
-          python-version: "3.12"
-      - name: Install requirements
-        run: |
-          python -m pip install -U pip
-          python -m pip install -r requirements/build.txt
-      - name: Build sdist wheel
-        run: |
-          SOURCE_DATE_EPOCH=$(git log -1 --pretty=%ct) \
-          python -m build --no-isolation  # already isolated & build deps pinned
-      - name: Check distribution
-        run: |
-          python -m pip install twine
-          twine check --strict dist/*
+      - name: Build inspect and upload
+        id: baipp
+        uses: hynek/build-and-inspect-python-package@v2.3.0
       - name: Set outputs
         id: outputs
         run: |
-          echo "wheelname=$( echo ./dist/*.whl )" >> $GITHUB_OUTPUT
           echo "settings=$( 
               tar cz \
               pyproject.toml \
               requirements/install.txt \
               requirements/test.txt \
               | base64 -w 0
           )" >> $GITHUB_OUTPUT
-          cd dist && sha256sum * >> $GITHUB_STEP_SUMMARY
-      - name: Upload build artifact
-        uses: actions/upload-artifact@v3.1.3
-        with:
-          name: Build
-#         by default build puts sdist and wheel here
-          path: dist/
-          if-no-files-found: error
+          cd ${{ steps.baipp.outputs.dist }} && sha256sum *.* >> $GITHUB_STEP_SUMMARY
 
   Test:
-    name: 'Test ${{ matrix.os }} (${{ matrix.python }} ${{ matrix.arch }})'
+    name: 'Test ${{ matrix.os }} (${{ matrix.python }})'
     needs: Build
     timeout-minutes: 10
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
       fail-fast: false
       matrix:
         experimental: [ false ]
         test-timeout: [ 10 ]
         os:
           - windows-latest
           - ubuntu-latest
           - macos-latest
-        python:
-          - '3.8'
-          - '3.9'
-          - '3.10'
-          - '3.11'
-          - '3.12'
-          - 'pypy-3.8'
-          - 'pypy-3.9'
-          - 'pypy-3.10'
-        arch: [ x64 ]
+        python: ${{ fromJson(needs.Build.outputs.python-versions) }}
         include:
+          # pypy/linux is comparable to cpy/win
           - os: ubuntu-latest
-            python: 'pypy-3.10-nightly'
-            arch: x64
-            experimental: true
+            python: 'pypy-3.10'
+            experimental: false
             test-timeout: 10
 #          - os: ubuntu-latest
 #            python: '3.13-dev'
-#            arch: x64
 #            experimental: true
 #            test-timeout: 3
-          - os: windows-latest
-            python: '3.8'
-            arch: x86
-            experimental: false
-            test-timeout: 10
         exclude:
           - os: macos-latest
             python: '3.8'
-          - os: macos-latest
-            python: 'pypy-3.8'
-          - os: macos-latest
-            python: 'pypy-3.9'
     steps:
       - name: Input settings
         run: echo "${{ needs.Build.outputs.settings }}" | base64 -d | tar xz
         shell: bash
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
-          cache: pip
-          cache-dependency-path: requirements/test.txt
           python-version: '${{ matrix.python }}'
-          architecture: '${{ matrix.arch }}'
+      - name: Setup and Cache UV
+        uses: hynek/setup-cached-uv@v1.1.0
+        with:
+          cache-suffix: '-${{ matrix.python }}'
+          cache-dependency-path: '**/requirements/test.txt'
       - name: Download build artifact
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.2
         with:
-          name: Build
+          name: Packages
           path: dist
       - name: Install requirements
         run: |
-          python -m pip install -U pip
-          python -m pip install -r requirements/test.txt
+          uv pip install --system -r requirements/test.txt
       - name: Install wheel
+        shell: bash
         run: |
-          python -m pip install ${{ needs.Build.outputs.wheelname }} --no-deps
+          uv pip install --system `echo ./dist/*.whl` --no-deps
       - name: Run tests
         timeout-minutes: ${{ matrix.test-timeout }}
         run: |
-          pytest trio_parallel --cov-report xml:coverage-${{ matrix.os }}-${{ matrix.arch }}-${{ matrix.python }}.xml
+          pytest trio_parallel --cov-report xml:coverage-${{ matrix.os }}-${{ matrix.python }}.xml
           coverage report
-          mv .coverage .coverage.${{ matrix.os }}-${{ matrix.arch }}-${{ matrix.python }}
+          mv .coverage .coverage.${{ matrix.os }}-${{ matrix.python }}
         shell: bash
       - name: Upload coverage
         if: always()
-        uses: actions/upload-artifact@v3.1.3
+        uses: actions/upload-artifact@v4.3.1
         with:
-          name: Coverage
-          path: "*coverage*${{ matrix.os }}-${{ matrix.arch }}-${{ matrix.python }}*"
+          name: Coverage-${{ matrix.os }}-${{ matrix.python }}
+          path: "*coverage*${{ matrix.os }}-${{ matrix.python }}*"
           if-no-files-found: error
 
   Examples:
-    name: 'Test examples ${{ matrix.os }} (${{ matrix.python }} ${{ matrix.arch }})'
+    name: 'Test examples ${{ matrix.os }} (${{ matrix.python }})'
     timeout-minutes: 10
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
           - windows-latest
           - ubuntu-latest
           - macos-latest
         python:
           - '3.12'
-        arch:
-          - x64
+          - 'pypy-3.10'
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           cache: pip
           cache-dependency-path: requirements/test.txt
           python-version: '${{ matrix.python }}'
-          architecture: '${{ matrix.arch }}'
       - name: Install requirements
         run: |
           python -m pip install -U pip
           python -m pip install -r requirements/test.txt
       - name: Install editable source
         run: |
           python -m pip install -e . --no-deps
@@ -247,60 +205,45 @@
   Extras:
     name: 'Test [test] extra'
     timeout-minutes: 5
     runs-on: ubuntu-latest
     needs: Build
     steps:
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: '3.12'
       - name: Download build artifact
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.2
         with:
-          name: Build
+          name: Packages
           path: dist
       - name: Run tests
+        shell: bash
         run: |
-          python -m pip install ${{ needs.Build.outputs.wheelname }}[test]
+          wheel=`echo ./dist/*.whl`
+          python -m pip install $wheel[test]
           pytest --pyargs trio_parallel
 
-  Codecov: # Codecov is naughty and will be forever isolated
-    name: Codecov
-    if: always()
-    needs: Test
-    timeout-minutes: 1
-    runs-on: ubuntu-latest
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v4.1.1
-      - name: Download coverage artifact
-        uses: actions/download-artifact@v3.0.2
-        with:
-          name: Coverage
-      - name: Upload to Codecov
-        uses: codecov/codecov-action@v3.1.4
-        with:
-          fail_ci_if_error: true
-
   Coverage:
     name: Coverage
     if: always()
     needs: Test
     timeout-minutes: 1
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
       - name: Download coverage artifact
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.2
         with:
-          name: Coverage
+          pattern: Coverage-*
+          merge-multiple: true
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           cache: pip
           cache-dependency-path: requirements/coverage.txt
           python-version: "3.12"
       - name: Install coverage
         run: |
           pip install -U pip
@@ -309,25 +252,25 @@
         run: |
           coverage combine
           coverage html
           coverage report --fail-under=100 --show-missing --format markdown \
           >> $GITHUB_STEP_SUMMARY
       - name: Upload report
         if: always()
-        uses: actions/upload-artifact@v3.1.3
+        uses: actions/upload-artifact@v4.3.1
         with:
           name: Report
           path: htmlcov/
           if-no-files-found: error
 
   All:
     name: All checks and tests
     if: always()
     timeout-minutes: 1
-    needs: [ Verify, Blacken, Build, Examples, Test, Extras, Codecov, Coverage ]
+    needs: [ Verify, Blacken, Build, Examples, Test, Extras, Coverage ]
     runs-on: ubuntu-latest
     steps:
       - name: Check all needs have passed
         uses: re-actors/alls-green@v1.2.2
         with:
           jobs: ${{ toJSON(needs) }}
 
@@ -340,18 +283,33 @@
     environment:
       name: release
       url: https://pypi.org/p/trio-parallel
     permissions:
       id-token: write
     steps:
       - name: Download build artifact
-        uses: actions/download-artifact@v3.0.2
+        uses: actions/download-artifact@v4.1.2
         with:
-          name: Build
+          name: Packages
           path: dist
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
+
+  Update:
+    name: Update GitHub Release
+    if: github.event_name == 'release'
+    needs: All
+    timeout-minutes: 1
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+    steps:
+      - name: Download build artifact
+        uses: actions/download-artifact@v4.1.2
+        with:
+          name: Packages
+          path: dist
       - name: Upload to GitHub
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           gh release upload ${{ github.ref_name }} dist/* --repo ${{ github.repository }}
```

### Comparing `trio-parallel-1.2.1/.github/workflows/periodic.yml` & `trio_parallel-1.2.2/.github/workflows/periodic.yml`

 * *Files 18% similar despite different names*

```diff
@@ -20,22 +20,22 @@
           - ubuntu-latest
           - macos-latest
         python:
           - '3.12'
           - 'pypy-3.10'
         source:
           - 'trio-parallel'
-          - 'trio-parallel git+https://github.com/python-trio/trio.git'
+          - 'git+https://github.com/python-trio/trio.git trio-parallel'
           - '-e .'
     steps:
       - name: Checkout
         if: matrix.source == '-e .'
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
       - name: Setup python
-        uses: actions/setup-python@v4.7.1
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: ${{ matrix.python }}
       - name: Run tests
         run: |
           python -m pip install ${{ matrix.source }}[test]
           cd ..  # Disguise normal pytest config file
           python -m pytest --pyargs trio_parallel
```

### Comparing `trio-parallel-1.2.1/.gitignore` & `trio_parallel-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/CHEATSHEET.rst` & `trio_parallel-1.2.2/CHEATSHEET.rst`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/LICENSE.APACHE2` & `trio_parallel-1.2.2/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/LICENSE.MIT` & `trio_parallel-1.2.2/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/PKG-INFO` & `trio_parallel-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-parallel
-Version: 1.2.1
+Version: 1.2.2
 Summary: CPU parallelism for Trio
 Home-page: https://github.com/richardsheridan/trio-parallel
 Author: Richard Sheridan
 Author-email: richard.sheridan@gmail.com
 License: MIT OR Apache-2.0
 Keywords: parallel,trio,async,dispatch
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trio-parallel-1.2.1/README.rst` & `trio_parallel-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/_trio_parallel_workers/__init__.py` & `trio_parallel-1.2.2/_trio_parallel_workers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         install_pickling_support(e)
         raise e
 
 
 def safe_dumps(result):
     try:
         return dumps(result, protocol=HIGHEST_PROTOCOL)
-    except BaseException as exc:  # noqa: TRIO103
-        return dumps(Error(exc), protocol=HIGHEST_PROTOCOL)  # noqa: TRIO104
+    except BaseException as exc:  # noqa: ASYNC103
+        return dumps(Error(exc), protocol=HIGHEST_PROTOCOL)  # noqa: ASYNC104
 
 
 def safe_poll(recv_pipe, timeout):
     deadline = perf_counter() + timeout
     while timeout > MAX_TIMEOUT:
         if recv_pipe.poll(MAX_TIMEOUT):
             return True
@@ -57,19 +57,19 @@
 
 
 def worker_behavior(recv_pipe, send_pipe, idle_timeout, init, retire):
     # Intercept keyboard interrupts to avoid passing KeyboardInterrupt
     # between processes. (Trio will take charge via cancellation.)
     signal.signal(signal.SIGINT, signal.SIG_IGN)
     try:
-        if isinstance(init, bytes):  # true except on "fork"
-            # Signal successful startup to spawn/forkserver parents.
+        if sys.platform == "win32":
+            # Signal successful startup.
             send_pipe.send_bytes(ACK)
+        if isinstance(init, bytes):  # true except on "fork"
             init = loads(init)
-        if isinstance(retire, bytes):  # true except on "fork"
             retire = loads(retire)
         init()
         while safe_poll(recv_pipe, idle_timeout):
             send_pipe.send_bytes(
                 safe_dumps(capture(handle_job, recv_pipe.recv_bytes()))
             )
             if retire():
```

### Comparing `trio-parallel-1.2.1/_trio_parallel_workers/_funcs.py` & `trio_parallel-1.2.2/_trio_parallel_workers/_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,14 @@
 def _never_halts(ev):  # pragma: no cover, worker will be killed
     # important difference from blocking call is cpu usage
     ev.set()
     while True:
         pass
 
 
-def _segfault_out_of_bounds_pointer():  # pragma: no cover, worker will be killed
-    # https://wiki.python.org/moin/CrashingPython
-    import ctypes
-
-    i = ctypes.c_char(b"a")
-    j = ctypes.pointer(i)
-    c = 1
-    while True:
-        j[c] = i
-        c *= 2  # grow fast to crash sooner
-
-
 def _raise_ki():
     import signal, trio
 
     trio._util.signal_raise(signal.SIGINT)
 
 
 _lambda = lambda: None  # pragma: no cover, never run
```

### Comparing `trio-parallel-1.2.1/docs/Makefile` & `trio_parallel-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/make.bat` & `trio_parallel-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/conf.py` & `trio_parallel-1.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/examples/async_parallel_pipeline.py` & `trio_parallel-1.2.2/docs/source/examples/async_parallel_pipeline.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/examples/cancellation.py` & `trio_parallel-1.2.2/docs/source/examples/cancellation.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/examples/parallel_map.py` & `trio_parallel-1.2.2/docs/source/examples/parallel_map.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/examples/single_use_workers.py` & `trio_parallel-1.2.2/docs/source/examples/single_use_workers.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/docs/source/history.rst` & `trio_parallel-1.2.2/docs/source/history.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 Release history
 ===============
 
 .. currentmodule:: trio_parallel
 
 .. towncrier release notes start
 
+trio-parallel 1.2.2 (2024-04-24)
+--------------------------------
+
+Bugfixes
+~~~~~~~~
+
+- Fixed a rare race condition during cleanup that could trigger unraisable error tracebacks. (`#398 <https://github.com/richardsheridan/trio-parallel/issues/398>`__)
+- Made several internal changes that may make compatibility with future Trio versions more stable (`#412 <https://github.com/richardsheridan/trio-parallel/issues/412>`__)
+
+
 trio-parallel 1.2.1 (2023-11-04)
 --------------------------------
 
 Bugfixes
 ~~~~~~~~
 
 - Resolved a deprecation warning on python 3.12. (`#380 <https://github.com/richardsheridan/trio-parallel/issues/380>`__)
```

### Comparing `trio-parallel-1.2.1/docs/source/reference.rst` & `trio_parallel-1.2.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/newsfragments/README.rst` & `trio_parallel-1.2.2/newsfragments/README.rst`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/pyproject.toml` & `trio_parallel-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 filename = "docs/source/history.rst"
 directory = "newsfragments"
 name = "trio-parallel"
 underlines = ["-", "~", "^"]
 issue_format = "`#{issue} <https://github.com/richardsheridan/trio-parallel/issues/{issue}>`__"
 
 [tool.pytest.ini_options]
-addopts = "--pyargs -r a --verbose --cov --cov-config=pyproject.toml --cov-context=test"
+addopts = "--pyargs -r a -n auto --verbose --cov --cov-config=pyproject.toml --cov-context=test"
 filterwarnings = ["error"]
 xfail_strict = true
 faulthandler_timeout = 60
 
 [tool.coverage.run]
 branch = true
 concurrency = ["multiprocessing", "thread"]
```

### Comparing `trio-parallel-1.2.1/requirements/build.txt` & `trio_parallel-1.2.2/requirements/build.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # SHA1:ace7503a2d1aa53a1cf9f3fc8f628c57912c7e2a
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-build==1.0.3
+build==1.2.1
     # via -r requirements\build.in
 colorama==0.4.6
     # via build
-packaging==23.2
+packaging==24.0
     # via
     #   build
     #   setuptools-scm
 pyproject-hooks==1.0.0
     # via build
 setuptools-scm==8.0.4
     # via -r requirements\build.in
-typing-extensions==4.8.0
+typing-extensions==4.10.0
     # via setuptools-scm
-wheel==0.41.3
+wheel==0.43.0
     # via -r requirements\build.in
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==68.2.2
-    # via
-    #   -r requirements\build.in
-    #   setuptools-scm
+# setuptools
```

### Comparing `trio-parallel-1.2.1/requirements/docs.txt` & `trio_parallel-1.2.2/requirements/docs.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,76 +2,71 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r install.txt
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
-babel==2.13.1
+babel==2.14.0
     # via sphinx
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via towncrier
 colorama==0.4.6
     # via
     #   click
     #   sphinx
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
 imagesize==1.4.1
     # via sphinx
 incremental==22.10.0
     # via towncrier
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   sphinx
     #   towncrier
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via jinja2
-packaging==23.2
+packaging==24.0
     # via sphinx
-pygments==2.16.1
+pygments==2.17.2
     # via sphinx
 requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
 sphinx==7.2.6
     # via
     #   -r requirements\docs.in
     #   sphinx-rtd-theme
-    #   sphinxcontrib-applehelp
-    #   sphinxcontrib-devhelp
-    #   sphinxcontrib-htmlhelp
     #   sphinxcontrib-jquery
-    #   sphinxcontrib-qthelp
-    #   sphinxcontrib-serializinghtml
     #   sphinxcontrib-trio
-sphinx-rtd-theme==1.3.0
+sphinx-rtd-theme==2.0.0
     # via -r requirements\docs.in
-sphinxcontrib-applehelp==1.0.7
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.5
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.4
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.6
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.9
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxcontrib-trio==1.1.2
     # via -r requirements\docs.in
-towncrier==23.10.0
+towncrier==23.11.0
     # via -r requirements\docs.in
-urllib3==2.0.7
+urllib3==2.2.1
     # via requests
```

### Comparing `trio-parallel-1.2.1/requirements/install.txt` & `trio_parallel-1.2.2/requirements/install.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # SHA1:63e73656a123a857e40bd1da6cce5906958410ed
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-attrs==23.1.0
+attrs==23.2.0
     # via
     #   -r requirements\install.in
     #   outcome
     #   trio
 cffi==1.16.0 ; os_name == "nt" and implementation_name != "pypy"
     # via
     #   -r requirements\install.in
     #   trio
-idna==3.4
+idna==3.6
     # via trio
 outcome==1.3.0.post0
     # via
     #   -r requirements\install.in
     #   trio
-pycparser==2.21
+pycparser==2.22
     # via cffi
-sniffio==1.3.0
+sniffio==1.3.1
     # via trio
 sortedcontainers==2.4.0
     # via trio
 tblib==3.0.0
     # via -r requirements\install.in
-trio==0.23.1
+trio==0.25.0
     # via -r requirements\install.in
```

### Comparing `trio-parallel-1.2.1/requirements/lint.txt` & `trio_parallel-1.2.2/requirements/lint.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-# SHA1:f58ba84c95fb69356c5f7f07b941bd44e736ec6d
+# SHA1:6c87e66b8ae90e26b9c63847f5558cd02603fc9e
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-black==23.10.1
+black==24.3.0
     # via -r requirements\lint.in
 click==8.1.7
     # via black
 colorama==0.4.6
     # via click
-flake8==6.1.0
+flake8==7.0.0
     # via
     #   -r requirements\lint.in
-    #   flake8-trio
-flake8-trio==23.5.1
+    #   flake8-async
+flake8-async==24.3.6
     # via -r requirements\lint.in
-libcst==1.1.0
-    # via flake8-trio
+libcst==1.3.1
+    # via flake8-async
 mccabe==0.7.0
     # via flake8
 mypy-extensions==1.0.0
-    # via
-    #   black
-    #   typing-inspect
-packaging==23.2
     # via black
-pathspec==0.11.2
+packaging==24.0
+    # via black
+pathspec==0.12.1
     # via black
-platformdirs==3.11.0
+platformdirs==4.2.0
     # via black
 pycodestyle==2.11.1
     # via flake8
-pyflakes==3.1.0
+pyflakes==3.2.0
     # via flake8
 pyyaml==6.0.1
     # via libcst
-typing-extensions==4.8.0
-    # via
-    #   libcst
-    #   typing-inspect
-typing-inspect==0.9.0
-    # via libcst
```

### Comparing `trio-parallel-1.2.1/setup.cfg` & `trio_parallel-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/trio_parallel/__init__.py` & `trio_parallel-1.2.2/trio_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/trio_parallel/_abc.py` & `trio_parallel-1.2.2/trio_parallel/_abc.py`

 * *Files identical despite different names*

### Comparing `trio-parallel-1.2.1/trio_parallel/_impl.py` & `trio_parallel-1.2.2/trio_parallel/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
     waiting_task = attr.ib(None)
     entrances = attr.ib(0)
     exits = attr.ib(0)
     # Counters are used for thread safety of the default cache
     enter_counter = attr.ib(factory=lambda: count(1))
     exit_counter = attr.ib(factory=lambda: count(1))
 
-    async def __aenter__(self):  # noqa: TRIO910
+    async def __aenter__(self):  # noqa: ASYNC910
         # only async to save indentation
         if self.waiting_task:
             raise trio.ClosedResourceError
         self.entrances = next(self.enter_counter)
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):  # noqa: TRIO910
+    async def __aexit__(self, exc_type, exc_val, exc_tb):  # noqa: ASYNC910
         # only async to save indentation
         self.exits = next(self.exit_counter)
         if self.waiting_task:
             if self.calc_running() == 0:
                 trio.lowlevel.reschedule(self.waiting_task)
 
     def calc_running(self):
@@ -124,15 +124,15 @@
     )
     grace_period: float = attr.ib(
         default=30.0,
         validator=check_non_negative,
     )
     worker_type: WorkerType = attr.ib(
         default=WorkerType.SPAWN,
-        validator=attr.validators.in_(WorkerType),
+        validator=attr.validators.in_(set(WorkerType)),
     )
     _worker_class: Type[AbstractWorker] = attr.ib(repr=False, init=False)
     _worker_cache: WorkerCache = attr.ib(repr=False, init=False)
     _lifetime: ContextLifetimeManager = attr.ib(
         factory=ContextLifetimeManager, repr=False, init=False
     )
 
@@ -285,15 +285,15 @@
 
     @trio.lowlevel.enable_ki_protection
     async def close_at_run_end(ctx):
         try:
             await trio.sleep_forever()
         finally:
             # KeyboardInterrupt here could leak the context
-            await ctx._aclose()  # noqa: TRIO102
+            await ctx._aclose()  # noqa: ASYNC102
 
 else:
 
     def get_default_context():
         return DEFAULT_CONTEXT
 
     def graceful_default_shutdown(ctx):
@@ -365,15 +365,15 @@
        :func:`WorkerContext.run_sync` call.
 
     """
     ctx = WorkerContext._create(idle_timeout, init, retire, grace_period, worker_type)
     try:
         yield ctx
     finally:
-        await ctx._aclose()  # noqa: TRIO102
+        await ctx._aclose()  # noqa: ASYNC102
 
 
 def atexit_shutdown_grace_period(
     grace_period=DEFAULT_CONTEXT.grace_period,
 ):  # pragma: no cover, deprecated
     """Set the default worker cache shutdown grace period.
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_proc.py` & `trio_parallel-1.2.2/trio_parallel/_proc.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,36 +65,42 @@
 
     async def start(self):
         await trio.to_thread.run_sync(self.proc.start)
         # XXX: We must explicitly close these after start to see child closures
         self._child_send_pipe.close()
         self._child_recv_pipe.close()
 
-        # The following is mainly needed in the case of accidental recursive spawn
-        async def wait_then_fail():
-            await self.wait()
-            raise BrokenWorkerProcessError("Worker failed to start", self.proc)
+        if sys.platform != "win32":
+            return
 
-        async with trio.open_nursery() as nursery:
-            nursery.start_soon(wait_then_fail)
+        # Give a nice error on accidental recursive spawn instead of hanging
+        async def wait_for_ack():
             try:
                 code = await self._receive_chan.receive()
+                assert code == tp_workers.ACK
             except BaseException:
                 self.kill()
                 with trio.CancelScope(shield=True):
-                    await self.wait()  # noqa: TRIO102
+                    await self.wait()  # noqa: ASYNC102
                 raise
-            assert code == tp_workers.ACK
             nursery.cancel_scope.cancel()
 
+        exitcode = None
+        async with trio.open_nursery() as nursery:
+            nursery.start_soon(wait_for_ack)
+            exitcode = await self.wait()
+            nursery.cancel_scope.cancel()
+        if exitcode is not None:
+            raise BrokenWorkerProcessError("Worker failed to start", self.proc)
+
     async def run_sync(self, sync_fn: Callable, *args) -> Optional[Outcome]:
         try:
             job = dumps((sync_fn, args), protocol=HIGHEST_PROTOCOL)
-        except BaseException as exc:  # noqa: TRIO103
-            return Error(exc)  # noqa: TRIO104, TRIO910
+        except BaseException as exc:  # noqa: ASYNC103
+            return Error(exc)  # noqa: ASYNC104, ASYNC910
 
         try:
             try:
                 await self._send_chan.send(job)
             except trio.BrokenResourceError:
                 with trio.CancelScope(shield=True):
                     await self.wait()
@@ -111,15 +117,15 @@
                 ) from None
         except BaseException:
             # cancellations require kill by contract
             # other exceptions will almost certainly leave us in an
             # unrecoverable state requiring kill as well
             self.kill()
             with trio.CancelScope(shield=True):
-                await self.wait()  # noqa: TRIO102
+                await self.wait()  # noqa: ASYNC102
             raise
 
     def is_alive(self):
         # if the proc is alive, there is a race condition where it could be
         # dying. This call reaps zombie children on Unix.
         return self.proc.is_alive()
 
@@ -138,23 +144,14 @@
             return None  # waiting before started
         await lowlevel_wait(self.proc.sentinel)
         # fix a macos race: Trio GH#1296
         self.proc.join()
         # unfortunately join does not return exitcode
         return self.proc.exitcode
 
-    def __del__(self):
-        # Avoid __del__ errors on cleanup: Trio GH#174, GH#1767
-        # multiprocessing will close them for us if initialized
-        # but practically they are always initialized, hence pragma
-        if hasattr(self, "_send_chan"):  # pragma: no branch
-            self._send_chan.detach()
-        if hasattr(self, "_receive_chan"):  # pragma: no branch
-            self._receive_chan.detach()
-
 
 class WorkerProcCache(_abc.WorkerCache[SpawnProcWorker]):
     def prune(self):
         # remove procs that have died from the idle timeout
         while True:
             try:
                 worker = self.popleft()
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_tests/test_cache.py` & `trio_parallel-1.2.2/trio_parallel/_tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Tests of internal cache API ("contract" tests)"""
+
 import math
 
 import pytest
 import trio
 
 from _trio_parallel_workers._funcs import (
     _init_run_twice,
@@ -44,15 +45,15 @@
     assert dead_worker not in cache
 
 
 async def test_retire(cache_and_workertype):
     cache, worker_type = cache_and_workertype
     worker = worker_type(math.inf, _init_run_twice, _retire_run_twice)
     await worker.start()
-    with trio.fail_after(2):
+    with trio.fail_after(4):
         assert await worker.run_sync(bool) is not None
         assert await worker.run_sync(bool) is not None
         assert await worker.run_sync(bool) is None
         assert await worker.wait() == 0
 
 
 async def test_bad_retire_fn(cache_and_workertype, capfd):
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_tests/test_defaults.py` & `trio_parallel-1.2.2/trio_parallel/_tests/test_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,24 +202,24 @@
     # case of startup that I have run into.
     script_path = tmp_path / "script.py"
     with script_path.open("w") as f:
         f.write(
             "import trio,trio_parallel; trio.run(trio_parallel.run_sync, int)\n",
         )
     result = subprocess.run(
-        # note str used because cpython subprocess added the feature
-        # to understand path-like objects in version 3.8
-        [sys.executable, str(script_path)],
+        [sys.executable, script_path],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         check=False,  # we expect a failure
         timeout=20,
     )
     assert not result.stdout
     assert b"An attempt has been made to start a new process" in result.stderr
+    assert b"ExceptionGroup" not in result.stderr
+    assert b"MultiError" not in result.stderr
     assert result.returncode
 
 
 async def _compare_pids():
     first = await run_sync(os.getpid)
     second = await run_sync(os.getpid)
     return first == second
@@ -241,15 +241,15 @@
 
 
 async def test_configure_default_context_thread(shutdown_cache):
     with pytest.raises(RuntimeError, match="thread"):
         await trio.to_thread.run_sync(configure_default_context)
 
 
-async def test_get_default_context_stats():  # noqa: TRIO910
+async def test_get_default_context_stats():  # noqa: ASYNC910
     s = default_context_statistics()
     assert hasattr(s, "idle_workers")
     assert hasattr(s, "running_workers")
     assert s == get_default_context().statistics()
 
 
 @pytest.mark.xfail(
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_tests/test_impl.py` & `trio_parallel-1.2.2/trio_parallel/_tests/test_impl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Tests of public API with mocked-out workers ("collaboration" tests)"""
+
 import sys
-import warnings
 from typing import Callable, Optional
 
 import pytest
 import trio
 from outcome import Outcome, capture
 
 from .. import _impl
@@ -132,37 +132,48 @@
         worker = ctx._worker_cache.pop()
         assert not ctx._worker_cache
         assert worker.init is float
         assert worker.retire is int
         assert worker.idle_timeout == 33
 
 
-async def test_erroneous_scope_inputs():  # pragma: no cover, ugly branching
-    with pytest.raises(TypeError):
-        async with _impl.open_worker_context(idle_timeout=[-1]):
-            pytest.fail("should be unreachable")
-    with pytest.raises(TypeError):
-        async with _impl.open_worker_context(init=0):
-            pytest.fail("should be unreachable")
-    with pytest.raises(TypeError):
-        async with _impl.open_worker_context(retire=None):
-            pytest.fail("should be unreachable")
+def _idfn(val):
+    k = next(iter(val))
+    v = val[k]
+    return f"{k}-{v}"
+
+
+@pytest.mark.parametrize(
+    "kwargs",
+    [
+        dict(idle_timeout=[-1]),
+        dict(init=0),
+        dict(retire=None),
+        dict(grace_period=None),
+    ],
+    ids=_idfn,
+)
+async def test_erroneous_scope_types(kwargs):
     with pytest.raises(TypeError):
-        async with _impl.open_worker_context(grace_period=object()):
-            pytest.fail("should be unreachable")
-    with pytest.raises(ValueError):
-        with warnings.catch_warnings():  # spurious DeprecationWarning on 3.7
-            warnings.simplefilter("ignore")
-            async with _impl.open_worker_context(worker_type="wrong"):
-                pytest.fail("should be unreachable")
-    with pytest.raises(ValueError):
-        async with _impl.open_worker_context(grace_period=-1):
+        async with _impl.open_worker_context(**kwargs):
             pytest.fail("should be unreachable")
+
+
+@pytest.mark.parametrize(
+    "kwargs",
+    [
+        dict(worker_type="wrong"),
+        dict(grace_period=-1),
+        dict(idle_timeout=-1),
+    ],
+    ids=_idfn,
+)
+async def test_erroneous_scope_values(kwargs):
     with pytest.raises(ValueError):
-        async with _impl.open_worker_context(idle_timeout=-1):
+        async with _impl.open_worker_context(**kwargs):
             pytest.fail("should be unreachable")
 
 
 async def test_worker_returning_none_can_be_cancelled():
     with trio.move_on_after(0.1) as cs:
         ctx = MockContext._create(retire=_special_none_making_retire)
         assert await ctx.run_sync(int)
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_tests/test_proc.py` & `trio_parallel-1.2.2/trio_parallel/_tests/test_proc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ Tests of internal worker process API ("contract" tests)
 
     These are specific to subprocesses and you wouldn't expect these to pass
     with thread or subinterpreter workers.
 """
+
 import math
+import os
 
 import trio
 import pytest
 
 from _trio_parallel_workers._funcs import (
     _lambda,
     _return_lambda,
     _raise_ki,
     _never_halts,
-    _segfault_out_of_bounds_pointer,
     _no_trio,
 )
 from .._proc import WORKER_PROC_MAP
 from .._abc import BrokenWorkerError
 
 
 @pytest.fixture(params=list(WORKER_PROC_MAP.values()), ids=list(WORKER_PROC_MAP.keys()))
@@ -47,32 +48,40 @@
         nursery.cancel_scope.cancel()
     with trio.fail_after(1):
         assert await worker.wait() in (-15, -9)
 
 
 async def test_run_sync_raises_on_kill(worker, manager):
     ev = manager.Event()
-    await worker.run_sync(int)  # running start so actual test is less racy
-    with pytest.raises(BrokenWorkerError) as exc_info, trio.fail_after(5):
-        async with trio.open_nursery() as nursery:
-            nursery.start_soon(worker.run_sync, _never_halts, ev)
+
+    async def killer():
+        try:
             await trio.to_thread.run_sync(ev.wait, abandon_on_cancel=True)
+        finally:
             worker.kill()  # also tests multiple calls to worker.kill
+
+    await worker.run_sync(int)  # running start so actual test is less racy
+    with trio.fail_after(5):
+        async with trio.open_nursery() as nursery:
+            nursery.start_soon(killer)
+            with pytest.raises(BrokenWorkerError) as exc_info:
+                await worker.run_sync(_never_halts, ev)
     exitcode = await worker.wait()
     assert exitcode in (-15, -9)
     assert exc_info.value.args[-1].exitcode == exitcode
 
 
-async def test_run_sync_raises_on_segfault(worker, capfd):
+async def test_run_sync_raises_on_sudden_death(worker, capfd):
+    expected_code = 42
     with pytest.raises(BrokenWorkerError) as excinfo:
         with trio.fail_after(20):
-            assert (await worker.run_sync(_segfault_out_of_bounds_pointer)).unwrap()
+            assert (await worker.run_sync(os._exit, expected_code)).unwrap()
     exitcode = await worker.wait()
-    assert exitcode  # not sure if we expect a universal value, but not 0 or None
-    assert excinfo.value.args[-1].exitcode == exitcode
+    assert exitcode == expected_code
+    assert excinfo.value.args[-1].exitcode == expected_code
 
 
 # to test that cancellation does not ever leave a living process behind
 # currently requires manually targeting all but last checkpoints
 
 
 async def test_exhaustively_cancel_run_sync(worker, manager):
@@ -91,15 +100,15 @@
     (await worker.run_sync(_raise_ki)).unwrap()
 
 
 @pytest.mark.parametrize("job", [_lambda, _return_lambda])
 async def test_unpickleable(job, worker):
     from pickle import PicklingError
 
-    with pytest.raises((PicklingError, AttributeError)):
+    with pytest.raises(PicklingError):
         (await worker.run_sync(job)).unwrap()
 
 
 async def test_no_trio_in_subproc(worker):
     if worker.mp_context._name == "fork":
         pytest.skip("Doesn't matter on ForkProcWorker")
     assert (await worker.run_sync(_no_trio)).unwrap()
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_tests/test_worker.py` & `trio_parallel-1.2.2/trio_parallel/_tests/test_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Tests of internal worker API ("contract" tests)
 
     All workers should pass these tests, regardless of implementation
 """
+
 import math
-import os
-import sys
 
 import pytest
 import trio
 
 from _trio_parallel_workers._funcs import _null_async_fn, _chained_exc, SpecialError
 from .._impl import WORKER_MAP
 
@@ -59,15 +58,15 @@
         pytest.skip("capfd doesn't work on ForkserverProcWorker")
     await worker.start()
     # This could happen on weird __del__/weakref/atexit situations.
     # It was not visible on normal, clean exits because multiprocessing
     # would call terminate before pipes were GC'd.
     assert (await worker.run_sync(bool)).unwrap() is False
     worker.shutdown()
-    with trio.fail_after(1):
+    with trio.fail_after(2):
         exitcode = await worker.wait()
     out, err = capfd.readouterr()
     assert not err
     assert exitcode == 0
     assert not out
```

### Comparing `trio-parallel-1.2.1/trio_parallel/_windows_cffi.py` & `trio_parallel-1.2.2/trio_parallel/_windows_cffi.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,37 +51,24 @@
 
 ################################################################
 # Generic helpers
 ################################################################
 
 
 # vendored from trio, so no coverage
-def _handle(obj):  # pragma: no cover
-    # For now, represent handles as either cffi HANDLEs or as ints.  If you
-    # try to pass in a file descriptor instead, it's not going to work
-    # out. (For that msvcrt.get_osfhandle does the trick, but I don't know if
-    # we'll actually need that for anything...) For sockets this doesn't
-    # matter, Python never allocates an fd. So let's wait until we actually
-    # encounter the problem before worrying about it.
-    if type(obj) is int:
-        return ffi.cast("HANDLE", obj)
-    else:
-        return obj
-
-
-# vendored from trio, so no coverage
 def raise_winerror(winerror=None, *, filename=None, filename2=None):  # pragma: no cover
     if winerror is None:
         winerror, msg = ffi.getwinerror()
     else:
         _, msg = ffi.getwinerror(winerror)
     # https://docs.python.org/3/library/exceptions.html#OSError
     raise OSError(0, msg, filename, winerror, filename2)
 
 
-def peek_pipe_message_left(handle):
+def peek_pipe_message_left(handle: int):
+    # If you try to pass in a file descriptor instead, it's not going to work out.
+    assert type(handle) is int
+    handle = ffi.cast("HANDLE", handle)
     left = ffi.new("LPDWORD")
-    if not kernel32.PeekNamedPipe(
-        _handle(handle), ffi.NULL, 0, ffi.NULL, ffi.NULL, left
-    ):
+    if not kernel32.PeekNamedPipe(handle, ffi.NULL, 0, ffi.NULL, ffi.NULL, left):
         raise_winerror()  # pragma: no cover
     return left[0]
```

### Comparing `trio-parallel-1.2.1/trio_parallel.egg-info/PKG-INFO` & `trio_parallel-1.2.2/trio_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-parallel
-Version: 1.2.1
+Version: 1.2.2
 Summary: CPU parallelism for Trio
 Home-page: https://github.com/richardsheridan/trio-parallel
 Author: Richard Sheridan
 Author-email: richard.sheridan@gmail.com
 License: MIT OR Apache-2.0
 Keywords: parallel,trio,async,dispatch
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trio-parallel-1.2.1/trio_parallel.egg-info/SOURCES.txt` & `trio_parallel-1.2.2/trio_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

