# Comparing `tmp/glpic-99.0.202404252104.tar.gz` & `tmp/glpic-99.0.202404252106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404252104.tar", last modified: Thu Apr 25 21:04:04 2024, max compression
+gzip compressed data, was "glpic-99.0.202404252106.tar", last modified: Thu Apr 25 21:06:51 2024, max compression
```

## Comparing `glpic-99.0.202404252104.tar` & `glpic-99.0.202404252106.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:03:52.000000 glpic-99.0.202404252104/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:04:04.989731 glpic-99.0.202404252104/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:04:04.000000 glpic-99.0.202404252104/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:51.203957 glpic-99.0.202404252106/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:06:51.203957 glpic-99.0.202404252106/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:06:38.000000 glpic-99.0.202404252106/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:51.203957 glpic-99.0.202404252106/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-25 21:06:38.000000 glpic-99.0.202404252106/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:06:38.000000 glpic-99.0.202404252106/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:06:51.203957 glpic-99.0.202404252106/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:06:51.207957 glpic-99.0.202404252106/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:06:51.000000 glpic-99.0.202404252106/setup.py
```

### Comparing `glpic-99.0.202404252104/README.md` & `glpic-99.0.202404252106/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252104/glpic/__init__.py` & `glpic-99.0.202404252106/glpic/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,42 +50,53 @@
                         value[index] = v
             overrides[key] = value
     return overrides
 
 
 def _delete(url, headers):
     request = Request(url, headers=headers, method='DELETE')
-    return urlopen(request)
+    try:
+        return urlopen(request)
+    except Exception as e:
+        error(e)
 
 
 def _get(url, headers):
     if not os.path.basename(url).split('?')[0].isnumeric():
         encoded_params = urlencode({"range": '0-9999'})
         delimiter = '&' if '?' in url else '?'
         url += f'{delimiter}{encoded_params}'
-    request = Request(url, headers=headers)
-    return json.loads(urlopen(request).read())
+    try:
+        return json.loads(urlopen(Request(url, headers=headers)).read())
+    except Exception as e:
+        error(e)
 
 
 def _patch(url, headers, data):
     data = json.dumps(data).encode('utf-8')
-    request = Request(url, data=data, headers=headers, method='PATCH')
-    return urlopen(request)
+    try:
+        return urlopen(Request(url, data=data, headers=headers, method='PATCH'))
+    except Exception as e:
+        error(e)
 
 
 def _post(url, headers, data):
     data = json.dumps(data).encode('utf-8')
-    request = Request(url, data=data, headers=headers, method='POST')
-    return urlopen(request)
+    try:
+        return urlopen(Request(url, data=data, headers=headers, method='POST'))
+    except Exception as e:
+        error(e)
 
 
 def _put(url, headers, data):
     data = json.dumps(data).encode('utf-8')
-    request = Request(url, data=data, headers=headers, method='PUT')
-    return urlopen(request)
+    try:
+        return urlopen(Request(url, data=data, headers=headers, method='PUT'))
+    except Exception as e:
+        error(e)
 
 
 def error(text):
     color = "31"
     print(f'\033[0;{color}m{text}\033[0;0m')
 
 
@@ -221,18 +232,15 @@
             print(msg)
         return _post(f'{self.base_url}/Reservation/{reservation}', self.headers, data)
 
     def delete_reservation(self, reservation):
         if self.debug:
             base_curl = curl_base(self.headers)
             print(f"{base_curl} -X DELETE -Lk {self.base_url}/Reservation/{reservation}")
-        try:
-            _delete(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
-        except Exception as e:
-            error(e)
+        return _delete(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
 
     def update_reservation(self, reservation, overrides):
         valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys()) + ['user']
         wrong_keys = [key for key in overrides if key not in valid_keys]
         if wrong_keys:
             error(f"Ignoring keys {','.join(wrong_keys)}")
             for key in wrong_keys:
```

### Comparing `glpic-99.0.202404252104/glpic/cli.py` & `glpic-99.0.202404252106/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252104/setup.py` & `glpic-99.0.202404252106/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404252104',
+    version='99.0.202404252106',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

