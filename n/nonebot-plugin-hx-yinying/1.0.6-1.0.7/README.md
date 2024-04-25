# Comparing `tmp/nonebot-plugin-hx-yinying-1.0.6.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.6.tar", last modified: Thu Apr 25 16:12:09 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.7.tar", last modified: Thu Apr 25 16:52:55 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.0.6.tar` & `nonebot-plugin-hx-yinying-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     5087 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.262818 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    61842 2024-04-25 15:58:39.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    84465 2024-04-25 16:10:17.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-25 14:22:54.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     5087 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-25 16:12:09.553215 nonebot-plugin-hx-yinying-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-25 16:11:47.000000 nonebot-plugin-hx-yinying-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:52:55.076918 nonebot-plugin-hx-yinying-1.0.7/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-25 16:52:55.078921 nonebot-plugin-hx-yinying-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:52:54.925921 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    61842 2024-04-25 15:58:39.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    84465 2024-04-25 16:10:17.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-25 14:22:54.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:52:55.069929 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-25 16:52:53.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-25 16:52:54.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:52:53.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2024-04-25 16:52:53.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-25 16:52:53.000000 nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-25 16:52:55.111925 nonebot-plugin-hx-yinying-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      895 2024-04-25 16:52:24.000000 nonebot-plugin-hx-yinying-1.0.7/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.0.6/LICENSE` & `nonebot-plugin-hx-yinying-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.6/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.6
+Version: 1.0.7
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.7 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.6/README.md` & `nonebot-plugin-hx-yinying-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying/chat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.6
+Version: 1.0.7
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.7 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.0.6/setup.py` & `nonebot-plugin-hx-yinying-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.0.6",
+    version="1.0.7",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
-    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0'],
+    install_requires=['nonebot2>=2.2.1', 'ujson>=5.9.0', 'httpx>=0.27.0', 'nonebot-adapter-onebot>=2.4.3', 'nonebot_plugin_localstore>=0.6.0', 'pydantic>=1.10.12','requests>=2.31.0','nonebot_plugin_apscheduler>=0.4.0'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

