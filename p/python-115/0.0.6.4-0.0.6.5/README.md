# Comparing `tmp/python_115-0.0.6.4.tar.gz` & `tmp/python_115-0.0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.4.tar", max compression
+gzip compressed data, was "python_115-0.0.6.5.tar", max compression
```

## Comparing `python_115-0.0.6.4.tar` & `python_115-0.0.6.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.4/LICENSE
--rwxr-xr-x   0        0        0   275249 2024-04-25 02:00:17.850869 python_115-0.0.6.4/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.4/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.4/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.4/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.4/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.4/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.4/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.4/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.4/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.4/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.4/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.4/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.4/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6.4/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.4/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.4/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.4/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.4/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.4/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.4/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.4/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.4/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.4/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.4/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.4/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-25 02:00:46.390576 python_115-0.0.6.4/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.4/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.5/LICENSE
+-rwxr-xr-x   0        0        0   275665 2024-04-25 02:47:37.342012 python_115-0.0.6.5/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.5/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.5/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.5/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-21 18:19:00.204183 python_115-0.0.6.5/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1445 2024-04-20 20:02:42.644715 python_115-0.0.6.5/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.5/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.5/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.5/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.5/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.6.5/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.5/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.5/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.6.5/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.5/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.5/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.5/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.5/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.5/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.6.5/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.5/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.6.5/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.5/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.5/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.5/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-25 02:47:55.533442 python_115-0.0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.5/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.5/PKG-INFO
```

### Comparing `python_115-0.0.6.4/LICENSE` & `python_115-0.0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/__init__.py` & `python_115-0.0.6.5/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4176,21 +4176,23 @@
     def download(
         self, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         no_root: bool = False, 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
+        **get_url_kwargs, 
     ):
         return self.fs.download_tree(
             self, 
             local_dir, 
             pid=pid, 
             no_root=no_root, 
             write_mode=write_mode, 
+            **get_url_kwargs, 
         )
 
     def exists(self, /) -> bool:
         return self.fs.exists(self)
 
     @property
     def file_extension(self, /) -> Optional[str]:
@@ -4655,32 +4657,37 @@
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
         submit = None, 
+        **get_url_kwargs, 
     ) -> Optional[DownloadTask]:
         if not hasattr(local_path_or_file, "write"):
             if not local_path_or_file:
                 local_path_or_file = self.attr(id_or_path, pid)["name"]
             if ospath.lexists(local_path_or_file): # type: ignore
                 if write_mode == "x":
                     raise FileExistsError(
                         errno.EEXIST, 
                         f"local path already exists: {local_path_or_file!r}", 
                     )
                 elif write_mode == "i":
                     return None
-        kwargs = {"resume": write_mode == "a", "headers": self.client.session.headers}
+        kwargs = {"resume": write_mode == "a"}
         if submit is not None:
             kwargs["submit"] = submit
         task = DownloadTask.create_task(
-            lambda: self.get_url(id_or_path, pid), 
+            lambda: self.get_url(id_or_path, pid, **get_url_kwargs), 
             local_path_or_file, 
+            headers=lambda: {
+                **self.client.session.headers, 
+                "Cookie": "; ".join(f"{c.name}={c.value}" for c in self.client.session.cookies), 
+            }, 
             **kwargs, 
         )
         if submit is None:
             task.run_wait()
         else:
             task.run()
         return task
@@ -4692,14 +4699,15 @@
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["i", "x", "w", "a"] = "a", 
         submit = None, 
         no_root: bool = False, 
         predicate: Optional[Callable[[P115PathType], bool]] = None, 
         onerror: None | bool | Callable[[BaseException], Any] = None, 
+        **get_url_kwargs, 
     ) -> Iterator[DownloadTask]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
         pathes: Iterable[P115PathType]
         if attr["is_directory"]:
@@ -4718,22 +4726,24 @@
                     subpath["id"], 
                     ospath.join(local_dir, subpath["name"]), 
                     write_mode=write_mode, 
                     submit=submit, 
                     no_root=True, 
                     predicate=predicate, 
                     onerror=onerror, 
+                    **get_url_kwargs, 
                 )
             else:
                 try:
                     task = self.download(
                         subpath["id"], 
                         ospath.join(local_dir, subpath["name"]), 
                         write_mode=write_mode, 
                         submit=submit, 
+                        **get_url_kwargs, 
                     )
                 except KeyboardInterrupt:
                     raise
                 except BaseException as exc:
                     if onerror is None or onerror is True:
                         raise
                     elif callable(onerror):
@@ -6357,21 +6367,22 @@
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
+        use_web_api: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.download_url(
             attr["pickcode"], 
-            use_web_api=attr["size"] < 1024 * 1024 * 115, 
+            use_web_api=use_web_api and attr["size"] < 1024 * 1024 * 115, 
             detail=detail, 
             headers=headers, 
         )
 
     def get_url_from_pickcode(
         self, 
         /,
```

### Comparing `python_115-0.0.6.4/p115/cmd/iterdir.py` & `python_115-0.0.6.5/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/cmd/qrcode.py` & `python_115-0.0.6.5/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/_init_mimetypes.py` & `python_115-0.0.6.5/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/cipher.py` & `python_115-0.0.6.5/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/concurrent.py` & `python_115-0.0.6.5/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/download.py` & `python_115-0.0.6.5/p115/util/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,22 +182,24 @@
 
 
 def download_iter(
     url: str | Callable[[], str], 
     file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
     resume: bool = False, 
     chunksize: int = COPY_BUFSIZE, 
-    headers: Optional[dict[str, str]] = None, 
+    headers: None | dict[str, str] | Callable[[], dict[str, str]] = None, 
     urlopen: Callable = urlopen, 
 ) -> Iterator[DownloadProgress]:
     """
     """
     if not isinstance(url, str):
         url = url()
 
+    if callable(headers):
+        headers = headers()
     if headers:
         headers = {**headers, "Accept-Encoding": "identity"}
     else:
         headers = {"Accept-Encoding": "identity"}
 
     if chunksize <= 0:
         chunksize = COPY_BUFSIZE
@@ -267,15 +269,15 @@
 
 
 def download(
     url: str | Callable[[], str], 
     file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
     resume: bool = False, 
     chunksize: int = COPY_BUFSIZE, 
-    headers: Optional[dict[str, str]] = None, 
+    headers: None | dict[str, str] | Callable[[], dict[str, str]] = None, 
     urlopen: Callable = urlopen, 
     make_reporthook: Optional[Callable[[Optional[int]], Callable[[int], Any] | Generator[int, Any, Any]]] = None, 
 ):
     """
     """
     gen = download_iter(url, file, resume=resume, chunksize=chunksize, headers=headers, urlopen=urlopen)
     if make_reporthook:
```

### Comparing `python_115-0.0.6.4/p115/util/file.py` & `python_115-0.0.6.5/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/hash.py` & `python_115-0.0.6.5/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/ignore.py` & `python_115-0.0.6.5/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/iter.py` & `python_115-0.0.6.5/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/path.py` & `python_115-0.0.6.5/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/property.py` & `python_115-0.0.6.5/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/response.py` & `python_115-0.0.6.5/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/retry.py` & `python_115-0.0.6.5/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/text.py` & `python_115-0.0.6.5/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/p115/util/urlopen.py` & `python_115-0.0.6.5/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/pyproject.toml` & `python_115-0.0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.4"
+version = "0.0.6.5"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.4/readme.md` & `python_115-0.0.6.5/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.4/PKG-INFO` & `python_115-0.0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.4
+Version: 0.0.6.5
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

