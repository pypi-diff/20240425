# Comparing `tmp/onboard.client-1.9.3.tar.gz` & `tmp/onboard.client-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboard.client-1.9.3.tar", last modified: Wed Jul  5 17:11:49 2023, max compression
+gzip compressed data, was "onboard.client-1.9.4.tar", last modified: Fri Sep 15 19:40:04 2023, max compression
```

## Comparing `onboard.client-1.9.3.tar` & `onboard.client-1.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/
--rw-rw-r--   0 john      (1001) john      (1001)    10174 2022-11-08 18:10:09.000000 onboard.client-1.9.3/LICENSE
--rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-07-05 17:11:49.882492 onboard.client-1.9.3/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)     6477 2023-03-08 19:59:24.000000 onboard.client-1.9.3/README.md
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard/
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard/client/
--rw-rw-r--   0 john      (1001) john      (1001)      337 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/__init__.py
--rw-rw-r--   0 john      (1001) john      (1001)    10308 2023-03-29 16:59:46.000000 onboard.client-1.9.3/onboard/client/client.py
--rw-rw-r--   0 john      (1001) john      (1001)     3375 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/dataframes.py
--rw-rw-r--   0 john      (1001) john      (1001)      277 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/exceptions.py
--rw-rw-r--   0 john      (1001) john      (1001)     3722 2023-03-08 20:04:47.000000 onboard.client-1.9.3/onboard/client/helpers.py
--rw-rw-r--   0 john      (1001) john      (1001)     5789 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/models.py
--rw-rw-r--   0 john      (1001) john      (1001)        0 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/py.typed
--rw-rw-r--   0 john      (1001) john      (1001)     2954 2023-03-08 19:20:53.000000 onboard.client-1.9.3/onboard/client/staging.py
--rw-rw-r--   0 john      (1001) john      (1001)     1646 2023-03-08 18:47:59.000000 onboard.client-1.9.3/onboard/client/util.py
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard.client.egg-info/
--rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      449 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1001) john      (1001)        1 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1001) john      (1001)      126 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/requires.txt
--rw-rw-r--   0 john      (1001) john      (1001)        8 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/top_level.txt
--rw-rw-r--   0 john      (1001) john      (1001)       38 2023-07-05 17:11:49.882492 onboard.client-1.9.3/setup.cfg
--rw-rw-r--   0 john      (1001) john      (1001)     1319 2023-07-05 17:03:28.000000 onboard.client-1.9.3/setup.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-09-15 19:40:04.921791 onboard.client-1.9.4/
+-rw-rw-r--   0 john      (1001) john      (1001)    10174 2022-11-08 18:10:09.000000 onboard.client-1.9.4/LICENSE
+-rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-09-15 19:40:04.921791 onboard.client-1.9.4/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)     6477 2023-09-06 16:31:13.000000 onboard.client-1.9.4/README.md
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-09-15 19:40:04.917791 onboard.client-1.9.4/onboard/
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-09-15 19:40:04.921791 onboard.client-1.9.4/onboard/client/
+-rw-rw-r--   0 john      (1001) john      (1001)      337 2023-09-06 16:31:13.000000 onboard.client-1.9.4/onboard/client/__init__.py
+-rw-rw-r--   0 john      (1001) john      (1001)    10489 2023-09-15 19:25:36.000000 onboard.client-1.9.4/onboard/client/client.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3375 2023-09-06 16:31:13.000000 onboard.client-1.9.4/onboard/client/dataframes.py
+-rw-rw-r--   0 john      (1001) john      (1001)      277 2022-11-08 18:10:09.000000 onboard.client-1.9.4/onboard/client/exceptions.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3722 2023-09-06 16:31:13.000000 onboard.client-1.9.4/onboard/client/helpers.py
+-rw-rw-r--   0 john      (1001) john      (1001)     5811 2023-09-15 19:25:36.000000 onboard.client-1.9.4/onboard/client/models.py
+-rw-rw-r--   0 john      (1001) john      (1001)        0 2022-11-08 18:10:09.000000 onboard.client-1.9.4/onboard/client/py.typed
+-rw-rw-r--   0 john      (1001) john      (1001)     2954 2023-09-06 16:31:13.000000 onboard.client-1.9.4/onboard/client/staging.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1646 2023-09-06 16:31:13.000000 onboard.client-1.9.4/onboard/client/util.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-09-15 19:40:04.917791 onboard.client-1.9.4/onboard.client.egg-info/
+-rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-09-15 19:40:04.000000 onboard.client-1.9.4/onboard.client.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      449 2023-09-15 19:40:04.000000 onboard.client-1.9.4/onboard.client.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        1 2023-09-15 19:40:04.000000 onboard.client-1.9.4/onboard.client.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1001) john      (1001)      126 2023-09-15 19:40:04.000000 onboard.client-1.9.4/onboard.client.egg-info/requires.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        8 2023-09-15 19:40:04.000000 onboard.client-1.9.4/onboard.client.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       38 2023-09-15 19:40:04.921791 onboard.client-1.9.4/setup.cfg
+-rw-rw-r--   0 john      (1001) john      (1001)     1319 2023-09-15 19:25:36.000000 onboard.client-1.9.4/setup.py
```

### Comparing `onboard.client-1.9.3/LICENSE` & `onboard.client-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/PKG-INFO` & `onboard.client-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboard.client
-Version: 1.9.3
+Version: 1.9.4
 Summary: Onboard API SDK
 Home-page: https://github.com/onboard-data/client-py
 Author: Nathan Merritt, John Vines
 Author-email: support@onboarddata.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `onboard.client-1.9.3/README.md` & `onboard.client-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/onboard/client/client.py` & `onboard.client-1.9.4/onboard/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,20 @@
 
         @json
         def query_call():
             return self.post('/query-v2', json=query.json(), stream=True,
                              headers={'Accept': 'application/x-ndjson'})
         query_call.raw_response = True  # type: ignore[attr-defined]
 
-        point_data = PointData.__pydantic_model__.construct  # type: ignore[attr-defined]
+        try:
+            # Pydantic v1
+            point_data = PointData.__pydantic_model__.construct  # type: ignore[attr-defined]
+        except AttributeError:
+            # Pydantic v2
+            point_data = PointData.model_construct  # type: ignore[attr-defined]
 
         with query_call() as res:
             for line in res.iter_lines(chunk_size=20 * 1024):
                 parsed = loads(line)
                 yield point_data(**parsed)
 
     @json
```

### Comparing `onboard.client-1.9.3/onboard/client/dataframes.py` & `onboard.client-1.9.4/onboard/client/dataframes.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/onboard/client/helpers.py` & `onboard.client-1.9.4/onboard/client/helpers.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/onboard/client/models.py` & `onboard.client-1.9.4/onboard/client/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from datetime import datetime, timezone
 from typing import List, Optional, Union, Dict
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from pydantic import validator
+from pydantic import validator, BaseModel
 
 
 class PointDataUpdate(object):
     """Model for bulk-updating a point's data value and timestamp"""
     __slots__ = ['point_id', 'value', 'last_updated', 'first_updated']
 
     def __init__(self, point_id: int, value: Union[str, float, int],
@@ -149,13 +149,13 @@
             'selector': self.selector.json() if self.selector is not None else None,
             'point_ids': self.point_ids,
             'units': self.units,
         }
 
 
 @dataclass
-class PointData:
+class PointData(BaseModel):
     point_id: int
     raw: str
     unit: str
     columns: List[str]
     values: List[List[Union[str, float, int, None]]]
```

### Comparing `onboard.client-1.9.3/onboard/client/staging.py` & `onboard.client-1.9.4/onboard/client/staging.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/onboard/client/util.py` & `onboard.client-1.9.4/onboard/client/util.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.3/onboard.client.egg-info/PKG-INFO` & `onboard.client-1.9.4/onboard.client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboard.client
-Version: 1.9.3
+Version: 1.9.4
 Summary: Onboard API SDK
 Home-page: https://github.com/onboard-data/client-py
 Author: Nathan Merritt, John Vines
 Author-email: support@onboarddata.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `onboard.client-1.9.3/setup.py` & `onboard.client-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(name='onboard.client',
-      version='1.9.3',
+      version='1.9.4',
       author='Nathan Merritt, John Vines',
       author_email='support@onboarddata.io',
       description='Onboard API SDK',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/onboard-data/client-py',
       packages=['onboard.client'],
```

