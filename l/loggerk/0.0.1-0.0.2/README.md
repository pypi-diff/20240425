# Comparing `tmp/loggerk-0.0.1.tar.gz` & `tmp/loggerk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerk-0.0.1.tar", last modified: Wed Apr 24 23:09:35 2024, max compression
+gzip compressed data, was "loggerk-0.0.2.tar", last modified: Thu Apr 25 14:49:22 2024, max compression
```

## Comparing `loggerk-0.0.1.tar` & `loggerk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-24 23:09:35.480311 loggerk-0.0.1/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.1/LICENSE
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3299 2024-04-24 23:09:35.480125 loggerk-0.0.1/PKG-INFO
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-24 23:09:35.478765 loggerk-0.0.1/loggerk/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5070 2024-04-24 19:04:31.000000 loggerk-0.0.1/loggerk/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-24 23:09:35.479680 loggerk-0.0.1/loggerk/config/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3014 2024-04-24 19:03:25.000000 loggerk-0.0.1/loggerk/config/__init__.py
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.1/loggerk/formaters.py
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4776 2024-04-24 19:20:01.000000 loggerk-0.0.1/loggerk/handlers.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-24 23:09:35.479941 loggerk-0.0.1/loggerk.egg-info/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3299 2024-04-24 23:09:35.000000 loggerk-0.0.1/loggerk.egg-info/PKG-INFO
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      258 2024-04-24 23:09:35.000000 loggerk-0.0.1/loggerk.egg-info/SOURCES.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-24 23:09:35.000000 loggerk-0.0.1/loggerk.egg-info/dependency_links.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-24 23:09:35.000000 loggerk-0.0.1/loggerk.egg-info/requires.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-24 23:09:35.000000 loggerk-0.0.1/loggerk.egg-info/top_level.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-24 23:09:35.480349 loggerk-0.0.1/setup.cfg
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1019 2024-04-24 23:09:15.000000 loggerk-0.0.1/setup.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.443180 loggerk-0.0.2/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.2/LICENSE
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 14:49:22.442988 loggerk-0.0.2/PKG-INFO
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.441047 loggerk-0.0.2/loggerk/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5043 2024-04-25 14:38:07.000000 loggerk-0.0.2/loggerk/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.441766 loggerk-0.0.2/loggerk/config/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3015 2024-04-25 14:37:20.000000 loggerk-0.0.2/loggerk/config/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442198 loggerk-0.0.2/loggerk/formatters/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.2/loggerk/formatters/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442337 loggerk-0.0.2/loggerk/handlers/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4777 2024-04-25 14:38:13.000000 loggerk-0.0.2/loggerk/handlers/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 14:49:22.442796 loggerk-0.0.2/loggerk.egg-info/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/PKG-INFO
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      277 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/SOURCES.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/dependency_links.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/requires.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-25 14:49:22.000000 loggerk-0.0.2/loggerk.egg-info/top_level.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-25 14:49:22.443216 loggerk-0.0.2/setup.cfg
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1016 2024-04-25 14:47:18.000000 loggerk-0.0.2/setup.py
```

### Comparing `loggerk-0.0.1/LICENSE` & `loggerk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.1/PKG-INFO` & `loggerk-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loggerk-0.0.1/loggerk/__init__.py` & `loggerk-0.0.2/loggerk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-import importlib
 import logging
-import logging.config
-import logging.handlers
-import os
 from pathlib import Path
-from typing import Literal, Self
+from typing import Literal
 
 from loggerk.config import DEFAULT_CONFIG, ConfigDict
-from loggerk.formaters import BaseFormatter, Formatter
+from loggerk.formatters import BaseFormatter, Formatter
 from loggerk.handlers import BaseHandlerDictConfig, CustomHTTPHandler
 
 
-
 class LoggerK(logging.Logger):
     """
     A singleton logger class that allows for easy logging configuration and management.
     """
     _instances: dict[str, "LoggerK"] = {}
 
     def __new__(
         cls,
         name: str,
         *_,
         **kwargs,
-    ) -> Self:
+    ) -> "LoggerK":
         if not name in cls._instances:
             cls._instances[name] = super().__new__(cls)
         return cls._instances[name]
 
     def __init__(
         self,
         name: str,
@@ -46,14 +41,15 @@
             config (Config, optional): The logger configuration. Defaults to DEFAULT_CONFIG.
             file_path (str, optional): The file path for log files. Defaults to None. Will be ignored if config does not have a file handler. If provided, it will override the filename in the file handler.
 
         Raises:
             ValueError: If app_name is not provided as an argument and LOGGER_APP_NAME environment variable is not set.
         """
         if app_name is None:
+            import os
             app_name = os.getenv("LOGGER_APP_NAME")
             if not app_name:
                 raise ValueError(
                     "app_name is required, either pass it as an argument or set the LOGGER_APP_NAME environment variable"
                 )
 
         super().__init__(name, level=level)
@@ -73,14 +69,15 @@
 
     def _set_up_handler(
         self,
         file_path: str | None,
         handler_config: BaseHandlerDictConfig,
         formatters: dict[Formatter, BaseFormatter],
     ):
+        import importlib
 
         class_: str | None = handler_config.get("class")
         module_str = ".".join(class_.split(".")[:-1])
         module = importlib.import_module(module_str)
         cls_name = handler_config.get("class").split(".")[-1]
         cls = getattr(module, cls_name)
```

### Comparing `loggerk-0.0.1/loggerk/config/__init__.py` & `loggerk-0.0.2/loggerk/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Any, Literal, TypedDict
 
-from loggerk.formaters import BaseFormatter, Format, Formatter
+from loggerk.formatters import BaseFormatter, Format, Formatter
 from loggerk.handlers import BaseHandlerDictConfig, FileHandlerDictConfig, HTTPHandlerDictConfig, StreamHandlerDictConfig
 
 
 
 class RootLogger(TypedDict):
     handlers: list[str]
     level: Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
```

### Comparing `loggerk-0.0.1/loggerk/handlers.py` & `loggerk-0.0.2/loggerk/handlers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import logging.handlers
 import os
 from typing import Literal, Required, TypedDict
 
 import httpx
 
-from loggerk.formaters import Formatter
+from loggerk.formatters import Formatter
 
 LoggingLevel = Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
 
 
 class BaseHandlerDictConfig(TypedDict):
     class_: Required[
         Literal[
```

### Comparing `loggerk-0.0.1/loggerk.egg-info/PKG-INFO` & `loggerk-0.0.2/loggerk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loggerk-0.0.1/setup.py` & `loggerk-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 here: pathlib.Path = pathlib.Path(__file__).parent.resolve()
 
 long_description: str = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "This is a custom logger module for Python"
 
 # Setting up
 setup(
     name="loggerk",
     version=VERSION,
     author="Kuantik DataJump",
@@ -20,15 +20,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["httpx"],
     keywords=["python", "logging"],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

