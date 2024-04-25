# Comparing `tmp/brynq_sdk_successfactors-0.1.0.tar.gz` & `tmp/brynq_sdk_successfactors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_successfactors-0.1.0.tar", last modified: Wed Apr 17 12:47:18 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_successfactors-0.1.1.tar", last modified: Thu Apr 25 11:26:46 2024, max compression
```

## Comparing `brynq_sdk_successfactors-0.1.0.tar` & `brynq_sdk_successfactors-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk/successfactors/
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-17 12:47:01.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk/successfactors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-04-17 12:47:01.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk/successfactors/get_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      368 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/brynq_sdk_successfactors.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 12:47:18.000000 brynq_sdk_successfactors-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-17 12:47:01.000000 brynq_sdk_successfactors-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk/successfactors/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-25 11:26:27.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk/successfactors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-25 11:26:27.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk/successfactors/get_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      368 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/brynq_sdk_successfactors.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 11:26:46.000000 brynq_sdk_successfactors-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-25 11:26:27.000000 brynq_sdk_successfactors-0.1.1/setup.py
```

### Comparing `brynq_sdk_successfactors-0.1.0/brynq_sdk/successfactors/get_data.py` & `brynq_sdk_successfactors-0.1.1/brynq_sdk/successfactors/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         return base_url, headers
 
     @staticmethod
     def _convert_date_columns(df):
         max_timestamp = pd.Timestamp.max.value // 10**6
         for col in df.columns:
-            if df[col].dtype == 'object':  # if the column is of object type
+            if df[col].dtype == 'object' and df[col].apply(lambda x: isinstance(x, str)).any():  # if the column is of object type
                 # Check if any cell in the column matches the pattern
                 if df[col].str.contains(r'/Date\(\d+(\+\d+)?\)/', regex=True).any():
                     # Extract the timestamp and convert it to datetime
                     df[col] = df[col].str.extract(r'(\d+)', expand=False).astype('float')
                     # If timestamp is too large, set value to None
                     df[col] = df[col].apply(lambda x: pd.to_datetime(x, unit='ms') if x <= max_timestamp else None)
         return df
```

