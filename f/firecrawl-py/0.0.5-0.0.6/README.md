# Comparing `tmp/firecrawl-py-0.0.5.tar.gz` & `tmp/firecrawl-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.5.tar", last modified: Fri Apr 12 02:03:48 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.6.tar", last modified: Thu Apr 25 18:11:13 2024, max compression
```

## Comparing `firecrawl-py-0.0.5.tar` & `firecrawl-py-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 02:03:48.230082 firecrawl-py-0.0.5/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 02:03:48.229977 firecrawl-py-0.0.5/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3405 2024-04-12 01:24:06.000000 firecrawl-py-0.0.5/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 02:03:48.229197 firecrawl-py-0.0.5/firecrawl/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-12 01:00:36.000000 firecrawl-py-0.0.5/firecrawl/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     4119 2024-04-12 02:03:19.000000 firecrawl-py-0.0.5/firecrawl/firecrawl.py
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 02:03:48.229811 firecrawl-py-0.0.5/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 02:03:48.000000 firecrawl-py-0.0.5/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 02:03:48.000000 firecrawl-py-0.0.5/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 02:03:48.000000 firecrawl-py-0.0.5/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 02:03:48.000000 firecrawl-py-0.0.5/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 02:03:48.000000 firecrawl-py-0.0.5/firecrawl_py.egg-info/top_level.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 02:03:48.230126 firecrawl-py-0.0.5/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 02:03:35.000000 firecrawl-py-0.0.5/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.958743 firecrawl-py-0.0.6/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-04-25 18:11:13.958635 firecrawl-py-0.0.6/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3363 2024-04-18 02:03:35.000000 firecrawl-py-0.0.6/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.957776 firecrawl-py-0.0.6/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-15 21:00:54.000000 firecrawl-py-0.0.6/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     5168 2024-04-25 18:06:19.000000 firecrawl-py-0.0.6/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.958488 firecrawl-py-0.0.6/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-25 18:11:13.958781 firecrawl-py-0.0.6/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      346 2024-04-25 18:10:23.000000 firecrawl-py-0.0.6/setup.py
```

### Comparing `firecrawl-py-0.0.5/README.md` & `firecrawl-py-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,22 +26,20 @@
 
 # Scrape a single URL
 url = 'https://mendable.ai'
 scraped_data = app.scrape_url(url)
 
 # Crawl a website
 crawl_url = 'https://mendable.ai'
-crawl_params = {
-    'crawlerOptions': {
-        'excludes': ['blog/*'],
-        'includes': [], # leave empty for all pages
-        'limit': 1000,
+params = {
+    'pageOptions': {
+        'onlyMainContent': True
     }
 }
-crawl_result = app.crawl_url(crawl_url, params=crawl_params)
+crawl_result = app.crawl_url(crawl_url, params=params)
 ```
 
 ### Scraping a URL
 
 To scrape a single URL, use the `scrape_url` method. It takes the URL as a parameter and returns the scraped data as a dictionary.
 
 ```python
@@ -53,22 +51,25 @@
 
 To crawl a website, use the `crawl_url` method. It takes the starting URL and optional parameters as arguments. The `params` argument allows you to specify additional options for the crawl job, such as the maximum number of pages to crawl, allowed domains, and the output format.
 
 The `wait_until_done` parameter determines whether the method should wait for the crawl job to complete before returning the result. If set to `True`, the method will periodically check the status of the crawl job until it is completed or the specified `timeout` (in seconds) is reached. If set to `False`, the method will return immediately with the job ID, and you can manually check the status of the crawl job using the `check_crawl_status` method.
 
 ```python
 crawl_url = 'https://example.com'
-crawl_params = {
+params = {
     'crawlerOptions': {
         'excludes': ['blog/*'],
         'includes': [], # leave empty for all pages
         'limit': 1000,
+    },
+    'pageOptions': {
+        'onlyMainContent': True
     }
 }
-crawl_result = app.crawl_url(crawl_url, params=crawl_params, wait_until_done=True, timeout=5)
+crawl_result = app.crawl_url(crawl_url, params=params, wait_until_done=True, timeout=5)
 ```
 
 If `wait_until_done` is set to `True`, the `crawl_url` method will return the crawl result once the job is completed. If the job fails or is stopped, an exception will be raised.
 
 ### Checking Crawl Status
 
 To check the status of a crawl job, use the `check_crawl_status` method. It takes the job ID as a parameter and returns the current status of the crawl job.
```

### Comparing `firecrawl-py-0.0.5/firecrawl/firecrawl.py` & `firecrawl-py-0.0.6/firecrawl/firecrawl.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,40 @@
                 raise Exception(f'Failed to scrape URL. Error: {response["error"]}')
             
         elif response.status_code in [402, 409, 500]:
             error_message = response.json().get('error', 'Unknown error occurred')
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}. Error: {error_message}')
         else:
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}')
+        
+    def search(self, query, params=None):
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.api_key}'
+        }
+        json_data = {'query': query}
+        if params:
+            json_data.update(params)
+        response = requests.post(
+            'https://api.firecrawl.dev/v0/search',
+            headers=headers,
+            json=json_data
+        )
+        if response.status_code == 200:
+            response = response.json()
+            if response['success'] == True:
+                return response['data']
+            else:
+                raise Exception(f'Failed to search. Error: {response["error"]}')
+            
+        elif response.status_code in [402, 409, 500]:
+            error_message = response.json().get('error', 'Unknown error occurred')
+            raise Exception(f'Failed to search. Status code: {response.status_code}. Error: {error_message}')
+        else:
+            raise Exception(f'Failed to search. Status code: {response.status_code}')
 
     def crawl_url(self, url, params=None, wait_until_done=True, timeout=2):
         headers = self._prepare_headers()
         json_data = {'url': url}
         if params:
             json_data.update(params)
         response = self._post_request('https://api.firecrawl.dev/v0/crawl', json_data, headers)
```

