# Comparing `tmp/alert_on_exception-0.1.4.tar.gz` & `tmp/alert_on_exception-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alert_on_exception-0.1.4.tar", last modified: Wed Apr 24 11:14:38 2024, max compression
+gzip compressed data, was "alert_on_exception-0.1.5.tar", last modified: Wed Apr 24 12:15:26 2024, max compression
```

## Comparing `alert_on_exception-0.1.4.tar` & `alert_on_exception-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/
--rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.4/LICENSE
--rw-r--r--   0 user1     (1001) user1     (1001)     1066 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      859 2024-04-24 11:06:44.000000 alert_on_exception-0.1.4/README.md
--rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.4/pyproject.toml
--rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/setup.cfg
--rw-rw-r--   0 user1     (1001) user1     (1001)      684 2024-04-24 11:14:22.000000 alert_on_exception-0.1.4/setup.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/src/
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/src/alert_on_exception/
--rw-rw-r--   0 user1     (1001) user1     (1001)       36 2024-04-24 11:06:15.000000 alert_on_exception-0.1.4/src/alert_on_exception/__init__.py
--rw-rw-r--   0 user1     (1001) user1     (1001)      974 2024-04-24 11:05:02.000000 alert_on_exception-0.1.4/src/alert_on_exception/alert.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:14:38.429021 alert_on_exception-0.1.4/src/alert_on_exception.egg-info/
--rw-r--r--   0 user1     (1001) user1     (1001)     1066 2024-04-24 11:14:38.000000 alert_on_exception-0.1.4/src/alert_on_exception.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-24 11:14:38.000000 alert_on_exception-0.1.4/src/alert_on_exception.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 11:14:38.000000 alert_on_exception-0.1.4/src/alert_on_exception.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       19 2024-04-24 11:14:38.000000 alert_on_exception-0.1.4/src/alert_on_exception.egg-info/top_level.txt
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/
+-rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.5/LICENSE
+-rw-r--r--   0 user1     (1001) user1     (1001)     1014 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      807 2024-04-24 12:15:17.000000 alert_on_exception-0.1.5/README.md
+-rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.5/pyproject.toml
+-rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/setup.cfg
+-rw-rw-r--   0 user1     (1001) user1     (1001)      684 2024-04-24 12:15:24.000000 alert_on_exception-0.1.5/setup.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/src/
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/src/alert_on_exception/
+-rw-rw-r--   0 user1     (1001) user1     (1001)       36 2024-04-24 11:06:15.000000 alert_on_exception-0.1.5/src/alert_on_exception/__init__.py
+-rw-rw-r--   0 user1     (1001) user1     (1001)      974 2024-04-24 11:22:01.000000 alert_on_exception-0.1.5/src/alert_on_exception/alert.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 12:15:26.380335 alert_on_exception-0.1.5/src/alert_on_exception.egg-info/
+-rw-r--r--   0 user1     (1001) user1     (1001)     1014 2024-04-24 12:15:26.000000 alert_on_exception-0.1.5/src/alert_on_exception.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-24 12:15:26.000000 alert_on_exception-0.1.5/src/alert_on_exception.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 12:15:26.000000 alert_on_exception-0.1.5/src/alert_on_exception.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       19 2024-04-24 12:15:26.000000 alert_on_exception-0.1.5/src/alert_on_exception.egg-info/top_level.txt
```

### Comparing `alert_on_exception-0.1.4/LICENSE` & `alert_on_exception-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.4/PKG-INFO` & `alert_on_exception-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AlertOnException
 
@@ -31,11 +31,8 @@
 
 ```bash
 from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
 notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
-# Send a notification
-notifier.send_notification()
-
 ```
```

### Comparing `alert_on_exception-0.1.4/README.md` & `alert_on_exception-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,8 @@
 
 ```bash
 from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
 notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
-# Send a notification
-notifier.send_notification()
-
 ```
```

### Comparing `alert_on_exception-0.1.4/setup.py` & `alert_on_exception-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="alert_on_exception",
-    version="0.1.4",
+    version="0.1.5",
     package_dir={"": "src"},  # This line is added
     packages=find_packages(where="src"),  # And this line is modified
     install_requires=[],
     python_requires=">=3.6",
     description="A Python package to alert users about exceptions.",  # Short, concise description
     long_description=long_description,  # Detailed description
     long_description_content_type="text/markdown",  # Content type for long description, assuming it's in Markdown
```

### Comparing `alert_on_exception-0.1.4/src/alert_on_exception/alert.py` & `alert_on_exception-0.1.5/src/alert_on_exception/alert.py`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.4/src/alert_on_exception.egg-info/PKG-INFO` & `alert_on_exception-0.1.5/src/alert_on_exception.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AlertOnException
 
@@ -31,11 +31,8 @@
 
 ```bash
 from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
 notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
-# Send a notification
-notifier.send_notification()
-
 ```
```

