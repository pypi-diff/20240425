# Comparing `tmp/pantarei-0.2.1.tar.gz` & `tmp/pantarei-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantarei-0.2.1.tar", last modified: Fri Apr 12 20:24:32 2024, max compression
+gzip compressed data, was "pantarei-0.3.0.tar", last modified: Thu Apr 25 12:09:37 2024, max compression
```

## Comparing `pantarei-0.2.1.tar` & `pantarei-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:24:32.659109 pantarei-0.2.1/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.2.1/LICENSE
--rw-r--r--   0 coslo     (1000) coslo     (1000)     3813 2024-04-12 20:24:32.659109 pantarei-0.2.1/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3102 2024-04-09 18:30:04.000000 pantarei-0.2.1/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:24:32.659109 pantarei-0.2.1/pantarei/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      246 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5417 2024-04-10 21:22:43.000000 pantarei-0.2.1/pantarei/_attempt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2208 2024-04-11 20:42:29.000000 pantarei-0.2.1/pantarei/backends.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2427 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/cache.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8326 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    19978 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/database.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8329 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1111 2024-04-11 20:42:29.000000 pantarei-0.2.1/pantarei/hooks.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9579 2024-04-11 21:27:17.000000 pantarei-0.2.1/pantarei/job.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6587 2024-04-11 20:42:29.000000 pantarei-0.2.1/pantarei/parsers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5395 2024-04-11 20:42:29.000000 pantarei-0.2.1/pantarei/scheduler.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5381 2024-04-11 20:42:29.000000 pantarei-0.2.1/pantarei/task.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:24:32.659109 pantarei-0.2.1/pantarei.egg-info/
--rw-r--r--   0 coslo     (1000) coslo     (1000)     3813 2024-04-12 20:24:32.000000 pantarei-0.2.1/pantarei.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      464 2024-04-12 20:24:32.000000 pantarei-0.2.1/pantarei.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-12 20:24:32.000000 pantarei-0.2.1/pantarei.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       25 2024-04-12 20:24:32.000000 pantarei-0.2.1/pantarei.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2024-04-12 20:24:32.000000 pantarei-0.2.1/pantarei.egg-info/top_level.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      781 2024-04-12 20:24:04.000000 pantarei-0.2.1/pyproject.toml
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      178 2024-04-12 20:24:32.659109 pantarei-0.2.1/setup.cfg
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-12 20:24:32.659109 pantarei-0.2.1/tests/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6625 2024-04-11 21:27:17.000000 pantarei-0.2.1/tests/test.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13119 2024-04-11 21:27:17.000000 pantarei-0.2.1/tests/test_db.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.3.0/LICENSE
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-04-25 12:09:37.201454 pantarei-0.3.0/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3040 2024-04-23 18:58:43.000000 pantarei-0.3.0/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/pantarei/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      262 2024-04-23 18:51:12.000000 pantarei-0.3.0/pantarei/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5417 2024-04-10 21:22:43.000000 pantarei-0.3.0/pantarei/_attempt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2218 2024-04-25 06:03:54.000000 pantarei-0.3.0/pantarei/backends.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2480 2024-04-24 19:24:11.000000 pantarei-0.3.0/pantarei/cache.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8508 2024-04-23 18:51:59.000000 pantarei-0.3.0/pantarei/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    20484 2024-04-25 11:54:56.000000 pantarei-0.3.0/pantarei/database.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9085 2024-04-25 05:57:44.000000 pantarei-0.3.0/pantarei/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1111 2024-04-23 18:50:56.000000 pantarei-0.3.0/pantarei/hooks.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10936 2024-04-23 19:11:45.000000 pantarei-0.3.0/pantarei/job.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6587 2024-04-23 18:50:56.000000 pantarei-0.3.0/pantarei/parsers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5551 2024-04-25 05:52:37.000000 pantarei-0.3.0/pantarei/scheduler.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    11135 2024-04-25 07:31:07.000000 pantarei-0.3.0/pantarei/syncer.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5974 2024-04-23 19:13:14.000000 pantarei-0.3.0/pantarei/task.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/pantarei.egg-info/
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      483 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       25 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/top_level.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      781 2024-04-25 12:09:29.000000 pantarei-0.3.0/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      178 2024-04-25 12:09:37.201454 pantarei-0.3.0/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/tests/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     7227 2024-04-25 08:24:45.000000 pantarei-0.3.0/tests/test.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    12286 2024-04-25 11:56:48.000000 pantarei-0.3.0/tests/test_db.py
```

### Comparing `pantarei-0.2.1/LICENSE` & `pantarei-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pantarei-0.2.1/PKG-INFO` & `pantarei-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantarei
-Version: 0.2.1
+Version: 0.3.0
 Summary: A general-purpose workflow manager
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/pantarei
 Project-URL: homepage, https://framagit.org/coslo/pantarei
 Project-URL: documentation, https://coslo.frama.io/pantarei
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -77,21 +77,20 @@
 ```bash
 pantarei=timid python script.py
 ```
 
 ## TODO
 
 - [X] parametrize scheduler commands other than slurm
+- [X] allow job submission within function
 - [ ] add command line tool
+- [ ] submit on remote cluster
 - [ ] handle task dependencies
 - [ ] add Workflow / Queue
-- [ ] allow job submission within function
-- [ ] submit on remote cluster
 - [ ] perhaps add signac-like view() or checkout() method to check out a view of cache as folders
-- [ ] handle same function name from multiple modules/scripts
 
 ## Mockups
 
 Handle task dependencies
 ```python
 def run(path):
     pass
```

### Comparing `pantarei-0.2.1/README.md` & `pantarei-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,21 +57,20 @@
 ```bash
 pantarei=timid python script.py
 ```
 
 ## TODO
 
 - [X] parametrize scheduler commands other than slurm
+- [X] allow job submission within function
 - [ ] add command line tool
+- [ ] submit on remote cluster
 - [ ] handle task dependencies
 - [ ] add Workflow / Queue
-- [ ] allow job submission within function
-- [ ] submit on remote cluster
 - [ ] perhaps add signac-like view() or checkout() method to check out a view of cache as folders
-- [ ] handle same function name from multiple modules/scripts
 
 ## Mockups
 
 Handle task dependencies
 ```python
 def run(path):
     pass
```

### Comparing `pantarei-0.2.1/pantarei/_attempt.py` & `pantarei-0.3.0/pantarei/_attempt.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.2.1/pantarei/backends.py` & `pantarei-0.3.0/pantarei/backends.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Backends
+Scheduler backends
 """
 # TODO: add object attributes to dicts?
 # TODO: named tuple?
 
 # SLURM
 slurm = dict(
     command='squeue',
```

### Comparing `pantarei-0.2.1/pantarei/cache.py` & `pantarei-0.3.0/pantarei/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 Cache
 """
 import os
 import pickle
 import yaml
+import numpy
 from .helpers import actual_kwargs, mkdir, rmd
 
+# TODO: use something better than pickle, like marshmallow, to dump data
 
 def _itemize(data):
     """Itemize numpy arrays in data"""
-    if hasattr(data, 'shape') and len(data.shape) > 1:
-        return data
-    try:
+    if isinstance(data, dict):
+        # Turn all ndarrays into lists
         new_data = {}
         for key in data:
-            if hasattr(data[key], 'item') and data[key].size == 1:
-                new_data[key] = data[key].item()
+            if isinstance(data, numpy.ndarray):
+                new_data[key] = numpy.ndarray.tolist(data[key])
             else:
                 new_data[key] = data[key]
-    except TypeError:
-        # Also do it if data itself is a numpy array
-        if hasattr(data, 'item') and data.size == 1:
-            new_data = data.item()
-        else:
-            new_data = data
-    return new_data
+        return new_data
+    # If data is an ndarray, turn it to a list
+    if isinstance(data, numpy.ndarray):
+        return numpy.ndarray.tolist(data)
+    # Just return data if all else fails
+    return data
 
 class Cache:
     """
     Cache results of function evaluation on the basis of its name and
     keyword arguments
     """
```

### Comparing `pantarei-0.2.1/pantarei/core.py` & `pantarei-0.3.0/pantarei/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     # ETA
     import datetime
     started_jobs = states["ended"] + states["failed"] + states["running"]
     eta, so_far = _eta(_jobs)
     if eta is None:
         eta = 'N/A'
     if started_jobs == 0:
-        return
+        return lines
 
     mean_time = datetime.timedelta(seconds=int(so_far.total_seconds()/(started_jobs)))
     eta, so_far, mean_time = str(eta), str(so_far), str(mean_time)
     lines.append('')
     for key, value in [("Total CPU time", so_far),
                        ("Mean CPU time per job", mean_time),
                        ("Wall time left", eta)]:
@@ -250,16 +250,20 @@
     :param only: types of jobs to include. Possible values are:
       `failed`, `running`, `ended`, `queued`. By default, all jobs are
       shown
     """
     lines = _report(only)
     if len(lines) > 0:
         print('\n'.join(lines))
-    
+
 # Log at the end of scripts
 
-def __report():
+def __report():    
     report(only=('running', 'failed'))
 
 
+# We should not do this during unit tests
+# The jobs will be there but the cache may be gone
+# This will give a spurious final line
+# TODO: register these hooks somewhere else
 atexit.register(__report)
 atexit.register(orphans)
```

### Comparing `pantarei-0.2.1/pantarei/database.py` & `pantarei-0.3.0/pantarei/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from tinydb.storages import Storage, MemoryStorage
 from tinydb.table import Table
 
 from .helpers import _wget, pprint
 
 
 # Default query
-query = Query()
+# query = Query()
+def where(key):
+    return Query()[key]
 
 
 class maskablelist(list):
     """
     Data structure for heterogeneous arrays
     """
 
@@ -116,32 +118,35 @@
     def __init__(self, rows, columns):
         """
         :param rows: dataset as a sequence of sequences
         :param columns: names of each entry of the dataset
         """
         self.rows = rows
         self.columns = columns
+        self._maskable = False
 
     def __repr__(self):
         from .helpers import pprint
         from io import StringIO
         with StringIO() as io:
             pprint(self.rows, columns=self.columns, file=io)
             txt = io.getvalue()
         return txt
 
     def __len__(self):
         return len(self.rows)
 
     def __getitem__(self, key):
         if type(self.rows) == list:
-            if isinstance(key, str):
+            if isinstance(key, str):                
                 # We access a single row by key
+                if self._maskable:
+                    return maskablelist([row[key] for row in self.rows])
                 try:
-                    # Homogeneous
+                    # Homogenous
                     return ndarray(numpy.array([row[key] for row in self.rows]))
                 except ValueError:
                     # Non-homogeneous
                     return maskablelist([row[key] for row in self.rows])
             elif isinstance(key, int):
                 # Access list index
                 return self.rows[key]
@@ -345,20 +350,26 @@
     def __getitem__(self, key):
         return self.rows()[key]
 
     def groupby(self, key, condition=None, reverse=False):
         """
         Return a `Data` instance with entries with common `key` grouped
         along an extra first dimension
+
+        The results are sorted according to the `key`.
+
+        :param key: group entries according to `key` string
+        :param condition: only return entries matching query `cond`
+        :param reverse: revert the order of the sorting within the group
         """
         # This iterates over groups, hence the first dimension is the number of groups
         # The second dimension is the number of entries in each group
         # Then follows the shape of the data.
         # Hence to average we do:
-        # db.groupby('x').mean(axis=1)
+        #   db.groupby('x').mean(axis=1)
         # TODO: it would be more natural to have the number of entries as first dimension
         # and number of groups as second, so that we can average over axis=0
 
         # Sort and group (https://stackoverflow.com/questions/38013778/is-there-any-numpy-group-by-function)
         rows = self.find(sort_by=key, condition=condition)
         splits = rows[key].unique(return_index=True)[1][1:]
         groups = numpy.split(rows, splits)
@@ -372,15 +383,17 @@
             for column in columns:
                 data_dict[column] = [_group[column] for _group in group]
             data_all.append(data_dict)
 
         if reverse:
             data_all = sorted(data_all, key=lambda x: x[key], reverse=True)
 
-        return Data(data_all, columns)
+        data = Data(data_all, columns)
+        data._maskable = True
+        return data
 
     def pprint(self, condition=None, **kwargs):
         """Pretty print"""
         if 'ignore' not in kwargs:
             kwargs['ignore'] = ('_dirname', '_path')
         entries = self.search(condition)
         pprint(entries, **kwargs)
```

### Comparing `pantarei-0.2.1/pantarei/helpers.py` & `pantarei-0.3.0/pantarei/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """
 Helper functions
 """
+
+import sys
+import os
+import shutil
+import hashlib
 import inspect
 
 def actual_kwargs(func, *args, **kwargs):
     """Return all the arguments of a function as keyword arguments."""
     signature = inspect.signature(func)
     arg_names = tuple(param.name
                       for param in signature.parameters.values()
                       if param.default is param.empty)
-    # TODO: check if we passed a keyword argument we the same value as default
+    # TODO: check if we passed a keyword argument with the same value as default
     # Default keyword arguments
     # actual_args = {param.name: param.default
     #               for param in signature.parameters.values()
     #               if param.default is not param.empty}
     actual_args = {}
     actual_args.update({name: arg for name, arg in zip(arg_names, args)})
     actual_args.update(kwargs)
@@ -58,15 +63,15 @@
             pass
 
 def rmd(files):
     """Totally silent wrapper to shutil.rmtree."""
     import shutil
     try:
         shutil.rmtree(files)
-    except:
+    except BaseException:
         pass
 
 def rmf(files):
     """
     Remove `files` without complaining.
 
     The variable `files` can be a list or tuple of paths or a single
@@ -106,21 +111,14 @@
     func = FunctionType(f.__code__, f.__globals__, f.__name__ + '_' + name,
                         f.__defaults__, f.__closure__)
     if doc is not None:
         # func.__doc__ = '\n'.join((func.__doc__, doc))
         func.__doc__ = doc
     return func
 
-
-import sys
-import os
-import shutil
-import hashlib
-
-
 def pprint(rows, columns=None, ignore=(), sort_by=None, max_rows=100, file=sys.stdout, max_width=100):
     """Pretty print `rows` (a list of dicts)"""
 
     def _tabular(data, max_len=max_width):
         """General function to format `data` list in tabular table"""
 
         # Predict formatting
@@ -261,7 +259,31 @@
     try:
         return int(s)
     except ValueError:
         try:
             return float(s)
         except ValueError:
             return s
+
+def debug_stacks(stacks):
+    import dill
+    # DEBUG Try to fix...
+    # dill.settings['recurse'] = True
+    # print(s.frame.f_locals)
+    print('******')
+    for i, ss in enumerate(stacks):
+        print('-'*50)
+        print('Level:', i)
+        import pprint
+        print(ss.frame)
+        pprint.pprint(ss.frame.f_locals)
+        try:
+            dill.dump_module(f'/tmp/s{i}.pkl', module=inspect.getmodule(ss.frame.f_code), refimported=False)
+        except TypeError:
+            print('*WARNING*: cannot dill this frame!')
+        print('Source:')
+        print(dill.source.getsource(ss.frame.f_code))
+        print()
+        print('Trace:')
+        with dill.detect.trace():
+            dill.dumps(ss.frame.f_code)
+        print()
```

### Comparing `pantarei-0.2.1/pantarei/hooks.py` & `pantarei-0.3.0/pantarei/hooks.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.2.1/pantarei/job.py` & `pantarei-0.3.0/pantarei/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -189,34 +189,62 @@
             if self.scheduler.queued(self.qualified_name()):
                 # print('JOB IS IN QUEUE', self.qualified_name())
                 return
 
         # dirname = os.path.join(self.task.cache.path, self.qualified_name())
         mkdir(self.path)
         session_pkl = os.path.join(self.path, '.session.pkl')
+        context_pkl = os.path.join(self.path, '.context.pkl')
         job_state = os.path.join(self.path, 'job.yaml')
         job_output = os.path.join(self.path, 'job.out')
+        kwargs = serialize_kwargs(self.kwargs)
 
         n = _stack_index
-        # n=-2
+        n = -2  # for
         stacks = inspect.stack()
         s = stacks[n]
-        kwargs = serialize_kwargs(self.kwargs)
-        code = f"dill.load_module('{session_pkl}')"
+        for n in range(len(stacks)-1, -1, -1):
+            if 'job' in stacks[n].frame.f_locals:
+                s = stacks[n]
+                from .helpers import debug_stacks
+                # debug_stacks(stacks)
+                break            
+
+        # s = stacks[n]
+
+        from types import ModuleType
+        context = ModuleType('context')
+        # context.__dict__.update(s.frame.f_globals)
+        # args = s.frame.f_locals
+        # import pprint
+        # pprint.pprint(s.frame.f_locals)
+        # pprint.pprint(s.frame.f_globals)
+        # context.__dict__.update(s.frame.f_globals)
+        context.job = s.frame.f_locals['job']
+        # Store session and local context separately.
+        # The session stores all objects in the module of the frame
+        # containing the job instance
+        dill.dump_module(session_pkl, module=inspect.getmodule(s.frame.f_code), refimported=True)
+        # The context session stores the job instance itself
+        # to cover the case in which this is defined in a function
+        # TODO: query cannot be pickled in context? How come, we only have job here...
+        # print('query' in s.frame.f_globals)
+        # print('query' in s.frame.f_locals)
+        # Nothing of this works
+        # query = s.frame.f_globals.pop('query')
+        # del query
+        # s.frame.f_locals.pop('query')
+        dill.dump_module(context_pkl, module=context, refimported=True)
 
-        # print(s.frame.f_locals)
-        # print('******')
-        # for i, ss in enumerate(stacks):
-        #     print(i)
-        #     print(ss.frame.f_locals)
-        #     dill.dump_module(f'/tmp/s{i}.pkl', module=inspect.getmodule(ss.frame.f_code), refimported=True)
-        #     print()
+        # from .helpers import debug_stacks
+        # debug_stacks(stacks)
 
         # print('---------------')
         # print(s.frame)
+        # print(s.frame.f_locals)
         # print('---------------')
 
         # fix issues with emacs python shell execution
         var = s.frame.f_locals
         if '__pyfile' in var:
             # s = stacks[-2]
             s = stacks[n - 1]
@@ -237,16 +265,14 @@
         #                 print(i, l.strip())
         #                 found = True
         #             break
         #     if found:
         #         break
         # print(s.frame.f_locals)
         # https://stackoverflow.com/questions/1253528/is-there-an-easy-way-to-pickle-a-python-function-or-otherwise-serialize-its-cod
-        # print(s.frame.f_globals)
-        dill.dump_module(session_pkl, module=inspect.getmodule(s.frame.f_code), refimported=True)
         # TODO: process the calling line to get the job object instead of hardcoding job
         script = f"""\
 #!/usr/bin/env -S python -u
 __name__ = '__main__'
 import sys
 import os
 import time
@@ -260,26 +286,33 @@
 if 'HOSTNAME' in os.environ:
     hostname = os.environ['HOSTNAME']
 
 fh = open('{job_state}', 'a')
 print('job_node:', hostname, file=fh, flush=True)
 print('job_start:', time.time(), file=fh, flush=True)
 try:
-    {code}
-    # print(globals().keys())
-    job.task({kwargs})
+    dill.load_module('{session_pkl}')
+    context = dill.load_module('{context_pkl}')
+    import pprint
+    #pprint.pprint(locals())
+    #pprint.pprint(globals())
+    #print()
+    #pprint.pprint(context.__dict__)
+    context.job.task({kwargs})
+    #job.task({kwargs})
 except:
     print('job_fail:', time.time(), file=fh, flush=True)
     raise
 else:
     print('job_end:', time.time(), file=fh, flush=True)
 finally:
     fh.close()
     # Remove session data when job is over
     os.remove('{session_pkl}')
+    os.remove('{context_pkl}')
 """
         # TODO: drop this, it was only for synchronous, scheduler should always be not None
         if self.scheduler is None:
             import time
             with open(f'{job_state}', 'w') as fh:
                 print('job_queue:', time.time(), file=fh, flush=True)
```

### Comparing `pantarei-0.2.1/pantarei/parsers.py` & `pantarei-0.3.0/pantarei/parsers.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.2.1/pantarei/scheduler.py` & `pantarei-0.3.0/pantarei/scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,21 @@
 # Public:
 # submit()
 # wait()
 # queued()
 
 class Scheduler:
 
-    """Wrapper to scheduler for execution on a distributed memory environment"""
+    """
+    Wrapper to scheduler for execution on a distributed memory environment
+
+    `Scheduler` is entirely decoupled from `Job`. For job submission,
+    it only needs a script as a string and the relevant job
+    directives.
+    """
 
     # TODO: add custom header or args to __init__ so that we can customize the job at run time
 
     def __init__(self, host='localhost', verbose=False, backend='auto', jobs_limit=0):
         """
         :param host: hostname of the cluster
         :param verbose: verbose output
@@ -90,15 +96,15 @@
                 return True
         return False
 
     def submit(self, script, job_name, job_output=None, job_error=None, cores=1):
         """
         Submit a script for batch execution on the scheduler
 
-        :param script: string of python commands to execute 
+        :param script: string of python commands to execute
         :param job_name: name of job
         :param job_output: job output file
         :param job_error: job error file
         :param cores: number of cores for the job
         """
         name, output, error = job_name, job_output, job_error
         params = locals()
```

### Comparing `pantarei-0.2.1/pantarei/task.py` & `pantarei-0.3.0/pantarei/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Task
 """
 import os
+import time
 from .helpers import actual_kwargs, all_actual_kwargs, rmd, rmf, tag_function
 from .cache import default_cache
 
 
 class Task:
 
     """Cached execution of function"""
@@ -49,15 +50,27 @@
         # Store all argments as metadata, even default ones
         self.cache.setup(name, **all_kwargs)
         if self.done(**kwargs):
             # Task found in cache
             results = self.cache.read(name)
         else:
             # Execute task
-            results = self.func(**kwargs)
+            # The logging is identical to job, the latter may be avoided?
+            hostname = 'unknown'
+            if 'HOSTNAME' in os.environ:
+                hostname = os.environ['HOSTNAME']
+            path = os.path.join(self.cache.path, name)
+            fh = open(os.path.join(path, 'task.yaml'), 'a')
+            print('task_node:', hostname, file=fh, flush=True)
+            print('task_start:', time.time(), file=fh, flush=True)
+            try:
+                results = self.func(**kwargs)
+                print('task_end:', time.time(), file=fh, flush=True)
+            finally:
+                fh.close()
             self.cache.write(name, results)
         # Check whether task returned an artifacts entry and if so, store it
         try:
             self.artifacts = results['artifacts']
         except:
             pass
         return results
```

### Comparing `pantarei-0.2.1/pantarei.egg-info/PKG-INFO` & `pantarei-0.3.0/pantarei.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantarei
-Version: 0.2.1
+Version: 0.3.0
 Summary: A general-purpose workflow manager
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/pantarei
 Project-URL: homepage, https://framagit.org/coslo/pantarei
 Project-URL: documentation, https://coslo.frama.io/pantarei
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -77,21 +77,20 @@
 ```bash
 pantarei=timid python script.py
 ```
 
 ## TODO
 
 - [X] parametrize scheduler commands other than slurm
+- [X] allow job submission within function
 - [ ] add command line tool
+- [ ] submit on remote cluster
 - [ ] handle task dependencies
 - [ ] add Workflow / Queue
-- [ ] allow job submission within function
-- [ ] submit on remote cluster
 - [ ] perhaps add signac-like view() or checkout() method to check out a view of cache as folders
-- [ ] handle same function name from multiple modules/scripts
 
 ## Mockups
 
 Handle task dependencies
 ```python
 def run(path):
     pass
```

### Comparing `pantarei-0.2.1/pyproject.toml` & `pantarei-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pantarei"
 description = "A general-purpose workflow manager"
 readme = "README.md"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name = "Daniele Coslovich", email = "daniele.coslovich@umontpellier.fr"}
 ]
 requires-python = ">=3.8"
 license = {text = "GPLv3"}
 dependencies = [
     "numpy",
```

### Comparing `pantarei-0.2.1/tests/test.py` & `pantarei-0.3.0/tests/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,20 @@
         task.clear(x=1)
         self.assertFalse(task.done(x=1))
         ti = time.time()
         task(x=1)
         tf = time.time()
         self.assertGreater(tf-ti, 0.9)
 
+        # Check with arrays
+        # We should have a look at the .*.yaml files
+        import numpy
+        data = task(x=numpy.ndarray([1]))
+        data = task(x=numpy.ndarray([1]))
+        
     def test_task_ignore(self):
         import time
         def f(x, debug):
             return x
         cache = Cache('/tmp/data')
         task = Task(f, cache=cache, ignore=['debug'])
         task(x=1, debug=False)
@@ -98,30 +104,30 @@
         task(x=1)
         self.assertTrue(os.path.exists(cache._storage(task.qualified_name(x=1))))
         self.assertTrue(os.path.exists('/tmp/artifacts'))
         task.clear(x=1)
         self.assertFalse(os.path.exists('/tmp/artifacts'))
         self.assertFalse(os.path.exists(cache._storage(task.qualified_name(x=1))))
 
-    @unittest.skip('Job not working from unittest')
+    #@unittest.skip('Job not working from unittest')
     def test_job(self):
         import pantarei.job
         from pantarei import Task, Job, Scheduler, Cache
         pantarei.job._stack_index = 2 #-1
         def f(x):
             import time
             time.sleep(1)
             return x
         task = Task(f, cache=Cache('/tmp/data'))
         job = Job(task, scheduler=Scheduler(backend='nohupx', verbose=False))
         job(x=1)
         job.scheduler.wait(seconds=1.5)
         from pantarei.core import orphans, report
         missing = orphans()
-        self.assertTrue(len(missing) == 0)
+        #self.assertTrue(len(missing) == 0)
         report()
 
     def test_job_cmd(self):
         script = """
 from pantarei import Task, Job, Scheduler, Cache
 
 def f(x):
@@ -194,13 +200,26 @@
         self.assertTrue(db['debug'] == [False])
 
         # Check that order is preserved
         task(x=0, debug=False)
         db = pantarei.browse(path='/tmp/data')
         self.assertTrue(list(db['x']), [1, 0])
 
+    # def test_syncer(self):
+    #     from pantarei.helpers import mkdir
+    #     from pantarei.syncer import rsync, Syncer
+
+    #     mkdir('/tmp/data')
+    #     with open('/tmp/data/hello.txt', 'w') as fh:
+    #         fh.write('hello')
+
+    #     with Syncer(source="/tmp/data",
+    #                 dest="tmp",
+    #                 dest_ssh="varda") as s:
+    #         s.run()        
+        
     def tearDown(self):
         from pantarei.helpers import rmd
         rmd('/tmp/data')
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pantarei-0.2.1/tests/test_db.py` & `pantarei-0.3.0/tests/test_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 import os
 import numpy
 from pantarei import *
 from pantarei.helpers import mkdir, rmd
-from pantarei.database import query, VeryTinyDB
+from pantarei.database import Query, VeryTinyDB, where
 
+query = Query()
 
 class Test(unittest.TestCase):
 
     def setUp(self):
         import yaml, pickle
         for rho in [1.0]:
             for n in range(2):
@@ -37,14 +38,15 @@
 
     def _check_ds(self, ds):
         self.assertTrue(all(ds['rho'] == [1, 1]))
         self.assertTrue(all(ds['n'] == [0, 1]))
         self.assertTrue(all(ds['N'] == [0, 10]))
         self.assertTrue(all(ds['M'] == [0, 10]))
         self.assertTrue(all(ds.rows(query.n == 0)['rho'] == [1, ]))
+        self.assertTrue(all(ds.rows(where('n') == 0)['rho'] == [1, ]))
 
     def test_basic(self):
         ds = Dataset()
         ds.insert('/tmp/dataset/**/data.*')
         self._check_ds(ds)
         ds._missing()
 
@@ -202,21 +204,37 @@
         self.assertEqual(str(db.rows()), str(db))
         self.assertTrue(all(db.rows()['tag'] == ['a', 'abc']))
 
     def test_groupby(self):
         from pantarei.database import Data
 
         db = VeryTinyDB()
-        db.insert({'T': 1, 'x': numpy.array([1, 2, 3]), 'y': 20, 'seed': 1, 'tag': 'a'})
-        db.insert({'T': 1, 'x': numpy.array([2, 3, 4]), 'y': 22, 'seed': 2, 'tag': 'a'})
-        db.insert({'T': 2, 'x': numpy.array([10, 20, 30]), 'y': 10, 'seed': 1, 'tag': 'a'})
-        db.insert({'T': 2, 'x': numpy.array([20, 30, 40]), 'y': 12, 'seed': 2, 'tag': 'a'})
-        db.insert({'T': 3, 'x': numpy.array([100, 200, 300]), 'y': 30, 'seed': 1, 'tag': 'a'})
-        db.insert({'T': 3, 'x': numpy.array([200, 300, 400]), 'y': 32, 'seed': 2, 'tag': 'a'})
+        db.insert({'T': 1, 'x': numpy.array([1, 2, 3]), 'y': 20, 'seed': 1})
+        db.insert({'T': 1, 'x': numpy.array([2, 3, 4]), 'y': 22, 'seed': 2})
+        db.insert({'T': 2, 'x': numpy.array([10, 20, 30]), 'y': 10, 'seed': 1})
+        db.insert({'T': 2, 'x': numpy.array([20, 30, 40]), 'y': 12, 'seed': 2})
+        db.insert({'T': 3, 'x': numpy.array([100, 200, 300]), 'y': 30, 'seed': 1})
+        db.insert({'T': 3, 'x': numpy.array([200, 300, 400]), 'y': 32, 'seed': 2})
+
+        # Note: groupby() always returns a maskablelist.
+        # We get a (M, ...) array ,where M is the number of occurrences of the key
+        # in the group. Then that array can be averaged with numpy methods
+        dg = db.groupby('T')
+        self.assertEqual(list(dg['x'].mean(axis=0)[0]), [1.5, 2.5, 3.5])
 
+        db = VeryTinyDB()
+        db.insert({'T': 1, 'x': numpy.array([1, 2, 3]), 'y': 20, 'seed': 1})
+        db.insert({'T': 1, 'x': numpy.array([2, 3, 4]), 'y': 21, 'seed': 2})
+        db.insert({'T': 1, 'x': numpy.array([1, 2, 3]), 'y': 22, 'seed': 3})
+        db.insert({'T': 1, 'x': numpy.array([2, 3, 4]), 'y': 23, 'seed': 4})
+        db.insert({'T': 2, 'x': numpy.array([10, 20, 30]), 'y': 10, 'seed': 1})
+        db.insert({'T': 2, 'x': numpy.array([20, 30, 40]), 'y': 11, 'seed': 2})
+        dg = db.groupby('T')
+        self.assertEqual(list(dg['x'].mean(axis=0)[1]), [15, 25, 35])
+        
         # from pantarei.database import Data
         # def groupby(db, key):
         #     rows = db.find(sort_by=key)
         #     splits = rows[key].unique(return_index=True)[1][1:]
         #     return numpy.split(rows, splits) #, db.columns()
 
         # def groupby_one(db, key, what):
@@ -224,42 +242,14 @@
         #     columns = db.columns()
         #     data_all = []
         #     for group in groups:
         #         data = Data(list(group), columns)
         #         data_all.append(data[what])
         #     Data(data_mean, columns)
 
-        # def mean(db, key, include=(), exclude=()):
-        #     groups = groupby(db, key)
-        #     columns = db.columns()
-        #     columns.remove(key)
-        #     for excl in exclude:
-        #         columns.remove(excl)
-        #     columns = include
-        #     data_mean = []
-        #     exclude = []
-        #     for group in groups:
-        #         data = Data(list(group), columns)
-        #         data_dict = {}
-        #         for column in columns:
-        #             data_dict[column] = data[column].mean(axis=0)
-        #             data_mean.append(data_dict)
-        #             # try:
-        #             #     data_dict[column] = data[column].mean(axis=0)
-        #             #     #data_dict = {column: data[column].mean(axis=0) for column in columns}
-        #             #     data_mean.append(data_dict)
-        #             # except:
-        #             #     print('ex', column)
-        #             #     if column not in exclude: exclude.append(column)
-        #             #     pass
-        #     # print(exclude)
-        #     # for excl in exclude:
-        #     #     columns.remove(excl)
-        #     return Data(data_mean, columns)
-
         # def groupbyby(db, key, include=()):
         #     groups = groupby(db, key)
         #     columns = db.columns()
         #     columns.remove(key)
         #     columns = include
         #     for group in groups:
         #         for entry in group:
@@ -279,27 +269,14 @@
         #     for group in groups:
         #         data_dict = {}
         #         for column in columns:
         #             data_dict[column] = [_group[column] for _group in group]
         #         data_all.append(data_dict)
         #     return Data(data_all, columns)
 
-        # #print(mean(db, 'T', ['x', 'y']))
-        # #print(groupbyby(db, 'T', ['x', 'y']))
-        # dsg = groupby_all(db, 'T')
-        # print(dsg['x'].mean(axis=1))
-
-        # Return a (M, ...) array where M is the number of occurrences of the key in the group
-        # Then that array can be averaged with numpy features
-        dg = db.groupby('T')
-        # print(yg.shape, xg.shape)
-        # print(xg.mean(axis=1))
-        self.assertEqual(list(dg['y'].mean(axis=1)), [21, 11, 31])
-        self.assertEqual(list(dg['x'].mean(axis=1)[0]), [1.5, 2.5, 3.5])
-
     def test_maskable_attr(self):
         """Test dataset with inhomogeneous sizes forward attributes correctly"""
         from pantarei.database import Data
 
         db = VeryTinyDB()
         db.insert({'x': numpy.array([1, 2, 3]), 'y': 1, 'z': [1, 2]})
         db.insert({'x': numpy.array([2, 4]), 'y': 1, 'z': [1, 2, 3]})
```

