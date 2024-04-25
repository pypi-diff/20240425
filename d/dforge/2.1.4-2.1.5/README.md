# Comparing `tmp/dforge-2.1.4.tar.gz` & `tmp/dforge-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dforge-2.1.4.tar", last modified: Tue Apr 23 12:40:29 2024, max compression
+gzip compressed data, was "dforge-2.1.5.tar", last modified: Thu Apr 25 10:45:53 2024, max compression
```

## Comparing `dforge-2.1.4.tar` & `dforge-2.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:40:29.264623 dforge-2.1.4/
--rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.4/LICENSE
--rw-rw-rw-   0        0        0     3286 2024-04-23 12:40:29.264623 dforge-2.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 12:40:29.224614 dforge-2.1.4/dforge/
--rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.4/dforge/__init__.py
--rw-rw-rw-   0        0        0    27643 2024-04-23 12:39:08.000000 dforge-2.1.4/dforge/core.py
--rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.4/dforge/plotData.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:40:29.260631 dforge-2.1.4/dforge.egg-info/
--rw-rw-rw-   0        0        0     3286 2024-04-23 12:40:29.000000 dforge-2.1.4/dforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-23 12:40:29.000000 dforge-2.1.4/dforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:40:29.000000 dforge-2.1.4/dforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-23 12:40:29.000000 dforge-2.1.4/dforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 12:40:29.000000 dforge-2.1.4/dforge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 12:40:29.268625 dforge-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-23 12:40:20.000000 dforge-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:45:53.158080 dforge-2.1.5/
+-rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3286 2024-04-25 10:45:53.154088 dforge-2.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 10:45:53.110068 dforge-2.1.5/dforge/
+-rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.5/dforge/__init__.py
+-rw-rw-rw-   0        0        0    28726 2024-04-25 10:42:10.000000 dforge-2.1.5/dforge/core.py
+-rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.5/dforge/plotData.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:45:53.154088 dforge-2.1.5/dforge.egg-info/
+-rw-rw-rw-   0        0        0     3286 2024-04-25 10:45:52.000000 dforge-2.1.5/dforge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-25 10:45:52.000000 dforge-2.1.5/dforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:45:52.000000 dforge-2.1.5/dforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-25 10:45:52.000000 dforge-2.1.5/dforge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 10:45:52.000000 dforge-2.1.5/dforge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:45:53.158080 dforge-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-25 10:44:07.000000 dforge-2.1.5/setup.py
```

### Comparing `dforge-2.1.4/LICENSE` & `dforge-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dforge-2.1.4/PKG-INFO` & `dforge-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.4
+Version: 2.1.5
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.4/dforge/core.py` & `dforge-2.1.5/dforge/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,8 +543,31 @@
             label_column (str): The name of label columns for creating the folds.
         """
         skf = StratifiedKFold(n_splits=nr_folds, shuffle=True, random_state=42) 
         self.dataframe["fold"] = -1  
         for fold, (train_idx, val_idx) in enumerate(skf.split(self.dataframe, self.dataframe[label_column])):
             self.dataframe.loc[val_idx, 'fold'] = fold
 
+    def add_columns(self, column_names, values, default_value=None):
+        if isinstance(column_names, str):
+            column_names = [column_names]
+
+        if not isinstance(values, list):
+            values = [[values]] * len(column_names)
+        else:
+            if len(column_names) != len(values):
+                raise ValueError("Length of column_names and values must be the same.")
+            # Ensure values are lists
+            values = [[value] if not isinstance(value, list) else value for value in values]
+
+        for col_name, col_values in zip(column_names, values):
+            if len(col_values) == 1:
+                value = col_values[0]
+                if default_value is not None and value is None:
+                    value = default_value
+                self.dataframe[col_name] = value
+            else:
+                if len(col_values) != len(self.dataframe):
+                    raise ValueError("Length of values must match the number of rows in the DataFrame.")
+                self.dataframe[col_name] = col_values
+
```

### Comparing `dforge-2.1.4/dforge/plotData.py` & `dforge-2.1.5/dforge/plotData.py`

 * *Files identical despite different names*

### Comparing `dforge-2.1.4/dforge.egg-info/PKG-INFO` & `dforge-2.1.5/dforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.4
+Version: 2.1.5
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.4/setup.py` & `dforge-2.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dforge',
-    version='2.1.4',
+    version='2.1.5',
     packages=find_packages(),
     author='Luiza Rusnac',
     author_email='luiza.rusnac93@gmail.com',
     description='A package for efortless data manager.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/LuizaRusnac/dforge.git',
```

