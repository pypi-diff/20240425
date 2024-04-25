# Comparing `tmp/Flask-Compress-1.8.0.tar.gz` & `tmp/Flask-Compress-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Compress-1.8.0.tar", last modified: Tue Nov  3 13:25:41 2020, max compression
+gzip compressed data, was "Flask-Compress-1.9.0.tar", last modified: Wed Feb 17 07:52:11 2021, max compression
```

## Comparing `Flask-Compress-1.8.0.tar` & `Flask-Compress-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-11-03 13:25:41.266460 Flask-Compress-1.8.0/
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-11-03 13:25:41.265460 Flask-Compress-1.8.0/Flask_Compress.egg-info/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     7477 2020-11-03 13:25:41.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/PKG-INFO
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      406 2020-11-03 13:25:41.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/SOURCES.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2020-11-03 13:25:41.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/dependency_links.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2020-04-21 07:42:34.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/not-zip-safe
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       13 2020-11-03 13:25:41.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/requires.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       15 2020-11-03 13:25:41.000000 Flask-Compress-1.8.0/Flask_Compress.egg-info/top_level.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     1085 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/LICENSE.txt
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       94 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/MANIFEST.in
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     7477 2020-11-03 13:25:41.266460 Flask-Compress-1.8.0/PKG-INFO
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     5485 2020-11-02 08:38:17.000000 Flask-Compress-1.8.0/README.md
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     8829 2020-11-03 08:34:40.000000 Flask-Compress-1.8.0/flask_compress.py
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       38 2020-11-03 13:25:41.266460 Flask-Compress-1.8.0/setup.cfg
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)     1403 2020-11-03 13:20:11.000000 Flask-Compress-1.8.0/setup.py
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-11-03 13:25:41.265460 Flask-Compress-1.8.0/tests/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)        0 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/tests/__init__.py
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-11-03 13:25:41.266460 Flask-Compress-1.8.0/tests/static/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      239 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/tests/static/1.png
-drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-11-03 13:25:41.266460 Flask-Compress-1.8.0/tests/templates/
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)      507 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/tests/templates/large.html
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)       45 2020-04-21 07:38:27.000000 Flask-Compress-1.8.0/tests/templates/small.html
--rw-r--r--   0 osboxes   (1000) osboxes   (1000)    13908 2020-11-02 08:38:17.000000 Flask-Compress-1.8.0/tests/test_flask_compress.py
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2021-02-17 07:52:11.760740 Flask-Compress-1.9.0/
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2021-02-17 07:52:11.758741 Flask-Compress-1.9.0/Flask_Compress.egg-info/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     7491 2021-02-17 07:52:11.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/PKG-INFO
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      406 2021-02-17 07:52:11.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/SOURCES.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2021-02-17 07:52:11.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/dependency_links.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        1 2020-04-21 07:42:34.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/not-zip-safe
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       13 2021-02-17 07:52:11.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/requires.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       15 2021-02-17 07:52:11.000000 Flask-Compress-1.9.0/Flask_Compress.egg-info/top_level.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     1085 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/LICENSE.txt
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       94 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/MANIFEST.in
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     7491 2021-02-17 07:52:11.758741 Flask-Compress-1.9.0/PKG-INFO
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     5499 2021-02-17 07:51:15.000000 Flask-Compress-1.9.0/README.md
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     9012 2021-02-17 07:51:15.000000 Flask-Compress-1.9.0/flask_compress.py
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       38 2021-02-17 07:52:11.760740 Flask-Compress-1.9.0/setup.cfg
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)     1403 2021-02-17 07:51:15.000000 Flask-Compress-1.9.0/setup.py
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2021-02-17 07:52:11.758741 Flask-Compress-1.9.0/tests/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)        0 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/tests/__init__.py
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2021-02-17 07:52:11.758741 Flask-Compress-1.9.0/tests/static/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      239 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/tests/static/1.png
+drwxr-xr-x   0 osboxes   (1000) osboxes   (1000)        0 2021-02-17 07:52:11.758741 Flask-Compress-1.9.0/tests/templates/
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)      507 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/tests/templates/large.html
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)       45 2020-04-21 07:38:27.000000 Flask-Compress-1.9.0/tests/templates/small.html
+-rw-r--r--   0 osboxes   (1000) osboxes   (1000)    14888 2021-02-17 07:51:15.000000 Flask-Compress-1.9.0/tests/test_flask_compress.py
```

### Comparing `Flask-Compress-1.8.0/Flask_Compress.egg-info/PKG-INFO` & `Flask-Compress-1.9.0/Flask_Compress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Compress
-Version: 1.8.0
+Version: 1.9.0
 Summary: Compress responses in your Flask app with gzip, deflate or brotli.
 Home-page: https://github.com/colour-science/flask-compress
 Author: Thomas Mansencal
 Author-email: thomas.mansencal@gmail.com
 License: MIT
 Description: # Flask-Compress
         
@@ -35,21 +35,21 @@
         
         
         ## Installation
         
         If you use pip then installation is simply:
         
         ```shell
-        $ pip install flask-compress
+        $ pip install --user flask-compress
         ```
         
         or, if you want the latest github version:
         
         ```shell
-        $ pip install git+git://github.com/colour-science/flask-compress.git
+        $ pip install --user git+git://github.com/colour-science/flask-compress.git
         ```
         
         You can also install Flask-Compress via Easy Install:
         
         ```shell
         $ easy_install flask-compress
         ```
```

### Comparing `Flask-Compress-1.8.0/LICENSE.txt` & `Flask-Compress-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-Compress-1.8.0/PKG-INFO` & `Flask-Compress-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Compress
-Version: 1.8.0
+Version: 1.9.0
 Summary: Compress responses in your Flask app with gzip, deflate or brotli.
 Home-page: https://github.com/colour-science/flask-compress
 Author: Thomas Mansencal
 Author-email: thomas.mansencal@gmail.com
 License: MIT
 Description: # Flask-Compress
         
@@ -35,21 +35,21 @@
         
         
         ## Installation
         
         If you use pip then installation is simply:
         
         ```shell
-        $ pip install flask-compress
+        $ pip install --user flask-compress
         ```
         
         or, if you want the latest github version:
         
         ```shell
-        $ pip install git+git://github.com/colour-science/flask-compress.git
+        $ pip install --user git+git://github.com/colour-science/flask-compress.git
         ```
         
         You can also install Flask-Compress via Easy Install:
         
         ```shell
         $ easy_install flask-compress
         ```
```

### Comparing `Flask-Compress-1.8.0/README.md` & `Flask-Compress-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 
 
 ## Installation
 
 If you use pip then installation is simply:
 
 ```shell
-$ pip install flask-compress
+$ pip install --user flask-compress
 ```
 
 or, if you want the latest github version:
 
 ```shell
-$ pip install git+git://github.com/colour-science/flask-compress.git
+$ pip install --user git+git://github.com/colour-science/flask-compress.git
 ```
 
 You can also install Flask-Compress via Easy Install:
 
 ```shell
 $ easy_install flask-compress
 ```
```

### Comparing `Flask-Compress-1.8.0/flask_compress.py` & `Flask-Compress-1.9.0/flask_compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.cache = backend() if backend else None
         self.cache_key = app.config['COMPRESS_CACHE_KEY']
 
         algo = app.config['COMPRESS_ALGORITHM']
         if isinstance(algo, str):
             self.enabled_algorithms = [i.strip() for i in algo.split(',')]
         else:
-            self.enabled_algorithms = algo
+            self.enabled_algorithms = list(algo)
 
         if (app.config['COMPRESS_REGISTER'] and
                 app.config['COMPRESS_MIMETYPES']):
             app.after_request(self.after_request)
 
     def _choose_compress_algorithm(self, accept_encoding_header):
         """
@@ -104,62 +104,66 @@
         algorithms, together with a "quality factor" for each one (higher quality
         means the client prefers that algorithm more).
 
         :param accept_encoding_header: Content of the `Accept-Encoding` header
         :return: name of a compression algorithm (`gzip`, `deflate`, `br`) or `None` if
             the client and server don't agree on any.
         """
-        # Map quality factors to requested algorithm names.
-        algos_by_quality = defaultdict(set)
-
         # A flag denoting that client requested using any (`*`) algorithm,
         # in case a specific one is not supported by the server
         fallback_to_any = False
 
+        # Map quality factors to requested algorithm names.
+        algos_by_quality = defaultdict(set)
+
+        # Set of supported algorithms
+        server_algos_set = set(self.enabled_algorithms)
+
         for part in accept_encoding_header.lower().split(','):
             part = part.strip()
-            quality = 1.0
-
             if ';q=' in part:
                 # If the client associated a quality factor with an algorithm,
                 # try to parse it. We could do the matching using a regex, but
                 # the format is so simple that it would be overkill.
                 algo = part.split(';')[0].strip()
                 try:
                     quality = float(part.split('=')[1].strip())
                 except ValueError:
-                    pass
+                    quality = 1.0
             else:
                 # Otherwise, use the default quality
                 algo = part
+                quality = 1.0
 
-            algos_by_quality[quality].add(algo)
-            fallback_to_any = fallback_to_any or (algo == '*')
+            if algo == '*':
+                if quality > 0:
+                    fallback_to_any = True
+            elif algo == 'identity':  # identity means 'no compression asked'
+                algos_by_quality[quality].add(None)
+            elif algo in server_algos_set:
+                algos_by_quality[quality].add(algo)
 
         # Choose the algorithm with the highest quality factor that the server supports.
         #
         # If there are multiple equally good options, choose the first supported algorithm
         # from server configuration.
         #
         # If the server doesn't support any algorithm that the client requested but
         # there's a special wildcard algorithm request (`*`), choose the first supported
         # algorithm.
-        server_algo_set = set(self.enabled_algorithms)
-        for _, requested_algo_set in sorted(algos_by_quality.items(), reverse=True):
-            viable_algos = server_algo_set & requested_algo_set
+        for _, viable_algos in sorted(algos_by_quality.items(), reverse=True):
             if len(viable_algos) == 1:
                 return viable_algos.pop()
             elif len(viable_algos) > 1:
                 for server_algo in self.enabled_algorithms:
                     if server_algo in viable_algos:
                         return server_algo
-        else:
-            if fallback_to_any:
-                return self.enabled_algorithms[0]
 
+        if fallback_to_any:
+            return self.enabled_algorithms[0]
         return None
 
     def after_request(self, response):
         app = self.app or current_app
 
         accept_encoding = request.headers.get('Accept-Encoding', '')
         chosen_algorithm = self._choose_compress_algorithm(accept_encoding)
```

### Comparing `Flask-Compress-1.8.0/setup.py` & `Flask-Compress-1.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as fl:
     LONG_DESCRIPTION = fl.read()
 
 setuptools.setup(
     name='Flask-Compress',
-    version='1.8.0',
+    version='1.9.0',
     url='https://github.com/colour-science/flask-compress',
     license='MIT',
     author='Thomas Mansencal',
     author_email='thomas.mansencal@gmail.com',
     description='Compress responses in your Flask app with gzip, deflate or brotli.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `Flask-Compress-1.8.0/tests/test_flask_compress.py` & `Flask-Compress-1.9.0/tests/test_flask_compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,35 @@
     def test_default_wildcard_quality_is_0(self):
         """ Tests that a wildcard has a default q-factor of 0.0 """
         accept_encoding = 'br;q=0.001, *'
         self.app.config['COMPRESS_ALGORITHM'] = ['gzip', 'br', 'deflate']
         c = Compress(self.app)
         self.assertEqual(c._choose_compress_algorithm(accept_encoding), 'br')
 
+    def test_wildcard_quality(self):
+        """ Tests that a wildcard with q=0 is discarded """
+        accept_encoding = '*;q=0'
+        self.app.config['COMPRESS_ALGORITHM'] = ['gzip', 'br', 'deflate']
+        c = Compress(self.app)
+        self.assertEqual(c._choose_compress_algorithm(accept_encoding), None)
+
+    def test_identity(self):
+        """ Tests that identity is understood """
+        accept_encoding = 'identity;q=1, br;q=0.5, *;q=0'
+        self.app.config['COMPRESS_ALGORITHM'] = ['gzip', 'br', 'deflate']
+        c = Compress(self.app)
+        self.assertEqual(c._choose_compress_algorithm(accept_encoding), None)
+
+    def test_chrome_ranged_requests(self):
+        """ Tests that Chrome ranged requests behave as expected """
+        accept_encoding = 'identity;q=1, *;q=0'
+        self.app.config['COMPRESS_ALGORITHM'] = ['gzip', 'br', 'deflate']
+        c = Compress(self.app)
+        self.assertEqual(c._choose_compress_algorithm(accept_encoding), None)
+
     def test_content_encoding_is_correct(self):
         """ Test that the `Content-Encoding` header matches the compression algorithm """
         self.app.config['COMPRESS_ALGORITHM'] = ['br', 'gzip', 'deflate']
         Compress(self.app)
 
         headers_gzip = [('Accept-Encoding', 'gzip')]
         client = self.app.test_client()
```

