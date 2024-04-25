# Comparing `tmp/fina-cal-abhi-0.0.1.tar.gz` & `tmp/fina-cal-abhi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fina-cal-abhi-0.0.1.tar", last modified: Thu Apr 25 09:37:07 2024, max compression
+gzip compressed data, was "fina-cal-abhi-0.0.2.tar", last modified: Thu Apr 25 10:07:31 2024, max compression
```

## Comparing `fina-cal-abhi-0.0.1.tar` & `fina-cal-abhi-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 09:37:07.312354 fina-cal-abhi-0.0.1/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      256 2024-04-25 09:37:07.312354 fina-cal-abhi-0.0.1/PKG-INFO
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        9 2024-04-25 07:52:22.000000 fina-cal-abhi-0.0.1/README.md
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 09:37:07.312354 fina-cal-abhi-0.0.1/fin-cal-libs-files/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       32 2024-04-25 07:55:55.000000 fina-cal-abhi-0.0.1/fin-cal-libs-files/__init__.py
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      115 2024-04-25 07:55:38.000000 fina-cal-abhi-0.0.1/fin-cal-libs-files/abhi_hello.py
-drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 09:37:07.312354 fina-cal-abhi-0.0.1/fina_cal_abhi.egg-info/
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      256 2024-04-25 09:37:07.000000 fina-cal-abhi-0.0.1/fina_cal_abhi.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      230 2024-04-25 09:37:07.000000 fina-cal-abhi-0.0.1/fina_cal_abhi.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        1 2024-04-25 09:37:07.000000 fina-cal-abhi-0.0.1/fina_cal_abhi.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       19 2024-04-25 09:37:07.000000 fina-cal-abhi-0.0.1/fina_cal_abhi.egg-info/top_level.txt
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       38 2024-04-25 09:37:07.312354 fina-cal-abhi-0.0.1/setup.cfg
--rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      713 2024-04-25 09:36:58.000000 fina-cal-abhi-0.0.1/setup.py
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 10:07:31.566338 fina-cal-abhi-0.0.2/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      256 2024-04-25 10:07:31.566338 fina-cal-abhi-0.0.2/PKG-INFO
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        9 2024-04-25 07:52:22.000000 fina-cal-abhi-0.0.2/README.md
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 10:07:31.566338 fina-cal-abhi-0.0.2/fina_cal_abhi.egg-info/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      256 2024-04-25 10:07:31.000000 fina-cal-abhi-0.0.2/fina_cal_abhi.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      224 2024-04-25 10:07:31.000000 fina-cal-abhi-0.0.2/fina_cal_abhi.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)        1 2024-04-25 10:07:31.000000 fina-cal-abhi-0.0.2/fina_cal_abhi.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       16 2024-04-25 10:07:31.000000 fina-cal-abhi-0.0.2/fina_cal_abhi.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1001) abhishek  (1001)        0 2024-04-25 10:07:31.566338 fina-cal-abhi-0.0.2/fincallibsfiles/
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       32 2024-04-25 07:55:55.000000 fina-cal-abhi-0.0.2/fincallibsfiles/__init__.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      115 2024-04-25 07:55:38.000000 fina-cal-abhi-0.0.2/fincallibsfiles/abhi_hello.py
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)       38 2024-04-25 10:07:31.566338 fina-cal-abhi-0.0.2/setup.cfg
+-rw-rw-r--   0 abhishek  (1001) abhishek  (1001)      713 2024-04-25 10:07:27.000000 fina-cal-abhi-0.0.2/setup.py
```

### Comparing `fina-cal-abhi-0.0.1/setup.py` & `fina-cal-abhi-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A finance calculation package'
 LONG_DESCRIPTION = 'A package that makes it easy to do finance calculation'
 
 setup(
     name="fina-cal-abhi",
     version=VERSION,
     description=DESCRIPTION,
```

