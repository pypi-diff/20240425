# Comparing `tmp/sideseeing_tools-0.1.7.tar.gz` & `tmp/sideseeing_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing_tools-0.1.7.tar", last modified: Wed Apr 24 17:52:24 2024, max compression
+gzip compressed data, was "sideseeing_tools-0.2.0.tar", last modified: Wed Apr 24 23:30:08 2024, max compression
```

## Comparing `sideseeing_tools-0.1.7.tar` & `sideseeing_tools-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5582 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4670 2024-04-24 17:50:34.000000 sideseeing_tools-0.1.7/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      901 2024-04-24 16:06:08.000000 sideseeing_tools-0.1.7/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3655 2024-04-24 17:31:46.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-22 21:11:00.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/plot.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8748 2024-04-24 17:02:21.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     7397 2024-04-22 21:27:31.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5582 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      497 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      152 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/top_level.txt
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/tests/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      114 2024-04-24 16:01:51.000000 sideseeing_tools-0.1.7/tests/test_media.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.0/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11690 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    10778 2024-04-24 23:29:33.000000 sideseeing_tools-0.2.0/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      901 2024-04-24 21:08:29.000000 sideseeing_tools-0.2.0/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2830 2024-04-24 21:04:42.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-22 21:11:00.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/plot.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     9507 2024-04-24 22:03:17.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8178 2024-04-24 22:11:35.000000 sideseeing_tools-0.2.0/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11690 2024-04-24 23:30:08.000000 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      497 2024-04-24 23:30:08.000000 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-24 23:30:08.000000 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      152 2024-04-24 23:30:08.000000 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-24 23:30:08.000000 sideseeing_tools-0.2.0/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:30:08.134115 sideseeing_tools-0.2.0/tests/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      114 2024-04-24 16:01:51.000000 sideseeing_tools-0.2.0/tests/test_media.py
```

### Comparing `sideseeing_tools-0.1.7/LICENSE` & `sideseeing_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.7/pyproject.toml` & `sideseeing_tools-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sideseeing-tools"
-version = "0.1.7"
+version = "0.2.0"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `sideseeing_tools-0.1.7/src/sideseeing_tools/constants.py` & `sideseeing_tools-0.2.0/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.7/src/sideseeing_tools/plot.py` & `sideseeing_tools-0.2.0/src/sideseeing_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.7/src/sideseeing_tools/sideseeing.py` & `sideseeing_tools-0.2.0/src/sideseeing_tools/sideseeing.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,7 +234,29 @@
                 self.label = utils.load_csv_data(v.file_path, fieldnames=constants.LABELS_FILE_FIELDNAMES)
 
             if k == 'video':
                 self.video = v.file_path
                 if extract_media:
                     self.audio = media.extract_audio(v.file_path, v.file_path.replace('.mp4', '.wav'))
                     self.gif = media.extract_gif(v.file_path, v.file_path.replace('.mp4', '.gif'))
+
+    def extract_snippet(self, start_time, end_time, output_dir):
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+
+        sensor_dicts = [self.sensors1, self.sensors3, self.sensors6]
+
+        for sensor_dict in sensor_dicts:
+            for s, sensor in sensor_dict.items():
+                utils.extract_sensor_snippet(
+                    sensor,
+                    start_time,
+                    end_time,
+                    output_path=os.path.join(output_dir, f'{s.lower()}_{start_time}_{end_time}.csv')
+                )
+
+        media.extract_video_snippet(
+            self.video, 
+            start_time, 
+            end_time, 
+            os.path.join(output_dir, f'video_{start_time}_{end_time}.mp4'),
+        )
```

### Comparing `sideseeing_tools-0.1.7/src/sideseeing_tools/utils.py` & `sideseeing_tools-0.2.0/src/sideseeing_tools/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -235,7 +235,29 @@
             if 'country' in i.get('types'):
                 data['country'] = i.get('long_name')
 
             if 'administrative_area_level_2' in i.get('types'):
                 data['city'] = i.get('long_name')
 
     return data
+
+
+def extract_sensor_snippet(data: pd.DataFrame, start_time, end_time, output_path):
+    if data.empty:
+        print('ERROR. The input DataFrame is empty.')
+        return None
+    
+    required_columns = ['Time (s)',]
+    for col in required_columns:
+        if col not in data.columns:
+            print(f"ERROR. Column '{col}' is not present in the DataFrame.")
+            return None
+    
+    if not ((start_time >= data['Time (s)'].min()) and (end_time <= data['Time (s)'].max())):
+        print('ERROR. The specified time range is outside the data range.')
+        return None
+    
+    snippet = data[(data['Time (s)'] >= start_time) & (data['Time (s)'] <= end_time)]
+    
+    snippet.to_csv(output_path, sep=',', columns=data.columns, index=False)
+    
+    return snippet
```

