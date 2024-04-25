# Comparing `tmp/davml-1.2.0.tar.gz` & `tmp/davml-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davml-1.2.0.tar", last modified: Wed Apr 24 17:10:07 2024, max compression
+gzip compressed data, was "davml-1.3.0.tar", last modified: Thu Apr 25 01:03:13 2024, max compression
```

## Comparing `davml-1.2.0.tar` & `davml-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-24 17:10:07.945863 davml-1.2.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      193 2024-04-24 17:10:07.945863 davml-1.2.0/PKG-INFO
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-24 17:10:07.941863 davml-1.2.0/davml/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 davml-1.2.0/davml/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1557 2024-04-24 15:50:16.000000 davml-1.2.0/davml/m1.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      817 2024-04-24 15:53:16.000000 davml-1.2.0/davml/m2.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1228 2024-04-24 15:56:24.000000 davml-1.2.0/davml/m3.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1269 2024-04-24 16:06:51.000000 davml-1.2.0/davml/m4.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1211 2024-04-24 16:51:48.000000 davml-1.2.0/davml/m5.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      674 2024-04-24 17:00:41.000000 davml-1.2.0/davml/m6.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1743 2024-04-24 17:04:19.000000 davml-1.2.0/davml/m7.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1842 2024-04-24 17:06:53.000000 davml-1.2.0/davml/m8.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1323 2024-04-24 17:07:41.000000 davml-1.2.0/davml/m9.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      642 2024-04-23 18:00:43.000000 davml-1.2.0/davml/p1.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1489 2024-04-23 18:00:57.000000 davml-1.2.0/davml/p2.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1483 2024-04-23 18:01:12.000000 davml-1.2.0/davml/p3.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1705 2024-04-23 18:01:28.000000 davml-1.2.0/davml/p4.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2024-04-23 18:01:39.000000 davml-1.2.0/davml/p5.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4111 2024-04-23 18:01:51.000000 davml-1.2.0/davml/p6.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2383 2024-04-23 18:02:06.000000 davml-1.2.0/davml/p7.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-24 17:06:33.000000 davml-1.2.0/davml/p8.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1739 2024-04-24 17:07:45.000000 davml-1.2.0/davml/program.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1702 2024-04-23 18:44:46.000000 davml-1.2.0/davml/programs.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-24 17:10:07.945863 davml-1.2.0/davml.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      193 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      441 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       68 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-04-24 17:10:07.000000 davml-1.2.0/davml.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-24 17:10:07.945863 davml-1.2.0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      461 2024-04-24 17:09:43.000000 davml-1.2.0/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-25 01:03:13.218732 davml-1.3.0/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      253 2024-04-25 01:03:13.218732 davml-1.3.0/PKG-INFO
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-25 01:03:13.214732 davml-1.3.0/davml/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 davml-1.3.0/davml/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1681 2024-04-25 01:01:21.000000 davml-1.3.0/davml/chat.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1557 2024-04-24 15:50:16.000000 davml-1.3.0/davml/m1.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      817 2024-04-24 15:53:16.000000 davml-1.3.0/davml/m2.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1228 2024-04-24 15:56:24.000000 davml-1.3.0/davml/m3.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1269 2024-04-24 16:06:51.000000 davml-1.3.0/davml/m4.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1211 2024-04-24 16:51:48.000000 davml-1.3.0/davml/m5.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      674 2024-04-24 17:00:41.000000 davml-1.3.0/davml/m6.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1743 2024-04-24 17:04:19.000000 davml-1.3.0/davml/m7.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1842 2024-04-24 17:06:53.000000 davml-1.3.0/davml/m8.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1323 2024-04-24 17:07:41.000000 davml-1.3.0/davml/m9.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      642 2024-04-23 18:00:43.000000 davml-1.3.0/davml/p1.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1489 2024-04-23 18:00:57.000000 davml-1.3.0/davml/p2.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1483 2024-04-23 18:01:12.000000 davml-1.3.0/davml/p3.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1705 2024-04-23 18:01:28.000000 davml-1.3.0/davml/p4.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2024-04-23 18:01:39.000000 davml-1.3.0/davml/p5.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4111 2024-04-23 18:01:51.000000 davml-1.3.0/davml/p6.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2383 2024-04-23 18:02:06.000000 davml-1.3.0/davml/p7.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-24 17:06:33.000000 davml-1.3.0/davml/p8.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1739 2024-04-24 17:07:45.000000 davml-1.3.0/davml/program.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1702 2024-04-23 18:44:46.000000 davml-1.3.0/davml/programs.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-25 01:03:13.214732 davml-1.3.0/davml.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      253 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      455 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       91 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-04-25 01:03:13.000000 davml-1.3.0/davml.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-25 01:03:13.218732 davml-1.3.0/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      553 2024-04-25 01:02:42.000000 davml-1.3.0/setup.py
```

### Comparing `davml-1.2.0/davml/m1.py` & `davml-1.3.0/davml/m1.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m2.py` & `davml-1.3.0/davml/m2.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m3.py` & `davml-1.3.0/davml/m3.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m4.py` & `davml-1.3.0/davml/m4.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m5.py` & `davml-1.3.0/davml/m5.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m6.py` & `davml-1.3.0/davml/m6.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m7.py` & `davml-1.3.0/davml/m7.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m8.py` & `davml-1.3.0/davml/m8.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/m9.py` & `davml-1.3.0/davml/m9.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p1.py` & `davml-1.3.0/davml/p1.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p2.py` & `davml-1.3.0/davml/p2.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p3.py` & `davml-1.3.0/davml/p3.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p4.py` & `davml-1.3.0/davml/p4.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p5.py` & `davml-1.3.0/davml/p5.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p6.py` & `davml-1.3.0/davml/p6.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/p7.py` & `davml-1.3.0/davml/p7.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/program.py` & `davml-1.3.0/davml/program.py`

 * *Files identical despite different names*

### Comparing `davml-1.2.0/davml/programs.py` & `davml-1.3.0/davml/programs.py`

 * *Files identical despite different names*

