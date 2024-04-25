# Comparing `tmp/yunxiao-0.5.1.tar.gz` & `tmp/yunxiao-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.1.tar", last modified: Tue Apr  2 07:17:36 2024, max compression
+gzip compressed data, was "yunxiao-0.5.2.tar", last modified: Thu Apr 25 15:46:43 2024, max compression
```

## Comparing `yunxiao-0.5.1.tar` & `yunxiao-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:17:36.803225 yunxiao-0.5.1/
--rw-rw-rw-   0        0        0      509 2024-04-02 07:17:36.803225 yunxiao-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.1/README.md
--rw-rw-rw-   0        0        0     2035 2024-04-02 07:17:30.000000 yunxiao-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 07:17:36.803225 yunxiao-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 07:17:36.794648 yunxiao-0.5.1/yunxiao/
--rw-rw-rw-   0        0        0       53 2024-02-29 10:36:23.000000 yunxiao-0.5.1/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    35502 2024-04-02 07:16:34.000000 yunxiao-0.5.1/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:17:36.802226 yunxiao-0.5.1/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-02 07:17:36.000000 yunxiao-0.5.1/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-02 07:17:36.000000 yunxiao-0.5.1/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:17:36.000000 yunxiao-0.5.1/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 07:17:36.000000 yunxiao-0.5.1/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 07:17:36.000000 yunxiao-0.5.1/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.857073 yunxiao-0.5.2/
+-rw-rw-rw-   0        0        0      509 2024-04-25 15:46:43.857073 yunxiao-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.2/README.md
+-rw-rw-rw-   0        0        0     2101 2024-04-25 15:46:29.000000 yunxiao-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:46:43.858073 yunxiao-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.841073 yunxiao-0.5.2/yunxiao/
+-rw-rw-rw-   0        0        0       53 2024-02-29 10:36:23.000000 yunxiao-0.5.2/yunxiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.854079 yunxiao-0.5.2/yunxiao/schemas/
+-rw-rw-rw-   0        0        0      124 2024-04-25 15:13:05.000000 yunxiao-0.5.2/yunxiao/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2607 2024-04-25 15:38:16.000000 yunxiao-0.5.2/yunxiao/schemas/teachers.py
+-rw-rw-rw-   0        0        0    36704 2024-04-25 15:46:15.000000 yunxiao-0.5.2/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.855076 yunxiao-0.5.2/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.1/pyproject.toml` & `yunxiao-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.1"
+version = "0.5.2"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.1" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.5.0" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.4.9" = "新增: '账户明细'端点;\n改进: 尝试将会话重用"
 "0.4.8" = "修复: 因域名造成的远程服务不存在问题"
 "0.4.7" = "新增: 查询课消明细"
 "0.4.6" = "修复: 修复"
 "0.4.5" = "改进: 将token和cookie保存在对象内部，移除V3"
```

### Comparing `yunxiao-0.5.1/yunxiao/yunxiao.py` & `yunxiao-0.5.2/yunxiao/yunxiao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import time
 import requests
+from schemas import *
 
 
 def timestamp():
     return int(time.time() * 1000)
 
 
 class YunXiao:
@@ -106,14 +107,32 @@
                     page += 1  # 翻页
                 return data_list
 
             return wrapper
 
         return wrapper_func
 
+    def _loop_pages(self, endpoint, payload: [TeschersQueryPayload], schemas: [Teschers]) -> Teschers:
+        response = schemas()  # 结果列表
+        while payload.page.pageNum <= response.page.totalPage:
+            res = self.request(method="post", url=endpoint, json=payload)
+            try:
+                new = schemas(**res)
+                response.data.extend(new.data)
+                response.page.totalPage = new.page.totalPage
+                response.page.totalCount = new.page.totalCount
+
+                logging.debug(f"size: {payload.page.pageSize}, page: {payload.page.pageNum}/{response.page.totalPage}, "
+                              f"{payload.page.pageNum * payload.page.pageSize}/{response.page.totalCount}")  # 汇报数量
+
+                payload.page.pageNum += 1  # 翻页
+            except TypeError:
+                logging.error(res)
+        return response
+
     # 查询机构指定日期范围业绩。
     def company_query_performance(self, startdate: str, enddate: str) -> list:
         """
         查询机构指定日期范围业绩。
         :param startdate: 起始日期
         :param enddate: 截止日期
         :return:
@@ -200,14 +219,21 @@
                 "roleIds": [],
                 "orgStructureId": "",
                 "campusIds": self.campus,
                 "statusList": list(status)
             }
         )
 
+    def _teachers_query(self, payload: TeschersQueryPayload) -> Teschers:
+        """
+        查询老师。
+        :return: Teachers
+        """
+        return self._loop_pages(f"https://{self.host}/api/cs-pc-crm/teacher/pageList", payload, Teschers)
+
     # 查询意向（APP接口）
     @loop_pages()
     def intentions_query(self, page, size, distributeStatus: int = 1, keyWord: str = "", level: int = "",
                          nonFollowUpDays: int = "", startNextTime: str = "", endNextTime: str = "",
                          startLastCommunicateTime: str = "", endLastCommunicateTime: str = ""):
         """
         查询意向
```

