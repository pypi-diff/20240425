# Comparing `tmp/propertree-1.1.0.post4.tar.gz` & `tmp/propertree-1.1.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propertree-1.1.0.post4.tar", last modified: Sun Apr 21 17:06:57 2024, max compression
+gzip compressed data, was "propertree-1.1.0.post5.tar", last modified: Thu Apr 25 16:34:31 2024, max compression
```

## Comparing `propertree-1.1.0.post4.tar` & `propertree-1.1.0.post5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    10142 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/LICENSE
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4370 2024-03-27 20:33:51.000000 propertree-1.1.0.post4/README.md
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/examples/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1509 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/examples/checks.yaml
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1362 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/examples/checks2.yaml
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/propertree/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      730 2024-02-19 20:07:39.000000 propertree-1.1.0.post4/propertree/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1063 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/propertree/log.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    28218 2024-04-19 13:24:06.000000 propertree-1.1.0.post4/propertree/propertree.py
--rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    76049 2024-04-19 13:27:47.000000 propertree-1.1.0.post4/propertree/propertree2.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/propertree.egg-info/
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4648 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      566 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/SOURCES.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/dependency_links.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       47 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/requires.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       31 2024-04-21 17:06:57.000000 propertree-1.1.0.post4/propertree.egg-info/top_level.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      723 2024-04-21 17:06:48.000000 propertree-1.1.0.post4/pyproject.toml
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      118 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/setup.cfg
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       55 2023-08-29 19:53:10.000000 propertree-1.1.0.post4/setup.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/tests/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/tests/__init__.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:06:57.074092 propertree-1.1.0.post4/tests/unit/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      582 2023-02-09 15:05:05.000000 propertree-1.1.0.post4/tests/unit/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     7788 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/properties.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    15866 2024-04-19 13:19:06.000000 propertree-1.1.0.post4/tests/unit/test_ptree.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    53580 2024-04-19 13:18:49.000000 propertree-1.1.0.post4/tests/unit/test_ptree2.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     8697 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/test_ptree_basic.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    16820 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/test_ptree_mapped_properties.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      989 2024-03-27 13:10:41.000000 propertree-1.1.0.post4/tests/unit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10142 2023-03-12 12:35:32.000000 propertree-1.1.0.post5/LICENSE
+-rw-r--r--   0 user1     (1000) user1     (1000)     4648 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4370 2024-04-08 22:28:24.000000 propertree-1.1.0.post5/README.md
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/examples/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1509 2023-03-12 12:35:32.000000 propertree-1.1.0.post5/examples/checks.yaml
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1362 2024-02-16 17:17:42.000000 propertree-1.1.0.post5/examples/checks2.yaml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/propertree/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      730 2023-03-12 12:35:32.000000 propertree-1.1.0.post5/propertree/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1051 2024-04-25 16:32:14.000000 propertree-1.1.0.post5/propertree/log.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    28218 2024-04-22 09:54:25.000000 propertree-1.1.0.post5/propertree/propertree.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    76049 2024-04-22 09:54:25.000000 propertree-1.1.0.post5/propertree/propertree2.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/propertree.egg-info/
+-rw-r--r--   0 user1     (1000) user1     (1000)     4648 2024-04-25 16:34:31.000000 propertree-1.1.0.post5/propertree.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      566 2024-04-25 16:34:31.000000 propertree-1.1.0.post5/propertree.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-25 16:34:31.000000 propertree-1.1.0.post5/propertree.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       47 2024-04-25 16:34:31.000000 propertree-1.1.0.post5/propertree.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       31 2024-04-25 16:34:31.000000 propertree-1.1.0.post5/propertree.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      723 2024-04-08 22:28:24.000000 propertree-1.1.0.post5/pyproject.toml
+-rw-rw-r--   0 user1     (1000) user1     (1000)      118 2024-04-25 16:34:31.881350 propertree-1.1.0.post5/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       55 2023-07-26 09:52:32.000000 propertree-1.1.0.post5/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-03-12 12:35:32.000000 propertree-1.1.0.post5/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:31.877349 propertree-1.1.0.post5/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      582 2023-03-12 12:35:32.000000 propertree-1.1.0.post5/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7788 2024-03-25 10:38:03.000000 propertree-1.1.0.post5/tests/unit/properties.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    15866 2024-04-22 09:54:25.000000 propertree-1.1.0.post5/tests/unit/test_ptree.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    53580 2024-04-22 09:54:25.000000 propertree-1.1.0.post5/tests/unit/test_ptree2.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8697 2024-03-25 10:38:03.000000 propertree-1.1.0.post5/tests/unit/test_ptree_basic.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    16820 2024-03-25 10:38:03.000000 propertree-1.1.0.post5/tests/unit/test_ptree_mapped_properties.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      989 2024-03-25 10:38:03.000000 propertree-1.1.0.post5/tests/unit/utils.py
```

### Comparing `propertree-1.1.0.post4/LICENSE` & `propertree-1.1.0.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/PKG-INFO` & `propertree-1.1.0.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertree
-Version: 1.1.0.post4
+Version: 1.1.0.post5
 Summary: Library to help create meaningful structures from yaml or json.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 
 # Propertree
```

### Comparing `propertree-1.1.0.post4/README.md` & `propertree-1.1.0.post5/README.md`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/examples/checks.yaml` & `propertree-1.1.0.post5/examples/checks.yaml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/examples/checks2.yaml` & `propertree-1.1.0.post5/examples/checks2.yaml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/propertree/__init__.py` & `propertree-1.1.0.post5/propertree/__init__.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/propertree/log.py` & `propertree-1.1.0.post5/propertree/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 
 log = logging.getLogger('propertree')
-format = ("%(asctime)s.%(msecs)03d %(process)d %(levelname)s %(name)s [-] "  # noqa, pylint: disable=W0622
+format = ("%(asctime)s %(process)d %(levelname)s %(name)s [-] "  # noqa, pylint: disable=W0622
           "%(message)s")
 
 if not log.hasHandlers():
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter(format))
     log.addHandler(handler)
```

### Comparing `propertree-1.1.0.post4/propertree/propertree.py` & `propertree-1.1.0.post5/propertree/propertree.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/propertree/propertree2.py` & `propertree-1.1.0.post5/propertree/propertree2.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/propertree.egg-info/PKG-INFO` & `propertree-1.1.0.post5/propertree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertree
-Version: 1.1.0.post4
+Version: 1.1.0.post5
 Summary: Library to help create meaningful structures from yaml or json.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 
 # Propertree
```

### Comparing `propertree-1.1.0.post4/propertree.egg-info/SOURCES.txt` & `propertree-1.1.0.post5/propertree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/pyproject.toml` & `propertree-1.1.0.post5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/__init__.py` & `propertree-1.1.0.post5/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/properties.py` & `propertree-1.1.0.post5/tests/unit/properties.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/test_ptree.py` & `propertree-1.1.0.post5/tests/unit/test_ptree.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/test_ptree2.py` & `propertree-1.1.0.post5/tests/unit/test_ptree2.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/test_ptree_basic.py` & `propertree-1.1.0.post5/tests/unit/test_ptree_basic.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/test_ptree_mapped_properties.py` & `propertree-1.1.0.post5/tests/unit/test_ptree_mapped_properties.py`

 * *Files identical despite different names*

### Comparing `propertree-1.1.0.post4/tests/unit/utils.py` & `propertree-1.1.0.post5/tests/unit/utils.py`

 * *Files identical despite different names*

