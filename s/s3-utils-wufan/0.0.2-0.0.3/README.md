# Comparing `tmp/s3_utils_wufan-0.0.2.tar.gz` & `tmp/s3_utils_wufan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_utils_wufan-0.0.2.tar", last modified: Tue Apr  9 06:36:55 2024, max compression
+gzip compressed data, was "s3_utils_wufan-0.0.3.tar", last modified: Thu Apr 25 02:46:44 2024, max compression
```

## Comparing `s3_utils_wufan-0.0.2.tar` & `s3_utils_wufan-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)     1502 2024-04-09 05:13:08.000000 s3_utils_wufan-0.0.2/LICENSE
--rw-r--r--   0 wufan    (100000223) wufan    (100000223)       80 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/PKG-INFO
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)      150 2024-04-09 06:36:31.000000 s3_utils_wufan-0.0.2/pyproject.toml
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       38 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/setup.cfg
-drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/
-drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan/
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       76 2024-04-09 06:17:23.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan/__init__.py
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)    21497 2024-04-09 05:11:34.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan/s3_utils.py
-drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan.egg-info/
--rw-r--r--   0 wufan    (100000223) wufan    (100000223)       80 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan.egg-info/PKG-INFO
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)      252 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan.egg-info/SOURCES.txt
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)        1 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan.egg-info/dependency_links.txt
--rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       15 2024-04-09 06:36:55.000000 s3_utils_wufan-0.0.2/src/s3_utils_wufan.egg-info/top_level.txt
+drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)     1502 2024-04-09 05:13:08.000000 s3_utils_wufan-0.0.3/LICENSE
+-rw-r--r--   0 wufan    (100000223) wufan    (100000223)       80 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/PKG-INFO
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)      150 2024-04-25 02:45:07.000000 s3_utils_wufan-0.0.3/pyproject.toml
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       38 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/setup.cfg
+drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/
+drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan/
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       76 2024-04-09 06:17:23.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan/__init__.py
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)    19518 2024-04-25 02:42:58.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan/s3_utils.py
+drwxrwxr-x   0 wufan    (100000223) wufan    (100000223)        0 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan.egg-info/
+-rw-r--r--   0 wufan    (100000223) wufan    (100000223)       80 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan.egg-info/PKG-INFO
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)      252 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan.egg-info/SOURCES.txt
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)        1 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan.egg-info/dependency_links.txt
+-rw-rw-r--   0 wufan    (100000223) wufan    (100000223)       15 2024-04-25 02:46:44.000000 s3_utils_wufan-0.0.3/src/s3_utils_wufan.egg-info/top_level.txt
```

### Comparing `s3_utils_wufan-0.0.2/LICENSE` & `s3_utils_wufan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_utils_wufan-0.0.2/src/s3_utils_wufan/s3_utils.py` & `s3_utils_wufan-0.0.3/src/s3_utils_wufan/s3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -590,32 +590,7 @@
 
         if os.path.exists(lock_path):
             continue
 
         touch(lock_path)
         download_file()
         return local_path
-
-
-def get_s3_cfg_by_bucket(s3_path):
-    ### 根据bucket名称判断使用哪个配置 ###
-    s3_bucket_cfg = {
-        # 账号：langchao_xuchao
-        "llm-pdf-text": {'endpoint': 'http://10.140.85.161:80', 'ak': 'ZMC2CWSQ27B8FZ303OVM', 'sk': 'TyPUdzmWudNXUwFKVPAIlhFsKsAbNADKj0gMAUh9'},
-        "sci-hub": {'endpoint': 'http://10.140.85.161:80', 'ak': 'ZMC2CWSQ27B8FZ303OVM', 'sk': 'TyPUdzmWudNXUwFKVPAIlhFsKsAbNADKj0gMAUh9'},
-        "private-dataset-pnorm": {'endpoint': 'http://10.140.85.161:80', 'ak': 'ZMC2CWSQ27B8FZ303OVM', 'sk': 'TyPUdzmWudNXUwFKVPAIlhFsKsAbNADKj0gMAUh9'},
-        "public-dataset-pnorm": {'endpoint': 'http://10.140.85.161:80', 'ak': 'ZMC2CWSQ27B8FZ303OVM', 'sk': 'TyPUdzmWudNXUwFKVPAIlhFsKsAbNADKj0gMAUh9'},
-        "public-dataset-p2": {'endpoint': 'http://10.140.85.161:80', 'ak': 'ZMC2CWSQ27B8FZ303OVM', 'sk': 'TyPUdzmWudNXUwFKVPAIlhFsKsAbNADKj0gMAUh9'},
-        # 账号：wufan
-        "public-dataset": {'endpoint': 'http://10.135.3.248:80', 'ak': 'EG0IG2NWL0CLICB9FGRB', 'sk': 'bsIcc5nhPJu8EZN6vpJaZAqXgo5NxKQMFebsV5mO'},
-        "llm-raw-snew": {'endpoint': 'http://10.140.31.254:80', 'ak': 'EG0IG2NWL0CLICB9FGRB', 'sk': 'bsIcc5nhPJu8EZN6vpJaZAqXgo5NxKQMFebsV5mO'},
-        "llm-private-datasets": {'endpoint': 'http://10.135.3.248:80', 'ak': 'EG0IG2NWL0CLICB9FGRB', 'sk': 'bsIcc5nhPJu8EZN6vpJaZAqXgo5NxKQMFebsV5mO'},
-        "llm-private-dataset-snew": {'endpoint': 'http://10.140.31.254:80', 'ak': 'EG0IG2NWL0CLICB9FGRB', 'sk': 'bsIcc5nhPJu8EZN6vpJaZAqXgo5NxKQMFebsV5mO'},
-        # dataproc
-        "llm-raw": {'endpoint': 'http://10.140.14.204:80', 'ak': '4O3XVZGAA9SYYJED4X9H', 'sk': 'CEQo1IHOxTZ9qXAHFl5YbGQJYK4Tl1ZeHT3ssBzB'}
-    }
-    bucket_name = re.findall("/(.*)/", s3_path)[0].lstrip("/").split("/")[0]
-    if bucket_name in s3_bucket_cfg:
-        return s3_bucket_cfg[bucket_name]
-    else:
-        print("! Unkown bucket name: ", bucket_name, "try default cfg(langchao_xuchao)")
-        return s3_bucket_cfg['llm-pdf-text']
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

