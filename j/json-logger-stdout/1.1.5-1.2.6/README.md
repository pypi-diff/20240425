# Comparing `tmp/json_logger_stdout-1.1.5.tar.gz` & `tmp/json_logger_stdout-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_logger_stdout-1.1.5.tar", max compression
+gzip compressed data, was "json_logger_stdout-1.2.6.tar", max compression
```

## Comparing `json_logger_stdout-1.1.5.tar` & `json_logger_stdout-1.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4592 2023-03-20 11:55:33.895862 json_logger_stdout-1.1.5/README.md
--rw-r--r--   0        0        0       56 2023-03-20 11:55:33.895862 json_logger_stdout-1.1.5/json_logger_stdout/__init__.py
--rw-r--r--   0        0        0     3005 2023-03-20 11:55:33.895862 json_logger_stdout-1.1.5/json_logger_stdout/json_logger_stdout.py
--rw-r--r--   0        0        0      993 2023-03-20 11:55:45.095004 json_logger_stdout-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 json_logger_stdout-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4592 2024-04-25 16:03:35.105851 json_logger_stdout-1.2.6/README.md
+-rw-r--r--   0        0        0       56 2024-04-25 16:03:35.105851 json_logger_stdout-1.2.6/json_logger_stdout/__init__.py
+-rw-r--r--   0        0        0     3063 2024-04-25 16:03:35.105851 json_logger_stdout-1.2.6/json_logger_stdout/json_logger_stdout.py
+-rw-r--r--   0        0        0      993 2024-04-25 16:03:42.543796 json_logger_stdout-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 json_logger_stdout-1.2.6/PKG-INFO
```

### Comparing `json_logger_stdout-1.1.5/README.md` & `json_logger_stdout-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `json_logger_stdout-1.1.5/json_logger_stdout/json_logger_stdout.py` & `json_logger_stdout-1.2.6/json_logger_stdout/json_logger_stdout.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         else:
             log_record['level'] = record.levelname
 
 
 class JSONLoggerStdout:
     def __init__(self, loggerName=None, **kwargs):
         self.loggerName = loggerName
+        self.name = loggerName
         self.kwargs = kwargs
         self.logger = self.get_root_logger()
         self.setLevel(logging.INFO)
 
         self.logHandler = logging.StreamHandler()
         self.formatter = JSONStdFormatter('%(timestamp)s %(level)s %(message)s')
         self.logHandler.setFormatter(self.formatter)
@@ -33,14 +34,15 @@
     def get_root_logger(self):
         return logging.getLogger(self.loggerName) if self.loggerName else logging.getLogger()
 
     def getLogger(self):
         return self.logger
 
     def setLevel(self, level):
+        self.level = level
         self.logger.setLevel(level)
 
     def setFormatter(self, format, formatter=None):
         while self.logger.handlers:
             self.logger.handlers.pop()
 
         self.formatter = formatter if formatter else JSONStdFormatter(format)
```

### Comparing `json_logger_stdout-1.1.5/pyproject.toml` & `json_logger_stdout-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-logger-stdout"
-version = "1.1.5"
+version = "1.2.6"
 description = "JSON Logger for MicroServices. Prints logs to the stdout of the service and can be shipped to ES by leveraging a centralized tool like Fluentd."
 authors = ["Chalukya J <chalukyaj@gmail.com>"]
 
 license = "MIT"
 readme = "README.md"
 keywords = ["json-logger", "micro-services", "containers", "docker", "kubernetes", "fluetd", "stdout"]
 homepage = "https://gitlab.com/chalukyaj/json-logger-stdout"
```

### Comparing `json_logger_stdout-1.1.5/PKG-INFO` & `json_logger_stdout-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-logger-stdout
-Version: 1.1.5
+Version: 1.2.6
 Summary: JSON Logger for MicroServices. Prints logs to the stdout of the service and can be shipped to ES by leveraging a centralized tool like Fluentd.
 Home-page: https://gitlab.com/chalukyaj/json-logger-stdout
 License: MIT
 Keywords: json-logger,micro-services,containers,docker,kubernetes,fluetd,stdout
 Author: Chalukya J
 Author-email: chalukyaj@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Terminals :: Serial
 Requires-Dist: python-json-logger (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://gitlab.com/chalukyaj/json-logger-stdout
 Description-Content-Type: text/markdown
```

