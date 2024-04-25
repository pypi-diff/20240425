# Comparing `tmp/python-weather-2.0.1.tar.gz` & `tmp/python_weather-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-weather-2.0.1.tar", last modified: Sun Mar 24 22:13:13 2024, max compression
+gzip compressed data, was "python_weather-2.0.2.tar", last modified: Thu Apr 25 16:44:59 2024, max compression
```

## Comparing `python-weather-2.0.1.tar` & `python_weather-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 22:13:13.939456 python-weather-2.0.1/
--rw-rw-rw-   0        0        0     1106 2024-03-05 09:52:35.000000 python-weather-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      181 2024-03-24 16:50:02.000000 python-weather-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3249 2024-03-24 22:13:13.933560 python-weather-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1542 2024-03-18 08:54:47.000000 python-weather-2.0.1/README.md
--rw-rw-rw-   0        0        0     1518 2024-03-24 21:56:55.000000 python-weather-2.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-24 22:13:13.847905 python-weather-2.0.1/python_weather/
--rw-rw-rw-   0        0        0      341 2024-03-24 21:57:34.000000 python-weather-2.0.1/python_weather/__init__.py
--rw-rw-rw-   0        0        0     3875 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/base.py
--rw-rw-rw-   0        0        0     3998 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/client.py
--rw-rw-rw-   0        0        0      912 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/constants.py
--rw-rw-rw-   0        0        0     9679 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/enums.py
--rw-rw-rw-   0        0        0      126 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/errors.py
--rw-rw-rw-   0        0        0     8681 2024-03-24 16:53:13.000000 python-weather-2.0.1/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2024-03-24 22:13:13.930849 python-weather-2.0.1/python_weather.egg-info/
--rw-rw-rw-   0        0        0     3249 2024-03-24 22:13:13.000000 python-weather-2.0.1/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2024-03-24 22:13:13.000000 python-weather-2.0.1/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 22:13:13.000000 python-weather-2.0.1/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-24 22:13:13.000000 python-weather-2.0.1/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-24 22:13:13.000000 python-weather-2.0.1/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 22:13:13.940602 python-weather-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.950542 python_weather-2.0.2/
+-rw-rw-rw-   0        0        0     1080 2024-04-25 12:21:32.000000 python_weather-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      181 2024-04-25 12:21:32.000000 python_weather-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3702 2024-04-25 16:44:59.950542 python_weather-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-25 12:38:46.000000 python_weather-2.0.2/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-25 16:20:00.000000 python_weather-2.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.809916 python_weather-2.0.2/python_weather/
+-rw-rw-rw-   0        0        0      439 2024-04-25 16:20:30.000000 python_weather-2.0.2/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     3875 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/base.py
+-rw-rw-rw-   0        0        0     3998 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/client.py
+-rw-rw-rw-   0        0        0      912 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/constants.py
+-rw-rw-rw-   0        0        0     9679 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/enums.py
+-rw-rw-rw-   0        0        0      126 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/errors.py
+-rw-rw-rw-   0        0        0     8681 2024-04-25 12:21:32.000000 python_weather-2.0.2/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:44:59.950542 python_weather-2.0.2/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3702 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-25 16:44:59.000000 python_weather-2.0.2/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:44:59.950542 python_weather-2.0.2/setup.cfg
```

### Comparing `python-weather-2.0.1/LICENSE` & `python_weather-2.0.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2024 null (https://github.com/null8626)
+Copyright (c) 2021-2024 null8626
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `python-weather-2.0.1/PKG-INFO` & `python_weather-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 2.0.1
+Version: 2.0.2
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
+Project-URL: Donations, https://ko-fi.com/null8626
 Project-URL: Changelog, https://python-weather.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Documentation, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/null8626/python-weather
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: Natural Language :: English
 Classifier: Topic :: Education
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
@@ -29,21 +31,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.5
 
-# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url]
+# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url] [![ko-fi][ko-fi-brief-image]][ko-fi-url]
 
 [pypi-image]: https://img.shields.io/pypi/v/python-weather.svg?style=flat-square
 [pypi-url]: https://pypi.org/project/python-weather/
 [downloads-image]: https://img.shields.io/pypi/dm/python-weather?style=flat-square
+[ko-fi-brief-image]: https://img.shields.io/badge/donations-ko--fi-red?color=ff5e5b&style=flat-square
+[ko-fi-image]: https://ko-fi.com/img/githubbutton_sm.svg
+[ko-fi-url]: https://ko-fi.com/null8626
 
 A free and asynchronous weather Python API wrapper made in Python, for Python.
 
 ## Installation
 
 ```console
 $ pip install python-weather
@@ -81,7 +86,13 @@
   # see https://stackoverflow.com/questions/45600579/asyncio-event-loop-is-closed-when-getting-loop
   # for more details
   if os.name == 'nt':
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
   
   asyncio.run(getweather())
 ```
+
+## Donations
+
+If you want to support this project, consider donating! ❤
+
+[![ko-fi][ko-fi-image]][ko-fi-url]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-weather-2.0.1/README.md` & `python_weather-2.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url]
+# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url] [![ko-fi][ko-fi-brief-image]][ko-fi-url]
 
 [pypi-image]: https://img.shields.io/pypi/v/python-weather.svg?style=flat-square
 [pypi-url]: https://pypi.org/project/python-weather/
 [downloads-image]: https://img.shields.io/pypi/dm/python-weather?style=flat-square
+[ko-fi-brief-image]: https://img.shields.io/badge/donations-ko--fi-red?color=ff5e5b&style=flat-square
+[ko-fi-image]: https://ko-fi.com/img/githubbutton_sm.svg
+[ko-fi-url]: https://ko-fi.com/null8626
 
 A free and asynchronous weather Python API wrapper made in Python, for Python.
 
 ## Installation
 
 ```console
 $ pip install python-weather
@@ -44,7 +47,13 @@
   # see https://stackoverflow.com/questions/45600579/asyncio-event-loop-is-closed-when-getting-loop
   # for more details
   if os.name == 'nt':
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
   
   asyncio.run(getweather())
 ```
+
+## Donations
+
+If you want to support this project, consider donating! ❤
+
+[![ko-fi][ko-fi-image]][ko-fi-url]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-weather-2.0.1/pyproject.toml` & `python_weather-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "python-weather"
-version = "2.0.1"
+version = "2.0.2"
 description = "A free and asynchronous weather API wrapper made in Python, for Python."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "weather-api", "weather-forecast"]
-dependencies = ["aiohttp==3.9.3"]
+dependencies = ["aiohttp==3.9.5"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: aiohttp",
   "Framework :: AsyncIO",
   "Intended Audience :: Education",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
+  "Natural Language :: English",
   "Topic :: Education",
   "Topic :: Internet",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Astronomy",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "License :: OSI Approved :: MIT License",
@@ -32,11 +33,12 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.8"
 
 [project.urls]
+Donations = "https://ko-fi.com/null8626"
 Changelog = "https://python-weather.readthedocs.io/en/latest/changelog.html"
 Homepage = "https://python-weather.readthedocs.io/en/latest/"
 Documentation = "https://python-weather.readthedocs.io/en/latest/"
 Repository = "https://github.com/null8626/python-weather"
```

### Comparing `python-weather-2.0.1/python_weather/base.py` & `python_weather-2.0.2/python_weather/base.py`

 * *Files identical despite different names*

### Comparing `python-weather-2.0.1/python_weather/client.py` & `python_weather-2.0.2/python_weather/client.py`

 * *Files identical despite different names*

### Comparing `python-weather-2.0.1/python_weather/constants.py` & `python_weather-2.0.2/python_weather/constants.py`

 * *Files identical despite different names*

### Comparing `python-weather-2.0.1/python_weather/enums.py` & `python_weather-2.0.2/python_weather/enums.py`

 * *Files identical despite different names*

### Comparing `python-weather-2.0.1/python_weather/forecast.py` & `python_weather-2.0.2/python_weather/forecast.py`

 * *Files identical despite different names*

### Comparing `python-weather-2.0.1/python_weather.egg-info/PKG-INFO` & `python_weather-2.0.2/python_weather.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 2.0.1
+Version: 2.0.2
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
+Project-URL: Donations, https://ko-fi.com/null8626
 Project-URL: Changelog, https://python-weather.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Documentation, https://python-weather.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/null8626/python-weather
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: Natural Language :: English
 Classifier: Topic :: Education
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
@@ -29,21 +31,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.5
 
-# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url]
+# [python-weather][pypi-url] [![pypi][pypi-image]][pypi-url] [![downloads][downloads-image]][pypi-url] [![ko-fi][ko-fi-brief-image]][ko-fi-url]
 
 [pypi-image]: https://img.shields.io/pypi/v/python-weather.svg?style=flat-square
 [pypi-url]: https://pypi.org/project/python-weather/
 [downloads-image]: https://img.shields.io/pypi/dm/python-weather?style=flat-square
+[ko-fi-brief-image]: https://img.shields.io/badge/donations-ko--fi-red?color=ff5e5b&style=flat-square
+[ko-fi-image]: https://ko-fi.com/img/githubbutton_sm.svg
+[ko-fi-url]: https://ko-fi.com/null8626
 
 A free and asynchronous weather Python API wrapper made in Python, for Python.
 
 ## Installation
 
 ```console
 $ pip install python-weather
@@ -81,7 +86,13 @@
   # see https://stackoverflow.com/questions/45600579/asyncio-event-loop-is-closed-when-getting-loop
   # for more details
   if os.name == 'nt':
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
   
   asyncio.run(getweather())
 ```
+
+## Donations
+
+If you want to support this project, consider donating! ❤
+
+[![ko-fi][ko-fi-image]][ko-fi-url]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

