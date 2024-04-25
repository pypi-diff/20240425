# Comparing `tmp/lesscode_tag-0.0.8.tar.gz` & `tmp/lesscode_tag-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tag-0.0.8.tar", last modified: Wed Aug 23 06:10:51 2023, max compression
+gzip compressed data, was "dist/lesscode_tag-0.0.9.tar", last modified: Wed Sep 13 08:44:03 2023, max compression
```

## Comparing `lesscode_tag-0.0.8.tar` & `lesscode_tag-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/
--rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/PKG-INFO
--rw-r--r--   0 zhengy     (501) staff       (20)       52 2023-05-25 10:25:23.000000 lesscode_tag-0.0.8/README.md
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag/
--rw-r--r--   0 zhengy     (501) staff       (20)        0 2023-05-25 10:25:23.000000 lesscode_tag-0.0.8/lesscode_tag/__init__.py
--rw-r--r--   0 zhengy     (501) staff       (20)     9292 2023-08-23 06:02:59.000000 lesscode_tag-0.0.8/lesscode_tag/business.py
--rw-r--r--   0 zhengy     (501) staff       (20)       22 2023-08-23 06:10:43.000000 lesscode_tag-0.0.8/lesscode_tag/version.py
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/
--rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/PKG-INFO
--rw-r--r--   0 zhengy     (501) staff       (20)      271 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/SOURCES.txt
--rw-r--r--   0 zhengy     (501) staff       (20)        1 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/dependency_links.txt
--rw-r--r--   0 zhengy     (501) staff       (20)       22 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/requires.txt
--rw-r--r--   0 zhengy     (501) staff       (20)       13 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/lesscode_tag.egg-info/top_level.txt
--rw-r--r--   0 zhengy     (501) staff       (20)       38 2023-08-23 06:10:51.000000 lesscode_tag-0.0.8/setup.cfg
--rw-r--r--   0 zhengy     (501) staff       (20)     1299 2023-08-23 06:02:59.000000 lesscode_tag-0.0.8/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.9/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.9/lesscode_tag/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)    10151 2023-09-13 08:43:22.000000 lesscode_tag-0.0.9/lesscode_tag/business.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-09-13 08:43:22.000000 lesscode_tag-0.0.9/lesscode_tag/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      271 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/requires.txt
+-rw-r--r--   0 baai       (501) staff       (20)       13 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/lesscode_tag.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-09-13 08:44:03.000000 lesscode_tag-0.0.9/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1299 2023-07-18 07:15:14.000000 lesscode_tag-0.0.9/setup.py
```

### Comparing `lesscode_tag-0.0.8/lesscode_tag/business.py` & `lesscode_tag-0.0.9/lesscode_tag/business.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,43 @@
                                              "must_not": [{"terms": {"tags.diy_tag": ["国家级专精特新企业"]}}]}}]}})
     if tag in ["国家级专精特新", "国家级单项冠军", "瞪羚"]:
         should.append({"bool": {"must": [{"terms": {"tags.diy_tag": [tag + "企业"]}}]}})
     if tag in ["高新技术企业", "央企", "瞪羚企业", "中国企业500强"]:
         should.append({"bool": {"must": [{"terms": {"tags.diy_tag": [tag]}}]}})
     if tag in ["单项冠军"]:
         should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["国家级单项冠军企业"]}}]}})
+    if tag in ["单项冠军_ALL"]:
+        should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["国家级单项冠军企业"]}}]}})
+        should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["省级单项冠军企业"]}}]}})
     if tag in ["专精特新"]:
         should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["省级专精特新企业", "国家级专精特新企业"]}}]}})
     if tag in ["A股上市"]:
         should.append(
             {"bool": {"must": [{"terms": {"tags.market_tag.block": ["主板上市", "科创板上市", "创业板上市", "北交所"]}},
                                {"terms": {"tags.market_tag.status": ["已上市"]}}]}})
     if tag in ["新三板"]:
         should.append({"bool": {"must": [{"terms": {"tags.market_tag.status": ["新三板挂牌"]}}]}})
     if tag in ["已上市", "排队上市", "已退市"]:
         should.append({"bool": {"must": [{"terms": {"tags.market_tag.status": [tag]}}]}})
     if tag in ["主板上市", "创业板上市", "科创板上市", "新三板-基础层", "新三板-创新层", "新三板-精选层", "北交所"]:
         should.append({"bool": {"must": [{"terms": {"tags.market_tag.block": [tag]}}]}})
+    if tag in ["国有大型企业"]:
+        should.append({"bool": {"must": [{"terms": {"tags.capital_type": ["国有"]}},
+                                         {"terms": {"tags.scale_tag": ["大型"]}}]}})
+    if tag in ["大型企业"]:
+        should.append({"bool": {"must": [{"terms": {"tags.scale_tag": ["大型"]}}]}})
+    if tag in ["国有企业"]:
+        should.append({"bool": {"must": [{"terms": {"tags.capital_type": ["国有"]}}]}})
+    if tag in ["省级单项冠军"]:
+        should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["省级单项冠军企业"]}}]}})
+
     # 其他  -此类不标准，尽量不要使用
     if tag in ["小巨人", "一条龙"]:
         should.append({"bool": {"must": [{"wildcard": {"tags.national_tag.tag_name": f"*{tag}*"}}]}})
-    if tag in ["隐形冠军", "成长", "小巨人", "首台套", "雏鹰", "省级单项冠军"]:
+    if tag in ["隐形冠军", "成长", "小巨人", "首台套", "雏鹰"]:
         should.append({"bool": {"must": [{"wildcard": {"tags.province_tag.tag_name": f"*{tag}*"}}]}})
     if tag in ["雏鹰"]:
         should.append({"bool": {"must": [{"wildcard": {"tags.city_tag.tag_name": f"*{tag}*"}}]}})
     if tag in ["雏鹰"]:
         should.append({"bool": {"must": [{"wildcard": {"tags.district_tag.tag_name": f"*{tag}*"}}]}})
     if tag in ["独角兽"]:
         should.append({"bool": {"must": [{"wildcard": {"tags.rank_tag.rank_name": f"*{tag}*"}}]}})
@@ -107,22 +120,22 @@
             if tag in ["独角兽"]:
                 es_condition_by_wildcard(bool_should_list, "tags.rank_tag.rank_name", tag)
             if tag in ["科技型中小企业"]:
                 es_condition_by_terms(bool_should_list, "tags.certification.certification_name", [tag])
             if tag in ["规上企业"]:
                 es_condition_by_terms(bool_should_list, "tags.nonpublic_tag", [tag])
     bool_should_more_list.append(bool_should_list)
-    return bool_should_more_list
 
 
 def parse_special_tag_new(tags, tags_param_list=None):
     """新版产业通 特色标签 解析，临时用等数据组将标签添加到diy_tag修改此方法"""
     result = []
     for tag in tags.get("market_tag", []):
-        if tag.get("status", "") == "已上市" and tag.get("block", "") in ["主板上市", "科创板上市", "创业板上市", "北交所"]:
+        if tag.get("status", "") == "已上市" and tag.get("block", "") in ["主板上市", "科创板上市", "创业板上市",
+                                                                          "北交所"]:
             result.append("A股上市")
         if tag.get("status", "") == "新三板挂牌":
             result.append("新三板")
     for tag in tags.get("diy_tag", []):
         for t in ["国家级专精特新", "省级专精特新", "国家级单项冠军", '瞪羚']:
             if t in tag:
                 result.append(t)
```

### Comparing `lesscode_tag-0.0.8/setup.py` & `lesscode_tag-0.0.9/setup.py`

 * *Files identical despite different names*

