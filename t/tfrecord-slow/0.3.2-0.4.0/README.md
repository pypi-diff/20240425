# Comparing `tmp/tfrecord_slow-0.3.2.tar.gz` & `tmp/tfrecord_slow-0.4.0.tar.gz`

## Comparing `tfrecord_slow-0.3.2.tar` & `tfrecord_slow-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/requirements-dev.lock
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/requirements.lock
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/examples/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/examples/bench_reader.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/examples/bench_writer.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/examples/common.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/__main__.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/msgpack.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/reader.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/utils/__init__.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/utils/loader.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/src/tfrecord_slow/utils/masked_crc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/tests/test_ndarray.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/tests/test_pickle.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tfrecord_slow-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/requirements.lock
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/bench_reader.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/bench_writer.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/common.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/__init__.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/__main__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/msgpack.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/reader.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/__init__.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/loader.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/masked_crc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/test_ndarray.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/test_pickle.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.gitignore
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/PKG-INFO
```

### Comparing `tfrecord_slow-0.3.2/requirements-dev.lock` & `tfrecord_slow-0.4.0/requirements-dev.lock`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # generated by rye
 # use `rye lock` or `rye sync` to update this lockfile
 #
 # last locked with the following flags:
 #   pre: false
-#   features: ["msgpack"]
-#   all-features: false
+#   features: []
+#   all-features: true
 #   with-sources: false
 
 -e file:.
 asttokens==2.4.1
     # via stack-data
 crc32c==2.3.post0
     # via tfrecord-slow
@@ -17,16 +17,20 @@
 executing==2.0.1
     # via stack-data
 iniconfig==2.0.0
     # via pytest
 ipython==8.22.1
 jedi==0.19.1
     # via ipython
+loguru==0.7.2
+    # via tfrecord-slow
 matplotlib-inline==0.1.6
     # via ipython
+msgspec==0.18.6
+    # via tfrecord-slow
 numpy==1.26.4
     # via tfrecord-slow
 packaging==23.2
     # via pytest
 parso==0.8.3
     # via jedi
 pexpect==4.9.0
@@ -43,12 +47,14 @@
     # via ipython
 pytest==8.0.1
 safetensors==0.4.2
 six==1.16.0
     # via asttokens
 stack-data==0.6.3
     # via ipython
+tqdm==4.66.2
+    # via tfrecord-slow
 traitlets==5.14.1
     # via ipython
     # via matplotlib-inline
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `tfrecord_slow-0.3.2/.github/workflows/python-package.yml` & `tfrecord_slow-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.3.2/.github/workflows/python-publish.yml` & `tfrecord_slow-0.4.0/.github/workflows/python-publish.yml`

 * *Files 22% similar despite different names*

```diff
@@ -20,15 +20,13 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Setup rye
         id: setup-rye
-        uses: eifinger/setup-rye@v1
-        with:
-          enable-cache: true
+        uses: eifinger/setup-rye@v2
 
       - name: Publish package
         run: |
           rye build --clean
           rye publish --token ${{ secrets.PYPI_API_TOKEN }} --yes
```

### Comparing `tfrecord_slow-0.3.2/src/tfrecord_slow/__main__.py` & `tfrecord_slow-0.4.0/src/tfrecord_slow/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 """
 
 import argparse
 import logging
 from pathlib import Path
 from typing import Optional
 from .reader import TfRecordReader
-
-logger = logging.getLogger(__name__)
+from loguru import logger
+from tqdm import tqdm
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers()
-
-    count_parser = subparsers.add_parser("count")
-    count_parser.set_defaults(func=count)
-    count_parser.add_argument(
-        "path", type=Path, help="Path to tfrecord file or directory."
-    )
-    count_parser.add_argument("-m", "--mask", action="store_const", const="*.tfrec")
-    count_parser.add_argument(
-        "-c", "--check", action="store_true", help="Check integrity."
-    )
+    add_count_args(subparsers.add_parser("count"))
 
     return parser.parse_args()
 
 
+def add_count_args(parser: argparse.ArgumentParser):
+    parser.set_defaults(func=count)
+    parser.add_argument("path", type=Path, help="Path to tfrecord file or directory.")
+    parser.add_argument("-m", "--mask", action="store_const", const="*.tfrec")
+    parser.add_argument("-c", "--check", action="store_true", help="Check integrity.")
+
+
 def count(args):
     path: Path = args.path
     mask: Optional[str] = args.mask
     check_integrity: bool = args.check
 
     if mask is not None:
         paths = list(path.glob(mask))
```

### Comparing `tfrecord_slow-0.3.2/src/tfrecord_slow/reader.py` & `tfrecord_slow-0.4.0/src/tfrecord_slow/reader.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.3.2/src/tfrecord_slow/writer.py` & `tfrecord_slow-0.4.0/src/tfrecord_slow/writer.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.3.2/src/tfrecord_slow/utils/loader.py` & `tfrecord_slow-0.4.0/src/tfrecord_slow/utils/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,23 +33,25 @@
 
 
 class MsgpackTfrecordLoader:
     def __init__(
         self,
         datapipe: Iterable[BufferedIOBase],
         spec: Type[S],
-        func: Callable[[S], T],
         check_integrity: bool = False,
     ):
+        """
+        Args:
+            datapipe: iter of files
+            spec: msgspec.Struct, must have owned memory
+        """
         self.datapipe = datapipe
         self.check_integrity = check_integrity
-        self.func = func
         self.spec = spec
 
-    def __iter__(self) -> Iterator[T]:
+    def __iter__(self) -> Iterator[S]:
         decoder = msgspec.msgpack.Decoder(type=self.spec)
         for fp in self.datapipe:
             reader = TfRecordReader(fp, check_integrity=self.check_integrity)
             for buf in reader:
-                record = decoder.decode(buf)
-                example = self.func(record)
+                example = decoder.decode(buf)
                 yield example
```

### Comparing `tfrecord_slow-0.3.2/.gitignore` & `tfrecord_slow-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.3.2/pyproject.toml` & `tfrecord_slow-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tfrecord-slow"
-version = "0.3.2"
+version = "0.4.0"
 description = "Default template for PDM package"
 authors = [
     { name = "SunDoge", email = "triplez0@outlook.com" }
 ]
 dependencies = [
     "crc32c>=2.3.post0",
     "numpy>=1",
@@ -15,14 +15,18 @@
 [project.scripts]
 hello = "tfrecord_slow:hello"
 
 [project.optional-dependencies]
 msgpack = [
     "msgspec>=0.18.6",
 ]
+cli = [
+    "loguru>=0.7.2",
+    "tqdm>=4.66.2",
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

