# Comparing `tmp/pyibl-5.1.3.tar.gz` & `tmp/pyibl-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyibl-5.1.3.tar", last modified: Sun Mar 24 23:03:09 2024, max compression
+gzip compressed data, was "pyibl-5.1.4.tar", last modified: Wed Apr 24 22:26:33 2024, max compression
```

## Comparing `pyibl-5.1.3.tar` & `pyibl-5.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 dfm       (1000) dfm       (1000)        0 2024-03-24 23:03:09.616543 pyibl-5.1.3/
--rw-rw-r--   0 dfm       (1000) dfm       (1000)      707 2024-02-06 21:26:14.000000 pyibl-5.1.3/LICENSE.txt
--rw-rw-r--   0 dfm       (1000) dfm       (1000)     1774 2024-03-24 23:03:09.612543 pyibl-5.1.3/PKG-INFO
--rw-rw-r--   0 dfm       (1000) dfm       (1000)      919 2024-02-06 21:26:14.000000 pyibl-5.1.3/README.md
-drwxrwxr-x   0 dfm       (1000) dfm       (1000)        0 2024-03-24 23:03:09.612543 pyibl-5.1.3/pyibl.egg-info/
--rw-rw-r--   0 dfm       (1000) dfm       (1000)     1774 2024-03-24 23:03:09.000000 pyibl-5.1.3/pyibl.egg-info/PKG-INFO
--rw-rw-r--   0 dfm       (1000) dfm       (1000)      183 2024-03-24 23:03:09.000000 pyibl-5.1.3/pyibl.egg-info/SOURCES.txt
--rw-rw-r--   0 dfm       (1000) dfm       (1000)        1 2024-03-24 23:03:09.000000 pyibl-5.1.3/pyibl.egg-info/dependency_links.txt
--rw-rw-r--   0 dfm       (1000) dfm       (1000)       67 2024-03-24 23:03:09.000000 pyibl-5.1.3/pyibl.egg-info/requires.txt
--rw-rw-r--   0 dfm       (1000) dfm       (1000)        6 2024-03-24 23:03:09.000000 pyibl-5.1.3/pyibl.egg-info/top_level.txt
--rw-rw-r--   0 dfm       (1000) dfm       (1000)    85761 2024-03-24 23:02:16.000000 pyibl-5.1.3/pyibl.py
--rw-rw-r--   0 dfm       (1000) dfm       (1000)       38 2024-03-24 23:03:09.616543 pyibl-5.1.3/setup.cfg
--rw-rw-r--   0 dfm       (1000) dfm       (1000)     1402 2024-03-24 22:57:32.000000 pyibl-5.1.3/setup.py
+drwxrwxr-x   0 dfm       (1000) dfm       (1000)        0 2024-04-24 22:26:33.563239 pyibl-5.1.4/
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)      707 2024-02-06 21:26:14.000000 pyibl-5.1.4/LICENSE.txt
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)     1774 2024-04-24 22:26:33.563239 pyibl-5.1.4/PKG-INFO
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)      919 2024-02-06 21:26:14.000000 pyibl-5.1.4/README.md
+drwxrwxr-x   0 dfm       (1000) dfm       (1000)        0 2024-04-24 22:26:33.563239 pyibl-5.1.4/pyibl.egg-info/
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)     1774 2024-04-24 22:26:33.000000 pyibl-5.1.4/pyibl.egg-info/PKG-INFO
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)      183 2024-04-24 22:26:33.000000 pyibl-5.1.4/pyibl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)        1 2024-04-24 22:26:33.000000 pyibl-5.1.4/pyibl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)       67 2024-04-24 22:26:33.000000 pyibl-5.1.4/pyibl.egg-info/requires.txt
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)        6 2024-04-24 22:26:33.000000 pyibl-5.1.4/pyibl.egg-info/top_level.txt
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)    85773 2024-04-24 22:21:43.000000 pyibl-5.1.4/pyibl.py
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)       38 2024-04-24 22:26:33.563239 pyibl-5.1.4/setup.cfg
+-rw-rw-r--   0 dfm       (1000) dfm       (1000)     1402 2024-03-24 22:57:32.000000 pyibl-5.1.4/setup.py
```

### Comparing `pyibl-5.1.3/LICENSE.txt` & `pyibl-5.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyibl-5.1.3/PKG-INFO` & `pyibl-5.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyibl
-Version: 5.1.3
+Version: 5.1.4
 Summary: A Python implementation of a subset of Instance Based Learning Theory
 Home-page: http://pyibl.ddmlab.com/
 Author: Dynamic Decision Making Laboratory of Carnegie Mellon University
 Author-email: dfm2@cmu.edu
 License: Free for research purposes
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyibl-5.1.3/README.md` & `pyibl-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyibl-5.1.3/pyibl.egg-info/PKG-INFO` & `pyibl-5.1.4/pyibl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyibl
-Version: 5.1.3
+Version: 5.1.4
 Summary: A Python implementation of a subset of Instance Based Learning Theory
 Home-page: http://pyibl.ddmlab.com/
 Author: Dynamic Decision Making Laboratory of Carnegie Mellon University
 Author-email: dfm2@cmu.edu
 License: Free for research purposes
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyibl-5.1.3/pyibl.py` & `pyibl-5.1.4/pyibl.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 making decisions based on its experience from prior decisions, primarily by calls to its
 :meth:`choose` and :meth:`respond` methods. The decisions an agent is choosing
 between can be further decorated with information about their current state. There are
 facilities for inspecting details of the IBL decision making process programmatically
 facilitating debugging, logging and fine grained control of complex models.
 """
 
-__version__ = "5.1.3"
+__version__ = "5.1.4"
 
 PYACTUP_MINIMUM_VERSION = "2.2.3"
 
 if "dev" in __version__:
     print("PyIBL version", __version__)
 
 import collections.abc as abc
@@ -915,15 +915,15 @@
             utilities = []
             ret_probs = []
             agg_len = len(self._aggregate_details) if self._aggregate_details is not None else None
             def do_choose(history):
                 for c, q in zip(choices, queries):
                     u = self._memory.blend("_utility", q)
                     if u is None:
-                        if self._default_utility:
+                        if self._default_utility is not None:
                             if self._callable_default_utility:
                                 u = self._default_utility(c)
                             else:
                                 u = self._default_utility
                             if self._default_utility_populates:
                                 self._at_time(0, lambda: self._memory.learn(Agent._add_utility(q, u)))
                         else:
```

### Comparing `pyibl-5.1.3/setup.py` & `pyibl-5.1.4/setup.py`

 * *Files identical despite different names*

