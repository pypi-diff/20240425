# Comparing `tmp/pyhasura-1.0.4.tar.gz` & `tmp/pyhasura-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.4.tar", last modified: Thu Apr 25 13:22:11 2024, max compression
+gzip compressed data, was "pyhasura-1.0.5.tar", last modified: Thu Apr 25 20:17:42 2024, max compression
```

## Comparing `pyhasura-1.0.4.tar` & `pyhasura-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.219079 pyhasura-1.0.4/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.4/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 13:22:11.218865 pyhasura-1.0.4/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.4/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.217671 pyhasura-1.0.4/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.4/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.4/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.4/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    13008 2024-04-19 21:13:47.000000 pyhasura-1.0.4/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 13:22:11.218581 pyhasura-1.0.4/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 13:22:11.000000 pyhasura-1.0.4/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.4/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 13:22:11.219164 pyhasura-1.0.4/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.4/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.612037 pyhasura-1.0.5/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.5/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:17:42.611825 pyhasura-1.0.5/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.5/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.610924 pyhasura-1.0.5/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.5/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.5/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.5/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    13573 2024-04-25 20:17:13.000000 pyhasura-1.0.5/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:17:42.611551 pyhasura-1.0.5/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 20:17:42.000000 pyhasura-1.0.5/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.5/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 20:17:42.612081 pyhasura-1.0.5/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.5/setup.py
```

### Comparing `pyhasura-1.0.4/LICENSE` & `pyhasura-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.4/PKG-INFO` & `pyhasura-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.4/README.md` & `pyhasura-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.4/pyhasura/flatten_dict.py` & `pyhasura-1.0.5/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.4/pyhasura/hasura_client.py` & `pyhasura-1.0.5/pyhasura/hasura_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,24 +96,26 @@
 
     _convert_output_format(output_format: str) -> Any:
         Convert the output format of the last query result.
 
     _write_to_file(output_dir: Optional[str] = None, output_format: Optional[str] = None) -> List[str]:
         Writes the last query result data to file(s) in the specified output format and directory.
     """
+
     def __init__(self, uri, role=None, admin_secret=None, output_dir='.', headers=None):
         if headers is None:
             headers = {}
         if role is not None:
             headers['x-hasura-role'] = role
         if admin_secret is not None:
             headers['x-hasura-admin-secret'] = admin_secret
         self.uri = uri
         self.admin_secret = admin_secret
-        self.client = gql_client(self.uri, headers=headers)
+        if uri is not None:
+            self.client = gql_client(self.uri, headers=headers)
         self.result = {}
         self.native_result = {}
         self.vectorized_result = {}
         self.anomalies_result = {}
         self.output_dir = output_dir
         self.result_format = None
 
@@ -139,14 +141,29 @@
         return os.path.join(self.output_dir, extension)
 
     @staticmethod
     def _write_result_as_file(file_name, result_data):
         with open(file_name, 'w') as file:
             json.dump(result_data, file, indent=4)
 
+    def set_data(self, data, output_format=ExportFormat.NATURAL):
+        """
+        Set the data for the current instance.
+
+        Args:
+            data: The data to be set for the instance.
+            output_format: The output format to be used for the data (default is ExportFormat.NATURAL).
+
+        Returns:
+            The converted data based on the specified output format.
+        """
+        self.native_result = data
+        self.result = self.native_result
+        return self.convert_output_format(output_format)
+
     def vectorize_result(self):
         """
         Vectorizes the last query result using DictVectorizer.
 
         :return: self.vectorized_result, a dictionary with the same keys as the last query, but with the values
                  transformed into dense arrays using DictVectorizer.
         """
@@ -231,14 +248,15 @@
 
         :param training_files: A dictionary of training file paths for each key in the vectorized result. If provided, the model will be loaded from the file before fitting. Default is None
         *.
         :param threshold: The threshold score below which a data point is considered an anomaly. Default is 0.
         :return: A dictionary where each key corresponds to a category in the vectorized result, and the value is a list of anomalies with scores below the threshold.
 
         """
+
         def add_score(item, index, score):
             item['__score__'] = score
             item['__index__'] = index
             return item
 
         self.anomalies_result = {}
         self.vectorize_result()
```

### Comparing `pyhasura-1.0.4/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.5/pyhasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.4/pyproject.toml` & `pyhasura-1.0.5/pyproject.toml`

 * *Files identical despite different names*

