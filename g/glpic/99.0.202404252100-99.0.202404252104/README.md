# Comparing `tmp/glpic-99.0.202404252100.tar.gz` & `tmp/glpic-99.0.202404252104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404252100.tar", last modified: Thu Apr 25 21:00:50 2024, max compression
+gzip compressed data, was "glpic-99.0.202404252104.tar", last modified: Thu Apr 25 21:04:04 2024, max compression
```

## Comparing `glpic-99.0.202404252100.tar` & `glpic-99.0.202404252104.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:00:30.000000 glpic-99.0.202404252100/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:00:50.000000 glpic-99.0.202404252100/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:00:50.136817 glpic-99.0.202404252100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:00:49.000000 glpic-99.0.202404252100/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/setup.py
```

### Comparing `glpic-99.0.202404252100/README.md` & `glpic-99.0.202404252104/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252100/glpic/__init__.py` & `glpic-99.0.202404252104/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,18 @@
             print(msg)
         return _post(f'{self.base_url}/Reservation/{reservation}', self.headers, data)
 
     def delete_reservation(self, reservation):
         if self.debug:
             base_curl = curl_base(self.headers)
             print(f"{base_curl} -X DELETE -Lk {self.base_url}/Reservation/{reservation}")
-        return _delete(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
+        try:
+            _delete(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
+        except Exception as e:
+            error(e)
 
     def update_reservation(self, reservation, overrides):
         valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys()) + ['user']
         wrong_keys = [key for key in overrides if key not in valid_keys]
         if wrong_keys:
             error(f"Ignoring keys {','.join(wrong_keys)}")
             for key in wrong_keys:
```

### Comparing `glpic-99.0.202404252100/glpic/cli.py` & `glpic-99.0.202404252104/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252100/setup.py` & `glpic-99.0.202404252104/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404252100',
+    version='99.0.202404252104',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

