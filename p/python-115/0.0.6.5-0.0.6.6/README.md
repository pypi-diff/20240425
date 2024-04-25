# Comparing `tmp/python_115-0.0.6.5.tar.gz` & `tmp/python_115-0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.5.tar", max compression
+gzip compressed data, was "python_115-0.0.6.6.tar", max compression
```

## Comparing `python_115-0.0.6.5.tar` & `python_115-0.0.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.5/LICENSE
--rwxr-xr-x   0        0        0   275665 2024-04-25 02:47:37.342012 python_115-0.0.6.5/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.5/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.5/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.5/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.5/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.5/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.5/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.5/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.5/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.5/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.5/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.5/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.5/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.5/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.5/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.5/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.5/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.5/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.5/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.5/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.5/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.5/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.5/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.5/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.5/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-25 02:47:55.533442 python_115-0.0.6.5/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.5/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.6/LICENSE
+-rwxr-xr-x   0        0        0   276236 2024-04-25 03:09:59.573772 python_115-0.0.6.6/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.6/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.6/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.6/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.6/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.6/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.6/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.6/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.6/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.6/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.6/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.6/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.6/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.6/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.6/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.6/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.6/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.6/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.6/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.6/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.6/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.6/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.6/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.6/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.6/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-25 03:24:55.949053 python_115-0.0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.6/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.6/PKG-INFO
```

### Comparing `python_115-0.0.6.5/LICENSE` & `python_115-0.0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/__init__.py` & `python_115-0.0.6.6/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5909,14 +5909,33 @@
                                 path_to_id[new_subpath] = subid
                         if subattr["is_directory"]:
                             put(subid)
             if path_to_id is not None and pop_path is not None:
                 for k in tuple(k for k in path_to_id if startswith(k, old_path)):
                     pop_path(k)
 
+    def download(
+        self, 
+        id_or_path: IDOrPathType, 
+        /, 
+        local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
+        pid: Optional[int] = None, 
+        write_mode: Literal["a", "w", "x", "i"] = "a", 
+        submit = None, 
+        use_web_api: bool = True, 
+    ) -> Optional[DownloadTask]:
+        return super().download(
+            id_or_path, 
+            local_path_or_file, 
+            pid=pid, 
+            write_mode=write_mode, 
+            submit=submit, 
+            use_web_api=use_web_api, 
+        )
+
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         refresh: bool = False, 
     ) -> Iterator[AttrDict]:
```

### Comparing `python_115-0.0.6.5/p115/cmd/iterdir.py` & `python_115-0.0.6.6/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/cmd/qrcode.py` & `python_115-0.0.6.6/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/_init_mimetypes.py` & `python_115-0.0.6.6/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/cipher.py` & `python_115-0.0.6.6/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/concurrent.py` & `python_115-0.0.6.6/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/download.py` & `python_115-0.0.6.6/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/file.py` & `python_115-0.0.6.6/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/hash.py` & `python_115-0.0.6.6/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/ignore.py` & `python_115-0.0.6.6/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/iter.py` & `python_115-0.0.6.6/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/path.py` & `python_115-0.0.6.6/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/property.py` & `python_115-0.0.6.6/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/response.py` & `python_115-0.0.6.6/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/retry.py` & `python_115-0.0.6.6/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/text.py` & `python_115-0.0.6.6/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/p115/util/urlopen.py` & `python_115-0.0.6.6/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/pyproject.toml` & `python_115-0.0.6.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.5"
+version = "0.0.6.6"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.5/readme.md` & `python_115-0.0.6.6/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.5/PKG-INFO` & `python_115-0.0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.5
+Version: 0.0.6.6
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

