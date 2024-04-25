# Comparing `tmp/utipy-1.0.1.tar.gz` & `tmp/utipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utipy-1.0.1.tar", max compression
+gzip compressed data, was "utipy-1.0.2.tar", max compression
```

## Comparing `utipy-1.0.1.tar` & `utipy-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rwxr-xr-x   0        0        0     1075 2023-03-17 05:50:40.577416 utipy-1.0.1/LICENSE
--rw-r--r--   0        0        0     2578 2023-03-16 08:36:22.424392 utipy-1.0.1/README.md
--rw-r--r--   0        0        0      733 2023-03-17 05:49:49.881141 utipy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      976 2023-03-17 05:55:26.795179 utipy-1.0.1/utipy/__init__.py
--rw-r--r--   0        0        0      120 2022-02-11 16:02:18.395530 utipy-1.0.1/utipy/array/__init__.py
--rw-r--r--   0        0        0     1423 2023-03-16 08:18:33.916338 utipy-1.0.1/utipy/array/blend.py
--rw-r--r--   0        0        0     1767 2022-03-09 14:34:44.935858 utipy-1.0.1/utipy/array/nan_stats.py
--rw-r--r--   0        0        0     3719 2023-03-16 07:36:47.523525 utipy-1.0.1/utipy/array/window.py
--rw-r--r--   0        0        0     1152 2022-02-16 12:25:40.773592 utipy-1.0.1/utipy/array/windowed_reverse.py
--rw-r--r--   0        0        0      144 2022-02-11 16:59:22.154646 utipy-1.0.1/utipy/groups/__init__.py
--rw-r--r--   0        0        0     2374 2023-03-16 07:39:49.954904 utipy-1.0.1/utipy/groups/fold.py
--rw-r--r--   0        0        0     1196 2023-03-16 07:42:28.772441 utipy-1.0.1/utipy/groups/group.py
--rw-r--r--   0        0        0     1105 2023-03-16 07:41:11.500065 utipy-1.0.1/utipy/groups/group_uniques.py
--rw-r--r--   0        0        0       81 2022-02-11 16:19:37.542024 utipy-1.0.1/utipy/groups/methods/__init__.py
--rw-r--r--   0        0        0     2593 2022-03-30 15:50:52.548043 utipy-1.0.1/utipy/groups/methods/l_sizes.py
--rw-r--r--   0        0        0      716 2022-02-11 17:02:39.719083 utipy-1.0.1/utipy/groups/methods/n_dist.py
--rw-r--r--   0        0        0     2356 2023-03-16 07:44:32.504985 utipy-1.0.1/utipy/groups/partition.py
--rw-r--r--   0        0        0       46 2022-02-11 16:59:08.053991 utipy-1.0.1/utipy/measures/__init__.py
--rw-r--r--   0        0        0      177 2022-02-15 11:34:07.116109 utipy-1.0.1/utipy/measures/iqr.py
--rw-r--r--   0        0        0      226 2022-02-11 16:58:19.140171 utipy-1.0.1/utipy/pandas/__init__.py
--rw-r--r--   0        0        0     5134 2023-03-16 07:47:47.239763 utipy-1.0.1/utipy/pandas/distort.py
--rw-r--r--   0        0        0     5409 2023-03-16 08:19:37.688838 utipy-1.0.1/utipy/pandas/drop.py
--rw-r--r--   0        0        0     4872 2023-03-16 08:21:33.401661 utipy-1.0.1/utipy/pandas/makes_up.py
--rw-r--r--   0        0        0      502 2023-03-16 08:05:31.766579 utipy-1.0.1/utipy/pandas/move_column_inplace.py
--rw-r--r--   0        0        0     3572 2023-03-16 08:21:25.879843 utipy-1.0.1/utipy/pandas/polynomializer.py
--rw-r--r--   0        0        0     2178 2023-03-16 08:15:21.147759 utipy-1.0.1/utipy/pandas/resemble.py
--rw-r--r--   0        0        0     1340 2023-03-16 08:21:29.812641 utipy-1.0.1/utipy/pandas/subset_by_levels.py
--rw-r--r--   0        0        0       68 2022-07-07 15:01:15.515033 utipy-1.0.1/utipy/path/__init__.py
--rw-r--r--   0        0        0    30656 2023-03-03 07:55:53.704264 utipy-1.0.1/utipy/path/iopaths.py
--rw-r--r--   0        0        0     4407 2022-06-30 11:23:32.798235 utipy-1.0.1/utipy/path/mk_rm_dir.py
--rw-r--r--   0        0        0    12586 2023-01-17 21:58:42.348504 utipy-1.0.1/utipy/path/prepare_paths.py
--rw-r--r--   0        0        0       93 2022-06-14 14:12:30.559956 utipy-1.0.1/utipy/string/__init__.py
--rw-r--r--   0        0        0     2231 2023-03-16 08:22:51.115525 utipy-1.0.1/utipy/string/letter_strings.py
--rw-r--r--   0        0        0      982 2023-03-16 08:23:17.187262 utipy-1.0.1/utipy/string/random_strings.py
--rw-r--r--   0        0        0      109 2022-02-11 17:21:08.042971 utipy-1.0.1/utipy/time/__init__.py
--rw-r--r--   0        0        0     1320 2022-02-15 10:22:33.178533 utipy-1.0.1/utipy/time/format_time.py
--rw-r--r--   0        0        0     3566 2023-03-16 08:24:26.040778 utipy-1.0.1/utipy/time/timer.py
--rw-r--r--   0        0        0    12664 2023-03-16 08:25:44.001312 utipy-1.0.1/utipy/time/timestamps.py
--rw-r--r--   0        0        0      162 2023-03-15 13:55:12.350940 utipy-1.0.1/utipy/utils/__init__.py
--rw-r--r--   0        0        0      654 2023-03-16 08:26:25.869729 utipy-1.0.1/utipy/utils/check_instance.py
--rw-r--r--   0        0        0      820 2023-03-16 08:27:54.482169 utipy-1.0.1/utipy/utils/convert_to_df.py
--rw-r--r--   0        0        0     1152 2023-03-16 08:29:36.900562 utipy-1.0.1/utipy/utils/convert_to_type.py
--rw-r--r--   0        0        0      450 2023-03-16 08:12:21.640992 utipy-1.0.1/utipy/utils/extended_describe.py
--rw-r--r--   0        0        0    11892 2023-03-16 08:31:44.096804 utipy-1.0.1/utipy/utils/messenger.py
--rw-r--r--   0        0        0     1023 2022-02-16 11:57:25.655758 utipy-1.0.1/utipy/utils/step_idx.py
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 utipy-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1075 2023-03-17 05:50:40.577416 utipy-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2578 2023-03-16 08:36:22.424392 utipy-1.0.2/README.md
+-rw-r--r--   0        0        0      760 2024-04-25 19:44:04.530362 utipy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      976 2023-03-17 05:55:26.795179 utipy-1.0.2/utipy/__init__.py
+-rw-r--r--   0        0        0      120 2022-02-11 16:02:18.395530 utipy-1.0.2/utipy/array/__init__.py
+-rw-r--r--   0        0        0     1423 2023-03-16 08:18:33.916338 utipy-1.0.2/utipy/array/blend.py
+-rw-r--r--   0        0        0     1767 2022-03-09 14:34:44.935858 utipy-1.0.2/utipy/array/nan_stats.py
+-rw-r--r--   0        0        0     3719 2023-03-16 07:36:47.523525 utipy-1.0.2/utipy/array/window.py
+-rw-r--r--   0        0        0     1152 2022-02-16 12:25:40.773592 utipy-1.0.2/utipy/array/windowed_reverse.py
+-rw-r--r--   0        0        0      144 2022-02-11 16:59:22.154646 utipy-1.0.2/utipy/groups/__init__.py
+-rw-r--r--   0        0        0     2374 2023-03-16 07:39:49.954904 utipy-1.0.2/utipy/groups/fold.py
+-rw-r--r--   0        0        0     1196 2023-03-16 07:42:28.772441 utipy-1.0.2/utipy/groups/group.py
+-rw-r--r--   0        0        0     1105 2023-03-16 07:41:11.500065 utipy-1.0.2/utipy/groups/group_uniques.py
+-rw-r--r--   0        0        0       81 2022-02-11 16:19:37.542024 utipy-1.0.2/utipy/groups/methods/__init__.py
+-rw-r--r--   0        0        0     2593 2022-03-30 15:50:52.548043 utipy-1.0.2/utipy/groups/methods/l_sizes.py
+-rw-r--r--   0        0        0      716 2022-02-11 17:02:39.719083 utipy-1.0.2/utipy/groups/methods/n_dist.py
+-rw-r--r--   0        0        0     2356 2023-03-16 07:44:32.504985 utipy-1.0.2/utipy/groups/partition.py
+-rw-r--r--   0        0        0       46 2022-02-11 16:59:08.053991 utipy-1.0.2/utipy/measures/__init__.py
+-rw-r--r--   0        0        0      177 2022-02-15 11:34:07.116109 utipy-1.0.2/utipy/measures/iqr.py
+-rw-r--r--   0        0        0      226 2022-02-11 16:58:19.140171 utipy-1.0.2/utipy/pandas/__init__.py
+-rw-r--r--   0        0        0     5134 2023-03-16 07:47:47.239763 utipy-1.0.2/utipy/pandas/distort.py
+-rw-r--r--   0        0        0     5409 2023-03-16 08:19:37.688838 utipy-1.0.2/utipy/pandas/drop.py
+-rw-r--r--   0        0        0     4872 2023-03-16 08:21:33.401661 utipy-1.0.2/utipy/pandas/makes_up.py
+-rw-r--r--   0        0        0      502 2023-03-16 08:05:31.766579 utipy-1.0.2/utipy/pandas/move_column_inplace.py
+-rw-r--r--   0        0        0     3572 2023-03-16 08:21:25.879843 utipy-1.0.2/utipy/pandas/polynomializer.py
+-rw-r--r--   0        0        0     2178 2023-03-16 08:15:21.147759 utipy-1.0.2/utipy/pandas/resemble.py
+-rw-r--r--   0        0        0     1340 2023-03-16 08:21:29.812641 utipy-1.0.2/utipy/pandas/subset_by_levels.py
+-rw-r--r--   0        0        0       68 2022-07-07 15:01:15.515033 utipy-1.0.2/utipy/path/__init__.py
+-rw-r--r--   0        0        0    30425 2024-04-17 11:53:27.935813 utipy-1.0.2/utipy/path/iopaths.py
+-rw-r--r--   0        0        0     4407 2022-06-30 11:23:32.798235 utipy-1.0.2/utipy/path/mk_rm_dir.py
+-rw-r--r--   0        0        0    12586 2023-01-17 21:58:42.348504 utipy-1.0.2/utipy/path/prepare_paths.py
+-rw-r--r--   0        0        0       93 2022-06-14 14:12:30.559956 utipy-1.0.2/utipy/string/__init__.py
+-rw-r--r--   0        0        0     2231 2023-03-16 08:22:51.115525 utipy-1.0.2/utipy/string/letter_strings.py
+-rw-r--r--   0        0        0      982 2023-03-16 08:23:17.187262 utipy-1.0.2/utipy/string/random_strings.py
+-rw-r--r--   0        0        0      109 2022-02-11 17:21:08.042971 utipy-1.0.2/utipy/time/__init__.py
+-rw-r--r--   0        0        0     1320 2022-02-15 10:22:33.178533 utipy-1.0.2/utipy/time/format_time.py
+-rw-r--r--   0        0        0     3566 2023-03-16 08:24:26.040778 utipy-1.0.2/utipy/time/timer.py
+-rw-r--r--   0        0        0    12664 2023-03-16 08:25:44.001312 utipy-1.0.2/utipy/time/timestamps.py
+-rw-r--r--   0        0        0      162 2023-03-15 13:55:12.350940 utipy-1.0.2/utipy/utils/__init__.py
+-rw-r--r--   0        0        0      654 2023-03-16 08:26:25.869729 utipy-1.0.2/utipy/utils/check_instance.py
+-rw-r--r--   0        0        0      820 2023-03-16 08:27:54.482169 utipy-1.0.2/utipy/utils/convert_to_df.py
+-rw-r--r--   0        0        0     1152 2023-03-16 08:29:36.900562 utipy-1.0.2/utipy/utils/convert_to_type.py
+-rw-r--r--   0        0        0      450 2023-03-16 08:12:21.640992 utipy-1.0.2/utipy/utils/extended_describe.py
+-rw-r--r--   0        0        0    12391 2023-04-24 11:10:54.796673 utipy-1.0.2/utipy/utils/messenger.py
+-rw-r--r--   0        0        0     1023 2022-02-16 11:57:25.655758 utipy-1.0.2/utipy/utils/step_idx.py
+-rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 utipy-1.0.2/PKG-INFO
```

### Comparing `utipy-1.0.1/LICENSE` & `utipy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/README.md` & `utipy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/pyproject.toml` & `utipy-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utipy"
-version = "1.0.1"
+version = "1.0.2"
 description = "Utility functions for python"
 authors = ["Ludvig Renbo Olsen <mail@ludvigolsen.dk>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ludvigolsen/utipy"
 keywords = [
     "pandas",
@@ -12,27 +12,29 @@
     "array",
     "ndarray",
     "groups",
     "folds",
     "kfold",
     "partitioning",
     "utilities",
+    "logging",
+    "time",
     "tools",
     "rolling",
     "windows",
     "time"
 ]
 
 [tool.poetry.urls]
 issues = "https://github.com/ludvigolsen/utipy/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pandas = "^1.5.3"
-numpy = "^1.24.2"
+pandas = "^1.3.5"
+numpy = "^1.21.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `utipy-1.0.1/utipy/__init__.py` & `utipy-1.0.2/utipy/__init__.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/array/blend.py` & `utipy-1.0.2/utipy/array/blend.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/array/nan_stats.py` & `utipy-1.0.2/utipy/array/nan_stats.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/array/window.py` & `utipy-1.0.2/utipy/array/window.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/array/windowed_reverse.py` & `utipy-1.0.2/utipy/array/windowed_reverse.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/fold.py` & `utipy-1.0.2/utipy/groups/fold.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/group.py` & `utipy-1.0.2/utipy/groups/group.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/group_uniques.py` & `utipy-1.0.2/utipy/groups/group_uniques.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/methods/l_sizes.py` & `utipy-1.0.2/utipy/groups/methods/l_sizes.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/methods/n_dist.py` & `utipy-1.0.2/utipy/groups/methods/n_dist.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/groups/partition.py` & `utipy-1.0.2/utipy/groups/partition.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/distort.py` & `utipy-1.0.2/utipy/pandas/distort.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/drop.py` & `utipy-1.0.2/utipy/pandas/drop.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/makes_up.py` & `utipy-1.0.2/utipy/pandas/makes_up.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/polynomializer.py` & `utipy-1.0.2/utipy/pandas/polynomializer.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/resemble.py` & `utipy-1.0.2/utipy/pandas/resemble.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/pandas/subset_by_levels.py` & `utipy-1.0.2/utipy/pandas/subset_by_levels.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/path/iopaths.py` & `utipy-1.0.2/utipy/path/iopaths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-
 import os
 import pathlib
 from typing import Callable, Dict, List, Optional, Union
 
 from utipy.path.mk_rm_dir import mk_dir, rm_dir as remove_dir
 from utipy.path.prepare_paths import prepare_in_out_paths
 from utipy.utils.messenger import Messenger
 
 
 # TODO Add tests
 # TODO Allow keys to have a list of paths?
 # TODO Allow checking if dirs are empty (e.g. checkpoints)
 
+
 class IOPaths:
 
     COLLECTION_NAMES = [
         "in_files",
         "in_dirs",
         "out_files",
         "out_dirs",
         "tmp_files",
-        "tmp_dirs"
+        "tmp_dirs",
     ]
 
-    def __init__(self,
-                 in_files: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 in_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 out_files: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 out_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 tmp_files: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 tmp_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
-                 allow_none: bool = False,
-                 allow_overwriting: bool = True,
-                 allow_duplicates_in: List[str] = [
-                     "in_dirs", "out_dirs", "tmp_dirs"],
-                 disallowed_nestings: List[tuple] = [
-                     ("in_files", "tmp_dirs"),
-                     ("out_files", "tmp_dirs"),
-                     ("in_dirs", "tmp_dirs"),
-                     ("out_dirs", "tmp_dirs")
-                 ],
-                 print_note: bool = "",
-                 ) -> None:
+    def __init__(
+        self,
+        in_files: Dict[str, Union[str, pathlib.PurePath]] = None,
+        in_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
+        out_files: Dict[str, Union[str, pathlib.PurePath]] = None,
+        out_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
+        tmp_files: Dict[str, Union[str, pathlib.PurePath]] = None,
+        tmp_dirs: Dict[str, Union[str, pathlib.PurePath]] = None,
+        allow_none: bool = False,
+        allow_overwriting: bool = True,
+        allow_duplicates_in: List[str] = ["in_dirs", "out_dirs", "tmp_dirs"],
+        disallowed_nestings: List[tuple] = [
+            ("in_files", "tmp_dirs"),
+            ("out_files", "tmp_dirs"),
+            ("in_dirs", "tmp_dirs"),
+            ("out_dirs", "tmp_dirs"),
+        ],
+        print_note: bool = "",
+    ) -> None:
         """
         Collection of path collections for keeping track of in- and output paths,
         be it files or directories. Has relevant checks, such as duplication and
-        existence, and allows printing a summary of the paths. Paths are converted to 
+        existence, and allows printing a summary of the paths. Paths are converted to
         `pathlib.Path` objects and missing directories can be created.
 
-        Note: Even when `allow_overwriting` is enabled, 
+        Note: Even when `allow_overwriting` is enabled,
         `in_files` and `out_files` cannot contain the same paths.
 
         Keys must be unique across the path dictionaries.
 
         Parameters
         ----------
         in_files : dict
             Dict with named paths to input files, mapping `(argument) name -> input filepath`.
-            A path can also be "-" when streaming input. 
+            A path can also be "-" when streaming input.
             This value will remain a string and will not be checked
             for duplication, existence, etc.
         in_dirs : dict
             Dict with named paths to input directories, mapping `(argument) name -> input directory path`.
         out_files : dict
             Dict with named paths to output files, mapping `(argument) name -> output filepath`.
         out_dirs : dict
@@ -75,17 +75,17 @@
             in which case they will be ignored.
         allow_overwriting : bool
             Whether to allow `out_files` paths to already exist.
         allow_duplicates_in : list
             List of collections to allow duplicate paths in. One of:
                 {'in_files', 'in_dirs', 'out_files', 'out_dirs', 'tmp_files', 'tmp_dirs'}.
         disallowed_nestings : list of tuples
-            Pairs of collections where the paths of the first cannot 
+            Pairs of collections where the paths of the first cannot
             be nested inside the paths of the second.
-            By default, the in and out paths cannot be located within 
+            By default, the in and out paths cannot be located within
             the temporary directories, as these might be deleted.
         print_note : string
             String to add to end of `__str__` method.
             That is a suffix added when printing the collection.
 
         Examples
         --------
@@ -120,15 +120,15 @@
 
         Or set multiple at a time to avoid rerunning checks unnecessarily.
 
         >>> paths.set_paths(
         ...     paths={
         ...         "out_file_2": "../dir1/dir2/output/no_dennis.csv"
         ...         "out_file_3": "../dir1/dir2/output/readme.txt"
-        ...     }, 
+        ...     },
         ...     collection="out_files"
         ... )
 
         Create the output directories that do not exist.
 
         >>> paths.mk_output_dirs(collection="out_dirs")
 
@@ -138,15 +138,15 @@
         >>> paths.get_path(name="in_file", as_str=False, raise_on_fail=True)
 
         Remove file from disk.
 
         >>> paths.rm_file(name="in_file")
 
         Update collection with another `IOPaths` collection.
-        The sub collections are dicts, why this is just dict.update() 
+        The sub collections are dicts, why this is just dict.update()
         on each sub collection.
 
         >>> paths.update(other=other_paths)
 
         Find the combinations of keys and paths in the collections of this object
         that are not in the collections of another object.
 
@@ -189,16 +189,15 @@
         Sizes of collections (size: number of paths).
 
         Returns
         -------
         Dict mapping collection name -> number of paths.
         """
         return {
-            coll: self.get_collection_size(coll)
-            for coll in IOPaths.COLLECTION_NAMES
+            coll: self.get_collection_size(coll) for coll in IOPaths.COLLECTION_NAMES
         }
 
     def get_collection_size(self, name: str):
         """
         Get size (number of paths) of a given collection.
 
         Parameters
@@ -240,31 +239,32 @@
 
         See also: `update()`.
 
         Parameters
         ----------
         name : str
             Name of collection to set.
-        collection : dict 
-            Collection of paths as dict, mapping `name -> path`. 
+        collection : dict
+            Collection of paths as dict, mapping `name -> path`.
             Replaces existing dict.
         """
         # NOTE: Avoid internal use
         # as it may cause an infinite loop with
         # `self._prepare_paths()`
         self._set_collection(name=name, coll=collection)
         # Ensure consistency
         self._prepare_paths()
 
     def _set_collection(self, name: str, coll: Union[dict, None]):
         assert isinstance(name, str)
         assert coll is None or isinstance(coll, dict)
         if name not in IOPaths.COLLECTION_NAMES:
             raise ValueError(
-                f"`name` was not one of the allowed collection names: {IOPaths.COLLECTION_NAMES}")
+                f"`name` was not one of the allowed collection names: {IOPaths.COLLECTION_NAMES}"
+            )
         self._collections[name] = coll
 
     def _update_collection(self, paths: dict, collection: str):
         assert isinstance(paths, dict)
         assert isinstance(collection, str)
         self._check_collection_name(collection)
         if self._collections[collection] is None:
@@ -275,15 +275,17 @@
         """
         Get path from its key:
 
         e.g. d['key']
         """
         return self.get_path(name=name)
 
-    def get_path(self, name: str, as_str: bool = False, raise_on_fail: bool = True):
+    def get_path(
+        self, name: str, as_str: bool = False, raise_on_fail: bool = True
+    ) -> Optional[Union[pathlib.Path, str]]:
         """
         Get a path.
 
         Parameters
         ----------
         name : str
             Name of path to get.
@@ -297,37 +299,39 @@
         -------
         `pathlib.Path`, str or `None`
         """
         if name in self.all_paths:
             return self._format_path_out(path=self.all_paths[name], as_str=as_str)
         if raise_on_fail:
             raise ValueError(
-                f"{name} was not a known key in any of the path collections.")
+                f"{name} was not a known key in any of the path collections."
+            )
         return None
 
-    def set_path(self, name: str, path: Union[str, pathlib.PurePath], collection: str) -> None:
+    def set_path(
+        self, name: str, path: Union[str, pathlib.PurePath], collection: str
+    ) -> None:
         """
         Set a path in a collection.
 
         Parameters
         ----------
         name : str
             Name of path for collection dict.
-        path : str or `pathlib.Path` 
+        path : str or `pathlib.Path`
             The path to set.
         collection : str
             Name of collection to set the path in.
             When a name already exist it is overwritten.
         """
         # NOTE: Avoid internal use
         # as it may cause an infinite loop
         assert isinstance(name, str)
         assert isinstance(path, (str, pathlib.PurePath))
-        self._update_collection(
-            paths={name: path}, collection=collection)
+        self._update_collection(paths={name: path}, collection=collection)
 
         # Ensure consistency
         self._prepare_paths()
 
     def set_paths(self, paths: dict, collection: str) -> None:
         """
         Set one or more paths in a collection.
@@ -371,29 +375,29 @@
         """
         [self.rm_path(name=name) for name in names]
 
     def rm_paths_in_dir(
         self,
         dir_path_name: Optional[str] = None,
         dir_path: Optional[Union[str, pathlib.PurePath]] = None,
-        rm_dir_path: bool = True
+        rm_dir_path: bool = True,
     ) -> None:
         """
         Remove paths from collection that are within a directory.
 
         Directory can be specified either as the name of a path in the collections
         or a new path. The directory does not need to exist.
 
         Parameters
         ----------
         dir_path_name : str or `None`
             Name of path in the collections.
         dir_path : str or `pathlib.Path` or `None`
             A path to a directory.
-            No checks are done on this path but it is 
+            No checks are done on this path but it is
             resolved with `pathlib.Path.resolve()`.
         rm_dir_path : bool
             Whether to remove the path to the directory itself.
         """
         if sum([dir_path_name is not None, dir_path is not None]) != 1:
             raise ValueError(
                 "Exactly one of {`dir_path_name`, `dir_path`} should be specified."
@@ -404,18 +408,15 @@
 
         path_names_to_remove = [
             path_key
             for path_key, path_val in self.all_paths.items()
             if dir_path in path_val.resolve().parents
         ]
         if not rm_dir_path:
-            path_names_to_remove = [
-                p for p in path_names_to_remove
-                if p != dir_path
-            ]
+            path_names_to_remove = [p for p in path_names_to_remove if p != dir_path]
         self.rm_paths(names=path_names_to_remove)
 
     def get_collection_name_by_path_name(self, name: str) -> str:
         """
         Get name of the collection a path is in.
 
         Parameters
@@ -434,42 +435,42 @@
             if coll_paths_dict is not None and name in coll_paths_dict:
                 return coll_name
 
     # Handle paths
 
     def check_paths(self):
         """
-        Call path checks manually. 
+        Call path checks manually.
 
-        These checks are automatically called after each mutation with 
-        setter methods, but when overwriting attributes (like check settings) 
+        These checks are automatically called after each mutation with
+        setter methods, but when overwriting attributes (like check settings)
         manually, we may need to call it externally.
 
-        May be meaningful to run after removing files and paths, as this 
+        May be meaningful to run after removing files and paths, as this
         does not rerun the checks.
         """
         # TODO Add better description of the checks
         self._prepare_paths()
 
     def _prepare_paths(self):
         # Prepare paths
         self._collections, self.all_paths = prepare_in_out_paths(
             named_collections=self._collections,
             allow_none=self.allow_none,
             allow_overwriting=self.allow_overwriting,
             allow_duplicates_in=self.allow_duplicates_in,
             disallowed_nestings=self.disallowed_nestings,
             pathlib_out=True,
-            copy=True)
+            copy=True,
+        )
 
     def mk_output_dir(
         self,
         name: str,
-        messenger: Optional[Callable] = Messenger(
-            verbose=True, indent=0, msg_fn=print)
+        messenger: Optional[Callable] = Messenger(verbose=True, indent=0, msg_fn=print),
     ):
         """
         Create non-existing output directory for a given path.
 
         For filepaths, it creates the directory the file is located in.
 
         Parameters
@@ -480,25 +481,20 @@
             A `utipy.Messenger` instance used to print/log/... information.
             When `None`, no printing/logging is performed.
             The messenger determines the messaging function (e.g. `print`)
             and potential indentation.
         """
         path = self.get_path(name=name)
         dir_path = pathlib.Path(path).parent
-        mk_dir(
-            path=dir_path,
-            arg_name=name,
-            messenger=messenger
-        )
+        mk_dir(path=dir_path, arg_name=name, messenger=messenger)
 
     def mk_output_dirs(
         self,
         collection: str = None,
-        messenger: Optional[Callable] = Messenger(
-            verbose=True, indent=0, msg_fn=print)
+        messenger: Optional[Callable] = Messenger(verbose=True, indent=0, msg_fn=print),
     ):
         """
         Create non-existing output directories.
 
         For filepaths, it creates the directory the file is located in.
 
         Parameters
@@ -518,15 +514,16 @@
         mkdirs_for_out_files = True
         mkdirs_for_out_dirs = True
         mkdirs_for_tmp_files = True
         mkdirs_for_tmp_dirs = True
         if collection is not None:
             if collection not in ["out_files", "out_dirs", "tmp_files", "tmp_dirs"]:
                 raise ValueError(
-                    f"`collection` must be one of the output path collections but was {collection}.")
+                    f"`collection` must be one of the output path collections but was {collection}."
+                )
             if collection != "out_files":
                 mkdirs_for_out_files = False
             if collection != "out_dirs":
                 mkdirs_for_out_dirs = False
             if collection != "tmp_files":
                 mkdirs_for_tmp_files = False
             if collection != "tmp_dirs":
@@ -578,92 +575,92 @@
         ----------
         name : str
             Name of path to a file to remove from disk.
         rm_path : bool
             Whether to remove path from path collection.
             NOTE: For files that need to exist (e.g. those in the `in_files` collection),
             leaving the path after removing the file will cause downstream
-            checking of the paths (see `.check_paths()`) will fail 
-            (as we removed the files). Those checks are called as part of 
+            checking of the paths (see `.check_paths()`) will fail
+            (as we removed the files). Those checks are called as part of
             some of the methods.
         raise_on_fail : bool
             Whether to raise an error when the path does not exist.
         """
         path = self[name]
         if path is None:
             raise ValueError(f"Path object for `{name}` was `None`.")
         if not path.is_file():
             if raise_on_fail:
                 raise RuntimeError(
-                    f"Path for `{name}` was not an existing file: {path}")
+                    f"Path for `{name}` was not an existing file: {path}"
+                )
         else:
             os.remove(str(path))
 
         if rm_path:
             self.rm_path(name=name)
 
     def rm_dir(
         self,
         name: str,
         rm_paths: bool = True,
         raise_on_fail: bool = True,
-        messenger: Optional[Callable] = Messenger(
-            verbose=True, indent=0, msg_fn=print)
+        messenger: Optional[Callable] = Messenger(verbose=True, indent=0, msg_fn=print),
     ) -> None:
         """
         Remove a directory from disk.
 
         Parameters
         ----------
         name : str
             Name of path to a directory to remove from disk.
         rm_paths : bool
-            Whether to remove all paths that are within the 
-            removed directory as well as the path to the 
+            Whether to remove all paths that are within the
+            removed directory as well as the path to the
             directory itself.
             NOTE: For files that need to exist (e.g. those in the `in_files` collection),
             leaving the path after removing the file will cause downstream
-            checking of the paths (see `.check_paths()`) will fail 
-            (as we removed the files). Those checks are called as part of 
+            checking of the paths (see `.check_paths()`) will fail
+            (as we removed the files). Those checks are called as part of
             some of the methods.
         raise_on_fail : bool
             Whether to raise an error when the path does not exist.
         messenger : `utipy.Messenger` or None
             A `utipy.Messenger` instance used to print/log/... information.
             When `None`, no printing/logging is performed.
             The messenger determines the messaging function (e.g. `print`)
             and potential indentation.
         """
         path = self[name]
         if path is None:
             raise ValueError(f"Path object for `{name}` was `None`.")
         remove_dir(
             path=path,
-            arg_name=f'{name} path',
+            arg_name=f"{name} path",
             raise_missing=raise_on_fail,
             raise_not_dir=raise_on_fail,
-            messenger=messenger
+            messenger=messenger,
         )
         if rm_paths:
             self.rm_paths_in_dir(dir_path=path, rm_dir_path=True)
 
     def rm_tmp_dirs(
         self,
         rm_paths: bool = True,
         raise_on_fail: bool = True,
-        messenger: Optional[Callable] = Messenger(
-            verbose=True, indent=0, msg_fn=print)) -> None:
+        messenger: Optional[Callable] = Messenger(verbose=True, indent=0, msg_fn=print),
+    ) -> None:
         """
         Remove all temporary directories from disk.
 
         Parameters
         ----------
         rm_paths : bool
-            Whether to remove all paths that are within the 
-            removed directories and the paths to the directories 
+            Whether to remove all paths that are within the
+            removed directories and the paths to the directories
             themselves.
         raise_on_fail : bool
             Whether to raise an error when the path does not exist.
         messenger : `utipy.Messenger` or None
             A `utipy.Messenger` instance used to print/log/... information.
             When `None`, no printing/logging is performed.
             The messenger determines the messaging function (e.g. `print`)
@@ -674,33 +671,29 @@
         # before deleting some of the directories, as that might
         # delete the existing ones
         # (I.e. find the top-level tmp dirs and remove those, and don't
         # try to remove those contained in them)
 
         # Delete each path in `tmp_dirs``
         for path in self.get_collection(name="tmp_dirs").keys():
-            self.rm_dir(
-                name=path,
-                raise_on_fail=raise_on_fail,
-                messenger=messenger
-            )
+            self.rm_dir(name=path, raise_on_fail=raise_on_fail, messenger=messenger)
             if rm_paths:
                 self.rm_paths_in_dir(dir_path=path, rm_dir_path=True)
 
     def mv_file(
         self,
         name: str,
         new_path: Union[str, pathlib.PurePath],
-        update_path: bool = True
+        update_path: bool = True,
     ) -> None:
         """
         Move a file to a new path.
         Optionally update the path for `name` in the collection.
 
-        When updating the path after moving the file, it re-checks 
+        When updating the path after moving the file, it re-checks
         the paths. See `.check_paths()` for details.
         """
         coll_name = self.get_collection_name_by_path_name(name=name)
         self[name].rename(new_path)
         if update_path:
             self._collections[coll_name][name] = new_path
             self._prepare_paths()
@@ -714,16 +707,15 @@
         other : `IOPaths` instance
             Another `IOPaths` instance with paths.
             Each sub collection is dict-updated one at a time.
         """
         assert isinstance(other, IOPaths)
         for coll_name in IOPaths.COLLECTION_NAMES:
             self._update_collection(
-                paths=other.get_collection(name=coll_name),
-                collection=coll_name
+                paths=other.get_collection(name=coll_name), collection=coll_name
             )
 
         # Ensure consistency
         self._prepare_paths()
 
     def difference(self, other: object):
         """
@@ -736,16 +728,16 @@
         other : `IOPaths` instance
             Another `IOPaths` instance with paths.
             Each sub collection is dict-updated one at a time.
 
         Returns
         -------
         `IOPaths` instance
-            A new `IOPaths` instance with the keys and paths in 
-            the collections of this object that are not in the collections 
+            A new `IOPaths` instance with the keys and paths in
+            the collections of this object that are not in the collections
             of the `other` object.
         """
         assert isinstance(other, IOPaths)
         diff_dicts = {}
         for coll_name in IOPaths.COLLECTION_NAMES:
             this_coll = self.get_collection(name=coll_name)
             if this_coll is None:
@@ -767,15 +759,15 @@
             tmp_dirs=diff_dicts["tmp_dirs"],
         )
 
     def __eq__(self, other: object) -> bool:
         """
         Check equality of this `IOPaths` instance and another.
 
-        Checks that all sub collections are the same. 
+        Checks that all sub collections are the same.
         No other attributes are considered.
 
         Parameters
         ----------
         other : `IOPaths` instance
             Another `IOPaths` instance with paths.
         """
@@ -787,23 +779,31 @@
             other_coll = other.get_collection(name=coll_name)
             if sum([other_coll is None, this_coll is None]) == 1:
                 return False
             if this_coll != other_coll:
                 return False
         return True
 
-    def _new(self, in_files: dict = None, in_dirs: dict = None, out_files: dict = None, out_dirs: dict = None, tmp_files: dict = None, tmp_dirs: dict = None):
+    def _new(
+        self,
+        in_files: dict = None,
+        in_dirs: dict = None,
+        out_files: dict = None,
+        out_dirs: dict = None,
+        tmp_files: dict = None,
+        tmp_dirs: dict = None,
+    ):
         """
         Create new `IOPaths` object with new collections but keeping the rest of the settings.
 
         Parameters
         ----------
         in_files : dict
             Dict with named paths to input files, mapping `(argument) name -> input filepath`.
-            A path can also be "-" when streaming input. 
+            A path can also be "-" when streaming input.
             This value will remain a string and will not be checked
             for duplication, existence, etc.
         in_dirs : dict
             Dict with named paths to input directories, mapping `(argument) name -> input directory path`.
         out_files : dict
             Dict with named paths to output files, mapping `(argument) name -> output filepath`.
         out_dirs : dict
@@ -823,15 +823,15 @@
             out_files=out_files,
             out_dirs=out_dirs,
             tmp_files=tmp_files,
             tmp_dirs=tmp_dirs,
             allow_none=self.allow_none,
             allow_overwriting=self.allow_overwriting,
             allow_duplicates_in=self.allow_duplicates_in,
-            print_note=self.print_note
+            print_note=self.print_note,
         )
 
     def _check_collection_name(self, name: str):
         if name not in IOPaths.COLLECTION_NAMES:
             raise ValueError(f"Collection name was unknown: {name}.")
 
     def _format_path_out(self, path, as_str: bool):
```

### Comparing `utipy-1.0.1/utipy/path/mk_rm_dir.py` & `utipy-1.0.2/utipy/path/mk_rm_dir.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/path/prepare_paths.py` & `utipy-1.0.2/utipy/path/prepare_paths.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/string/letter_strings.py` & `utipy-1.0.2/utipy/string/letter_strings.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/string/random_strings.py` & `utipy-1.0.2/utipy/string/random_strings.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/time/format_time.py` & `utipy-1.0.2/utipy/time/format_time.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/time/timer.py` & `utipy-1.0.2/utipy/time/timer.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/time/timestamps.py` & `utipy-1.0.2/utipy/time/timestamps.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/utils/check_instance.py` & `utipy-1.0.2/utipy/utils/check_instance.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/utils/convert_to_df.py` & `utipy-1.0.2/utipy/utils/convert_to_df.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/utils/convert_to_type.py` & `utipy-1.0.2/utipy/utils/convert_to_type.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/utipy/utils/messenger.py` & `utipy-1.0.2/utipy/utils/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,38 +133,49 @@
         return self._indent
 
     def __call__(
             self,
             *objects: Any,
             verbose: Union[None, bool] = None,
             indent: Union[None, int] = None,
+            add_indent: Union[None, int] = None,
             sep: str = ' ',
             add_msg_fn: Optional[Callable] = None,
             **kwargs: Any) -> None:
         """
         Perform messaging using `self.msg_fn`.
 
         Parameters
         ----------
         objects : objects
             Objects to message. Anything printable (i.e. with a `__str__` method).
         verbose : bool
             Whether to perform the messaging for this specific call.
         indent : int
             Number of whitespaces to indent the message in this specific call.
+        add_indent : int
+            Number of whitespaces to add to the current indent state 
+            for the message in this specific call.
         sep : str
             String used to separate `objects`.
         add_msg_fn : Callable or `None`
             Additional messaging function to use. 
             E.g. `warnings.warn` for throwing a warning as well.
         kwargs : keyword arguments
             Named arguments for the messaging function.
         """
         if verbose is None:
             verbose = self._verbose
+        if add_indent is not None:
+            if indent is not None:
+                raise ValueError(
+                    "`indent` and `add_indent` were both specified. "
+                    "Please only specify one (or none) of them."
+                )
+            indent = self._indent + add_indent
         if indent is None:
             indent = self._indent
 
         # Get kwargs for current call
         call_kwargs = self.kwargs.copy()
         call_kwargs.update(kwargs)
```

### Comparing `utipy-1.0.1/utipy/utils/step_idx.py` & `utipy-1.0.2/utipy/utils/step_idx.py`

 * *Files identical despite different names*

### Comparing `utipy-1.0.1/PKG-INFO` & `utipy-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: utipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility functions for python
 Home-page: https://github.com/ludvigolsen/utipy
 License: MIT
-Keywords: pandas,numpy,array,ndarray,groups,folds,kfold,partitioning,utilities,tools,rolling,windows,time
+Keywords: pandas,numpy,array,ndarray,groups,folds,kfold,partitioning,utilities,logging,time,tools,rolling,windows,time
 Author: Ludvig Renbo Olsen
 Author-email: mail@ludvigolsen.dk
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (>=1.21.6,<2.0.0)
+Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Project-URL: Repository, https://github.com/ludvigolsen/utipy
 Project-URL: issues, https://github.com/ludvigolsen/utipy/issues
 Description-Content-Type: text/markdown
 
 utipy
 --------
```

