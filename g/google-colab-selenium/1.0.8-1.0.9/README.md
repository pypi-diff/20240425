# Comparing `tmp/google-colab-selenium-1.0.8.tar.gz` & `tmp/google-colab-selenium-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-colab-selenium-1.0.8.tar", last modified: Sun Nov 12 00:55:21 2023, max compression
+gzip compressed data, was "google-colab-selenium-1.0.9.tar", last modified: Sun Nov 12 00:58:14 2023, max compression
```

## Comparing `google-colab-selenium-1.0.8.tar` & `google-colab-selenium-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:55:21.753537 google-colab-selenium-1.0.8/
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     1070 2023-11-11 04:43:17.000000 google-colab-selenium-1.0.8/LICENSE
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     2709 2023-11-12 00:55:21.753258 google-colab-selenium-1.0.8/PKG-INFO
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     2210 2023-11-12 00:43:38.000000 google-colab-selenium-1.0.8/README.md
-drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:55:21.751874 google-colab-selenium-1.0.8/google_colab_selenium/
--rw-r--r--   0 jacobpadilla   (501) staff       (20)      951 2023-11-11 19:13:26.000000 google-colab-selenium-1.0.8/google_colab_selenium/__init__.py
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     1437 2023-11-11 06:15:04.000000 google-colab-selenium-1.0.8/google_colab_selenium/chromedriver.py
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     2819 2023-11-11 06:15:24.000000 google-colab-selenium-1.0.8/google_colab_selenium/colab_selenium_manager.py
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     1114 2023-11-11 18:29:28.000000 google-colab-selenium-1.0.8/google_colab_selenium/exceptions.py
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     2031 2023-11-11 04:34:59.000000 google-colab-selenium-1.0.8/google_colab_selenium/spinner.py
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     1837 2023-11-11 06:15:09.000000 google-colab-selenium-1.0.8/google_colab_selenium/undetected_chromedriver.py
-drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:55:21.752850 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/
--rw-r--r--   0 jacobpadilla   (501) staff       (20)     2709 2023-11-12 00:55:21.000000 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/PKG-INFO
--rw-r--r--   0 jacobpadilla   (501) staff       (20)      488 2023-11-12 00:55:21.000000 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 jacobpadilla   (501) staff       (20)        1 2023-11-12 00:55:21.000000 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 jacobpadilla   (501) staff       (20)       47 2023-11-12 00:55:21.000000 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/requires.txt
--rw-r--r--   0 jacobpadilla   (501) staff       (20)       22 2023-11-12 00:55:21.000000 google-colab-selenium-1.0.8/google_colab_selenium.egg-info/top_level.txt
--rw-r--r--   0 jacobpadilla   (501) staff       (20)       38 2023-11-12 00:55:21.753584 google-colab-selenium-1.0.8/setup.cfg
--rw-r--r--   0 jacobpadilla   (501) staff       (20)      718 2023-11-12 00:55:04.000000 google-colab-selenium-1.0.8/setup.py
+drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:58:14.898601 google-colab-selenium-1.0.9/
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     1070 2023-11-11 04:43:17.000000 google-colab-selenium-1.0.9/LICENSE
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     2785 2023-11-12 00:58:14.898326 google-colab-selenium-1.0.9/PKG-INFO
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     2286 2023-11-12 00:57:58.000000 google-colab-selenium-1.0.9/README.md
+drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:58:14.897019 google-colab-selenium-1.0.9/google_colab_selenium/
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)      951 2023-11-11 19:13:26.000000 google-colab-selenium-1.0.9/google_colab_selenium/__init__.py
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     1437 2023-11-11 06:15:04.000000 google-colab-selenium-1.0.9/google_colab_selenium/chromedriver.py
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     2819 2023-11-11 06:15:24.000000 google-colab-selenium-1.0.9/google_colab_selenium/colab_selenium_manager.py
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     1114 2023-11-11 18:29:28.000000 google-colab-selenium-1.0.9/google_colab_selenium/exceptions.py
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     2031 2023-11-11 04:34:59.000000 google-colab-selenium-1.0.9/google_colab_selenium/spinner.py
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     1837 2023-11-11 06:15:09.000000 google-colab-selenium-1.0.9/google_colab_selenium/undetected_chromedriver.py
+drwxr-xr-x   0 jacobpadilla   (501) staff       (20)        0 2023-11-12 00:58:14.897936 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)     2785 2023-11-12 00:58:14.000000 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)      488 2023-11-12 00:58:14.000000 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)        1 2023-11-12 00:58:14.000000 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)       47 2023-11-12 00:58:14.000000 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/requires.txt
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)       22 2023-11-12 00:58:14.000000 google-colab-selenium-1.0.9/google_colab_selenium.egg-info/top_level.txt
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)       38 2023-11-12 00:58:14.898649 google-colab-selenium-1.0.9/setup.cfg
+-rw-r--r--   0 jacobpadilla   (501) staff       (20)      718 2023-11-12 00:58:06.000000 google-colab-selenium-1.0.9/setup.py
```

### Comparing `google-colab-selenium-1.0.8/LICENSE` & `google-colab-selenium-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/PKG-INFO` & `google-colab-selenium-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: google-colab-selenium
-Version: 1.0.8
-Summary: Easily use Selenium in Google Colab Notebooks!
-Home-page: https://github.com/jpjacobpadilla/Google-Colab-Selenium
-Author: Jacob Padilla
-Author-email: jp@jacobpadilla.com
-License: MIT
-Keywords: selenium google-colab webdriver automation chromedriver
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: selenium
-Provides-Extra: undetected
-Requires-Dist: undetected-chromedriver; extra == "undetected"
-
 # Google-Colab-Selenium
 The best way to use Selenium in Google Colab Notebooks!
 
 - Simple setup of Selenium and ChromeDriver.
 - Seamless integration with Google Colab.
 - Support for undetected ChromeDriver for more advanced use cases.
 <br>
@@ -86,9 +71,9 @@
 You can also contact me [here](https://jacobpadilla.com/contact).
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uApofPD-uTbZQ8dVq2IVTGHZOxdJtiel?usp=sharing)
 
 
-![logo](logo.png)
+![logo](https://raw.githubusercontent.com/jpjacobpadilla/Google-Colab-Selenium/main/logo.png)
```

### Comparing `google-colab-selenium-1.0.8/README.md` & `google-colab-selenium-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: google-colab-selenium
+Version: 1.0.9
+Summary: Easily use Selenium in Google Colab Notebooks!
+Home-page: https://github.com/jpjacobpadilla/Google-Colab-Selenium
+Author: Jacob Padilla
+Author-email: jp@jacobpadilla.com
+License: MIT
+Keywords: selenium google-colab webdriver automation chromedriver
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: selenium
+Provides-Extra: undetected
+Requires-Dist: undetected-chromedriver; extra == "undetected"
+
 # Google-Colab-Selenium
 The best way to use Selenium in Google Colab Notebooks!
 
 - Simple setup of Selenium and ChromeDriver.
 - Seamless integration with Google Colab.
 - Support for undetected ChromeDriver for more advanced use cases.
 <br>
@@ -71,9 +86,9 @@
 You can also contact me [here](https://jacobpadilla.com/contact).
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uApofPD-uTbZQ8dVq2IVTGHZOxdJtiel?usp=sharing)
 
 
-![logo](logo.png)
+![logo](https://raw.githubusercontent.com/jpjacobpadilla/Google-Colab-Selenium/main/logo.png)
```

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/__init__.py` & `google-colab-selenium-1.0.9/google_colab_selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/chromedriver.py` & `google-colab-selenium-1.0.9/google_colab_selenium/chromedriver.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/colab_selenium_manager.py` & `google-colab-selenium-1.0.9/google_colab_selenium/colab_selenium_manager.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/exceptions.py` & `google-colab-selenium-1.0.9/google_colab_selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/spinner.py` & `google-colab-selenium-1.0.9/google_colab_selenium/spinner.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium/undetected_chromedriver.py` & `google-colab-selenium-1.0.9/google_colab_selenium/undetected_chromedriver.py`

 * *Files identical despite different names*

### Comparing `google-colab-selenium-1.0.8/google_colab_selenium.egg-info/PKG-INFO` & `google-colab-selenium-1.0.9/google_colab_selenium.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-colab-selenium
-Version: 1.0.8
+Version: 1.0.9
 Summary: Easily use Selenium in Google Colab Notebooks!
 Home-page: https://github.com/jpjacobpadilla/Google-Colab-Selenium
 Author: Jacob Padilla
 Author-email: jp@jacobpadilla.com
 License: MIT
 Keywords: selenium google-colab webdriver automation chromedriver
 Description-Content-Type: text/markdown
@@ -86,9 +86,9 @@
 You can also contact me [here](https://jacobpadilla.com/contact).
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uApofPD-uTbZQ8dVq2IVTGHZOxdJtiel?usp=sharing)
 
 
-![logo](logo.png)
+![logo](https://raw.githubusercontent.com/jpjacobpadilla/Google-Colab-Selenium/main/logo.png)
```

### Comparing `google-colab-selenium-1.0.8/setup.py` & `google-colab-selenium-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='google-colab-selenium',
     description='Easily use Selenium in Google Colab Notebooks!',
-    version='1.0.8',
+    version='1.0.9',
     packages=['google_colab_selenium'],
     install_requires=['selenium'],
     extras_require={
         'undetected': ['undetected-chromedriver']
     },
     author = 'Jacob Padilla',
     author_email = 'jp@jacobpadilla.com',
```

