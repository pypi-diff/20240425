# Comparing `tmp/openlxp_authentication-1.1.2.tar.gz` & `tmp/openlxp_authentication-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlxp_authentication-1.1.2.tar", last modified: Thu Apr 18 18:13:05 2024, max compression
+gzip compressed data, was "openlxp_authentication-1.1.3.tar", last modified: Thu Apr 25 20:09:58 2024, max compression
```

## Comparing `openlxp_authentication-1.1.2.tar` & `openlxp_authentication-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.545068 openlxp_authentication-1.1.2/
--rw-r--r--   0 jametobin   (502) staff       (20)    11357 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.2/LICENSE
--rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-18 18:13:05.544900 openlxp_authentication-1.1.2/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     5415 2022-07-14 15:24:15.000000 openlxp_authentication-1.1.2/README.md
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.537721 openlxp_authentication-1.1.2/openlxp_authentication/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-04-18 18:06:37.000000 openlxp_authentication-1.1.2/openlxp_authentication/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)      199 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/admin.py
--rw-r--r--   0 jametobin   (502) staff       (20)      242 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/apps.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.543800 openlxp_authentication-1.1.2/openlxp_authentication/migrations/
--rw-r--r--   0 jametobin   (502) staff       (20)      839 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/migrations/0001_initial.py
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2021-10-29 19:09:44.000000 openlxp_authentication-1.1.2/openlxp_authentication/migrations/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     2362 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/models.py
--rw-r--r--   0 jametobin   (502) staff       (20)      283 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/serializers.py
--rw-r--r--   0 jametobin   (502) staff       (20)      241 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/urls.py
--rw-r--r--   0 jametobin   (502) staff       (20)      512 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.2/openlxp_authentication/views.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-18 18:13:05.544303 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/
--rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)      593 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       87 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/requires.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       28 2024-04-18 18:13:05.000000 openlxp_authentication-1.1.2/openlxp_authentication.egg-info/top_level.txt
--rw-r--r--   0 jametobin   (502) staff       (20)     1110 2024-04-18 18:13:05.545574 openlxp_authentication-1.1.2/setup.cfg
--rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.2/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-25 20:09:58.093680 openlxp_authentication-1.1.3/
+-rw-r--r--   0 jametobin   (502) staff       (20)    11357 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.3/LICENSE
+-rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-25 20:09:58.093498 openlxp_authentication-1.1.3/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     5415 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-25 20:09:58.087107 openlxp_authentication-1.1.3/openlxp_authentication/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-04-19 12:43:22.000000 openlxp_authentication-1.1.3/openlxp_authentication/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      199 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/openlxp_authentication/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      242 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.3/openlxp_authentication/apps.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-25 20:09:58.091902 openlxp_authentication-1.1.3/openlxp_authentication/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)      839 2022-07-14 15:35:49.000000 openlxp_authentication-1.1.3/openlxp_authentication/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2021-10-29 19:09:44.000000 openlxp_authentication-1.1.3/openlxp_authentication/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     2362 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/openlxp_authentication/models.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      283 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/openlxp_authentication/serializers.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      241 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/openlxp_authentication/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      512 2024-04-19 12:43:13.000000 openlxp_authentication-1.1.3/openlxp_authentication/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-04-25 20:09:58.092789 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     6297 2024-04-25 20:09:58.000000 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)      593 2024-04-25 20:09:58.000000 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-04-25 20:09:58.000000 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       87 2024-04-25 20:09:58.000000 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       28 2024-04-25 20:09:58.000000 openlxp_authentication-1.1.3/openlxp_authentication.egg-info/top_level.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)     1110 2024-04-25 20:09:58.094162 openlxp_authentication-1.1.3/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-07-14 15:17:33.000000 openlxp_authentication-1.1.3/setup.py
```

### Comparing `openlxp_authentication-1.1.2/LICENSE` & `openlxp_authentication-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/PKG-INFO` & `openlxp_authentication-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-authentication
-Version: 1.1.2
+Version: 1.1.3
 Summary: Installable OpenLXP Authentication that adds support for SAML
 Home-page: https://github.com/OpenLXP/openlxp-authentication/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: social-auth-app-django>=5.0.0
+Requires-Dist: social-auth-app-django>=5.4.1
 Requires-Dist: social-auth-core[all]>=4.1.0
 Requires-Dist: djangorestframework>=3.13.0
 
 # OpenLXP-Authentication
 
 This is a Django package built on the social-auth-app-django package to allow additional authentication options for the OpenLXP project.
```

### Comparing `openlxp_authentication-1.1.2/README.md` & `openlxp_authentication-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/openlxp_authentication/migrations/0001_initial.py` & `openlxp_authentication-1.1.3/openlxp_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/openlxp_authentication/models.py` & `openlxp_authentication-1.1.3/openlxp_authentication/models.py`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/openlxp_authentication/views.py` & `openlxp_authentication-1.1.3/openlxp_authentication/views.py`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/openlxp_authentication.egg-info/PKG-INFO` & `openlxp_authentication-1.1.3/openlxp_authentication.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-authentication
-Version: 1.1.2
+Version: 1.1.3
 Summary: Installable OpenLXP Authentication that adds support for SAML
 Home-page: https://github.com/OpenLXP/openlxp-authentication/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: social-auth-app-django>=5.0.0
+Requires-Dist: social-auth-app-django>=5.4.1
 Requires-Dist: social-auth-core[all]>=4.1.0
 Requires-Dist: djangorestframework>=3.13.0
 
 # OpenLXP-Authentication
 
 This is a Django package built on the social-auth-app-django package to allow additional authentication options for the OpenLXP project.
```

### Comparing `openlxp_authentication-1.1.2/openlxp_authentication.egg-info/SOURCES.txt` & `openlxp_authentication-1.1.3/openlxp_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlxp_authentication-1.1.2/setup.cfg` & `openlxp_authentication-1.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openlxp-authentication
-version = 1.1.2
+version = 1.1.3
 description = Installable OpenLXP Authentication that adds support for SAML
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/openlxp-authentication/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
@@ -24,15 +24,15 @@
 [options]
 include_package_data = true
 packages = find_namespace:
 python_requires = >=3.7
 setup_requires = 
 	setuptools >= 38.3.0
 install_requires = 
-	social-auth-app-django>=5.0.0
+	social-auth-app-django>=5.4.1
 	social-auth-core[all]>=4.1.0
 	djangorestframework>=3.13.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

