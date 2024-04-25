# Comparing `tmp/pytip-0.0.2-py2.py3-none-any.whl.zip` & `tmp/pytip-0.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 23566 bytes, number of entries: 25
--rw-rw-r--  2.0 unx      848 b- defN 23-Dec-19 04:23 pytip/__init__.py
+Zip file size: 23737 bytes, number of entries: 25
+-rw-rw-r--  2.0 unx      860 b- defN 24-Apr-25 02:48 pytip/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Dec-19 03:50 pytip/calender/__init__.py
 -rw-rw-r--  2.0 unx       75 b- defN 23-Dec-19 04:18 pytip/calender/base.py
 -rw-rw-r--  2.0 unx     3139 b- defN 23-Dec-19 04:28 pytip/calender/datago.py
 -rw-rw-r--  2.0 unx     2088 b- defN 23-Dec-19 04:22 pytip/calender/koscom.py
 -rw-rw-r--  2.0 unx    42686 b- defN 23-Apr-16 06:56 pytip/json/browsers.json
 -rw-rw-r--  2.0 unx      389 b- defN 23-Dec-19 03:50 pytip/tools/__init__.py
--rw-rw-r--  2.0 unx      591 b- defN 23-Dec-19 03:49 pytip/tools/base.py
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-25 02:45 pytip/tools/base.py
 -rw-rw-r--  2.0 unx     3888 b- defN 23-Dec-19 04:26 pytip/tools/item.py
 -rw-rw-r--  2.0 unx      835 b- defN 23-Nov-27 12:24 pytip/tools/plot.py
--rw-rw-r--  2.0 unx     1598 b- defN 23-Dec-19 03:40 pytip/tools/sheet.py
+-rw-rw-r--  2.0 unx     1665 b- defN 24-Apr-25 02:46 pytip/tools/sheet.py
 -rw-rw-r--  2.0 unx     1589 b- defN 23-Dec-19 03:42 pytip/tools/table.py
 -rw-rw-r--  2.0 unx     2448 b- defN 24-Jan-20 08:20 pytip/tools/tokens.py
 -rw-rw-r--  2.0 unx      423 b- defN 23-Dec-19 04:56 pytip/utils/__init__.py
--rw-rw-r--  2.0 unx      291 b- defN 23-Dec-19 03:48 pytip/utils/base.py
+-rw-rw-r--  2.0 unx      312 b- defN 24-Apr-25 02:47 pytip/utils/base.py
 -rw-rw-r--  2.0 unx     3856 b- defN 23-Dec-19 03:45 pytip/utils/celery.py
--rw-rw-r--  2.0 unx     2177 b- defN 23-Dec-19 03:45 pytip/utils/checker.py
+-rw-rw-r--  2.0 unx     2476 b- defN 24-Apr-25 03:08 pytip/utils/checker.py
 -rw-rw-r--  2.0 unx     1256 b- defN 23-Dec-19 03:45 pytip/utils/deco.py
 -rw-rw-r--  2.0 unx     1568 b- defN 24-Mar-21 11:48 pytip/utils/file.py
 -rw-rw-r--  2.0 unx     1259 b- defN 23-Dec-19 03:46 pytip/utils/func.py
 -rw-rw-r--  2.0 unx     1817 b- defN 23-Dec-19 03:46 pytip/utils/web.py
--rw-rw-r--  2.0 unx     1055 b- defN 24-Mar-21 11:51 pytip-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Mar-21 11:51 pytip-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Mar-21 11:51 pytip-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1915 b- defN 24-Mar-21 11:51 pytip-0.0.2.dist-info/RECORD
-25 files, 75907 bytes uncompressed, 20528 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     1014 b- defN 24-Apr-25 03:09 pytip-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-25 03:09 pytip-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-25 03:09 pytip-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1915 b- defN 24-Apr-25 03:09 pytip-0.0.3.dist-info/RECORD
+25 files, 76269 bytes uncompressed, 20699 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: pytip/utils/func.py
 Comment: 
 
 Filename: pytip/utils/web.py
 Comment: 
 
-Filename: pytip-0.0.2.dist-info/METADATA
+Filename: pytip-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.0.2.dist-info/WHEEL
+Filename: pytip-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.0.2.dist-info/top_level.txt
+Filename: pytip-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.0.2.dist-info/RECORD
+Filename: pytip-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/__init__.py

```diff
@@ -2,15 +2,15 @@
 # `utility` is a program designed to perform a single or a small range of tasks
 # `tool` is A mechanical device intended to make a task easier.
 
 # utility : 독립적 프로그램
 # tools   : 부가적
 
 from .utils.celery import Celery
-from .utils.checker import Message, check_folder_file, check_ip
+from .utils.checker import Message, check_folder_file, check_ip, pkg_missed
 from .utils.deco import web_retries, elapsed_time
 from .utils.web import FakeAgent
 from .utils.func import progressBar
 from .utils.file import (
     multiprocess_items, file_pickle
 ) # file_download
```

## pytip/tools/base.py

```diff
@@ -1,16 +1,16 @@
 import re
-import xlrd
+# import xlrd
 import numpy
 import pandas
 import string
 import random
 import datetime
 import itertools
-import openpyxl
+# import openpyxl
 
 
 # import matplotlib.pyplot as plt
 # from matplotlib.font_manager import fontManager
 REGEX_DATETIME = {
     '[\d]{4}-[\d]{2}-[\d]{2}.[A-Z]{2}[\d]{1,2}:[\d]{1,2}:[\d]{1,2}':
     '%Y-%m-%d.%p%I:%M:%S', # '2022-07-31.AM3:02:30'
```

## pytip/tools/sheet.py

```diff
@@ -24,20 +24,21 @@
         if name == 'xls': 
             return True
         else: return False
 
     @property
     def names(self) -> list:
         r"""Excel WorkSheet 목록 가져오기"""
-        if self._check_xls:
-            wb = xlrd.open_workbook_xls(self.file)
-            return wb.sheet_names()
-        else:
-            wb = openpyxl.load_workbook(self.file)
-            return wb.sheetnames
+        return pandas.ExcelFile(self.file).sheet_names
+        # if self._check_xls:
+        #     wb = xlrd.open_workbook_xls(self.file)
+        #     return wb.sheet_names()
+        # else:
+        #     wb = openpyxl.load_workbook(self.file)
+        #     return wb.sheetnames
 
     def sheet(self, name=None, header:int=None):
         r"""시트 데이터 가져오기
         wb = openpyxl.load_workbook(self.file)
         df = pandas.DataFrame(wb[name].values)        
         """
         if name:
```

## pytip/utils/base.py

```diff
@@ -4,14 +4,15 @@
 import glob
 import json
 import random
 import socket
 import pandas
 import pickle
 import datetime
-import subprocess
 import termcolor
+import subprocess
+import pkg_resources
 from tqdm import tqdm
 from urllib import request
 from functools import wraps
 from multiprocessing import Pool
 # import requests
```

## pytip/utils/checker.py

```diff
@@ -34,14 +34,24 @@
         file_creation_date = datetime.datetime.fromtimestamp(os.path.getatime(file_name)).date()
         if file_creation_date == datetime.datetime.today().date():
             return True, file_name
     
     return False, file_name
 
 
+# 패키지 설치여부 확인
+def pkg_missed(pkgs:list):
+    r"""missing pkg checker -> list"""
+    if type(pkgs) == str: 
+        pkgs = [pkgs]
+    required  = set(pkgs)
+    installed = {pkg.key for pkg in pkg_resources.working_set}
+    missing   = required - installed
+    return list(missing)
+
 # 터미널 메세지 출력기
 # http://www.dreamy.pe.kr/zbxe/CodeClip/165424
 class Message:
     r"""Text Message Color"""
     # grey, red, green, yellow, blue, magenta, cyan, white
     def __repr__(self): 
         return """Text 내용을 상황별 칼라로 출력\n[process, done, alert, warning]"""
```

## Comparing `pytip-0.0.2.dist-info/METADATA` & `pytip-0.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personally tiny useful Python tips
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Requires-Dist: xlrd
 Requires-Dist: termcolor
-Requires-Dist: openpyxl
+Requires-Dist: requests
 Requires-Dist: pandas
-Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # Personally tiny useful Python tips
 
 [![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE)
 [![Docs](https://img.shields.io/badge/docs-stable-blue.svg)](https://domschl.github.io/ml-indie-tools/index.html)
 [![PyPI version fury.io](https://badge.fury.io/py/ml-indie-tools.svg)](https://pypi.python.org/pypi/ml-indie-tools/)
```

## Comparing `pytip-0.0.2.dist-info/RECORD` & `pytip-0.0.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-pytip/__init__.py,sha256=yv73nZoORNTlOs_jaNgDmGl9cJzpYihdAd9GFamtwCg,848
+pytip/__init__.py,sha256=SDZ7SCT6Hp_oYqeaoZK4w2_WzdwJGnoN65qN3N7Nve0,860
 pytip/calender/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytip/calender/base.py,sha256=A-JmM8fv4tGksr06lcOugu56iLhxj9Z1xJRgtbMWpXg,75
 pytip/calender/datago.py,sha256=RP6sF5sPEGa_mxMOZCzjyEshJxNf5zL2Sn1kQO1lpu4,3139
 pytip/calender/koscom.py,sha256=iyqUk2ZYPla-oC7CjMg11G-pTGx9wAAZ4BKXsoYwsko,2088
 pytip/json/browsers.json,sha256=fgvByElwtpg9QpigM0ss-Rpjnc_Uql4-3y0gJDB7dVI,42686
 pytip/tools/__init__.py,sha256=KKqbkgk5EkEh_2jwQdxUtXATP6peuk43t9zGBN0lQE8,389
-pytip/tools/base.py,sha256=fdU-_YzvSerJeJrh5XJ1uDjK8nEYuy4509XU7Egi75w,591
+pytip/tools/base.py,sha256=rNwZ2KUYzSzNGvHyMzBVKp-Xmywo8D1CAh84-WzCM9U,595
 pytip/tools/item.py,sha256=vgaq6s8eSSQcmyCI4dIpdsIrSrfLsaW459I-hFZRLB8,3888
 pytip/tools/plot.py,sha256=DB6ncsJSdA-O7g5rrzqtEBSdidq95LFSaPgACXOYUgU,835
-pytip/tools/sheet.py,sha256=HUsQp1yhewiYpXzITZQjW5C5oCL82bKrYLxIaQgregg,1598
+pytip/tools/sheet.py,sha256=-gM8fGUrMoVd_VRx1xsvNCJb8xrsrXzOPb0kkIJ9H1s,1665
 pytip/tools/table.py,sha256=pvom1VRwMcUINFp-km6eobcT3TASoFR37Jr9EeAcvZc,1589
 pytip/tools/tokens.py,sha256=2a-qszXtuLkA4_fh0giPkjWmWiHMHkHgOPyYqy8N9po,2448
 pytip/utils/__init__.py,sha256=ptGGMFwDewyV4fCaRR3BSwZIGAlug5Z_8xs-scpEDYk,423
-pytip/utils/base.py,sha256=FOqvPx-P0jkKahBylor0Tcv8V01iWlLIVrbtie89LqM,291
+pytip/utils/base.py,sha256=RhqjwInb0TceNZY8mDxrAz70LMX6vGKCRKxDoZfEcXE,312
 pytip/utils/celery.py,sha256=wp1q2kPDZzaMlYiz0VYN0t-606nXqGb72bIyy7r6AOQ,3856
-pytip/utils/checker.py,sha256=8TLbkz-AIoHfbsSC1q7_lr80eAVstBO98aGxd1ggYFM,2177
+pytip/utils/checker.py,sha256=e5jWH5dz4AfDJxu520uvMPryKtv2HGgIeou5ptQexNA,2476
 pytip/utils/deco.py,sha256=mK5gt61NjzKPT4MGclLQ5DlZyMgT5itNF3I_bZ8YH1g,1256
 pytip/utils/file.py,sha256=n1YEDQgAekW6uWl_DxP-KGvqN98iGUAUP6j0oP_kkFA,1568
 pytip/utils/func.py,sha256=dVSSwx9vtU3B-8Ok6wYqLY3BVkgmqs0G39_K8JghU-Q,1259
 pytip/utils/web.py,sha256=nPYZRbvHsx_DsVzea-XUmcxRUTcb-fmNxEUkSTvM2a8,1817
-pytip-0.0.2.dist-info/METADATA,sha256=A1kRFS03OQNXP7yzzAYQ-aUYWhrw0bqFDnpvZKw948M,1055
-pytip-0.0.2.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-pytip-0.0.2.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
-pytip-0.0.2.dist-info/RECORD,,
+pytip-0.0.3.dist-info/METADATA,sha256=HNSft5TZrpG2Me8q92Oit22QvxMOwSq59nPz_E8koI0,1014
+pytip-0.0.3.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+pytip-0.0.3.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
+pytip-0.0.3.dist-info/RECORD,,
```

