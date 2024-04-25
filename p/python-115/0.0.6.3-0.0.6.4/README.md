# Comparing `tmp/python_115-0.0.6.3.tar.gz` & `tmp/python_115-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.3.tar", max compression
+gzip compressed data, was "python_115-0.0.6.4.tar", max compression
```

## Comparing `python_115-0.0.6.3.tar` & `python_115-0.0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.3/LICENSE
--rwxr-xr-x   0        0        0   273428 2024-04-20 20:12:10.926457 python_115-0.0.6.3/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.3/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.3/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.3/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-19 15:25:32.941526 python_115-0.0.6.3/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.3/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.3/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.3/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.3/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.3/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.6.3/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.3/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.3/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6.3/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.3/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.3/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.3/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.3/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.3/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.6.3/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.3/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.6.3/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.3/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.3/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.3/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-20 20:25:11.423803 python_115-0.0.6.3/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.3/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.4/LICENSE
+-rwxr-xr-x   0        0        0   275249 2024-04-25 02:00:17.850869 python_115-0.0.6.4/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.4/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.4/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.4/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.4/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.4/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.4/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.4/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.4/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.4/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.4/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.4/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.4/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6.4/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.4/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.4/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.4/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.4/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.4/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.4/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.4/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.4/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.4/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.4/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.4/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-25 02:00:46.390576 python_115-0.0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.4/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.4/PKG-INFO
```

### Comparing `python_115-0.0.6.3/LICENSE` & `python_115-0.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/__init__.py` & `python_115-0.0.6.4/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,25 @@
                     info2[k3] = t
             except ValueError:
                 pass
     if "pc" in info:
         info2["pickcode"] = info["pc"]
     if "m" in info:
         info2["star"] = bool(info["m"])
+    if "fl" in info:
+        info2["labels"] = info["fl"]
+    if "fdes" in info:
+        info2["comment"] = info["fdes"]
+    if "score" in info:
+        info2["score"] = info["score"]
     if "u" in info:
         info2["thumb"] = info["u"]
     if "play_long" in info:
         info2["play_long"] = info["play_long"]
+    info2["is_violation"] = bool(info.get("c", False))
     if keep_raw:
         info2["raw"] = info
     if extra_data:
         info2.update(extra_data)
     return info2
 
 
@@ -523,14 +530,26 @@
     ) -> dict:
         """检查当前用户的登录状态
         GET http://passportapi.115.com/app/1.0/web/1.0/check/sso/
         """
         api = "http://passportapi.115.com/app/1.0/web/1.0/check/sso/"
         return self.request(api, async_=async_, **request_kwargs)
 
+    def login_devices(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        """获取已登录设备的信息
+        GET https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices
+        """
+        api = "https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices"
+        return self.request(api, async_=async_, **request_kwargs)
+
     def login_qrcode_status(
         self, 
         payload: dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
@@ -1043,15 +1062,15 @@
     def fs_get_repeat(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        """文件查重
+        """文件查重（罗列除此以外的 sha1 相同的文件）
         GET https://webapi.115.com/files/get_repeat_sha
         payload:
             file_id: int | str
         """
         api = "https://webapi.115.com/files/get_repeat_sha"
         if isinstance(payload, (int, str)):
             payload = {"file_id": payload}
@@ -1810,41 +1829,63 @@
 
     def download_url(
         self, 
         pickcode: str, 
         /, 
         detail: bool = False, 
         strict: bool = True, 
+        use_web_api: bool = False, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取文件的下载链接，此接口是对 `download_url_app` 的封装
         """
-        resp = self.download_url_app(
-            {"pickcode": pickcode}, 
-            async_=async_, 
-            **request_kwargs, 
-        )
-        def get_url(resp: dict) -> str:
-            data = check_response(resp)["data"]
-            for fid, info in data.items():
-                url = info["url"]
-                if strict and not url:
-                    raise IsADirectoryError(errno.EISDIR, f"{fid} is a directory")
-                if not detail:
-                    return url["url"] if url else ""
-                return UrlStr(
-                    url["url"] if url else "", 
-                    id=int(fid), 
-                    pickcode=info["pick_code"], 
-                    file_name=info["file_name"], 
-                    file_size=int(info["file_size"]), 
-                    is_directory=not url,
-                )
-            raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
+        if use_web_api:
+            resp = self.download_url_web(
+                {"pickcode": pickcode}, 
+                async_=async_, 
+                **request_kwargs, 
+            )
+            def get_url(resp: dict) -> str:
+                if "pickcode" not in resp:
+                    raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
+                if detail:
+                    return UrlStr(
+                        resp.get("file_url", ""), 
+                        id=int(resp["file_id"]), 
+                        pickcode=resp["pickcode"], 
+                        file_name=resp["file_name"], 
+                        file_size=int(resp["file_size"]), 
+                        is_directory=not resp["state"], 
+                    )
+                return resp.get("file_url", "")
+        else:
+            resp = self.download_url_app(
+                {"pickcode": pickcode}, 
+                async_=async_, 
+                **request_kwargs, 
+            )
+            def get_url(resp: dict) -> str:
+                if not resp["state"]:
+                    raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
+                for fid, info in resp["data"].items():
+                    url = info["url"]
+                    if strict and not url:
+                        raise IsADirectoryError(errno.EISDIR, f"{fid} is a directory")
+                    if not detail:
+                        return url["url"] if url else ""
+                    return UrlStr(
+                        url["url"] if url else "", 
+                        id=int(fid), 
+                        pickcode=info["pick_code"], 
+                        file_name=info["file_name"], 
+                        file_size=int(info["file_size"]), 
+                        is_directory=not url,
+                    )
+                raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
         if async_:
             async def wrapper() -> str:
                 return get_url(await resp)  # type: ignore
             return wrapper() # type: ignore
         return get_url(resp)
 
     ########## Upload API ##########
@@ -6296,25 +6337,18 @@
         pid: Optional[int] = None, 
     ) -> int:
         return self.fs_files(self.get_id(id_or_path, pid), limit=1)["count"]
 
     def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
         if not pickcode:
             return 0
-        data = self.get_info_from_pickcode(pickcode)
-        for fid in data:
-            return int(fid)
-        raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}") 
+        return self.get_info_from_pickcode(pickcode)["id"]
 
-    def get_info_from_pickcode(
-        self, 
-        /, 
-        pickcode: str, 
-    ) -> dict:
-        return check_response(self.client.download_url_app(pickcode))["data"]
+    def get_info_from_pickcode(self, /, pickcode: str) -> dict:
+        return self.client.download_url(pickcode, strict=False, detail=True).__dict__
 
     def get_pickcode(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> str:
@@ -6327,24 +6361,35 @@
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
-        return self.client.download_url(attr["pickcode"], detail=detail, headers=headers)
+        return self.client.download_url(
+            attr["pickcode"], 
+            use_web_api=attr["size"] < 1024 * 1024 * 115, 
+            detail=detail, 
+            headers=headers, 
+        )
 
     def get_url_from_pickcode(
         self, 
         /, 
         pickcode: str, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
+        use_web_api: bool = False, 
     ) -> str:
-        return self.client.download_url(pickcode, detail=detail, headers=headers)
+        return self.client.download_url(
+            pickcode, 
+            detail=detail, 
+            headers=headers, 
+            use_web_api=use_web_api, 
+        )
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
```

### Comparing `python_115-0.0.6.3/p115/cmd/iterdir.py` & `python_115-0.0.6.4/p115/cmd/iterdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,16 @@
         file.close()
 
 
 parser.add_argument("path", nargs="?", default="0", help="文件夹路径或 id，默认值 0，即根目录")
 parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果缺失，则从 115-cookie.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
 parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
 parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
-parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""输出类型，默认为 json
+parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""
+输出类型，默认为 log
 - log   每行输出一条数据，每条数据输出为一个 json 的 object
 - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
 - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
 """)
 parser.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
 parser.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于或等于 0 时不限")
 parser.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
```

### Comparing `python_115-0.0.6.3/p115/cmd/qrcode.py` & `python_115-0.0.6.4/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/_init_mimetypes.py` & `python_115-0.0.6.4/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/cipher.py` & `python_115-0.0.6.4/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/concurrent.py` & `python_115-0.0.6.4/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/download.py` & `python_115-0.0.6.4/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/file.py` & `python_115-0.0.6.4/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/hash.py` & `python_115-0.0.6.4/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/ignore.py` & `python_115-0.0.6.4/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/iter.py` & `python_115-0.0.6.4/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/path.py` & `python_115-0.0.6.4/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/property.py` & `python_115-0.0.6.4/p115/util/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["funcproperty", "lazyproperty", "cacheproperty", "final_cacheproperty"]
 
+from collections.abc import Callable
 from typing import Any
 
 
 class funcproperty:
 
-    def __init__(self, func, /):
+    def __init__(self, func: Callable, /):
         self.__func__ = func
         self.__name__ = getattr(func, "__name__", None)
         self.__doc__  = getattr(func, "__doc__", None)
 
     def __repr__(self, /):
         return f"{type(self).__qualname__}({self.__func__!r})"
 
-    def __set_name__(self, cls, name, /):
+    def __set_name__(self, cls, name: str, /):
         self.__name__ = name
 
     def __get__(self, instance, cls, /):
         if instance is None:
             return self
         return self.__func__(instance)
```

### Comparing `python_115-0.0.6.3/p115/util/response.py` & `python_115-0.0.6.4/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/retry.py` & `python_115-0.0.6.4/p115/util/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["retry", "raise_for_value"]
 
+from collections.abc import Callable, Iterable
 from asyncio import sleep as asleep
 from functools import partial, update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from itertools import count
 from time import sleep
-from typing import Any, Callable, Iterable, Optional, TypeVar
+from typing import Any, Optional, TypeVar
 
 
 T = TypeVar("T")
 
 
 async def ensure_awaitable(o, /):
     "Make an object awaitable."
```

### Comparing `python_115-0.0.6.3/p115/util/text.py` & `python_115-0.0.6.4/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/p115/util/urlopen.py` & `python_115-0.0.6.4/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/pyproject.toml` & `python_115-0.0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.3"
+version = "0.0.6.4"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.3/readme.md` & `python_115-0.0.6.4/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.3/PKG-INFO` & `python_115-0.0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

