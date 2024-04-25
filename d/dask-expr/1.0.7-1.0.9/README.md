# Comparing `tmp/dask-expr-1.0.7.tar.gz` & `tmp/dask-expr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-expr-1.0.7.tar", last modified: Tue Apr  2 15:39:06 2024, max compression
+gzip compressed data, was "dask-expr-1.0.9.tar", last modified: Tue Apr  2 18:01:21 2024, max compression
```

## Comparing `dask-expr-1.0.7.tar` & `dask-expr-1.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 15:39:06.886156 dask-expr-1.0.7/
--rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-08-02 08:54:32.000000 dask-expr-1.0.7/LICENSE.txt
--rw-r--r--   0 patrick    (502) staff       (20)     2426 2024-04-02 15:39:06.886080 dask-expr-1.0.7/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)     1358 2024-03-14 18:38:28.000000 dask-expr-1.0.7/README.md
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 15:39:06.886536 dask-expr-1.0.7/dask_expr/
--rw-r--r--   0 patrick    (502) staff       (20)      714 2024-03-15 18:34:20.000000 dask-expr-1.0.7/dask_expr/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)     3495 2024-02-06 10:39:38.000000 dask-expr-1.0.7/dask_expr/_accessor.py
--rw-r--r--   0 patrick    (502) staff       (20)     3089 2024-03-02 13:10:24.000000 dask-expr-1.0.7/dask_expr/_backends.py
--rw-r--r--   0 patrick    (502) staff       (20)     5913 2024-01-10 12:42:12.000000 dask-expr-1.0.7/dask_expr/_categorical.py
--rw-r--r--   0 patrick    (502) staff       (20)   201017 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/_collection.py
--rw-r--r--   0 patrick    (502) staff       (20)    12014 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/_concat.py
--rw-r--r--   0 patrick    (502) staff       (20)    23241 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/_core.py
--rw-r--r--   0 patrick    (502) staff       (20)     3402 2024-02-24 11:18:02.000000 dask-expr-1.0.7/dask_expr/_cumulative.py
--rw-r--r--   0 patrick    (502) staff       (20)     1423 2023-12-13 22:55:14.000000 dask-expr-1.0.7/dask_expr/_datetime.py
--rw-r--r--   0 patrick    (502) staff       (20)     3125 2024-01-05 09:26:35.000000 dask-expr-1.0.7/dask_expr/_describe.py
--rw-r--r--   0 patrick    (502) staff       (20)      123 2024-02-06 10:39:38.000000 dask-expr-1.0.7/dask_expr/_dispatch.py
--rw-r--r--   0 patrick    (502) staff       (20)     5500 2024-01-12 09:44:45.000000 dask-expr-1.0.7/dask_expr/_dummies.py
--rw-r--r--   0 patrick    (502) staff       (20)   119003 2024-04-02 15:22:44.000000 dask-expr-1.0.7/dask_expr/_expr.py
--rw-r--r--   0 patrick    (502) staff       (20)    66714 2024-04-02 15:22:44.000000 dask-expr-1.0.7/dask_expr/_groupby.py
--rw-r--r--   0 patrick    (502) staff       (20)      110 2023-10-16 12:23:51.000000 dask-expr-1.0.7/dask_expr/_helpers.py
--rw-r--r--   0 patrick    (502) staff       (20)    11390 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/_indexing.py
--rw-r--r--   0 patrick    (502) staff       (20)    30030 2024-04-02 15:22:44.000000 dask-expr-1.0.7/dask_expr/_merge.py
--rw-r--r--   0 patrick    (502) staff       (20)    11712 2024-03-06 13:47:43.000000 dask-expr-1.0.7/dask_expr/_merge_asof.py
--rw-r--r--   0 patrick    (502) staff       (20)     3903 2023-12-19 16:33:28.000000 dask-expr-1.0.7/dask_expr/_quantile.py
--rw-r--r--   0 patrick    (502) staff       (20)     2491 2023-12-13 22:55:14.000000 dask-expr-1.0.7/dask_expr/_quantiles.py
--rw-r--r--   0 patrick    (502) staff       (20)    43097 2024-04-02 15:23:05.000000 dask-expr-1.0.7/dask_expr/_reductions.py
--rw-r--r--   0 patrick    (502) staff       (20)    16908 2024-04-02 15:22:44.000000 dask-expr-1.0.7/dask_expr/_repartition.py
--rw-r--r--   0 patrick    (502) staff       (20)     7020 2024-02-06 10:39:38.000000 dask-expr-1.0.7/dask_expr/_resample.py
--rw-r--r--   0 patrick    (502) staff       (20)     8765 2024-03-06 13:47:43.000000 dask-expr-1.0.7/dask_expr/_rolling.py
--rw-r--r--   0 patrick    (502) staff       (20)    43784 2024-04-02 15:22:44.000000 dask-expr-1.0.7/dask_expr/_shuffle.py
--rw-r--r--   0 patrick    (502) staff       (20)     5022 2024-03-14 18:38:28.000000 dask-expr-1.0.7/dask_expr/_str_accessor.py
--rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-1.0.7/dask_expr/_typing.py
--rw-r--r--   0 patrick    (502) staff       (20)     6825 2024-03-14 18:38:28.000000 dask-expr-1.0.7/dask_expr/_util.py
--rw-r--r--   0 patrick    (502) staff       (20)      497 2024-04-02 15:39:06.886568 dask-expr-1.0.7/dask_expr/_version.py
--rw-r--r--   0 patrick    (502) staff       (20)     6636 2024-03-02 13:39:21.000000 dask-expr-1.0.7/dask_expr/datasets.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 15:39:06.882030 dask-expr-1.0.7/dask_expr/diagnostics/
--rw-r--r--   0 patrick    (502) staff       (20)      136 2024-03-26 18:32:00.000000 dask-expr-1.0.7/dask_expr/diagnostics/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)     5125 2024-03-26 18:32:00.000000 dask-expr-1.0.7/dask_expr/diagnostics/_analyze.py
--rw-r--r--   0 patrick    (502) staff       (20)     3943 2024-03-26 18:32:00.000000 dask-expr-1.0.7/dask_expr/diagnostics/_analyze_plugin.py
--rw-r--r--   0 patrick    (502) staff       (20)     2614 2024-02-24 14:19:27.000000 dask-expr-1.0.7/dask_expr/diagnostics/_explain.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 15:39:06.885538 dask-expr-1.0.7/dask_expr/io/
--rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-1.0.7/dask_expr/io/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)     3938 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/_delayed.py
--rw-r--r--   0 patrick    (502) staff       (20)      171 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/bag.py
--rw-r--r--   0 patrick    (502) staff       (20)     3947 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/csv.py
--rw-r--r--   0 patrick    (502) staff       (20)     1056 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/hdf.py
--rw-r--r--   0 patrick    (502) staff       (20)    19484 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/io.py
--rw-r--r--   0 patrick    (502) staff       (20)     1657 2024-04-02 15:36:59.000000 dask-expr-1.0.7/dask_expr/io/json.py
--rw-r--r--   0 patrick    (502) staff       (20)     1076 2024-04-02 15:36:59.000000 dask-expr-1.0.7/dask_expr/io/orc.py
--rw-r--r--   0 patrick    (502) staff       (20)    62734 2024-04-02 15:36:59.000000 dask-expr-1.0.7/dask_expr/io/parquet.py
--rw-r--r--   0 patrick    (502) staff       (20)       90 2024-01-10 12:42:12.000000 dask-expr-1.0.7/dask_expr/io/records.py
--rw-r--r--   0 patrick    (502) staff       (20)     2272 2024-03-26 18:32:06.000000 dask-expr-1.0.7/dask_expr/io/sql.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 15:39:06.885833 dask-expr-1.0.7/dask_expr.egg-info/
--rw-r--r--   0 patrick    (502) staff       (20)     2426 2024-04-02 15:39:06.000000 dask-expr-1.0.7/dask_expr.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)     1296 2024-04-02 15:39:06.000000 dask-expr-1.0.7/dask_expr.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (502) staff       (20)        1 2024-04-02 15:39:06.000000 dask-expr-1.0.7/dask_expr.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (502) staff       (20)       40 2024-04-02 15:39:06.000000 dask-expr-1.0.7/dask_expr.egg-info/requires.txt
--rw-r--r--   0 patrick    (502) staff       (20)       10 2024-04-02 15:39:06.000000 dask-expr-1.0.7/dask_expr.egg-info/top_level.txt
--rw-r--r--   0 patrick    (502) staff       (20)     2195 2024-04-02 15:36:59.000000 dask-expr-1.0.7/pyproject.toml
--rw-r--r--   0 patrick    (502) staff       (20)      230 2024-04-02 15:39:06.886412 dask-expr-1.0.7/setup.cfg
--rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-08-04 10:47:33.000000 dask-expr-1.0.7/setup.py
--rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-1.0.7/versioneer.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 18:01:21.384607 dask-expr-1.0.9/
+-rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-08-02 08:54:32.000000 dask-expr-1.0.9/LICENSE.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     2426 2024-04-02 18:01:21.384549 dask-expr-1.0.9/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)     1358 2024-03-14 18:38:28.000000 dask-expr-1.0.9/README.md
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 18:01:21.385131 dask-expr-1.0.9/dask_expr/
+-rw-r--r--   0 patrick    (502) staff       (20)      714 2024-03-15 18:34:20.000000 dask-expr-1.0.9/dask_expr/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3495 2024-02-06 10:39:38.000000 dask-expr-1.0.9/dask_expr/_accessor.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3089 2024-03-02 13:10:24.000000 dask-expr-1.0.9/dask_expr/_backends.py
+-rw-r--r--   0 patrick    (502) staff       (20)     5913 2024-01-10 12:42:12.000000 dask-expr-1.0.9/dask_expr/_categorical.py
+-rw-r--r--   0 patrick    (502) staff       (20)   201017 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/_collection.py
+-rw-r--r--   0 patrick    (502) staff       (20)    12014 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/_concat.py
+-rw-r--r--   0 patrick    (502) staff       (20)    23241 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/_core.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3402 2024-02-24 11:18:02.000000 dask-expr-1.0.9/dask_expr/_cumulative.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1423 2023-12-13 22:55:14.000000 dask-expr-1.0.9/dask_expr/_datetime.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3125 2024-01-05 09:26:35.000000 dask-expr-1.0.9/dask_expr/_describe.py
+-rw-r--r--   0 patrick    (502) staff       (20)      123 2024-02-06 10:39:38.000000 dask-expr-1.0.9/dask_expr/_dispatch.py
+-rw-r--r--   0 patrick    (502) staff       (20)     5500 2024-01-12 09:44:45.000000 dask-expr-1.0.9/dask_expr/_dummies.py
+-rw-r--r--   0 patrick    (502) staff       (20)   119003 2024-04-02 15:22:44.000000 dask-expr-1.0.9/dask_expr/_expr.py
+-rw-r--r--   0 patrick    (502) staff       (20)    67239 2024-04-02 17:51:46.000000 dask-expr-1.0.9/dask_expr/_groupby.py
+-rw-r--r--   0 patrick    (502) staff       (20)      110 2023-10-16 12:23:51.000000 dask-expr-1.0.9/dask_expr/_helpers.py
+-rw-r--r--   0 patrick    (502) staff       (20)    11390 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/_indexing.py
+-rw-r--r--   0 patrick    (502) staff       (20)    30030 2024-04-02 15:22:44.000000 dask-expr-1.0.9/dask_expr/_merge.py
+-rw-r--r--   0 patrick    (502) staff       (20)    11712 2024-03-06 13:47:43.000000 dask-expr-1.0.9/dask_expr/_merge_asof.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3903 2023-12-19 16:33:28.000000 dask-expr-1.0.9/dask_expr/_quantile.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2491 2023-12-13 22:55:14.000000 dask-expr-1.0.9/dask_expr/_quantiles.py
+-rw-r--r--   0 patrick    (502) staff       (20)    43097 2024-04-02 15:23:05.000000 dask-expr-1.0.9/dask_expr/_reductions.py
+-rw-r--r--   0 patrick    (502) staff       (20)    16908 2024-04-02 15:22:44.000000 dask-expr-1.0.9/dask_expr/_repartition.py
+-rw-r--r--   0 patrick    (502) staff       (20)     7020 2024-02-06 10:39:38.000000 dask-expr-1.0.9/dask_expr/_resample.py
+-rw-r--r--   0 patrick    (502) staff       (20)     8765 2024-03-06 13:47:43.000000 dask-expr-1.0.9/dask_expr/_rolling.py
+-rw-r--r--   0 patrick    (502) staff       (20)    43784 2024-04-02 15:22:44.000000 dask-expr-1.0.9/dask_expr/_shuffle.py
+-rw-r--r--   0 patrick    (502) staff       (20)     5022 2024-03-14 18:38:28.000000 dask-expr-1.0.9/dask_expr/_str_accessor.py
+-rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-1.0.9/dask_expr/_typing.py
+-rw-r--r--   0 patrick    (502) staff       (20)     6825 2024-03-14 18:38:28.000000 dask-expr-1.0.9/dask_expr/_util.py
+-rw-r--r--   0 patrick    (502) staff       (20)      497 2024-04-02 18:01:21.385172 dask-expr-1.0.9/dask_expr/_version.py
+-rw-r--r--   0 patrick    (502) staff       (20)     6636 2024-03-02 13:39:21.000000 dask-expr-1.0.9/dask_expr/datasets.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 18:01:21.380479 dask-expr-1.0.9/dask_expr/diagnostics/
+-rw-r--r--   0 patrick    (502) staff       (20)      136 2024-03-26 18:32:00.000000 dask-expr-1.0.9/dask_expr/diagnostics/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     5125 2024-03-26 18:32:00.000000 dask-expr-1.0.9/dask_expr/diagnostics/_analyze.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3943 2024-03-26 18:32:00.000000 dask-expr-1.0.9/dask_expr/diagnostics/_analyze_plugin.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2614 2024-02-24 14:19:27.000000 dask-expr-1.0.9/dask_expr/diagnostics/_explain.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 18:01:21.384043 dask-expr-1.0.9/dask_expr/io/
+-rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-1.0.9/dask_expr/io/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3938 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/_delayed.py
+-rw-r--r--   0 patrick    (502) staff       (20)      171 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/bag.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3947 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/csv.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1056 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/hdf.py
+-rw-r--r--   0 patrick    (502) staff       (20)    19484 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/io.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1657 2024-04-02 15:36:59.000000 dask-expr-1.0.9/dask_expr/io/json.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1076 2024-04-02 15:36:59.000000 dask-expr-1.0.9/dask_expr/io/orc.py
+-rw-r--r--   0 patrick    (502) staff       (20)    62734 2024-04-02 15:36:59.000000 dask-expr-1.0.9/dask_expr/io/parquet.py
+-rw-r--r--   0 patrick    (502) staff       (20)       90 2024-01-10 12:42:12.000000 dask-expr-1.0.9/dask_expr/io/records.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2272 2024-03-26 18:32:06.000000 dask-expr-1.0.9/dask_expr/io/sql.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2024-04-02 18:01:21.384318 dask-expr-1.0.9/dask_expr.egg-info/
+-rw-r--r--   0 patrick    (502) staff       (20)     2426 2024-04-02 18:01:21.000000 dask-expr-1.0.9/dask_expr.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)     1296 2024-04-02 18:01:21.000000 dask-expr-1.0.9/dask_expr.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (502) staff       (20)        1 2024-04-02 18:01:21.000000 dask-expr-1.0.9/dask_expr.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       40 2024-04-02 18:01:21.000000 dask-expr-1.0.9/dask_expr.egg-info/requires.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       10 2024-04-02 18:01:21.000000 dask-expr-1.0.9/dask_expr.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     2195 2024-04-02 15:36:59.000000 dask-expr-1.0.9/pyproject.toml
+-rw-r--r--   0 patrick    (502) staff       (20)      230 2024-04-02 18:01:21.384859 dask-expr-1.0.9/setup.cfg
+-rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-08-04 10:47:33.000000 dask-expr-1.0.9/setup.py
+-rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-1.0.9/versioneer.py
```

### Comparing `dask-expr-1.0.7/LICENSE.txt` & `dask-expr-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/PKG-INFO` & `dask-expr-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 1.0.7
+Version: 1.0.9
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-expr-1.0.7/README.md` & `dask-expr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/__init__.py` & `dask-expr-1.0.9/dask_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_accessor.py` & `dask-expr-1.0.9/dask_expr/_accessor.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_backends.py` & `dask-expr-1.0.9/dask_expr/_backends.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_categorical.py` & `dask-expr-1.0.9/dask_expr/_categorical.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_collection.py` & `dask-expr-1.0.9/dask_expr/_collection.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_concat.py` & `dask-expr-1.0.9/dask_expr/_concat.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_core.py` & `dask-expr-1.0.9/dask_expr/_core.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_cumulative.py` & `dask-expr-1.0.9/dask_expr/_cumulative.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_datetime.py` & `dask-expr-1.0.9/dask_expr/_datetime.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_describe.py` & `dask-expr-1.0.9/dask_expr/_describe.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_dummies.py` & `dask-expr-1.0.9/dask_expr/_dummies.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_expr.py` & `dask-expr-1.0.9/dask_expr/_expr.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_groupby.py` & `dask-expr-1.0.9/dask_expr/_groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     _value_counts,
     _value_counts_aggregate,
     _var_agg,
     _var_chunk,
 )
 from dask.dataframe.utils import insert_meta_param_description
 from dask.utils import M, apply, derived_from, is_index_like
+from pandas.core.apply import reconstruct_func, validate_func_kwargs
 
 from dask_expr._collection import FrameBase, Index, Series, new_collection
 from dask_expr._expr import (
     Assign,
     Blockwise,
     Expr,
     MapPartitions,
@@ -1880,34 +1881,44 @@
         )
         return self._postprocess_series_squeeze(result)
 
     @_aggregate_docstring(based_on="pd.core.groupby.DataFrameGroupBy.agg")
     def aggregate(
         self, arg=None, split_every=8, split_out=None, shuffle_method=None, **kwargs
     ):
+        relabeling, order, columns = None, None, None
         if arg is None:
-            raise NotImplementedError("arg=None not supported")
+            if not isinstance(self, SeriesGroupBy):
+                relabeling, arg, columns, order = reconstruct_func(arg, **kwargs)
+            elif isinstance(self, SeriesGroupBy):
+                columns, arg = validate_func_kwargs(kwargs)
+                relabeling = True
 
         if arg == "size":
             return self.size()
 
-        return new_collection(
+        result = new_collection(
             GroupbyAggregation(
                 self.obj.expr,
                 arg,
                 self.observed,
                 self.dropna,
                 split_every,
                 split_out,
                 self.sort,
                 shuffle_method,
                 self._slice,
                 *self.by,
             )
         )
+        if relabeling and result is not None:
+            if order is not None:
+                result = result.iloc[:, order]
+            result.columns = columns
+        return result
 
     def agg(self, *args, **kwargs):
         return self.aggregate(*args, **kwargs)
 
     def _warn_if_no_meta(self, meta):
         if meta is no_default:
             msg = (
```

### Comparing `dask-expr-1.0.7/dask_expr/_indexing.py` & `dask-expr-1.0.9/dask_expr/_indexing.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_merge.py` & `dask-expr-1.0.9/dask_expr/_merge.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_merge_asof.py` & `dask-expr-1.0.9/dask_expr/_merge_asof.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_quantile.py` & `dask-expr-1.0.9/dask_expr/_quantile.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_quantiles.py` & `dask-expr-1.0.9/dask_expr/_quantiles.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_reductions.py` & `dask-expr-1.0.9/dask_expr/_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_repartition.py` & `dask-expr-1.0.9/dask_expr/_repartition.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_resample.py` & `dask-expr-1.0.9/dask_expr/_resample.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_rolling.py` & `dask-expr-1.0.9/dask_expr/_rolling.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_shuffle.py` & `dask-expr-1.0.9/dask_expr/_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_str_accessor.py` & `dask-expr-1.0.9/dask_expr/_str_accessor.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/_util.py` & `dask-expr-1.0.9/dask_expr/_util.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/datasets.py` & `dask-expr-1.0.9/dask_expr/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/diagnostics/_analyze.py` & `dask-expr-1.0.9/dask_expr/diagnostics/_analyze.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/diagnostics/_analyze_plugin.py` & `dask-expr-1.0.9/dask_expr/diagnostics/_analyze_plugin.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/diagnostics/_explain.py` & `dask-expr-1.0.9/dask_expr/diagnostics/_explain.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/_delayed.py` & `dask-expr-1.0.9/dask_expr/io/_delayed.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/csv.py` & `dask-expr-1.0.9/dask_expr/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/hdf.py` & `dask-expr-1.0.9/dask_expr/io/hdf.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/io.py` & `dask-expr-1.0.9/dask_expr/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/json.py` & `dask-expr-1.0.9/dask_expr/io/json.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/orc.py` & `dask-expr-1.0.9/dask_expr/io/orc.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/parquet.py` & `dask-expr-1.0.9/dask_expr/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr/io/sql.py` & `dask-expr-1.0.9/dask_expr/io/sql.py`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/dask_expr.egg-info/PKG-INFO` & `dask-expr-1.0.9/dask_expr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 1.0.7
+Version: 1.0.9
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-expr-1.0.7/dask_expr.egg-info/SOURCES.txt` & `dask-expr-1.0.9/dask_expr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/pyproject.toml` & `dask-expr-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-expr-1.0.7/versioneer.py` & `dask-expr-1.0.9/versioneer.py`

 * *Files identical despite different names*

