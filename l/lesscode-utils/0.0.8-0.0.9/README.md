# Comparing `tmp/lesscode_utils-0.0.8.tar.gz` & `tmp/lesscode_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_utils-0.0.8.tar", last modified: Wed Jul 26 10:40:46 2023, max compression
+gzip compressed data, was "dist/lesscode_utils-0.0.9.tar", last modified: Wed Jul 26 12:51:53 2023, max compression
```

## Comparing `lesscode_utils-0.0.8.tar` & `lesscode_utils-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.8/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.8/lesscode_utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     3733 2023-07-26 10:40:37.000000 lesscode_utils-0.0.8/lesscode_utils/company_es_utils.py
--rw-r--r--   0 baai       (501) staff       (20)      261 2023-07-26 01:02:54.000000 lesscode_utils-0.0.8/lesscode_utils/const_utils.py
--rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.8/lesscode_utils/date_time_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/
--rw-r--r--   0 baai       (501) staff       (20)      226 2022-04-19 02:49:20.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1817 2023-07-18 06:03:34.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/aes.py
--rw-r--r--   0 baai       (501) staff       (20)      621 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/base64.py
--rw-r--r--   0 baai       (501) staff       (20)     1722 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/des.py
--rw-r--r--   0 baai       (501) staff       (20)      609 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/hmac.py
--rw-r--r--   0 baai       (501) staff       (20)      289 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/md5.py
--rw-r--r--   0 baai       (501) staff       (20)     2264 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/rsa.py
--rw-r--r--   0 baai       (501) staff       (20)      288 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/sha1.py
--rw-r--r--   0 baai       (501) staff       (20)      292 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/sha256.py
--rw-r--r--   0 baai       (501) staff       (20)     3896 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/smx.py
--rw-r--r--   0 baai       (501) staff       (20)    10058 2023-07-26 10:22:36.000000 lesscode_utils-0.0.8/lesscode_utils/es_utils.py
--rw-r--r--   0 baai       (501) staff       (20)      854 2023-07-26 04:19:20.000000 lesscode_utils-0.0.8/lesscode_utils/json_utils.py
--rw-r--r--   0 baai       (501) staff       (20)     2162 2023-07-26 07:38:35.000000 lesscode_utils-0.0.8/lesscode_utils/mongo_util.py
--rw-r--r--   0 baai       (501) staff       (20)      266 2023-07-26 01:12:20.000000 lesscode_utils-0.0.8/lesscode_utils/single_instance_utils.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-26 10:40:37.000000 lesscode_utils-0.0.8/lesscode_utils/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      927 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/requires.txt
--rw-r--r--   0 baai       (501) staff       (20)       15 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1265 2023-07-18 07:12:36.000000 lesscode_utils-0.0.8/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/
+-rw-r--r--   0 navy      (1000) navy      (1000)      375 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)       50 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     3522 2023-07-26 12:49:16.000000 lesscode_utils-0.0.9/lesscode_utils/company_es_utils.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      261 2023-07-26 12:28:39.000000 lesscode_utils-0.0.9/lesscode_utils/const_utils.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2777 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/date_time_utils.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/
+-rw-r--r--   0 navy      (1000) navy      (1000)      226 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1817 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/aes.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      621 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/base64.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1722 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/des.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      609 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/hmac.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      289 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/md5.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2264 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/rsa.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      288 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/sha1.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      292 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/sha256.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     3896 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/smx.py
+-rw-r--r--   0 navy      (1000) navy      (1000)    10058 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/lesscode_utils/es_utils.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      854 2023-07-26 12:28:47.000000 lesscode_utils-0.0.9/lesscode_utils/json_utils.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2162 2023-07-26 12:28:47.000000 lesscode_utils-0.0.9/lesscode_utils/mongo_util.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      266 2023-07-25 15:57:34.000000 lesscode_utils-0.0.9/lesscode_utils/single_instance_utils.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-07-26 12:49:16.000000 lesscode_utils-0.0.9/lesscode_utils/version.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)      375 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      927 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       16 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/requires.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       15 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/lesscode_utils.egg-info/top_level.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-07-26 12:51:53.000000 lesscode_utils-0.0.9/setup.cfg
+-rw-r--r--   0 navy      (1000) navy      (1000)     1265 2023-07-25 15:23:06.000000 lesscode_utils-0.0.9/setup.py
```

### Comparing `lesscode_utils-0.0.8/lesscode_utils/company_es_utils.py` & `lesscode_utils-0.0.9/lesscode_utils/company_es_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,87 @@
 def parse_company_industry_tag(tags):
+    tag_list = []
     industry_tag = tags.get("industry_tag", [])
-    tag_info = {
-        "type": "产业标签",
-        "tags": []
-    }
     if industry_tag:
         for _ in industry_tag:
             if _:
                 tag_name = _.get("tag_name")
                 if tag_name:
-                    tag_info["tags"].append(tag_name)
-    return tag_info
+                    tag_list.append(tag_name)
+    return tag_list
 
 
 def parse_company_permission_level_tag(tags):
     permission = tags.get("permission", [])
-    tag_info = {
-        "type": "备案许可级别",
-        "tags": []
-    }
+    tag_list = []
     if permission:
         for _ in permission:
             if _:
                 level = _.get("level")
                 if level:
-                    tag_info["tags"].append(level)
-    return tag_info
+                    tag_list.append(level)
+    return tag_list
 
 
 def parse_company_permission_name_tag(tags):
     permission = tags.get("permission", [])
-    tag_info = {
-        "type": "备案许可名称",
-        "tags": []
-    }
+    tag_list = []
     if permission:
         for _ in permission:
             if _:
                 permission_name = _.get("permission_name")
                 if permission_name:
-                    tag_info["tags"].append(permission_name)
-    return tag_info
+                    tag_list.append(permission_name)
+    return tag_list
 
 
 def parse_company_certification_tag(tags):
     certification = tags.get("certification", [])
-    tag_info = {
-        "type": "资质认证名称",
-        "tags": []
-    }
+    tag_list = []
     if certification:
         for _ in certification:
             if _:
                 certification_name = _.get("certification_name")
                 if certification_name:
-                    tag_info["tags"].append(certification_name)
-    return tag_info
+                    tag_list.append(certification_name)
+    return tag_list
 
 
 def parse_company_award_tag(tags):
     award_tag = tags.get("award_tag", [])
-    tag_info = {
-        "type": "奖项名称",
-        "tags": []
-    }
+    tag_list = []
     if award_tag:
         for _ in award_tag:
             if _:
                 tag_name = _.get("tag_name")
                 if tag_name:
-                    tag_info["tags"].append(tag_name)
-    return tag_info
+                    tag_list.append(tag_name)
+    return tag_list
 
 
 def parse_company_rank_tag(tags):
     rank_tag = tags.get("rank_tag", [])
-    tag_info = {
-        "type": "榜单名称",
-        "tags": []
-    }
+    tag_list = []
     if rank_tag:
         for _ in rank_tag:
             if _:
                 rank_name = _.get("rank_name")
                 if rank_name:
-                    tag_info["tags"].append(rank_name)
-    return tag_info
+                    tag_list.append(rank_name)
+    return tag_list
 
 
 def parse_company_diy_tag(tags):
     diy_tag = tags.get("diy_tag", [])
-    tag_info = {
-        "type": "diy标签",
-        "tags": []
-    }
+    tag_list = []
     if diy_tag:
         for _ in diy_tag:
             if _:
-                tag_info["tags"].append(_)
-    return tag_info
+                tag_list.append(_)
+    return tag_list
 
 
 def parse_company_tag(tags: dict, return_type: bool = False, tag_type_list: list = None):
     _tags = []
     tag_dict = {
         "产业标签": parse_company_industry_tag,
         "备案许可级别": parse_company_permission_level_tag,
@@ -112,18 +91,26 @@
         "榜单名称": parse_company_rank_tag,
         "diy标签": parse_company_diy_tag
     }
     if tag_type_list:
         for tag_type in tag_dict:
             if tag_type in tag_type_list and tag_type in tag_dict:
                 if not return_type:
-                    _tags.extend(tag_dict.get(tag_type)(tags).get("tags", []))
-                else:
                     _tags.extend(tag_dict.get(tag_type)(tags))
+                else:
+                    tag_info = {
+                        "tag_type": tag_type,
+                        "tags": tag_dict.get(tag_type)(tags)
+                    }
+                    _tags.append(tag_info)
     else:
         for tag_type in tag_dict:
             if tag_type in tag_dict:
                 if not return_type:
-                    _tags.extend(tag_dict.get(tag_type)(tags).get("tags", []))
-                else:
                     _tags.extend(tag_dict.get(tag_type)(tags))
+                else:
+                    tag_info = {
+                        "tag_type": tag_type,
+                        "tags": tag_dict.get(tag_type)(tags)
+                    }
+                    _tags.append(tag_info)
     return _tags
```

### Comparing `lesscode_utils-0.0.8/lesscode_utils/date_time_utils.py` & `lesscode_utils-0.0.9/lesscode_utils/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/aes.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/base64.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/base64.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/des.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/des.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/hmac.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/hmac.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/rsa.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/rsa.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/smx.py` & `lesscode_utils-0.0.9/lesscode_utils/encryption_algorithm/smx.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/es_utils.py` & `lesscode_utils-0.0.9/lesscode_utils/es_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/json_utils.py` & `lesscode_utils-0.0.9/lesscode_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils/mongo_util.py` & `lesscode_utils-0.0.9/lesscode_utils/mongo_util.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/lesscode_utils.egg-info/SOURCES.txt` & `lesscode_utils-0.0.9/lesscode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.8/setup.py` & `lesscode_utils-0.0.9/setup.py`

 * *Files identical despite different names*

