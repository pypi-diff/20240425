# Comparing `tmp/file_iter-0.1.2.tar.gz` & `tmp/file_iter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_iter-0.1.2.tar", max compression
+gzip compressed data, was "file_iter-0.1.3.tar", max compression
```

## Comparing `file_iter-0.1.2.tar` & `file_iter-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.2/LICENSE
--rw-r--r--   0        0        0     1894 2024-04-12 14:11:20.845268 file_iter-0.1.2/README.md
--rw-r--r--   0        0        0      146 2024-04-19 13:24:01.364289 file_iter-0.1.2/file_iter/__init__.py
--rw-r--r--   0        0        0    10041 2024-04-19 13:24:01.364289 file_iter-0.1.2/file_iter/file_iter.py
--rw-r--r--   0        0        0      986 2024-04-19 13:24:01.364289 file_iter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 file_iter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1894 2024-04-12 14:11:20.845268 file_iter-0.1.3/README.md
+-rw-r--r--   0        0        0      146 2024-04-19 13:24:01.364289 file_iter-0.1.3/file_iter/__init__.py
+-rw-r--r--   0        0        0    11787 2024-04-24 14:47:11.459622 file_iter-0.1.3/file_iter/file_iter.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:52:42.788121 file_iter-0.1.3/file_iter/py.typed
+-rw-r--r--   0        0        0      986 2024-04-24 14:36:36.505864 file_iter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 file_iter-0.1.3/PKG-INFO
```

### Comparing `file_iter-0.1.2/LICENSE` & `file_iter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `file_iter-0.1.2/README.md` & `file_iter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `file_iter-0.1.2/file_iter/file_iter.py` & `file_iter-0.1.3/file_iter/file_iter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """A Swiss Army knife iterator for files (or any iterator of strings)."""
 
+import gzip
 import itertools
 from collections import deque
+from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Callable, Iterable, Iterator, Literal, overload
+from tempfile import NamedTemporaryFile
+from typing import IO, Any, Callable, Iterable, Iterator, Literal, overload
 
 _marker: Any = object()
 
 
 class FileIter(Iterator[str]):
     """
     A Swiss Army knife iterator for files (or any iterator of strings).
@@ -18,14 +21,15 @@
         - Specify position if entering in the middle of a file: `FileIter(f, position=10)`
     - Peek at the next line: `peek()`
     - Jump ahead `n` lines `jump(n)`
     - Check if empty: `isempty()`
     - Filter out unimportant lines:
         - Always filter: `FileIter(f, filter_func=is_data)`
         - Filter only single next(): `filter_next(filter_func)`
+    - Supports gzip
 
     >>> def is_data(line:  str) -> bool:
     ...    return len(line) > 0 and (line[0] != "#")
     >>> file_iter = FileIter(
     ...     ["Hello", "", "# comment", "World", "How", "are", "you?"],
     ...     filter_func=is_data
     ... )
@@ -274,51 +278,68 @@
 class FileIterContextManager:
     r"""
     Manage opening and closing a file for iteration.
 
     See FileIter for more information
     Note: contextlib.contextmanager is not used to avoid mypy issues
 
-    >>> from tempfile import NamedTemporaryFile
-    >>> with NamedTemporaryFile("w") as f:
-    ...     _ = f.write("Hello\n# comment\n\nWorld")
-    ...     _ = f.seek(0)
-    ...
+    Test regular files
+    >>> with tmp_file("Hello\n# comment\n\nWorld") as f:
     ...     with FileIterContextManager(f.name, filter_func=is_data) as file_iter:
     ...         for line in file_iter:
     ...             print(line, file_iter.position)
     Hello 0
     World 3
-    >>> with NamedTemporaryFile("w") as f:  # doctest: +ELLIPSIS
-    ...     name = f.name
-    ...     _ = f.write("Hello\n# comment\n\nWorld")
-    ...     _ = f.seek(0)
-    ...
+
+    Test gzipped files (tmp_file automatically recognizes gzipped files)
+    >>> with tmp_file("Hello\n# comment\n\nWorld", gzipped=True) as f:
+    ...     with FileIterContextManager(f.name, filter_func=is_data) as file_iter:
+    ...         for line in file_iter:
+    ...             print(line, file_iter.position)
+    Hello 0
+    World 3
+
+    Test jumping
+    >>> with tmp_file("Hello\n# comment\n\nWorld") as f:  # doctest: +ELLIPSIS
     ...     with FileIterContextManager(f.name, filter_func=is_data) as file_iter:
-    ...         _ = next(file_iter), next(file_iter)
+    ...         _ = file_iter.jump(2)
     ...         file_iter.jump(-1)
     Traceback (most recent call last):
     ...
     IndexError: Can only jump forward
     Error reading ... at line=3
     """
 
     def __init__(
         self,
         filename: str | Path,
         position: int = -1,
         filter_func: Callable[[str], bool] | None = None,
+        gzipped: bool | Literal["auto"] = "auto",
     ) -> None:
+        """
+        Initialize the FileIterContextManager object.
+
+        :param filename: the name of the file to open
+        :param position: the current position in the file
+        :param filter_func: a function that checks if the line is useful
+        :param gzipped: whether the file is gzipped
+        """
         self.filename = Path(filename)
         self.start_position = position
         self.filter_func = filter_func
+        self.gzipped = gzipped
 
     def __enter__(self) -> FileIter:
         """Open the file and return a FileIter object."""
-        self.file = open(self.filename)
+        filename, gzipped = self.filename, self.gzipped
+        if gzipped == "auto":
+            gzipped = filename.suffix == ".gz"
+
+        self.file = gzip.open(filename, "rt") if gzipped else open(filename)
         self.file_iter = FileIter(self.file, self.start_position, self.filter_func)
         return self.file_iter
 
     def __exit__(
         self, exc_type: type | None, exc_value: Exception | None, traceback: Any | None
     ) -> Literal[False]:
         """Close the file and indicate the position if there is an exception."""
@@ -336,7 +357,36 @@
     True
     >>> is_data("# comment")
     False
     >>> is_data("")
     False
     """
     return len(line) > 0 and (line[0] != "#")
+
+
+@contextmanager  # type: ignore
+def tmp_file(data_str: str, gzipped=False, **kwargs: Any) -> Iterable[IO[str]]:
+    r"""
+    Create a NamedTemporaryFile file with contents `data_str`.
+
+    :param data_str: the string to write to the file
+    :param gzipped: whether to write a gzipped file
+    :param kwargs: additional keyword arguments to pass to NamedTemporaryFile
+    :return: a readable/writable file object
+
+    >>> with tmp_file("Hello\nWorld") as f:
+    ...     for line in f:
+    ...         print(line.strip())
+    Hello
+    World
+    """
+    if gzipped:
+        with NamedTemporaryFile("w+", delete=True, suffix=".gz", **kwargs) as f:
+            with gzip.open(f.name, "wt") as fgz:
+                _ = fgz.write(data_str)
+            yield f
+
+    else:
+        with NamedTemporaryFile("w+", delete=True, **kwargs) as f:
+            _ = f.write(data_str)
+            _ = f.seek(0)
+            yield f
```

### Comparing `file_iter-0.1.2/pyproject.toml` & `file_iter-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file_iter"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Swiss Army knife iterator for files (or any iterator of strings)"
 authors = ["Jonathon Vandezande"]
 keywords = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jevandezande/file_iter"
```

### Comparing `file_iter-0.1.2/PKG-INFO` & `file_iter-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_iter
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Swiss Army knife iterator for files (or any iterator of strings)
 Home-page: https://github.com/jevandezande/file_iter
 License: MIT
 Author: Jonathon Vandezande
 Requires-Python: >=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

