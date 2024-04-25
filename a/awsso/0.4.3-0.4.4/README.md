# Comparing `tmp/awsso-0.4.3.tar.gz` & `tmp/awsso-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsso-0.4.3.tar", last modified: Mon Jan 22 04:05:56 2024, max compression
+gzip compressed data, was "awsso-0.4.4.tar", last modified: Thu Apr 25 09:59:42 2024, max compression
```

## Comparing `awsso-0.4.3.tar` & `awsso-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-01-22 04:05:56.328378 awsso-0.4.3/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-01-22 04:05:56.327980 awsso-0.4.3/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.4.3/README.md
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-01-22 04:05:56.317621 awsso-0.4.3/awsso/
--rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.4.3/awsso/__init__.py
--rwxr-xr-x   0 hanpenny   (501) staff       (20)    34122 2024-01-22 04:05:14.000000 awsso-0.4.3/awsso/awsso.py
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-01-22 04:05:56.326995 awsso-0.4.3/awsso.egg-info/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      227 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/SOURCES.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        1 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/dependency_links.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       43 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/entry_points.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       60 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/requires.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        6 2024-01-22 04:05:56.000000 awsso-0.4.3/awsso.egg-info/top_level.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       38 2024-01-22 04:05:56.328513 awsso-0.4.3/setup.cfg
--rw-r--r--   0 hanpenny   (501) staff       (20)      986 2024-01-22 04:05:42.000000 awsso-0.4.3/setup.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.600549 awsso-0.4.4/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 09:59:42.600258 awsso-0.4.4/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.4.4/README.md
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.597368 awsso-0.4.4/awsso/
+-rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.4.4/awsso/__init__.py
+-rwxr-xr-x   0 hanpenny   (501) staff       (20)    33354 2024-04-25 09:46:39.000000 awsso-0.4.4/awsso/awsso.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2024-04-25 09:59:42.599790 awsso-0.4.4/awsso.egg-info/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      227 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/SOURCES.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        1 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/dependency_links.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       43 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/entry_points.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       60 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/requires.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        6 2024-04-25 09:59:42.000000 awsso-0.4.4/awsso.egg-info/top_level.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       38 2024-04-25 09:59:42.600626 awsso-0.4.4/setup.cfg
+-rw-r--r--   0 hanpenny   (501) staff       (20)      986 2024-04-25 09:59:40.000000 awsso-0.4.4/setup.py
```

### Comparing `awsso-0.4.3/PKG-INFO` & `awsso-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.4.3
+Version: 0.4.4
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.4.3/README.md` & `awsso-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `awsso-0.4.3/awsso/awsso.py` & `awsso-0.4.4/awsso/awsso.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from dateutil.parser import parse
 from dateutil.tz import UTC, tzlocal
 
 AWS_CONFIG_DIR = f'{Path.home()}/.aws'
 AWS_CONFIG_PATH = f'{Path.home()}/.aws/config'
 AWS_CREDENTIAL_PATH = f'{Path.home()}/.aws/credentials'
 AWS_SSO_CACHE_PATH = f'{Path.home()}/.aws/sso/cache'
-AWS_DEFAULT_REGION = 'us-west-1'
+AWS_DEFAULT_REGION = 'us-west-2'
 CURRENT_REGION = os.getenv('AWS_REGION')
 AWS_OPS1_ACCOUNT = '101790543458'
 AWS_OPS1_REGION = 'us-west-1'
 AWS_OPS2_ACCOUNT = '731045533415'
 AWS_OPS2_REGION = 'us-west-2'
 
 if not CURRENT_REGION:
@@ -84,31 +84,14 @@
         help='aws sso switch account.')
     parser.add_argument('-g',
         action='store_true',
         help='aws sso logout.')
     parser.add_argument('-i',
         action='store_true',
         help='check aws session.')
-#    parser_sso = subparsers.add_parser('sso')
-#    parser_sso_sub = parser_sso.add_subparsers()
-#    parser_sso_config = parser_sso_sub.add_parser('config',
-#                        help='config aws sso.')
-#    parser_sso_config.set_defaults(func=_sso_config)
-#
-#    parser_sso_login = parser_sso_sub.add_parser('login',
-#                        help='ssm login into sso.')
-#    parser_sso_login.set_defaults(func=_sso_login)
-#
-#    parser_sso_switch = parser_sso_sub.add_parser('switch',
-#                        help='switch to another config.')
-#    parser_sso_switch.set_defaults(func=_sso_switch)
-#
-#    parser_sso_logout = parser_sso_sub.add_parser('logout',
-#                        help='logout aws sso.')
-#    parser_sso_logout.set_defaults(func=_sso_logout)
 
     parser_env = subparsers.add_parser('env')
     parser_env_sub = parser_env.add_subparsers()
     parser_env_get = parser_env_sub.add_parser('get',
                         help='get service env.')
     parser_env_get.add_argument('service')
     parser_env_get.set_defaults(func=_env_get)
@@ -503,15 +486,15 @@
             region = account_map.get(account_name)[1]
             r1 = client.list_account_roles(
                 accessToken=accessToken,
                 accountId=accountId)
             if r1.get('ResponseMetadata').get('HTTPStatusCode') == 200:
                 for role in r1.get('roleList'):
                     role = role.get('roleName')
-                    p_name = 'profile {}{}'.format(profile_name, role)
+                    p_name = 'profile {}_{}'.format(profile_name, role)
                     if config.has_section(p_name):
                         config.remove_section(p_name)
                     #if not re.match('^[A-Z].*', role):
                     #    p_name = '{}{}'.format(p_name, role)
                     #if n == 1 and config.has_section(p_name):
                     #    config.remove_section(p_name)
                     #elif n > 1 and config.has_section(p_name):
```

### Comparing `awsso-0.4.3/awsso.egg-info/PKG-INFO` & `awsso-0.4.4/awsso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.4.3
+Version: 0.4.4
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.4.3/setup.py` & `awsso-0.4.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import awsso
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="awsso",
-    version="0.4.3",
+    version="0.4.4",
     author="linhan",
     author_email="lynnpen@gmail.com",  
     description="aws command line tool",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/Hireteammate/tools.git",
     packages=setuptools.find_packages(),
```

