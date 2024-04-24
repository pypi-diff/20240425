# Comparing `tmp/navigator_session-0.5.3-py3-none-any.whl.zip` & `tmp/navigator_session-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 17532 bytes, number of entries: 15
--rw-r--r--  2.0 unx     3038 b- defN 24-Mar-22 23:30 navigator_session/__init__.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-22 23:30 navigator_session/conf.py
--rw-r--r--  2.0 unx     5798 b- defN 24-Mar-22 23:30 navigator_session/data.py
--rw-r--r--  2.0 unx     1942 b- defN 24-Mar-22 23:30 navigator_session/middleware.py
--rw-r--r--  2.0 unx     2188 b- defN 24-Mar-22 23:30 navigator_session/session.py
--rw-r--r--  2.0 unx      394 b- defN 24-Mar-22 23:30 navigator_session/version.py
--rw-r--r--  2.0 unx      132 b- defN 24-Mar-22 23:30 navigator_session/storages/__init__.py
--rw-r--r--  2.0 unx     6043 b- defN 24-Mar-22 23:30 navigator_session/storages/abstract.py
--rw-r--r--  2.0 unx     2468 b- defN 24-Mar-22 23:30 navigator_session/storages/cookie.py
--rw-r--r--  2.0 unx     9345 b- defN 24-Mar-22 23:30 navigator_session/storages/redis.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-22 23:30 navigator_session-0.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2288 b- defN 24-Mar-22 23:30 navigator_session-0.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 23:30 navigator_session-0.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-22 23:30 navigator_session-0.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1318 b- defN 24-Mar-22 23:30 navigator_session-0.5.3.dist-info/RECORD
-15 files, 47887 bytes uncompressed, 15326 bytes compressed:  68.0%
+Zip file size: 17540 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3038 b- defN 24-Apr-24 22:19 navigator_session/__init__.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-24 22:19 navigator_session/conf.py
+-rw-r--r--  2.0 unx     5798 b- defN 24-Apr-24 22:19 navigator_session/data.py
+-rw-r--r--  2.0 unx     1942 b- defN 24-Apr-24 22:19 navigator_session/middleware.py
+-rw-r--r--  2.0 unx     2188 b- defN 24-Apr-24 22:19 navigator_session/session.py
+-rw-r--r--  2.0 unx      394 b- defN 24-Apr-24 22:19 navigator_session/version.py
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-24 22:19 navigator_session/storages/__init__.py
+-rw-r--r--  2.0 unx     6043 b- defN 24-Apr-24 22:19 navigator_session/storages/abstract.py
+-rw-r--r--  2.0 unx     2468 b- defN 24-Apr-24 22:19 navigator_session/storages/cookie.py
+-rw-r--r--  2.0 unx     9345 b- defN 24-Apr-24 22:19 navigator_session/storages/redis.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-24 22:19 navigator_session-0.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2339 b- defN 24-Apr-24 22:19 navigator_session-0.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 22:19 navigator_session-0.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-24 22:19 navigator_session-0.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1318 b- defN 24-Apr-24 22:19 navigator_session-0.5.4.dist-info/RECORD
+15 files, 47938 bytes uncompressed, 15334 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: navigator_session/storages/cookie.py
 Comment: 
 
 Filename: navigator_session/storages/redis.py
 Comment: 
 
-Filename: navigator_session-0.5.3.dist-info/LICENSE
+Filename: navigator_session-0.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: navigator_session-0.5.3.dist-info/METADATA
+Filename: navigator_session-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: navigator_session-0.5.3.dist-info/WHEEL
+Filename: navigator_session-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: navigator_session-0.5.3.dist-info/top_level.txt
+Filename: navigator_session-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: navigator_session-0.5.3.dist-info/RECORD
+Filename: navigator_session-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## navigator_session/version.py

```diff
@@ -1,11 +1,11 @@
 """Navigator Session Meta information.
    Navigator Session allows us to store user-specific data into session object.
 """
 
 __title__ = 'navigator_session'
 __description__ = ('Navigator Session allows us to store user-specific data '
                    'into session object.')
-__version__ = '0.5.3'
+__version__ = '0.5.4'
 __author__ = 'Jesus Lara'
 __author_email__ = 'jesuslarag@gmail.com'
 __license__ = 'Apache-2.0'
```

## Comparing `navigator_session-0.5.3.dist-info/LICENSE` & `navigator_session-0.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `navigator_session-0.5.3.dist-info/METADATA` & `navigator_session-0.5.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigator-session
-Version: 0.5.3
+Version: 0.5.4
 Summary: Navigator Session allows us to store user-specific data into session object.
 Home-page: https://github.com/phenobarbital/navigator-session
 Author: Jesus Lara
 Author-email: jesuslarag@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/phenobarbital/navigator-session
 Project-URL: Funding, https://paypal.me/phenobarbital
@@ -17,20 +17,21 @@
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Requires-Python: >=3.9.16
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp ==3.9.3
+Requires-Dist: aiohttp >=3.9.5
 Requires-Dist: uvloop ==0.19.0
 Requires-Dist: asyncio ==3.4.3
 Requires-Dist: jsonpickle ==3.0.2
 Requires-Dist: redis ==5.0.1
 Requires-Dist: python-datamodel >=0.2.1
 Requires-Dist: navconfig[default] >=1.6.3
```

## Comparing `navigator_session-0.5.3.dist-info/RECORD` & `navigator_session-0.5.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 navigator_session/__init__.py,sha256=xsmc90K04EgQEtYidPN7bsXn0WIqw6GucNwy138Mmno,3038
 navigator_session/conf.py,sha256=PwCGoYpg_2MEq5_zObvbx4yXKf7AIKObO-lzTh2AvxM,1466
 navigator_session/data.py,sha256=tD40x16dujarX3F1RMPAuYqDP3oiG_8kyqLNYyD3Ik4,5798
 navigator_session/middleware.py,sha256=7RO83pz4q16_56GvmbswEukbDZQ0JutJdVdF4UHbEw8,1942
 navigator_session/session.py,sha256=I6qWkMbqIpVX1RjxmccGsk1sCcqWZ_ZBVGwLXjV8wjw,2188
-navigator_session/version.py,sha256=ZLk7Wt5xlc7MSppNZmPBeL5ogFgNpd7HawJUWB5JfPg,394
+navigator_session/version.py,sha256=qSxTZ3mS3AQhfwhuDIjPEcFTmAJHRYc0K4Ax5JRAzFc,394
 navigator_session/storages/__init__.py,sha256=ln0Xli0lppUopDMrvQGt69BFtUAe1Grmy2DGkEpANNU,132
 navigator_session/storages/abstract.py,sha256=5nqEF0I0G3p4pcTNfOQYspbXp-U7QJntJWVsKYDu9KY,6043
 navigator_session/storages/cookie.py,sha256=_qL5kIGbT4rtCMze4yj1h4J7Zauz_e7HnorPnFbi90w,2468
 navigator_session/storages/redis.py,sha256=qk8V3FGYDLbfTT851NOU864hSsgup661b8GY1u_uhtQ,9345
-navigator_session-0.5.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-navigator_session-0.5.3.dist-info/METADATA,sha256=plJi8EJAbzFmxdbAViAkfcLbc_KasF34eedFM2OqZS4,2288
-navigator_session-0.5.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-navigator_session-0.5.3.dist-info/top_level.txt,sha256=ZpOEy3wLKGsxG2rc0nHqcqJCV3HIOG_XCfE6mtsYYYY,18
-navigator_session-0.5.3.dist-info/RECORD,,
+navigator_session-0.5.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+navigator_session-0.5.4.dist-info/METADATA,sha256=jM_jzjllmFiA2LESsLvD-9cd2CG3w-bHcFMGOGfJx18,2339
+navigator_session-0.5.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+navigator_session-0.5.4.dist-info/top_level.txt,sha256=ZpOEy3wLKGsxG2rc0nHqcqJCV3HIOG_XCfE6mtsYYYY,18
+navigator_session-0.5.4.dist-info/RECORD,,
```
