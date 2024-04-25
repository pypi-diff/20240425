# Comparing `tmp/progress-api-0.1.0a3.tar.gz` & `tmp/progress_api-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-api-0.1.0a3.tar", last modified: Tue Feb 20 18:51:41 2024, max compression
+gzip compressed data, was "progress_api-0.1.0a4.tar", last modified: Thu Apr 25 01:02:01 2024, max compression
```

## Comparing `progress-api-0.1.0a3.tar` & `progress_api-0.1.0a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.406649 progress-api-0.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-02-20 18:51:41.406649 progress-api-0.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.398649 progress-api-0.1.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.398649 progress-api-0.1.0a3/docs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/docs/backends/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.398649 progress-api-0.1.0a3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.402649 progress-api-0.1.0a3/examples/enlighten/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/.header.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/ftp_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/multicolored.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/multiple_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/multiprocessing_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/enlighten/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/examples/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.402649 progress-api-0.1.0a3/progress_api/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.402649 progress-api-0.1.0a3/progress_api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/backends/enlighten.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/backends/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/backends/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/progress_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 18:51:41.402649 progress-api-0.1.0a3/progress_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-20 18:51:41.000000 progress-api-0.1.0a3/progress_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-20 18:51:33.000000 progress-api-0.1.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 18:51:41.406649 progress-api-0.1.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/docs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/backends/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.927286 progress_api-0.1.0a4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/examples/enlighten/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/.header.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/ftp_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multicolored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multiple_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/multiprocessing_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/enlighten/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/examples/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/enlighten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/backends/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/progress_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:02:01.931286 progress_api-0.1.0a4/progress_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 01:02:01.000000 progress_api-0.1.0a4/progress_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 01:01:57.000000 progress_api-0.1.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:02:01.935287 progress_api-0.1.0a4/setup.cfg
```

### Comparing `progress-api-0.1.0a3/.gitignore` & `progress_api-0.1.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/LICENSE.md` & `progress_api-0.1.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/PKG-INFO` & `progress_api-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress-api-0.1.0a3/docs/api.rst` & `progress_api-0.1.0a4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/docs/backends/index.rst` & `progress_api-0.1.0a4/docs/backends/index.rst`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/docs/conf.py` & `progress_api-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/docs/index.rst` & `progress_api-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/LICENSE` & `progress_api-0.1.0a4/examples/enlighten/LICENSE`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/basic.py` & `progress_api-0.1.0a4/examples/enlighten/basic.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/demo.py` & `progress_api-0.1.0a4/examples/enlighten/demo.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/floats.py` & `progress_api-0.1.0a4/examples/enlighten/floats.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/ftp_downloader.py` & `progress_api-0.1.0a4/examples/enlighten/ftp_downloader.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/multicolored.py` & `progress_api-0.1.0a4/examples/enlighten/multicolored.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/multiple_logging.py` & `progress_api-0.1.0a4/examples/enlighten/multiple_logging.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/multiprocessing_queues.py` & `progress_api-0.1.0a4/examples/enlighten/multiprocessing_queues.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/enlighten/prefixes.py` & `progress_api-0.1.0a4/examples/enlighten/prefixes.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/examples/training_loop.py` & `progress_api-0.1.0a4/examples/training_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             _log.info("beginning epoch %d", epoch + 1)
             batches = make_progress(_log, "batches", BATCHES)
             for batch in range(BATCHES):
                 _log.debug("training batch %d", batch)
                 delay = time.samples(1)[0]
                 sleep(delay * delay / 1000)
                 loss += adjust.samples(1)[0]
-                batches.set_meter("loss", loss, "{:.3f}")
+                batches.set_metric("loss", loss, "{:.3f}")
                 batches.update(1)
             batches.finish()
             epochs.update(1)
         epochs.finish()
 
 
 if __name__ == "__main__":
```

### Comparing `progress-api-0.1.0a3/progress_api/__init__.py` & `progress_api-0.1.0a4/progress_api/__init__.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/progress_api/api.py` & `progress_api-0.1.0a4/progress_api/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     when the context is exited.
 
     Attributes:
         name: The name of the logger this progress bar is attached to.
     """
 
     name: str
+    spec: backends.ProgressBarSpec
 
     @abstractmethod
     def set_label(self, label: Optional[str]) -> None:
         """
         Set a label to be used for this progress bar.
         """
         raise NotImplementedError()
@@ -36,35 +37,48 @@
     @abstractmethod
     def set_total(self, total: int) -> None:
         """
         Update the progress bar's total.
         """
         raise NotImplementedError()
 
-    def set_meter(self, label: str, value: int | str | float | None, fmt: str | None = None):
+    def set_metric(
+        self, label: str, value: int | str | float | None, fmt: str | None = None
+    ) -> None:
         """
-        Set a meter on the progress bar.
-
-        The format specifier is put into a format string that is passed to `str.format`, and must
-        include the braces.  For example, to format a percentage with 2 decimal points::
+        Set an ”metric” on the progress bar.  This is a secondary value
+        that will be displayed along with ETA; it is intended for things like a
+        current measurement (e.g. the current training loss for training a
+        machine learning model).
+
+        The format specifier is put into a format string that is passed to
+        :meth:`str.format`, and must include the braces.  For example, to format
+        a percentage with 2 decimal points::
 
             progress.set_meter('buffer', buf_fill_pct, '{:.2f}%')
 
-        Only one meter can be set at a time.  A new meter will replace any existing meter.
+        Only one meter can be set at a time.  A new meter will replace any
+        existing meter.  This method remembers the label and format, even
+        if ``value`` is ``None``, so the metric value can be supplied in
+        ``update``.
 
         Args:
-            label: the meter label
-            value: the meter value
+            label: the label for the metric
+            value: the metric value, or ``None`` to hide the metric.
             fmt: a format specifier (suitable for use in :meth:`str.format`)
         """
         pass
 
     @abstractmethod
     def update(
-        self, n: int = 1, state: Optional[str] = None, src_state: Optional[str] = None
+        self,
+        n: int = 1,
+        state: Optional[str] = None,
+        src_state: Optional[str] = None,
+        metric: int | str | float | None = None,
     ) -> None:
         """
         Update the progress bar.
 
         Args:
             n: the amount to increment the progress bar counter by.
             state: the name of the progress bar state to increment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `progress-api-0.1.0a3/progress_api/backends/__init__.py` & `progress_api-0.1.0a4/progress_api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/progress_api/backends/enlighten.py` & `progress_api-0.1.0a4/progress_api/backends/enlighten.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # pyright: basic
 from __future__ import annotations
 
 from typing import Optional
 
 from enlighten import Counter, Manager
 
-from progress_api.util import format_meter
+from progress_api.util import format_metric
 
 from .. import api
 from . import ProgressBackend, ProgressBarSpec
 
 _lead = "{desc}{desc_pad}"
 _dft_meter = "[{elapsed}, {rate:.2f}{unit_pad}{unit}/s{meter_pad}{meter}]"
 _byte_meter = "[{elapsed}, {rate:.2f}{unit_pad}{unit}/s{meter_pad}{meter}]"
@@ -90,38 +90,55 @@
         return EnlightenProgress(spec, bar, bars)
 
 
 class EnlightenProgress(api.Progress):
     spec: ProgressBarSpec
     bar: Counter
     bars: dict[str, Counter]
+    _metric_display: Optional[tuple[str, Optional[str]]] = None
 
     def __init__(self, spec: ProgressBarSpec, bar: Counter, bars: dict[str, Counter]):
         self.spec = spec
         self.bar = bar
         self.bars = bars
 
     def set_label(self, label: Optional[str]):
         self.bar.desc = label
 
     def set_total(self, total: int):
         self.bar.total = total
 
-    def set_meter(self, label: str, value: int | str | float | None, fmt: str | None = None):
+    def set_metric(self, label: str, value: int | str | float | None, fmt: str | None = None):
+        self._metric_display = (label, fmt)
+        self._update_metric(value)
+
+    def _update_metric(self, value: int | str | float | None):
+        if self._metric_display is None:
+            return
+
+        lbl, fmt = self._metric_display
         if value:
             self.bar.fields["meter_pad"] = ", "
-            self.bar.fields["meter"] = format_meter(label, value, fmt)
+            self.bar.fields["meter"] = format_metric(lbl, value, fmt)
         else:
             self.bar.fields["meter_pad"] = ""
             self.bar.fields["meter"] = ""
 
-    def update(self, n: int = 1, state: Optional[str] = None, src_state: Optional[str] = None):
+    def update(
+        self,
+        n: int = 1,
+        state: Optional[str] = None,
+        src_state: Optional[str] = None,
+        metric: int | str | float | None = None,
+    ):
         if state is None:
             state = self.spec.states[0].name
         bar = self.bars[state]
+        if metric is not None:
+            self._update_metric(metric)
         if src_state:
             src = self.bars[src_state]
             bar.update_from(src, float(n))  # type: ignore
         else:
             bar.update(float(n))  # type: ignore
 
     def finish(self):
```

### Comparing `progress-api-0.1.0a3/progress_api/backends/tqdm.py` & `progress_api-0.1.0a4/progress_api/backends/tqdm.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from tqdm import tqdm
 from tqdm.auto import tqdm as auto_tqdm
 
-from progress_api.util import format_meter
+from progress_api.util import format_metric
 
 from .. import api
 from . import ProgressBackend, ProgressBarSpec
 
 
 class TQDMProgressBackend(ProgressBackend):
     """
@@ -40,31 +40,48 @@
         return TQDMProgress(spec, tqdm)
 
 
 class TQDMProgress(api.Progress):
     spec: ProgressBarSpec
     tqdm: tqdm
     final_states: set[str]
+    _metric_display: Optional[tuple[str, Optional[str]]] = None
 
     def __init__(self, spec: ProgressBarSpec, tqdm: "tqdm"):
         self.spec = spec
         self.tqdm = tqdm
         self.final_states = set(s.name for s in spec.states if s.final)
 
     def set_label(self, label: Optional[str]):
         self.tqdm.set_description(label)
 
     def set_total(self, total: int):
         self.tqdm.total = total
 
-    def set_meter(self, label: str, value: int | str | float | None, fmt: str | None = None):
+    def set_metric(self, label: str, value: int | str | float | None, fmt: str | None = None):
+        self._metric_display = (label, fmt)
+        self._update_metric(value)
+
+    def _update_metric(self, value: int | str | float | None):
+        if self._metric_display is None:
+            return
+
+        lbl, fmt = self._metric_display
         if value is not None:
-            self.tqdm.set_postfix_str(format_meter(label, value, fmt))
+            self.tqdm.set_postfix_str(format_metric(lbl, value, fmt))
         else:
             self.tqdm.set_postfix_str("")
 
-    def update(self, n: int = 1, state: Optional[str] = None, src_state: Optional[str] = None):
+    def update(
+        self,
+        n: int = 1,
+        state: Optional[str] = None,
+        src_state: Optional[str] = None,
+        metric: int | str | float | None = None,
+    ):
+        if metric is not None:
+            self._update_metric(metric)
         if state is None or state in self.final_states and src_state not in self.final_states:
             self.tqdm.update(n)
 
     def finish(self):
         self.tqdm.close()
```

### Comparing `progress-api-0.1.0a3/progress_api/config.py` & `progress_api-0.1.0a4/progress_api/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import os
 import threading
 from importlib.metadata import entry_points
-from typing import Any, cast
+from typing import Any, Callable, ParamSpec, cast, overload
 
 from . import backends
 
 _backend_lock = threading.Lock()
 _backend: backends.ProgressBackend | None = None
+BCP = ParamSpec("BCP")
 
 
 def _lazy_init():
     if _backend is not None:
         return
 
     env = os.environ.get("PROGRESS_BACKEND", None)
@@ -38,17 +39,36 @@
             _lazy_init()
 
     if _backend is None:
         raise RuntimeError("backend not initialized")
     return _backend
 
 
+@overload
+def set_backend(impl: backends.ProgressBackend) -> None:
+    ...
+
+
+@overload
+def set_backend(
+    impl: Callable[BCP, backends.ProgressBackend], *args: BCP.args, **kwargs: BCP.kwargs
+) -> None:
+    ...
+
+
+@overload
+def set_backend(impl: str, *args: Any, **kwargs: Any) -> None:
+    ...
+
+
 def set_backend(
-    impl: str | backends.ProgressBackend | type[backends.ProgressBackend], *args: Any, **kwargs: Any
-):
+    impl: str | backends.ProgressBackend | Callable[BCP, backends.ProgressBackend],
+    *args: Any,
+    **kwargs: Any,
+) -> None:
     """
     Set the progress backend.  The backend can be specified in one of several ways:
 
     *   A string naming a progress backend.  For the backends included with Progress API,
         this name matches the implementing module name (e.g. ``"enlighten"``).  Other
         backends can be registered with an entry point (see :ref:`implementing-backends`).
     *   An object implementing the :class:`backends.ProgressBackend` interface.
```

### Comparing `progress-api-0.1.0a3/progress_api.egg-info/PKG-INFO` & `progress_api-0.1.0a4/progress_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress-api-0.1.0a3/progress_api.egg-info/SOURCES.txt` & `progress_api-0.1.0a4/progress_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-api-0.1.0a3/pyproject.toml` & `progress_api-0.1.0a4/pyproject.toml`

 * *Files identical despite different names*

