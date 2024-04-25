# Comparing `tmp/next_api_starter-0.1.3.tar.gz` & `tmp/next_api_starter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next_api_starter-0.1.3.tar", last modified: Tue Apr 23 12:58:46 2024, max compression
+gzip compressed data, was "next_api_starter-0.1.4.tar", last modified: Thu Apr 25 08:55:35 2024, max compression
```

## Comparing `next_api_starter-0.1.3.tar` & `next_api_starter-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/next_api_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 12:58:46.000000 next_api_starter-0.1.3/next_api_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/src/next_api_starter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/next_api_starter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6083 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/next_api_starter/create_nextapi.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/next_api_starter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:46.716051 next_api_starter-0.1.3/src/next_api_starter/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/next_api_starter/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-23 12:58:38.000000 next_api_starter-0.1.3/src/next_api_starter/update_nextapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/next_api_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 08:55:35.000000 next_api_starter-0.1.4/next_api_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/src/next_api_starter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/next_api_starter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11218 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/next_api_starter/create_nextapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/next_api_starter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:35.111095 next_api_starter-0.1.4/src/next_api_starter/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/next_api_starter/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-25 08:55:27.000000 next_api_starter-0.1.4/src/next_api_starter/update_nextapi.py
```

### Comparing `next_api_starter-0.1.3/setup.py` & `next_api_starter-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="next-api-starter",  # Replace with your desired package name
-    version="0.1.3",  # Start with version 0.1.0 for initial release
+    version="0.1.4",  # Start with version 0.1.0 for initial release
     description="Starter template for Next.js and FastAPI projects",
     long_description="...",  # Add detailed description in README format
     long_description_content_type="text/markdown",
     packages=find_packages(),  # Exclude frontend/backend for separate installation
     install_requires=[  # List dependencies for backend
         "uvicorn[standard]",
         # ... other dependencies
```

### Comparing `next_api_starter-0.1.3/src/next_api_starter/update_nextapi.py` & `next_api_starter-0.1.4/src/next_api_starter/update_nextapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import os
 import subprocess
 import argparse
-
+import sqlalchemy
+import alembic
 def update_database(service_dir):
     """
     Update the database schema for a service
 
     Args:
         service_dir (str): Path to the service directory
     """
     
-    alembic_ini = os.path.join(service_dir,"alembic.ini")
-    
-    if not os.path.exists(alembic_ini):
-        print(f"No Alembic configuration found for {service_dir}")
+    currrent_dir = os.path.abspath(os.getcwd())
+    try:
+        os.chdir(service_dir)
+        # alembic_ini = os.path.join(service_dir,"alembic.ini")
         
-        return
-    
-    subprocess.run(['alembic', "-c", alembic_ini, 'revision', "--autogenerate", "-m", "Updating database schema"])
-    
-    subprocess.run(["alembic","-c", alembic_ini, "upgrade", "head"])
+        # if not os.path.exists(alembic_ini):
+        #     print(f"No Alembic configuration found for {service_dir}")
+            
+        #     return
+        
+        subprocess.run(['alembic', 'revision', "--autogenerate", "-m", "Updating database schema"])
+        
+        subprocess.run(["alembic","upgrade", "head"])
+    except sqlalchemy.exc.NoSuchModuleError:
+        print("Please edit the sqlalchemy.url = driver://user:pass@localhost/dbname in your alembic.ini file")
+    finally:
+        os.chdir(currrent_dir)
     
     
     
 def update_all_services(backened_dir):
     """
     Update the database schema for all services in the backened directory
```

