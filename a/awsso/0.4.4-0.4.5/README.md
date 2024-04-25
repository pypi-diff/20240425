# Comparing `tmp/awsso-0.4.4.tar.gz` & `tmp/awsso-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsso-0.4.4.tar", last modified: Thu Apr 25 09:59:42 2024, max compression
+gzip compressed data, was "awsso-0.4.5.tar", last modified: Thu Apr 25 10:14:34 2024, max compression
```

## Comparing `awsso-0.4.4.tar` & `awsso-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.600549 awsso-0.4.4/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 09:59:42.600258 awsso-0.4.4/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.4.4/README.md
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.597368 awsso-0.4.4/awsso/
--rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.4.4/awsso/__init__.py
--rwxr-xr-x   0 hanpenny   (501) staff       (20)    33354 2024-04-25 09:46:39.000000 awsso-0.4.4/awsso/awsso.py
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.599790 awsso-0.4.4/awsso.egg-info/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      227 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/SOURCES.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        1 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/dependency_links.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       43 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/entry_points.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       60 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/requires.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        6 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/top_level.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       38 2024-04-25 09:59:42.600626 awsso-0.4.4/setup.cfg
--rw-r--r--   0 hanpenny   (501) staff       (20)      986 2024-04-25 09:59:40.000000 awsso-0.4.4/setup.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 10:14:34.786454 awsso-0.4.5/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 10:14:34.786212 awsso-0.4.5/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.4.5/README.md
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 10:14:34.783375 awsso-0.4.5/awsso/
+-rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.4.5/awsso/__init__.py
+-rwxr-xr-x   0 hanpenny   (501) staff       (20)    33387 2024-04-25 10:14:23.000000 awsso-0.4.5/awsso/awsso.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 10:14:34.785703 awsso-0.4.5/awsso.egg-info/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      227 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/SOURCES.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        1 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/dependency_links.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       43 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/entry_points.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       60 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/requires.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        6 2024-04-25 10:14:34.000000 awsso-0.4.5/awsso.egg-info/top_level.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       38 2024-04-25 10:14:34.786514 awsso-0.4.5/setup.cfg
+-rw-r--r--   0 hanpenny   (501) staff       (20)      986 2024-04-25 10:14:31.000000 awsso-0.4.5/setup.py
```

### Comparing `awsso-0.4.4/PKG-INFO` & `awsso-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.4.4
+Version: 0.4.5
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.4.4/README.md` & `awsso-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `awsso-0.4.4/awsso/awsso.py` & `awsso-0.4.5/awsso/awsso.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
             region = account_map.get(account_name)[1]
             r1 = client.list_account_roles(
                 accessToken=accessToken,
                 accountId=accountId)
             if r1.get('ResponseMetadata').get('HTTPStatusCode') == 200:
                 for role in r1.get('roleList'):
                     role = role.get('roleName')
-                    p_name = 'profile {}_{}'.format(profile_name, role)
+                    p_name = 'profile {}{}'.format(profile_name, role.replace(profile_name.upper(), ''))
                     if config.has_section(p_name):
                         config.remove_section(p_name)
                     #if not re.match('^[A-Z].*', role):
                     #    p_name = '{}{}'.format(p_name, role)
                     #if n == 1 and config.has_section(p_name):
                     #    config.remove_section(p_name)
                     #elif n > 1 and config.has_section(p_name):
```

### Comparing `awsso-0.4.4/awsso.egg-info/PKG-INFO` & `awsso-0.4.5/awsso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.4.4
+Version: 0.4.5
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.4.4/setup.py` & `awsso-0.4.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import awsso
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="awsso",
-    version="0.4.4",
+    version="0.4.5",
     author="linhan",
     author_email="lynnpen@gmail.com",  
     description="aws command line tool",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/Hireteammate/tools.git",
     packages=setuptools.find_packages(),
```

