# Comparing `tmp/gtagora-connector-1.4.3.tar.gz` & `tmp/gtagora_connector-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtagora-connector-1.4.3.tar", last modified: Tue Feb 20 11:21:45 2024, max compression
+gzip compressed data, was "gtagora_connector-1.4.4.tar", last modified: Thu Apr 25 11:46:34 2024, max compression
```

## Comparing `gtagora-connector-1.4.3.tar` & `gtagora_connector-1.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.677181 gtagora-connector-1.4.3/gtagora/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/agora.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.681182 gtagora-connector-1.4.3/gtagora/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/gtagora/models/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/datafile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/exam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/import_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/parameter_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/patient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/project_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/series.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/trash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/gtagora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/gtagora_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-02-20 11:21:45.000000 gtagora-connector-1.4.3/gtagora_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-20 11:21:45.000000 gtagora-connector-1.4.3/gtagora_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 11:21:45.000000 gtagora-connector-1.4.3/gtagora_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-20 11:21:45.000000 gtagora-connector-1.4.3/gtagora_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 11:21:45.000000 gtagora-connector-1.4.3/gtagora_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 11:21:45.685181 gtagora-connector-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-02-20 11:21:38.000000 gtagora-connector-1.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.876129 gtagora_connector-1.4.4/gtagora/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/agora.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.880129 gtagora_connector-1.4.4/gtagora/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/gtagora/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/exam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/parameter_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/patient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/project_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/trash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/gtagora_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/tests/test_utils.py
```

### Comparing `gtagora-connector-1.4.3/LICENSE` & `gtagora_connector-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/PKG-INFO` & `gtagora_connector-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtagora-connector
-Version: 1.4.3
+Version: 1.4.4
 Summary: The Agora Connector for Python
 Home-page: https://github.com/gyrotools/gtagora
 Author: Martin Bührer, Felix Eichenberger
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gtagora-connector-1.4.3/README.md` & `gtagora_connector-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/agora.py` & `gtagora_connector-1.4.4/gtagora/agora.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,10 +356,14 @@
 
         if id:
             return Tag.get(id, http_client=self.http_client)
         elif name:
             tags = self.get_tags()
             return next((x for x in tags if x.label == name), None)
 
+    def create_tag(self, name, user: int=None, project=None, group: str = None, color: str = None):
+        tag = Tag(http_client=self.http_client)
+        return tag.create(name, user, project, group, color)
+
 
     def close(self):
         pass
```

### Comparing `gtagora-connector-1.4.3/gtagora/http/auth.py` & `gtagora_connector-1.4.4/gtagora/http/auth.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/http/client.py` & `gtagora_connector-1.4.4/gtagora/http/client.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/http/connection.py` & `gtagora_connector-1.4.4/gtagora/http/connection.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/base.py` & `gtagora_connector-1.4.4/gtagora/models/base.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/datafile.py` & `gtagora_connector-1.4.4/gtagora/models/datafile.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/dataset.py` & `gtagora_connector-1.4.4/gtagora/models/dataset.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/exam.py` & `gtagora_connector-1.4.4/gtagora/models/exam.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/folder.py` & `gtagora_connector-1.4.4/gtagora/models/folder.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/folder_item.py` & `gtagora_connector-1.4.4/gtagora/models/folder_item.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/group.py` & `gtagora_connector-1.4.4/gtagora/models/group.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/host.py` & `gtagora_connector-1.4.4/gtagora/models/host.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/import_package.py` & `gtagora_connector-1.4.4/gtagora/models/import_package.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/parameter_set.py` & `gtagora_connector-1.4.4/gtagora/models/parameter_set.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/patient.py` & `gtagora_connector-1.4.4/gtagora/models/patient.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/project.py` & `gtagora_connector-1.4.4/gtagora/models/project.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/series.py` & `gtagora_connector-1.4.4/gtagora/models/series.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/task.py` & `gtagora_connector-1.4.4/gtagora/models/task.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/timeline.py` & `gtagora_connector-1.4.4/gtagora/models/timeline.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/trash.py` & `gtagora_connector-1.4.4/gtagora/models/trash.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/upload_session.py` & `gtagora_connector-1.4.4/gtagora/models/upload_session.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/user.py` & `gtagora_connector-1.4.4/gtagora/models/user.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/models/version.py` & `gtagora_connector-1.4.4/gtagora/models/version.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora/utils.py` & `gtagora_connector-1.4.4/gtagora/utils.py`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/gtagora_connector.egg-info/PKG-INFO` & `gtagora_connector-1.4.4/gtagora_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtagora-connector
-Version: 1.4.3
+Version: 1.4.4
 Summary: The Agora Connector for Python
 Home-page: https://github.com/gyrotools/gtagora
 Author: Martin Bührer, Felix Eichenberger
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gtagora-connector-1.4.3/gtagora_connector.egg-info/SOURCES.txt` & `gtagora_connector-1.4.4/gtagora_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtagora-connector-1.4.3/setup.py` & `gtagora_connector-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtagora-connector",
-    version="1.4.3",
+    version="1.4.4",
     author="Martin Bührer, Felix Eichenberger",
     author_email="info@gyrotools.com",
     description="The Agora Connector for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gyrotools/gtagora",
     packages=setuptools.find_packages(),
```

### Comparing `gtagora-connector-1.4.3/tests/test_utils.py` & `gtagora_connector-1.4.4/tests/test_utils.py`

 * *Files identical despite different names*

