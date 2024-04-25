# Comparing `tmp/ducktools_classbuilder-0.3.0.tar.gz` & `tmp/ducktools_classbuilder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools_classbuilder-0.3.0.tar", last modified: Tue Apr 23 13:34:43 2024, max compression
+gzip compressed data, was "ducktools_classbuilder-0.4.0.tar", last modified: Thu Apr 25 17:21:25 2024, max compression
```

## Comparing `ducktools_classbuilder-0.3.0.tar` & `ducktools_classbuilder-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/approach_vs_tool.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/extension_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/perf/performance_tests.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/prefab/
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/prefab/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/tests/prefab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.067505 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_compare_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_pre_post_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slots_novalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slotted_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.067505 ducktools_classbuilder-0.3.0/tests/prefab/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/creation_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/dunders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/inheritance_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/inheritance_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/frozen_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/funcs_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/init_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/repr_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_dunders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_frozen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.450300 ducktools_classbuilder-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/approach_vs_tool.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/extension_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.450300 ducktools_classbuilder-0.4.0/docs/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/perf/performance_tests.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.450300 ducktools_classbuilder-0.4.0/docs/prefab/
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/docs/prefab/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.446300 ducktools_classbuilder-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.446300 ducktools_classbuilder-0.4.0/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.450300 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27947 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/prefab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-25 17:21:25.000000 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-25 17:21:25.000000 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:21:25.000000 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 17:21:25.000000 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:21:25.000000 ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.454300 ducktools_classbuilder-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.446300 ducktools_classbuilder-0.4.0/tests/prefab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.454300 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_compare_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_pre_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_slots_novalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_slotted_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.454300 ducktools_classbuilder-0.4.0/tests/prefab/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:21:25.458300 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/prefab/shared/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/test_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-25 17:21:21.000000 ducktools_classbuilder-0.4.0/tests/test_core.py
```

### Comparing `ducktools_classbuilder-0.3.0/LICENSE.md` & `ducktools_classbuilder-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/PKG-INFO` & `ducktools_classbuilder-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.3.0
+Version: 0.4.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mypy; extra == "testing"
+Requires-Dist: typing_extensions; python_version < "3.10" and extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 # Ducktools: Class Builder #
 
@@ -117,15 +118,15 @@
 a similar manner to the `@dataclass` decorator from `dataclasses`. 
 
 > [!NOTE] 
 > `ducktools.classbuilder` includes a premade version of `slotclass` that can
 > be used directly. (The included version has some extra features).
 
 ```python
-from ducktools.classbuilder import Field, SlotFields
+from ducktools.classbuilder import Field, SlotFields, slotclass
 
 @slotclass
 class SlottedDC:
     __slots__ = SlotFields(
         the_answer=42,
         the_question=Field(
             default="What do you get if you multiply six by nine?",
@@ -202,26 +203,49 @@
 print(DataCoords())
 print(SlotCoords())
 
 print(f"{DataCoords is class_register[DataCoords.__name__] = }")
 print(f"{SlotCoords is class_register[SlotCoords.__name__] = }")
 ```
 
+## Using annotations anyway ##
+
+For those that really want to use type annotations a basic `annotation_gatherer`
+function and `@annotationclass` decorator are also included. Slots are not generated
+in this case.
+
+```python
+from ducktools.classbuilder import annotationclass
+
+@annotationclass
+class AnnotatedDC:
+    the_answer: int = 42
+    the_question: str = "What do you get if you multiply six by nine?"
+
+    
+ex = AnnotatedDC()
+print(ex)
+```
+
 ## What features does this have? ##
 
 Included as an example implementation, the `slotclass` generator supports 
 `default_factory` for creating mutable defaults like lists, dicts etc.
 It also supports default values that are not builtins (try this on 
 [Cluegen](https://github.com/dabeaz/cluegen)).
 
 It will copy values provided as the `type` to `Field` into the 
 `__annotations__` dictionary of the class. 
 Values provided to `doc` will be placed in the final `__slots__` 
 field so they are present on the class if `help(...)` is called.
 
+A fairly basic `annotations_gatherer` and `annotationclass` are included
+in `extras.py` which can be used to generate classbuilders that rely on 
+annotations.
+
 If you want something with more features you can look at the `prefab.py`
 implementation which provides a 'prebuilt' implementation.
 
 ## Will you add \<feature\> to `classbuilder.prefab`? ##
 
 No. Not unless it's something I need or find interesting.
```

### Comparing `ducktools_classbuilder-0.3.0/README.md` & `ducktools_classbuilder-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 a similar manner to the `@dataclass` decorator from `dataclasses`. 
 
 > [!NOTE] 
 > `ducktools.classbuilder` includes a premade version of `slotclass` that can
 > be used directly. (The included version has some extra features).
 
 ```python
-from ducktools.classbuilder import Field, SlotFields
+from ducktools.classbuilder import Field, SlotFields, slotclass
 
 @slotclass
 class SlottedDC:
     __slots__ = SlotFields(
         the_answer=42,
         the_question=Field(
             default="What do you get if you multiply six by nine?",
@@ -154,26 +154,49 @@
 print(DataCoords())
 print(SlotCoords())
 
 print(f"{DataCoords is class_register[DataCoords.__name__] = }")
 print(f"{SlotCoords is class_register[SlotCoords.__name__] = }")
 ```
 
+## Using annotations anyway ##
+
+For those that really want to use type annotations a basic `annotation_gatherer`
+function and `@annotationclass` decorator are also included. Slots are not generated
+in this case.
+
+```python
+from ducktools.classbuilder import annotationclass
+
+@annotationclass
+class AnnotatedDC:
+    the_answer: int = 42
+    the_question: str = "What do you get if you multiply six by nine?"
+
+    
+ex = AnnotatedDC()
+print(ex)
+```
+
 ## What features does this have? ##
 
 Included as an example implementation, the `slotclass` generator supports 
 `default_factory` for creating mutable defaults like lists, dicts etc.
 It also supports default values that are not builtins (try this on 
 [Cluegen](https://github.com/dabeaz/cluegen)).
 
 It will copy values provided as the `type` to `Field` into the 
 `__annotations__` dictionary of the class. 
 Values provided to `doc` will be placed in the final `__slots__` 
 field so they are present on the class if `help(...)` is called.
 
+A fairly basic `annotations_gatherer` and `annotationclass` are included
+in `extras.py` which can be used to generate classbuilders that rely on 
+annotations.
+
 If you want something with more features you can look at the `prefab.py`
 implementation which provides a 'prebuilt' implementation.
 
 ## Will you add \<feature\> to `classbuilder.prefab`? ##
 
 No. Not unless it's something I need or find interesting.
```

### Comparing `ducktools_classbuilder-0.3.0/docs/Makefile` & `ducktools_classbuilder-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/docs/api.md` & `ducktools_classbuilder-0.4.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/docs/approach_vs_tool.md` & `ducktools_classbuilder-0.4.0/docs/approach_vs_tool.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/docs/conf.py` & `ducktools_classbuilder-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/docs/extension_examples.md` & `ducktools_classbuilder-0.4.0/docs/extension_examples.md`

 * *Files 16% similar despite different names*

```diff
@@ -152,14 +152,17 @@
 
 When customising generator methods (or adding new ones) it may be useful to 
 extend the `Field` class which stores the information on named attributes for
 how to perform the generation. A convenient decorator `@fieldclass` is provided
 to allow simple extension by adding additional slots. By using this decorator
 the `__init__`, `__repr__` and `__eq__` methods will be generated for you.
 
+> Note: Field classes will be frozen when running under pytest.
+>       They are not frozen normally for performance reasons.
+
 ```python
 from ducktools.classbuilder import Field, SlotFields, fieldclass
 
 @fieldclass
 class WithInit(Field):
     __slots__ = SlotFields(init=True)
 
@@ -180,110 +183,34 @@
 ### How can I add `<method>` to the class ###
 
 To do this you need to write a code generator that returns source code
 along with a 'globals' dictionary of any names the code needs to refer 
 to, or an empty dictionary if none are needed. Many methods don't require
 any globals values, but it is essential for some.
 
-#### Iterable Classes ####
-
-Say you want to make the class iterable, so you want to add `__iter__`.
-
-```python
-from ducktools.classbuilder import (
-    default_methods, get_fields, slotclass, MethodMaker, SlotFields
-)
-
-
-def iter_maker(cls):
-    field_names = get_fields(cls).keys()
-    field_yield = "\n".join(f"    yield self.{f}" for f in field_names)
-    code = (
-        f"def __iter__(self):\n"
-        f"{field_yield}"
-    )
-    globs = {}
-    return code, globs
-
-
-iter_desc = MethodMaker("__iter__", iter_maker)
-new_methods = frozenset(default_methods | {iter_desc})
-
-
-def iterclass(cls=None, /):
-    return slotclass(cls, methods=new_methods)
-
-
-if __name__ == "__main__":
-    @iterclass
-    class IterDemo:
-        __slots__ = SlotFields(
-            a=1,
-            b=2,
-            c=3,
-            d=4,
-            e=5,
-        )
-
-
-    ex = IterDemo()
-    print([item for item in ex])
-```
-
-You could also choose to yield tuples of `name, value` pairs in your implementation.
-
 #### Frozen Classes ####
 
-Here's an example of frozen slotted classes that only allow assignment once
-(which happens in the `__init__` method generated).
+In order to make frozen classes you need to replace `__setattr__` and `__delattr__`
 
-> Note that these methods use `type(self).__name__` instead of `cls.__name__`
-> when generated so the name remains correct even if the class name is changed.
+The building blocks for this are actually already included as they're used to prevent 
+`fieldclass` instances from being mutated.
+
+These methods can be reused to make `slotclasses` 'frozen'.
 
 ```python
 from ducktools.classbuilder import (
     slotclass,
-    get_fields,
     SlotFields,
-    MethodMaker,
     default_methods,
+    frozen_setattr_desc,
+    frozen_delattr_desc,
 )
 
 
-def setattr_maker(cls):
-    globs = {
-        "object_setattr": object.__setattr__
-    }
-
-    field_names = set(get_fields(cls).keys())
-
-    code = (
-        f"def __setattr__(self, name, value):\n"
-        f"    fields = {field_names!r}\n"
-        f"    if name in fields and not hasattr(self, name):\n"
-        f"        object_setattr(self, name, value)\n"
-        f"    else:\n"
-        f'        raise TypeError(f"{{type(self).__name__!r}} object does not support attribute assignment")'
-    )
-    return code, globs
-
-
-def delattr_maker(cls):
-    code = (
-        f"def __delattr__(self, name):\n"
-        f'    raise TypeError(f"{{type(self).__name__!r}} object does not support attribute deletion")'
-    )
-    globs = {}
-    return code, globs
-
-
-setattr_desc = MethodMaker("__setattr__", setattr_maker)
-delattr_desc = MethodMaker("__delattr__", delattr_maker)
-
-new_methods = frozenset(default_methods | {setattr_desc, delattr_desc})
+new_methods = default_methods | {frozen_setattr_desc, frozen_delattr_desc}
 
 
 def frozen(cls, /):
     return slotclass(cls, methods=new_methods)
 
 
 if __name__ == "__main__":
@@ -311,14 +238,61 @@
 
     try:
         del ex.y
     except TypeError as e:
         print(e)
 ```
 
+#### Iterable Classes ####
+
+Say you want to make the class iterable, so you want to add `__iter__`.
+
+```python
+from ducktools.classbuilder import (
+    default_methods, get_fields, slotclass, MethodMaker, SlotFields
+)
+
+
+def iter_maker(cls):
+    field_names = get_fields(cls).keys()
+    field_yield = "\n".join(f"    yield self.{f}" for f in field_names)
+    code = (
+        f"def __iter__(self):\n"
+        f"{field_yield}"
+    )
+    globs = {}
+    return code, globs
+
+
+iter_desc = MethodMaker("__iter__", iter_maker)
+new_methods = frozenset(default_methods | {iter_desc})
+
+
+def iterclass(cls=None, /):
+    return slotclass(cls, methods=new_methods)
+
+
+if __name__ == "__main__":
+    @iterclass
+    class IterDemo:
+        __slots__ = SlotFields(
+            a=1,
+            b=2,
+            c=3,
+            d=4,
+            e=5,
+        )
+
+
+    ex = IterDemo()
+    print([item for item in ex])
+```
+
+You could also choose to yield tuples of `name, value` pairs in your implementation.
+
 ### Extending Field ###
 
 #### Excluding Attributes ####
 
 In order to exclude fields you first need to extend the `Field` class
 to add a new attribute. Thankfully the `@fieldclass` decorator mentioned earlier
 can be used to extend `Field` in the same way as `@slotclass` works for 
@@ -601,101 +575,23 @@
         )
 
     ex = ConverterEx("42", "42")
     print(ex)
 ```
 
 ### Gatherers ###
-#### Using type hints/annotations instead of slots? ####
-
-Have you heard of [dataclasses](https://docs.python.org/3/library/dataclasses.html)?
-
-But we can also do that. These classes will not be slotted, however, 
-due to the issues mentioned in the readme.
-
-```python
-import sys
-from ducktools.classbuilder import builder, default_methods, Field, NOTHING
-
-
-def _is_classvar(hint):
-    # Avoid importing typing if it's not already used
-    _typing = sys.modules.get("typing")
-    if _typing:
-        if (
-            hint is _typing.ClassVar
-            or getattr(hint, "__origin__", None) is _typing.ClassVar
-        ):
-            return True
-        # String used as annotation
-        elif isinstance(hint, str) and "ClassVar" in hint:
-            return True
-    return False
-
-
-def annotation_gatherer(cls):
-    cls_annotations = cls.__dict__.get("__annotations__", {})
-    cls_fields = {}
-
-    for k, v in cls_annotations.items():
-        # Ignore ClassVar
-        if _is_classvar(v):
-            continue
-
-        attrib = getattr(cls, k, NOTHING)
-
-        if attrib is not NOTHING:
-            if isinstance(attrib, Field):
-                attrib.type = v
-            else:
-                attrib = Field(default=attrib)
-
-            # Remove the class variable
-            delattr(cls, k)
-
-        else:
-            attrib = Field()
-
-        cls_fields[k] = attrib
-
-    return cls_fields
-
-
-def annotation_class(cls=None, /, *, methods=default_methods):
-    return builder(cls, gatherer=annotation_gatherer, methods=methods)
-
-
-if __name__ == "__main__":
-    import typing
-
-    @annotation_class
-    class H2G2:
-        the_answer: int = 42
-        the_question: str = Field(
-            default="What do you get if you multiply six by nine?",
-        )
-        the_book: typing.ClassVar[str] = "The Hitchhiker's Guide to the Galaxy"
-        the_author: "typing.ClassVar[str]" = "Douglas Adams"
-
-    ex = H2G2()
-    print(ex)
-    ex2 = H2G2(
-        the_question="What is the ultimate answer to the meaning of life, the universe, and everything?"
-    )
-    print(ex2)
-
-    print(H2G2.the_book)
-    print(H2G2.the_author)
-```
-
 #### What about using annotations instead of `Field(init=False, ...)` ####
 
 This seems to be a feature people keep requesting for `dataclasses`.
 This is also doable.
 
+> Note: Field classes will be frozen when running under pytest.
+>       They should not be mutated by gatherers.
+>       If you need to change the value of a field use Field.from_field(...) to make a new instance.
+
 ```python
 import inspect
 from pprint import pp
 from typing import Annotated, Any, ClassVar, get_origin
 
 from ducktools.classbuilder import (
     builder,
```

### Comparing `ducktools_classbuilder-0.3.0/docs/index.md` & `ducktools_classbuilder-0.4.0/docs/index.md`

 * *Files 17% similar despite different names*

```diff
@@ -59,11 +59,32 @@
         ),
     )
     
 ex = SlottedDC()
 print(ex)
 ```
 
+## Annotation Class Usage ##
+
+> Annotation based classes via 'extras' are only supported on Python 3.10 or later!
+
+Building classes based on annotations requires the `extras` submodule.
+This is separate because it relies on `inspect` to simplify the implementation
+but is a slow import.
+
+```python
+from ducktools.classbuilder import annotationclass
+
+@annotationclass
+class AnnotatedDC:
+    the_answer: int = 42
+    the_question: str = "What do you get if you multiply six by nine?"
+
+    
+ex = AnnotatedDC()
+print(ex)
+```
+
 ## Indices and tables ##
 
 * {ref}`genindex`
 * {ref}`search`
```

### Comparing `ducktools_classbuilder-0.3.0/docs/make.bat` & `ducktools_classbuilder-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/docs/perf/performance_tests.md` & `ducktools_classbuilder-0.4.0/docs/perf/performance_tests.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # Performance tests #
 
-Currently from an aging Dell XPS13 laptop running ubuntu 22.04 and Python 3.12.2.
-Windows tests with detailed specs soon.
+Rough specs: 2023 Windows 10 Desktop: Intel i5-13600KF, Crucial P3 1TB PCIe M.2 2280 SSD
 
 ## Import Times ##
 
 | Command | Mean [ms] | Min [ms] | Max [ms] | Relative |
 |:---|---:|---:|---:|---:|
-| `python -c "pass"` | 12.2 ± 1.0 | 11.2 | 15.2 | 1.00 |
-| `python -c "from ducktools.classbuilder import slotclass"` | 12.6 ± 1.0 | 11.8 | 15.0 | 1.03 ± 0.12 |
-| `python -c "from ducktools.classbuilder.prefab import prefab"` | 13.0 ± 0.8 | 12.3 | 15.7 | 1.06 ± 0.11 |
-| `python -c "from collections import namedtuple"` | 14.0 ± 0.7 | 13.3 | 15.9 | 1.15 ± 0.11 |
-| `python -c "from typing import NamedTuple"` | 23.5 ± 1.0 | 22.3 | 25.7 | 1.92 ± 0.18 |
-| `python -c "from dataclasses import dataclass"` | 32.8 ± 1.0 | 30.9 | 35.4 | 2.69 ± 0.23 |
-| `python -c "from attrs import define"` | 50.9 ± 1.3 | 48.4 | 53.9 | 4.17 ± 0.35 |
-| `python -c "from pydantic import BaseModel"` | 75.9 ± 1.3 | 73.8 | 80.9 | 6.22 ± 0.51 |
+| `python -c "pass"` | 23.2 ± 0.8 | 21.8 | 25.3 | 1.00 |
+| `python -c "from ducktools.classbuilder import slotclass"` | 23.4 ± 1.8 | 22.3 | 32.8 | 1.01 ± 0.09 |
+| `python -c "from ducktools.classbuilder.prefab import prefab"` | 23.7 ± 0.9 | 22.8 | 27.6 | 1.02 ± 0.05 |
+| `python -c "from collections import namedtuple"` | 24.2 ± 0.8 | 23.3 | 27.5 | 1.04 ± 0.05 |
+| `python -c "from typing import NamedTuple"` | 32.2 ± 0.8 | 30.7 | 35.7 | 1.39 ± 0.06 |
+| `python -c "from dataclasses import dataclass"` | 39.6 ± 1.1 | 37.9 | 43.2 | 1.70 ± 0.08 |
+| `python -c "from attrs import define"` | 54.0 ± 1.8 | 51.4 | 60.1 | 2.32 ± 0.11 |
+| `python -c "from pydantic import BaseModel"` | 70.2 ± 1.2 | 68.3 | 72.7 | 3.02 ± 0.12 |
+
+
 
 ## Loading a module with 100 classes defined ##
 
 | Command | Mean [ms] | Min [ms] | Max [ms] | Relative |
 |:---|---:|---:|---:|---:|
-| `python -c "pass"` | 11.6 ± 0.6 | 11.2 | 12.8 | 1.00 |
-| `python hyperfine_importers/native_classes_timer.py` | 13.9 ± 0.8 | 13.1 | 15.6 | 1.20 ± 0.09 |
-| `python hyperfine_importers/slotclasses_timer.py` | 15.0 ± 0.6 | 14.3 | 16.4 | 1.29 ± 0.08 |
-| `python hyperfine_importers/prefab_timer.py` | 16.9 ± 0.7 | 16.0 | 18.7 | 1.45 ± 0.09 |
-| `python hyperfine_importers/prefab_slots_timer.py` | 16.7 ± 0.7 | 15.8 | 17.8 | 1.43 ± 0.09 |
-| `python hyperfine_importers/prefab_eval_timer.py` | 41.0 ± 1.5 | 39.2 | 44.6 | 3.52 ± 0.21 |
-| `python hyperfine_importers/namedtuples_timer.py` | 22.3 ± 1.2 | 21.2 | 26.7 | 1.92 ± 0.14 |
-| `python hyperfine_importers/typed_namedtuples_timer.py` | 38.0 ± 1.2 | 36.2 | 41.3 | 3.27 ± 0.19 |
-| `python hyperfine_importers/dataclasses_timer.py` | 77.3 ± 3.5 | 74.5 | 93.1 | 6.65 ± 0.44 |
-| `python hyperfine_importers/attrs_noslots_timer.py` | 119.9 ± 1.6 | 117.1 | 122.5 | 10.32 ± 0.51 |
-| `python hyperfine_importers/attrs_slots_timer.py` | 123.4 ± 2.1 | 119.5 | 131.6 | 10.62 ± 0.54 |
-| `python hyperfine_importers/pydantic_timer.py` | 275.6 ± 6.3 | 267.8 | 304.8 | 23.72 ± 1.25 |
+| `python -c "pass"` | 22.9 ± 0.4 | 21.8 | 23.6 | 1.00 |
+| `python hyperfine_importers/native_classes_timer.py` | 24.2 ± 0.7 | 22.8 | 26.6 | 1.06 ± 0.04 |
+| `python hyperfine_importers/slotclasses_timer.py` | 24.9 ± 0.7 | 23.8 | 27.7 | 1.09 ± 0.04 |
+| `python hyperfine_importers/prefab_timer.py` | 25.8 ± 0.5 | 24.8 | 27.2 | 1.13 ± 0.03 |
+| `python hyperfine_importers/prefab_slots_timer.py` | 25.9 ± 0.6 | 24.9 | 27.5 | 1.13 ± 0.03 |
+| `python hyperfine_importers/prefab_eval_timer.py` | 35.1 ± 0.6 | 34.0 | 36.4 | 1.53 ± 0.04 |
+| `python hyperfine_importers/namedtuples_timer.py` | 28.3 ± 0.4 | 27.5 | 29.0 | 1.24 ± 0.03 |
+| `python hyperfine_importers/typed_namedtuples_timer.py` | 39.1 ± 0.9 | 37.4 | 41.8 | 1.71 ± 0.05 |
+| `python hyperfine_importers/dataclasses_timer.py` | 61.1 ± 2.1 | 58.1 | 69.1 | 2.67 ± 0.11 |
+| `python hyperfine_importers/attrs_noslots_timer.py` | 88.9 ± 2.2 | 86.7 | 98.3 | 3.88 ± 0.12 |
+| `python hyperfine_importers/attrs_slots_timer.py` | 90.9 ± 1.4 | 88.9 | 94.2 | 3.97 ± 0.10 |
+| `python hyperfine_importers/pydantic_timer.py` | 172.4 ± 5.3 | 164.5 | 181.5 | 7.53 ± 0.27 |
+
+
 
 ## Class Generation time without imports ##
 
 From `perf_profile.py`.
 
 ```
-Python Version: 3.12.1 (main, Dec 10 2023, 09:30:46) [GCC 11.4.0]
-Classbuilder version: v0.1.0
-Platform: Linux-5.15.0-91-generic-x86_64-with-glibc2.35
+Python Version: 3.12.2 (tags/v3.12.2:6abddd9, Feb  6 2024, 21:26:36) [MSC v.1937 64 bit (AMD64)]
+Classbuilder version: v0.4.0
+Platform: Windows-10-10.0.19045-SP0
 Time for 100 imports of 100 classes defined with 5 basic attributes
 ```
 
 | Method | Total Time (seconds) |
 | --- | --- |
-| standard classes | 0.13 |
-| namedtuple | 0.72 |
-| NamedTuple | 1.29 |
-| dataclasses | 4.24 |
-| attrs 23.2.0 | 7.04 |
-| pydantic 2.6.4 | 10.25 |
-| dabeaz/cluegen | 0.28 |
-| dabeaz/cluegen_eval | 2.50 |
-| dabeaz/dataklasses | 0.27 |
-| dabeaz/dataklasses_eval | 0.27 |
-| slotclass v0.1.0 | 0.28 |
-| prefab_slots v0.1.0 | 0.38 |
-| prefab v0.1.0 | 0.38 |
-| prefab_attributes v0.1.0 | 0.40 |
-| prefab_eval v0.1.0 | 2.98 |
+| standard classes | 0.07 |
+| namedtuple | 0.33 |
+| NamedTuple | 0.50 |
+| dataclasses | 2.05 |
+| attrs 23.2.0 | 3.73 |
+| pydantic 2.7.1 | 4.19 |
+| dabeaz/cluegen | 0.10 |
+| dabeaz/cluegen_eval | 0.91 |
+| dabeaz/dataklasses | 0.10 |
+| dabeaz/dataklasses_eval | 0.10 |
+| slotclass v0.4.0 | 0.12 |
+| prefab_slots v0.4.0 | 0.16 |
+| prefab v0.4.0 | 0.18 |
+| prefab_attributes v0.4.0 | 0.16 |
+| prefab_eval v0.4.0 | 1.12 |
```

### Comparing `ducktools_classbuilder-0.3.0/docs/prefab/index.md` & `ducktools_classbuilder-0.4.0/docs/prefab/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/pyproject.toml` & `ducktools_classbuilder-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ducktools.classbuilder.__version__"}
 
 [project.optional-dependencies]
-testing = ["pytest", "pytest-cov", "mypy"]
+testing = ["pytest", "pytest-cov", "mypy", "typing_extensions; python_version < '3.10'"]
 docs = ["sphinx", "myst-parser", "sphinx_rtd_theme"]
 
 [project.urls]
 "Homepage" = "https://github.com/davidcellis/ducktools-classbuilder"
 
 [tool.pytest.ini_options]
 addopts= "--cov=src/ --cov-report=term-missing"
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.py` & `ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,27 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "v0.3.0"
+import sys
+
+__version__ = "v0.4.0"
 
 # Change this name if you make heavy modifications
 INTERNALS_DICT = "__classbuilder_internals__"
 
 
+# If testing, make Field classes frozen to make sure attributes are not
+# overwritten. When running this is a performance penalty so it is not required.
+_UNDER_TESTING = "pytest" in sys.modules
+
+
 def get_fields(cls, *, local=False):
     """
     Utility function to gather the fields dictionary
     from the class internals.
 
     :param cls: generated class
     :param local: get only fields that were not inherited
@@ -98,54 +105,60 @@
         setattr(cls, self.funcname, method)
 
         # Use 'get' to return the generated function as a bound method
         # instead of as a regular function for first usage.
         return method.__get__(instance, cls)
 
 
-def init_maker(cls, *, null=NOTHING, extra_code=None):
-    fields = get_fields(cls)
-    flags = get_flags(cls)
+def get_init_maker(null=NOTHING, extra_code=None):
+    def cls_init_maker(cls):
+        fields = get_fields(cls)
+        flags = get_flags(cls)
 
-    arglist = []
-    assignments = []
-    globs = {}
+        arglist = []
+        assignments = []
+        globs = {}
 
-    if flags.get("kw_only", False):
-        arglist.append("*")
+        if flags.get("kw_only", False):
+            arglist.append("*")
 
-    for k, v in fields.items():
-        if v.default is not null:
-            globs[f"_{k}_default"] = v.default
-            arg = f"{k}=_{k}_default"
-            assignment = f"self.{k} = {k}"
-        elif v.default_factory is not null:
-            globs[f"_{k}_factory"] = v.default_factory
-            arg = f"{k}=None"
-            assignment = f"self.{k} = _{k}_factory() if {k} is None else {k}"
-        else:
-            arg = f"{k}"
-            assignment = f"self.{k} = {k}"
+        for k, v in fields.items():
+            if v.default is not null:
+                globs[f"_{k}_default"] = v.default
+                arg = f"{k}=_{k}_default"
+                assignment = f"self.{k} = {k}"
+            elif v.default_factory is not null:
+                globs[f"_{k}_factory"] = v.default_factory
+                arg = f"{k}=None"
+                assignment = f"self.{k} = _{k}_factory() if {k} is None else {k}"
+            else:
+                arg = f"{k}"
+                assignment = f"self.{k} = {k}"
 
-        arglist.append(arg)
-        assignments.append(assignment)
+            arglist.append(arg)
+            assignments.append(assignment)
 
-    args = ", ".join(arglist)
-    assigns = "\n    ".join(assignments) if assignments else "pass\n"
-    code = (
-        f"def __init__(self, {args}):\n" 
-        f"    {assigns}\n"
-    )
-    # Handle additional function calls
-    # Used for validate_field on fieldclasses
-    if extra_code:
-        for line in extra_code:
-            code += f"    {line}\n"
+        args = ", ".join(arglist)
+        assigns = "\n    ".join(assignments) if assignments else "pass\n"
+        code = (
+            f"def __init__(self, {args}):\n" 
+            f"    {assigns}\n"
+        )
+        # Handle additional function calls
+        # Used for validate_field on fieldclasses
+        if extra_code:
+            for line in extra_code:
+                code += f"    {line}\n"
 
-    return code, globs
+        return code, globs
+
+    return cls_init_maker
+
+
+init_maker = get_init_maker()
 
 
 def repr_maker(cls):
     fields = get_fields(cls)
     content = ", ".join(
         f"{name}={{self.{name}!r}}"
         for name, attrib in fields.items()
@@ -174,19 +187,62 @@
         f"    return {instance_comparison} if {class_comparison} else NotImplemented\n"
     )
     globs = {}
 
     return code, globs
 
 
+def frozen_setattr_maker(cls):
+    globs = {}
+    field_names = set(get_fields(cls))
+    flags = get_flags(cls)
+
+    globs["__field_names"] = field_names
+
+    # Better to be safe and use the method that works in both cases
+    # if somehow slotted has not been set.
+    if flags.get("slotted", True):
+        globs["__setattr_func"] = object.__setattr__
+        setattr_method = "__setattr_func(self, name, value)"
+    else:
+        setattr_method = "self.__dict__[name] = value"
+
+    body = (
+        f"    if hasattr(self, name) or name not in __field_names:\n"
+        f'        raise TypeError(\n'
+        f'            f"{{type(self).__name__!r}} object does not support "'
+        f'            f"attribute assignment"\n'
+        f'        )\n'
+        f"    else:\n"
+        f"        {setattr_method}\n"
+    )
+    code = f"def __setattr__(self, name, value):\n{body}"
+
+    return code, globs
+
+
+def frozen_delattr_maker(cls):
+    body = (
+        '    raise TypeError(\n'
+        '        f"{type(self).__name__!r} object "\n'
+        '        f"does not support attribute deletion"\n'
+        '    )\n'
+    )
+    code = f"def __delattr__(self, name):\n{body}"
+    globs = {}
+    return code, globs
+
+
 # As only the __get__ method refers to the class we can use the same
 # Descriptor instances for every class.
 init_desc = MethodMaker("__init__", init_maker)
 repr_desc = MethodMaker("__repr__", repr_maker)
 eq_desc = MethodMaker("__eq__", eq_maker)
+frozen_setattr_desc = MethodMaker("__setattr__", frozen_setattr_maker)
+frozen_delattr_desc = MethodMaker("__delattr__", frozen_delattr_maker)
 default_methods = frozenset({init_desc, repr_desc, eq_desc})
 
 
 def builder(cls=None, /, *, gatherer, methods, flags=None):
     """
     The main builder for class generation
 
@@ -240,14 +296,16 @@
 # However after this, the other methods can be generated.
 class Field:
     """
     A basic class to handle the assignment of defaults/factories with
     some metadata.
 
     Intended to be extendable by subclasses for additional features.
+
+    Note: When run under `pytest`, Field instances are Frozen.
     """
     __slots__ = {
         "default": "Standard default value to be used for attributes with"
                    "this field.",
         "default_factory": "A 0 argument function to be called to generate "
                            "a default value, useful for mutable objects like "
                            "lists.",
@@ -299,22 +357,27 @@
 _field_internal = {
     "default": Field(default=NOTHING),
     "default_factory": Field(default=NOTHING),
     "type": Field(default=NOTHING),
     "doc": Field(default=None),
 }
 
+_field_methods = {repr_desc, eq_desc}
+if _UNDER_TESTING:
+    _field_methods.update({frozen_setattr_desc, frozen_delattr_desc})
+
 builder(
     Field,
     gatherer=lambda cls_: _field_internal,
-    methods=frozenset({repr_desc, eq_desc}),
+    methods=_field_methods,
     flags={"slotted": True, "kw_only": True},
 )
 
 
+# Slot gathering tools
 # Subclass of dict to be identifiable by isinstance checks
 # For anything more complicated this could be made into a Mapping
 class SlotFields(dict):
     """
     A plain dict subclass.
 
     For declaring slotfields there are no additional features required
@@ -322,54 +385,160 @@
     generating dict and isn't a regular dictionary that ended up in
     `__slots__`.
 
     This should be replaced on `__slots__` after fields have been gathered.
     """
 
 
-def slot_gatherer(cls):
-    """
-    Gather field information for class generation based on __slots__
-    
-    :param cls: Class to gather field information from
-    :return: dict of field_name: Field(...)
-    """
-    cls_slots = cls.__dict__.get("__slots__", None)
-
-    if not isinstance(cls_slots, SlotFields):
-        raise TypeError(
-            "__slots__ must be an instance of SlotFields "
-            "in order to generate a slotclass"
-        )
+def make_slot_gatherer(field_type=Field):
+    def field_slot_gatherer(cls):
+        """
+        Gather field information for class generation based on __slots__
 
-    cls_annotations = cls.__dict__.get("__annotations__", {})
-    cls_fields = {}
-    slot_replacement = {}
-
-    for k, v in cls_slots.items():
-        if isinstance(v, Field):
-            attrib = v
-            if v.type is not NOTHING:
-                cls_annotations[k] = attrib.type
+        :param cls: Class to gather field information from
+        :return: dict of field_name: Field(...)
+        """
+        cls_slots = cls.__dict__.get("__slots__", None)
+
+        if not isinstance(cls_slots, SlotFields):
+            raise TypeError(
+                "__slots__ must be an instance of SlotFields "
+                "in order to generate a slotclass"
+            )
+
+        cls_annotations = cls.__dict__.get("__annotations__", {})
+        cls_fields = {}
+        slot_replacement = {}
+
+        for k, v in cls_slots.items():
+            if isinstance(v, field_type):
+                attrib = v
+                if attrib.type is not NOTHING:
+                    cls_annotations[k] = attrib.type
+            else:
+                # Plain values treated as defaults
+                attrib = field_type(default=v)
+
+            slot_replacement[k] = attrib.doc
+            cls_fields[k] = attrib
+
+        # Replace the SlotAttributes instance with a regular dict
+        # So that help() works
+        setattr(cls, "__slots__", slot_replacement)
+
+        # Update annotations with any types from the slots assignment
+        setattr(cls, "__annotations__", cls_annotations)
+        return cls_fields
+
+    return field_slot_gatherer
+
+
+slot_gatherer = make_slot_gatherer()
+
+
+# Annotation gathering tools
+def is_classvar(hint):
+    _typing = sys.modules.get("typing")
+
+    if _typing:
+        # Annotated is a nightmare I'm never waking up from
+        # 3.8 and 3.9 need Annotated from typing_extensions
+        # 3.8 also needs get_origin from typing_extensions
+        if sys.version_info < (3, 10):
+            _typing_extensions = sys.modules.get("typing_extensions")
+            if _typing_extensions:
+                _Annotated = _typing_extensions.Annotated
+                _get_origin = _typing_extensions.get_origin
+            else:
+                _Annotated, _get_origin = None, None
         else:
-            # Plain values treated as defaults
-            attrib = Field(default=v)
+            _Annotated = _typing.Annotated
+            _get_origin = _typing.get_origin
+
+        if _Annotated and _get_origin(hint) is _Annotated:
+            hint = getattr(hint, "__origin__", None)
+
+        if (
+            hint is _typing.ClassVar
+            or getattr(hint, "__origin__", None) is _typing.ClassVar
+        ):
+            return True
+        # String used as annotation
+        elif isinstance(hint, str) and "ClassVar" in hint:
+            return True
+    return False
+
+
+def make_annotation_gatherer(field_type=Field, leave_default_values=True):
+    """
+    Create a new annotation gatherer that will work with `Field` instances
+    of the creators definition.
+
+    :param field_type: The `Field` classes to be used when gathering fields
+    :param leave_default_values: Set to True if the gatherer should leave
+                                 default values in place as class variables.
+    :return: An annotation gatherer with these settings.
+    """
+    def field_annotation_gatherer(cls):
+        cls_annotations = cls.__dict__.get("__annotations__", {})
+
+        cls_fields: dict[str, field_type] = {}
+
+        for k, v in cls_annotations.items():
+            # Ignore ClassVar
+            if is_classvar(v):
+                continue
+
+            attrib = getattr(cls, k, NOTHING)
+
+            if attrib is not NOTHING:
+                if isinstance(attrib, field_type):
+                    attrib = field_type.from_field(attrib, type=v)
+                    if attrib.default is not NOTHING and leave_default_values:
+                        setattr(cls, k, attrib.default)
+                    else:
+                        delattr(cls, k)
+                else:
+                    attrib = field_type(default=attrib, type=v)
+                    if not leave_default_values:
+                        delattr(cls, k)
+
+            else:
+                attrib = field_type(type=v)
 
-        slot_replacement[k] = attrib.doc
-        cls_fields[k] = attrib
+            cls_fields[k] = attrib
 
-    # Replace the SlotAttributes instance with a regular dict
-    # So that help() works
-    setattr(cls, "__slots__", slot_replacement)
-
-    # Update annotations with any types from the slots assignment
-    setattr(cls, "__annotations__", cls_annotations)
-    return cls_fields
+        return cls_fields
 
+    return field_annotation_gatherer
+
+
+annotation_gatherer = make_annotation_gatherer()
+
+
+def check_argument_order(cls):
+    """
+    Raise a SyntaxError if the argument order will be invalid for a generated
+    `__init__` function.
 
+    :param cls: class being built
+    """
+    fields = get_fields(cls)
+    used_default = False
+    for k, v in fields.items():
+        if v.default is NOTHING and v.default_factory is NOTHING:
+            if used_default:
+                raise SyntaxError(
+                    f"non-default argument {k!r} follows default argument"
+                )
+        else:
+            used_default = True
+
+
+# Class Decorators
 def slotclass(cls=None, /, *, methods=default_methods, syntax_check=True):
     """
     Example of class builder in action using __slots__ to find fields.
 
     :param cls: Class to be analysed and modified
     :param methods: MethodMakers to be added to the class
     :param syntax_check: check there are no arguments without defaults
@@ -378,48 +547,58 @@
     """
     if not cls:
         return lambda cls_: slotclass(cls_, methods=methods, syntax_check=syntax_check)
 
     cls = builder(cls, gatherer=slot_gatherer, methods=methods, flags={"slotted": True})
 
     if syntax_check:
-        fields = get_fields(cls)
-        used_default = False
-        for k, v in fields.items():
-            if v.default is NOTHING and v.default_factory is NOTHING:
-                if used_default:
-                    raise SyntaxError(
-                        f"non-default argument {k!r} follows default argument"
-                    )
-            else:
-                used_default = True
+        check_argument_order(cls)
+
+    return cls
+
+
+def annotationclass(cls=None, /, *, methods=default_methods):
+    if not cls:
+        return lambda cls_: annotationclass(cls_, methods=methods)
+
+    cls = builder(cls, gatherer=annotation_gatherer, methods=methods, flags={"slotted": False})
+
+    check_argument_order(cls)
 
     return cls
 
 
-def _field_init_func(cls):
-    # Fields need a different Nothing for their __init__ generation
-    # And an extra call to validate_field
-    field_nothing = _NothingType()
-    extra_calls = ["self.validate_field()"]
-    return init_maker(cls, null=field_nothing, extra_code=extra_calls)
+_field_init_desc = MethodMaker(
+    funcname="__init__",
+    code_generator=get_init_maker(
+        null=_NothingType(),
+        extra_code=["self.validate_field()"],
+    )
+)
 
 
-def fieldclass(cls):
+def fieldclass(cls=None, /, *, frozen=False):
     """
     This is a special decorator for making Field subclasses using __slots__.
     This works by forcing the __init__ method to treat NOTHING as a regular
     value. This means *all* instance attributes always have defaults.
 
     :param cls: Field subclass
+    :param frozen: Make the field class a frozen class.
+                   Field classes are always frozen when running under `pytest`
     :return: Modified subclass
     """
+    if not cls:
+        return lambda cls_: fieldclass(cls_, frozen=frozen)
+
+    field_methods = {_field_init_desc, repr_desc, eq_desc}
 
-    field_init_desc = MethodMaker("__init__", _field_init_func)
-    field_methods = frozenset({field_init_desc, repr_desc, eq_desc})
+    # Always freeze when running tests
+    if frozen or _UNDER_TESTING:
+        field_methods.update({frozen_setattr_desc, frozen_delattr_desc})
 
     cls = builder(
         cls,
         gatherer=slot_gatherer,
         methods=field_methods,
         flags={"slotted": True, "kw_only": True}
     )
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.pyi` & `ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -22,26 +22,32 @@
 class MethodMaker:
     funcname: str
     code_generator: _codegen_type
     def __init__(self, funcname: str, code_generator: _codegen_type) -> None: ...
     def __repr__(self) -> str: ...
     def __get__(self, instance, cls) -> Callable: ...
 
-def init_maker(
-    cls: type,
-    *,
+def get_init_maker(
     null: _NothingType = NOTHING,
     extra_code: None | list[str] = None
-) -> tuple[str, dict[str, typing.Any]]: ...
+) -> Callable[[type], tuple[str, dict[str, typing.Any]]]: ...
+
+def init_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 def repr_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 def eq_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 
+def frozen_setattr_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
+
+def frozen_delattr_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
+
 init_desc: MethodMaker
 repr_desc: MethodMaker
 eq_desc: MethodMaker
+frozen_setattr_desc: MethodMaker
+frozen_delattr_desc: MethodMaker
 default_methods: frozenset[MethodMaker]
 
 _T = typing.TypeVar("_T")
 
 @typing.overload
 def builder(
     cls: type[_T],
@@ -85,17 +91,30 @@
     @classmethod
     def from_field(cls, fld: Field, /, **kwargs: typing.Any) -> Field: ...
 
 
 class SlotFields(dict):
     ...
 
+def make_slot_gatherer(field_type: type[Field] = Field) -> Callable[[type], dict[str, Field]]: ...
+
 def slot_gatherer(cls: type) -> dict[str, Field]:
     ...
 
+def is_classvar(hint: object) -> bool: ...
+
+def make_annotation_gatherer(
+    field_type: type[Field] = Field,
+    leave_default_values: bool = True,
+) -> Callable[[type], dict[str, Field]]: ...
+
+def annotation_gatherer(cls: type) -> dict[str, Field]: ...
+
+def check_argument_order(cls: type) -> None: ...
+
 @typing.overload
 def slotclass(
     cls: type[_T],
     /,
     *,
     methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
     syntax_check: bool = True
@@ -106,8 +125,28 @@
     cls: None = None,
     /,
     *,
     methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
     syntax_check: bool = True
 ) -> Callable[[type[_T]], type[_T]]: ...
 
-def fieldclass(cls: type[_T]) -> type[_T]: ...
+@typing.overload
+def annotationclass(
+    cls: type[_T],
+    /,
+    *,
+    methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
+) -> type[_T]: ...
+
+@typing.overload
+def annotationclass(
+        cls: None = None,
+        /,
+        *,
+        methods: frozenset[MethodMaker] | set[MethodMaker] = default_methods,
+) -> Callable[[type[_T]], type[_T]]: ...
+
+@typing.overload
+def fieldclass(cls: type[_T], /, *, frozen: bool = False) -> type[_T]: ...
+
+@typing.overload
+def fieldclass(cls: None = None, /, *, frozen: bool = False) -> Callable[[type[_T]], type[_T]]: ...
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.py` & `ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/prefab.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 """
 
 import sys
 
 from . import (
     INTERNALS_DICT, NOTHING,
     Field, MethodMaker, SlotFields,
-    builder, fieldclass, get_flags, get_fields, slot_gatherer
+    builder, fieldclass, get_flags, get_fields, make_slot_gatherer,
+    frozen_setattr_desc, frozen_delattr_desc, is_classvar,
 )
 
 PREFAB_FIELDS = "PREFAB_FIELDS"
 PREFAB_INIT_FUNC = "__prefab_init__"
 PRE_INIT_FUNC = "__prefab_pre_init__"
 POST_INIT_FUNC = "__prefab_post_init__"
 
@@ -51,28 +52,14 @@
 KW_ONLY = _KW_ONLY_TYPE()
 
 
 class PrefabError(Exception):
     pass
 
 
-def _is_classvar(hint):
-    _typing = sys.modules.get("typing")
-    if _typing:
-        if (
-            hint is _typing.ClassVar
-            or getattr(hint, "__origin__", None) is _typing.ClassVar
-        ):
-            return True
-        # String used as annotation
-        elif isinstance(hint, str) and "ClassVar" in hint:
-            return True
-    return False
-
-
 def get_attributes(cls):
     """
     Copy of get_fields, typed to return Attribute instead of Field.
     This is used in the prefab methods.
 
     :param cls: class built with _make_prefab
     :return: dict[str, Attribute] of all gathered attributes
@@ -336,65 +323,14 @@
         code = f"def __iter__(self):\n{values}"
         globs = {}
         return code, globs
 
     return MethodMaker("__iter__", __iter__)
 
 
-def get_frozen_setattr_maker():
-    def __setattr__(cls: "type") -> "tuple[str, dict]":
-        globs = {}
-        attributes = get_attributes(cls)
-        flags = get_flags(cls)
-
-        # Make the fields set literal
-        fields_delimited = ", ".join(f"{field!r}" for field in attributes)
-        field_set = f"{{ {fields_delimited} }}"
-
-        # Better to be safe and use the method that works in both cases
-        # if somehow slotted has not been set.
-        if flags.get("slotted", True):
-            globs["__prefab_setattr_func"] = object.__setattr__
-            setattr_method = "__prefab_setattr_func(self, name, value)"
-        else:
-            setattr_method = "self.__dict__[name] = value"
-
-        body = (
-            f"    if hasattr(self, name) or name not in {field_set}:\n"
-            f'        raise TypeError(\n'
-            f'            f"{{type(self).__name__!r}} object does not support "'
-            f'            f"attribute assignment"\n'
-            f'        )\n'
-            f"    else:\n"
-            f"        {setattr_method}\n"
-        )
-        code = f"def __setattr__(self, name, value):\n{body}"
-
-        return code, globs
-
-    # Pass the exception to exec
-    return MethodMaker("__setattr__", __setattr__)
-
-
-def get_frozen_delattr_maker():
-    # noinspection PyUnusedLocal
-    def __delattr__(cls: "type") -> "tuple[str, dict]":
-        body = (
-            '    raise TypeError(\n'
-            '        f"{type(self).__name__!r} object "\n'
-            '        f"does not support attribute deletion"\n'
-            '    )\n'
-        )
-        code = f"def __delattr__(self, name):\n{body}"
-        globs = {}
-        return code, globs
-
-    return MethodMaker("__delattr__", __delattr__)
-
-
 def get_asdict_maker():
     def as_dict_gen(cls: "type") -> "tuple[str, dict]":
         fields = get_attributes(cls)
 
         vals = ", ".join(
             f"'{name}': self.{name}"
             for name, attrib in fields.items()
@@ -410,16 +346,14 @@
 
 init_desc = get_init_maker()
 prefab_init_desc = get_init_maker(init_name=PREFAB_INIT_FUNC)
 repr_desc = get_repr_maker()
 recursive_repr_desc = get_repr_maker(recursion_safe=True)
 eq_desc = get_eq_maker()
 iter_desc = get_iter_maker()
-frozen_setattr_desc = get_frozen_setattr_maker()
-frozen_delattr_desc = get_frozen_delattr_maker()
 asdict_desc = get_asdict_maker()
 
 
 # Updated field with additional attributes
 @fieldclass
 class Attribute(Field):
     __slots__ = SlotFields(
@@ -487,20 +421,15 @@
         serialize=serialize,
         exclude_field=exclude_field,
         doc=doc,
         type=type,
     )
 
 
-def slot_prefab_gatherer(cls):
-    # For prefabs it's easier if everything is an attribute
-    return {
-        name: Attribute.from_field(fld)
-        for name, fld in slot_gatherer(cls).items()
-    }
+slot_prefab_gatherer = make_slot_gatherer(Attribute)
 
 
 # Gatherer for classes built on attributes or annotations
 def attribute_gatherer(cls):
     cls_annotations = cls.__dict__.get("__annotations__", {})
     cls_annotation_names = cls_annotations.keys()
 
@@ -515,59 +444,65 @@
     if set(cls_annotation_names).issuperset(set(cls_attribute_names)):
         # replace the classes' attributes dict with one with the correct
         # order from the annotations.
         kw_flag = False
         new_attributes = {}
         for name, value in cls_annotations.items():
             # Ignore ClassVar hints
-            if _is_classvar(value):
+            if is_classvar(value):
                 continue
 
             # Look for the KW_ONLY annotation
             if value is KW_ONLY or value == "KW_ONLY":
                 if kw_flag:
                     raise PrefabError(
                         "Class can not be defined as keyword only twice"
                     )
                 kw_flag = True
             else:
                 # Copy attributes that are already defined to the new dict
                 # generate Attribute() values for those that are not defined.
 
+                # Extra parameters to pass to each Attribute
+                extras = {
+                    "type": cls_annotations[name]
+                }
+                if kw_flag:
+                    extras["kw_only"] = True
+
                 # If a field name is also declared in slots it can't have a real
                 # default value and the attr will be the slot descriptor.
                 if hasattr(cls, name) and name not in cls_slots:
                     if name in cls_attribute_names:
-                        attrib = cls_attributes[name]
+                        attrib = Attribute.from_field(
+                            cls_attributes[name],
+                            **extras,
+                        )
                     else:
                         attribute_default = getattr(cls, name)
-                        attrib = attribute(default=attribute_default)
+                        attrib = attribute(default=attribute_default, **extras)
 
                     # Clear the attribute from the class after it has been used
                     # in the definition.
                     delattr(cls, name)
                 else:
-                    attrib = attribute()
-
-                if kw_flag:
-                    attrib.kw_only = True
+                    attrib = attribute(**extras)
 
-                attrib.type = cls_annotations[name]
                 new_attributes[name] = attrib
 
         cls_attributes = new_attributes
     else:
-        for name, attrib in cls_attributes.items():
-            delattr(cls, name)
+        for name in cls_attributes.keys():
+            attrib = cls_attributes[name]
+            delattr(cls, name)  # clear attrib from class
 
             # Some items can still be annotated.
-            try:
-                attrib.type = cls_annotations[name]
-            except KeyError:
-                pass
+            if name in cls_annotations:
+                new_attrib = Attribute.from_field(attrib, type=cls_annotations[name])
+                cls_attributes[name] = new_attrib
 
     return cls_attributes
 
 
 # Class Builders
 # noinspection PyShadowingBuiltins
 def _make_prefab(
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.pyi` & `ducktools_classbuilder-0.4.0/src/ducktools/classbuilder/prefab.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,41 +22,33 @@
 class _KW_ONLY_TYPE:
     def __repr__(self) -> str: ...
 
 KW_ONLY: _KW_ONLY_TYPE
 
 class PrefabError(Exception): ...
 
-def _is_classvar(hint: type | str) -> bool: ...
-
 def get_attributes(cls: type) -> dict[str, Attribute]: ...
 
 def get_init_maker(*, init_name: str="__init__") -> MethodMaker: ...
 
 def get_repr_maker(*, recursion_safe: bool = False) -> MethodMaker: ...
 
 def get_eq_maker() -> MethodMaker: ...
 
 def get_iter_maker() -> MethodMaker: ...
 
-def get_frozen_setattr_maker() -> MethodMaker: ...
-
-def get_frozen_delattr_maker() -> MethodMaker: ...
-
 def get_asdict_maker() -> MethodMaker: ...
 
 
 init_desc: MethodMaker
 prefab_init_desc: MethodMaker
 repr_desc: MethodMaker
 recursive_repr_desc: MethodMaker
 eq_desc: MethodMaker
 iter_desc: MethodMaker
-frozen_setattr_desc: MethodMaker
-frozen_delattr_desc: MethodMaker
 asdict_desc: MethodMaker
 
 class Attribute(Field):
     __slots__: dict
 
     init: bool
     repr: bool
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/PKG-INFO` & `ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.3.0
+Version: 0.4.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mypy; extra == "testing"
+Requires-Dist: typing_extensions; python_version < "3.10" and extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 # Ducktools: Class Builder #
 
@@ -117,15 +118,15 @@
 a similar manner to the `@dataclass` decorator from `dataclasses`. 
 
 > [!NOTE] 
 > `ducktools.classbuilder` includes a premade version of `slotclass` that can
 > be used directly. (The included version has some extra features).
 
 ```python
-from ducktools.classbuilder import Field, SlotFields
+from ducktools.classbuilder import Field, SlotFields, slotclass
 
 @slotclass
 class SlottedDC:
     __slots__ = SlotFields(
         the_answer=42,
         the_question=Field(
             default="What do you get if you multiply six by nine?",
@@ -202,26 +203,49 @@
 print(DataCoords())
 print(SlotCoords())
 
 print(f"{DataCoords is class_register[DataCoords.__name__] = }")
 print(f"{SlotCoords is class_register[SlotCoords.__name__] = }")
 ```
 
+## Using annotations anyway ##
+
+For those that really want to use type annotations a basic `annotation_gatherer`
+function and `@annotationclass` decorator are also included. Slots are not generated
+in this case.
+
+```python
+from ducktools.classbuilder import annotationclass
+
+@annotationclass
+class AnnotatedDC:
+    the_answer: int = 42
+    the_question: str = "What do you get if you multiply six by nine?"
+
+    
+ex = AnnotatedDC()
+print(ex)
+```
+
 ## What features does this have? ##
 
 Included as an example implementation, the `slotclass` generator supports 
 `default_factory` for creating mutable defaults like lists, dicts etc.
 It also supports default values that are not builtins (try this on 
 [Cluegen](https://github.com/dabeaz/cluegen)).
 
 It will copy values provided as the `type` to `Field` into the 
 `__annotations__` dictionary of the class. 
 Values provided to `doc` will be placed in the final `__slots__` 
 field so they are present on the class if `help(...)` is called.
 
+A fairly basic `annotations_gatherer` and `annotationclass` are included
+in `extras.py` which can be used to generate classbuilders that rely on 
+annotations.
+
 If you want something with more features you can look at the `prefab.py`
 implementation which provides a 'prebuilt' implementation.
 
 ## Will you add \<feature\> to `classbuilder.prefab`? ##
 
 No. Not unless it's something I need or find interesting.
```

### Comparing `ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/SOURCES.txt` & `ducktools_classbuilder-0.4.0/src/ducktools_classbuilder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/ducktools/classbuilder/prefab.pyi
 src/ducktools/classbuilder/py.typed
 src/ducktools_classbuilder.egg-info/PKG-INFO
 src/ducktools_classbuilder.egg-info/SOURCES.txt
 src/ducktools_classbuilder.egg-info/dependency_links.txt
 src/ducktools_classbuilder.egg-info/requires.txt
 src/ducktools_classbuilder.egg-info/top_level.txt
+tests/test_annotated.py
 tests/test_core.py
 tests/prefab/dynamic/test_compare_attrib.py
 tests/prefab/dynamic/test_construction.py
 tests/prefab/dynamic/test_internals.py
 tests/prefab/dynamic/test_pre_post_init.py
 tests/prefab/dynamic/test_slots_novalues.py
 tests/prefab/dynamic/test_slotted_class.py
```

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_construction.py` & `ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_construction.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_internals.py` & `ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_internals.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_pre_post_init.py` & `ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_pre_post_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slotted_class.py` & `ducktools_classbuilder-0.4.0/tests/prefab/dynamic/test_slotted_class.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/dunders.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/inheritance.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/init_ex.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/init_ex.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/kw_only.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/repr_func.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/examples/repr_func.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_creation.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_creation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for errors raised on class creation"""
+import sys
 
 from ducktools.classbuilder.prefab import PrefabError
 
 import pytest
 
 
 class TestEmptyClass:
@@ -97,30 +98,50 @@
 
     def test_keep_match_args(self):
         from creation import KeepDefinedMethods
 
         assert KeepDefinedMethods.__match_args__ == ("x",)
 
 
-def test_skipped_classvars():
-    from creation import IgnoreClassVars
-
-    fields = IgnoreClassVars.PREFAB_FIELDS
-    assert "v" not in fields
-    assert "w" not in fields
-    assert "x" not in fields
-    assert "y" not in fields
-    assert "z" not in fields
-    assert "actual" in fields
-
-    assert "v" in getattr(IgnoreClassVars, "__dict__")
-    assert "w" in getattr(IgnoreClassVars, "__dict__")
-    assert "x" in getattr(IgnoreClassVars, "__dict__")
-    assert "y" in getattr(IgnoreClassVars, "__dict__")
-    assert "z" in getattr(IgnoreClassVars, "__dict__")
+class TestClassVar:
+    def test_skipped_classvars(self):
+        from creation import IgnoreClassVars
+
+        fields = IgnoreClassVars.PREFAB_FIELDS
+        assert "v" not in fields
+        assert "w" not in fields
+        assert "x" not in fields
+        assert "y" not in fields
+        assert "z" not in fields
+        assert "actual" in fields
+
+        assert "v" in getattr(IgnoreClassVars, "__dict__")
+        assert "w" in getattr(IgnoreClassVars, "__dict__")
+        assert "x" in getattr(IgnoreClassVars, "__dict__")
+        assert "y" in getattr(IgnoreClassVars, "__dict__")
+        assert "z" in getattr(IgnoreClassVars, "__dict__")
+
+    def test_skipped_annotated_classvars(self):
+        from creation import IgnoreAnnotatedClassVars
+
+        fields = IgnoreAnnotatedClassVars.PREFAB_FIELDS
+        if sys.version_info >= (3, 11):
+            assert "v" not in fields
+            assert "w" not in fields
+        assert "x" not in fields
+        assert "y" not in fields
+        assert "z" not in fields
+        assert "actual" in fields
+
+        if sys.version_info >= (3, 11):
+            assert "v" in getattr(IgnoreAnnotatedClassVars, "__dict__")
+            assert "w" in getattr(IgnoreAnnotatedClassVars, "__dict__")
+        assert "x" in getattr(IgnoreAnnotatedClassVars, "__dict__")
+        assert "y" in getattr(IgnoreAnnotatedClassVars, "__dict__")
+        assert "z" in getattr(IgnoreAnnotatedClassVars, "__dict__")
 
 
 class TestExceptions:
     def test_kw_not_in_init(self):
         with pytest.raises(PrefabError) as e_info:
             from fails.creation_1 import Construct
```

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_dunders.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_frozen.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_frozen.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_funcs.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_funcs.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_hint_syntax.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_hint_syntax.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_inheritance.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_init.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_kw_only.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_repr.py` & `ducktools_classbuilder-0.4.0/tests/prefab/shared/test_repr.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.3.0/tests/test_core.py` & `ducktools_classbuilder-0.4.0/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     f2 = Field(default=False)
     f3 = Field(default_factory=list)
     f4 = Field(default=True, type=bool)
     f5 = Field(default=True, doc="True or False")
 
     for fld in [f1, f2, f3, f4, f5]:
         assert fld == Field.from_field(fld)
+        assert fld is not Field.from_field(fld)
 
 
 def test_repr_field():
     f1 = Field(default=True)
     f2 = Field(default=False)
     f3 = Field(default_factory=list)
     f4 = Field(default=True, type=bool)
@@ -121,14 +122,34 @@
     assert repr(f1) == f1_repr
     assert repr(f2) == f2_repr
     assert repr(f3) == f3_repr
     assert repr(f4) == f4_repr
     assert repr(f5) == f5_repr
 
 
+def test_frozen_field():
+    # UNDER TESTING FIELD SHOULD BE FROZEN
+    f = Field(default=True)
+
+    attr_changes = {
+        "default": False,
+        "default_factory": list,
+        "type": bool,
+        "doc": "This should fail",
+    }
+
+    for k, v in attr_changes.items():
+        with pytest.raises(TypeError):
+            setattr(f, k, v)
+
+    for k in attr_changes:
+        with pytest.raises(TypeError):
+            delattr(f, k)
+
+
 def test_slot_gatherer_success():
 
     fields = {
         "a": Field(default=1),
         "b": Field(default=2),
         "c": Field(default_factory=list, doc="a list"),
         "d": Field(type=str)
@@ -275,14 +296,15 @@
     assert "__eq__" not in SlotClass.__dict__
 
 
 def test_fieldclass():
     @fieldclass
     class NewField(Field):
         __slots__ = SlotFields(serialize=True)
+        serialize: bool
 
     f = NewField()
 
     assert f.default is NOTHING
     assert f.default_factory is NOTHING
     assert f.type is NOTHING
     assert f.doc is None
@@ -294,14 +316,46 @@
     assert f2.serialize is False
 
     with pytest.raises(TypeError):
         # All arguments are keyword only in fieldclasses
         NewField(42)
 
 
+def test_fieldclass_frozen():
+    @fieldclass(frozen=True)
+    class NewField(Field):
+        __slots__ = SlotFields(serialize=True)
+        serialize: bool
+
+    f = NewField()
+
+    attr_changes = {
+        "default": False,
+        "default_factory": list,
+        "type": bool,
+        "doc": "This should fail",
+        "serialize": False,
+    }
+
+    for k, v in attr_changes.items():
+        with pytest.raises(TypeError):
+            setattr(f, k, v)
+
+    for k in attr_changes:
+        with pytest.raises(TypeError):
+            delattr(f, k)
+
+    # Even slotted fields raise TypeError as setattr happens first
+    with pytest.raises(TypeError):
+        setattr(f, "new_attribute", False)
+
+    with pytest.raises(TypeError):
+        delattr(f, "new_attribute")
+
+
 def test_builder_noclass():
     mini_slotclass = builder(gatherer=slot_gatherer, methods={init_desc})
 
     @mini_slotclass
     class SlotClass:
         __slots__ = SlotFields(
             a=Field(),
```

