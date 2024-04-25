# Comparing `tmp/yunxiao-0.5.2.tar.gz` & `tmp/yunxiao-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.2.tar", last modified: Thu Apr 25 15:46:43 2024, max compression
+gzip compressed data, was "yunxiao-0.5.3.tar", last modified: Thu Apr 25 16:29:13 2024, max compression
```

## Comparing `yunxiao-0.5.2.tar` & `yunxiao-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.857073 yunxiao-0.5.2/
--rw-rw-rw-   0        0        0      509 2024-04-25 15:46:43.857073 yunxiao-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.2/README.md
--rw-rw-rw-   0        0        0     2101 2024-04-25 15:46:29.000000 yunxiao-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 15:46:43.858073 yunxiao-0.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.841073 yunxiao-0.5.2/yunxiao/
--rw-rw-rw-   0        0        0       53 2024-02-29 10:36:23.000000 yunxiao-0.5.2/yunxiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.854079 yunxiao-0.5.2/yunxiao/schemas/
--rw-rw-rw-   0        0        0      124 2024-04-25 15:13:05.000000 yunxiao-0.5.2/yunxiao/schemas/__init__.py
--rw-rw-rw-   0        0        0     2607 2024-04-25 15:38:16.000000 yunxiao-0.5.2/yunxiao/schemas/teachers.py
--rw-rw-rw-   0        0        0    36704 2024-04-25 15:46:15.000000 yunxiao-0.5.2/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:46:43.855076 yunxiao-0.5.2/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 15:46:43.000000 yunxiao-0.5.2/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 16:29:13.563712 yunxiao-0.5.3/
+-rw-rw-rw-   0        0        0      509 2024-04-25 16:29:13.562712 yunxiao-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.3/README.md
+-rw-rw-rw-   0        0        0     2167 2024-04-25 16:29:04.000000 yunxiao-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:29:13.563712 yunxiao-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 16:29:13.550712 yunxiao-0.5.3/yunxiao/
+-rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.3/yunxiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:29:13.560713 yunxiao-0.5.3/yunxiao/schemas/
+-rw-rw-rw-   0        0        0      124 2024-04-25 15:13:05.000000 yunxiao-0.5.3/yunxiao/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2607 2024-04-25 15:38:16.000000 yunxiao-0.5.3/yunxiao/schemas/teachers.py
+-rw-rw-rw-   0        0        0    36704 2024-04-25 15:46:15.000000 yunxiao-0.5.3/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:29:13.561712 yunxiao-0.5.3/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-25 16:29:13.000000 yunxiao-0.5.3/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-25 16:29:13.000000 yunxiao-0.5.3/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:29:13.000000 yunxiao-0.5.3/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 16:29:13.000000 yunxiao-0.5.3/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 16:29:13.000000 yunxiao-0.5.3/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.2/pyproject.toml` & `yunxiao-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.2"
+version = "0.5.3"
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
+"0.5.3" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.1" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.5.0" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.4.9" = "新增: '账户明细'端点;\n改进: 尝试将会话重用"
 "0.4.8" = "修复: 因域名造成的远程服务不存在问题"
 "0.4.7" = "新增: 查询课消明细"
 "0.4.6" = "修复: 修复"
```

### Comparing `yunxiao-0.5.2/yunxiao/schemas/teachers.py` & `yunxiao-0.5.3/yunxiao/schemas/teachers.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.2/yunxiao/yunxiao.py` & `yunxiao-0.5.3/yunxiao/yunxiao.py`

 * *Files identical despite different names*

