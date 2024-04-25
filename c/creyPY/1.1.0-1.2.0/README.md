# Comparing `tmp/creyPY-1.1.0.tar.gz` & `tmp/creyPY-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-1.1.0.tar", last modified: Tue Apr  2 11:20:20 2024, max compression
+gzip compressed data, was "creyPY-1.2.0.tar", last modified: Thu Apr 25 16:21:28 2024, max compression
```

## Comparing `creyPY-1.1.0.tar` & `creyPY-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 11:20:05.000000 creyPY-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 11:20:20.935569 creyPY-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-02 11:20:05.000000 creyPY-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.931569 creyPY-1.1.0/creyPY/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY/const/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/const/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/const/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/const/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY/fastapi/db/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/db/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY/fastapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY/fastapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-02 11:20:05.000000 creyPY-1.1.0/creyPY/fastapi/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:20:20.935569 creyPY-1.1.0/creyPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 11:20:20.000000 creyPY-1.1.0/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 11:20:20.000000 creyPY-1.1.0/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:20:20.000000 creyPY-1.1.0/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-02 11:20:20.000000 creyPY-1.1.0/creyPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 11:20:20.000000 creyPY-1.1.0/creyPY.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:20:20.935569 creyPY-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 11:20:05.000000 creyPY-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.566928 creyPY-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 16:21:12.000000 creyPY-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 16:21:28.566928 creyPY-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-25 16:21:12.000000 creyPY-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/const/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/const/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/const/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/fastapi/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/db/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/fastapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.562928 creyPY-1.2.0/creyPY/fastapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-25 16:21:12.000000 creyPY-1.2.0/creyPY/fastapi/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:21:28.566928 creyPY-1.2.0/creyPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 16:21:28.000000 creyPY-1.2.0/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 16:21:28.000000 creyPY-1.2.0/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:21:28.000000 creyPY-1.2.0/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 16:21:28.000000 creyPY-1.2.0/creyPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 16:21:28.000000 creyPY-1.2.0/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:21:28.566928 creyPY-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 16:21:12.000000 creyPY-1.2.0/setup.py
```

### Comparing `creyPY-1.1.0/LICENSE` & `creyPY-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/PKG-INFO` & `creyPY-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 1.1.0
+Version: 1.2.0
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
 Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
 Platform: any
```

### Comparing `creyPY-1.1.0/README.md` & `creyPY-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/const/i18n.py` & `creyPY-1.2.0/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/const/stripe.py` & `creyPY-1.2.0/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/app.py` & `creyPY-1.2.0/creyPY/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/crud.py` & `creyPY-1.2.0/creyPY/fastapi/crud.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/db/session.py` & `creyPY-1.2.0/creyPY/fastapi/db/session.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/models/base.py` & `creyPY-1.2.0/creyPY/fastapi/models/base.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/pagination.py` & `creyPY-1.2.0/creyPY/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY/fastapi/testing.py` & `creyPY-1.2.0/creyPY/fastapi/testing.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.1.0/creyPY.egg-info/PKG-INFO` & `creyPY-1.2.0/creyPY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 1.1.0
+Version: 1.2.0
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
 Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
 Platform: any
```

### Comparing `creyPY-1.1.0/creyPY.egg-info/SOURCES.txt` & `creyPY-1.2.0/creyPY.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 creyPY/const/__init__.py
 creyPY/const/groups.py
 creyPY/const/i18n.py
 creyPY/const/stripe.py
 creyPY/fastapi/__init__.py
 creyPY/fastapi/app.py
 creyPY/fastapi/crud.py
+creyPY/fastapi/order_by.py
 creyPY/fastapi/pagination.py
 creyPY/fastapi/testing.py
 creyPY/fastapi/db/__init__.py
 creyPY/fastapi/db/session.py
 creyPY/fastapi/models/__init__.py
 creyPY/fastapi/models/base.py
 creyPY/fastapi/schemas/__init__.py
```

### Comparing `creyPY-1.1.0/setup.py` & `creyPY-1.2.0/setup.py`

 * *Files identical despite different names*

