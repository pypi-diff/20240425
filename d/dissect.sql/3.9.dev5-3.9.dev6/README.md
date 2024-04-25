# Comparing `tmp/dissect.sql-3.9.dev5.tar.gz` & `tmp/dissect_sql-3.9.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.sql-3.9.dev5.tar", last modified: Thu Apr 11 11:57:23 2024, max compression
+gzip compressed data, was "dissect_sql-3.9.dev6.tar", last modified: Thu Apr 25 14:24:20 2024, max compression
```

## Comparing `dissect.sql-3.9.dev5.tar` & `dissect_sql-3.9.dev6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.043534 dissect.sql-3.9.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-11 11:57:23.043534 dissect.sql-3.9.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.035534 dissect.sql-3.9.dev5/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.039534 dissect.sql-3.9.dev5/dissect/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/dissect/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/dissect/sql/c_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/dissect/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/dissect/sql/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/dissect/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.043534 dissect.sql-3.9.dev5/dissect.sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-11 11:57:23.000000 dissect.sql-3.9.dev5/dissect.sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-11 11:57:23.000000 dissect.sql-3.9.dev5/dissect.sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:57:23.000000 dissect.sql-3.9.dev5/dissect.sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:57:23.000000 dissect.sql-3.9.dev5/dissect.sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:57:23.000000 dissect.sql-3.9.dev5/dissect.sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-11 11:57:17.000000 dissect.sql-3.9.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:57:23.043534 dissect.sql-3.9.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.039534 dissect.sql-3.9.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.039534 dissect.sql-3.9.dev5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/data/test.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:23.043534 dissect.sql-3.9.dev5/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:57:13.000000 dissect.sql-3.9.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.241118 dissect_sql-3.9.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 14:24:20.241118 dissect_sql-3.9.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.233117 dissect_sql-3.9.dev6/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.237118 dissect_sql-3.9.dev6/dissect/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/dissect/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/dissect/sql/c_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/dissect/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/dissect/sql/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/dissect/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.237118 dissect_sql-3.9.dev6/dissect.sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 14:24:20.000000 dissect_sql-3.9.dev6/dissect.sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 14:24:20.000000 dissect_sql-3.9.dev6/dissect.sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:24:20.000000 dissect_sql-3.9.dev6/dissect.sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:24:20.000000 dissect_sql-3.9.dev6/dissect.sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 14:24:20.000000 dissect_sql-3.9.dev6/dissect.sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-25 14:24:14.000000 dissect_sql-3.9.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:24:20.241118 dissect_sql-3.9.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.237118 dissect_sql-3.9.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.237118 dissect_sql-3.9.dev6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/data/empty.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/data/test.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:24:20.237118 dissect_sql-3.9.dev6/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-25 14:24:09.000000 dissect_sql-3.9.dev6/tox.ini
```

### Comparing `dissect.sql-3.9.dev5/LICENSE` & `dissect_sql-3.9.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/PKG-INFO` & `dissect_sql-3.9.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.9.dev5
+Version: 3.9.dev6
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.9.dev5/README.md` & `dissect_sql-3.9.dev6/README.md`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/dissect/sql/c_sqlite3.py` & `dissect_sql-3.9.dev6/dissect/sql/c_sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/dissect/sql/sqlite3.py` & `dissect_sql-3.9.dev6/dissect/sql/sqlite3.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.fh = fh
         self.wal = WAL(wal_fh) if wal_fh else None
 
         self.header = c_sqlite3.header(fh)
         if self.header.magic != SQLITE3_HEADER_MAGIC:
             raise InvalidDatabase("Invalid header magic")
 
-        self.encoding = ENCODING[self.header.text_encoding]
+        self.encoding = ENCODING.get(self.header.text_encoding, "utf-8")
         self.page_size = self.header.page_size
         if self.page_size == 1:
             self.page_size = 65536
 
         self.usable_page_size = self.page_size - self.header.reserved_size
         if self.usable_page_size < 480:
             raise InvalidDatabase("Usable page size is too small")
@@ -71,15 +71,17 @@
         for cell in walk_tree(self, self.page(1)):
             if cell.values[0] != "index":
                 continue
 
             yield Index(self, *cell.values)
 
     def raw_page(self, num):
-        if num < 1 or num > self.header.page_count:
+        # Only throw an out of bounds exception if the header contains a page_count.
+        # Some old versions of SQLite3 do not set/update the page_count correctly.
+        if (num < 1 or num > self.header.page_count) and self.header.page_count > 0:
             raise InvalidPageNumber("Page number exceeds boundaries")
         elif num == 1:  # Page 1 is root
             self.fh.seek(len(c_sqlite3.header))
         else:
             self.fh.seek((num - 1) * self.page_size)
         return self.fh.read(self.header.page_size)
 
@@ -96,16 +98,16 @@
                 yield cell
 
 
 class Column:
     """Describes a column of a sqlite table."""
 
     SPACE = r"\s"
-    EXPRESSION = r"\(.+\)"
-    STRING = r"['\"].+['\"]"
+    EXPRESSION = r"\(.+?\)"
+    STRING = r"['\"].+?['\"]"
     TOKENIZER_EXPRESSION = re.compile(f"({SPACE}|{EXPRESSION}|{STRING})")
 
     def __init__(self, name: str, description: str):
         self.name = name
         self.default_value = self._parse_default_value_from_description(description)
 
     def _parse_default_value_from_description(self, description: str):
```

### Comparing `dissect.sql-3.9.dev5/dissect/sql/utils.py` & `dissect_sql-3.9.dev6/dissect/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/dissect.sql.egg-info/PKG-INFO` & `dissect_sql-3.9.dev6/dissect.sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.9.dev5
+Version: 3.9.dev6
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.9.dev5/dissect.sql.egg-info/SOURCES.txt` & `dissect_sql-3.9.dev6/dissect.sql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 dissect/sql/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_default_values.py
 tests/test_row.py
 tests/test_sqlite.py
 tests/test_utils.py
+tests/data/empty.sqlite
 tests/data/test.sqlite
 tests/docs/Makefile
 tests/docs/conf.py
 tests/docs/index.rst
```

### Comparing `dissect.sql-3.9.dev5/pyproject.toml` & `dissect_sql-3.9.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tests/data/test.sqlite` & `dissect_sql-3.9.dev6/tests/data/test.sqlite`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tests/docs/Makefile` & `dissect_sql-3.9.dev6/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tests/docs/conf.py` & `dissect_sql-3.9.dev6/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tests/test_default_values.py` & `dissect_sql-3.9.dev6/tests/test_default_values.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,27 +40,31 @@
             id INTEGER PRIMARY KEY,
             hello_default TEXT DEFAULT "hello" NOT NULL,
             nullable_default TEXT,
             default_integer INTEGER DEFAULT 0,
             new_test DEFAULT (1),
             extra_test DEFAULT ("hello world"),
             all_tests DEFAULT (-1.1),
-            test DEFAULT (x == NULL)
+            test DEFAULT (x == NULL),
+            some_test INTEGER DEFAULT (0) NOT NULL,
+            another_test VARCHAR(1337) DEFAULT ("test") NOT NULL
         );
     """
     table = Table(sqlite=None, type_=None, name=None, table_name=None, page=None, sql=table_definition)
     assertion_data = [
         ("id", None),
         ("hello_default", "hello"),
         ("nullable_default", None),
         ("default_integer", 0),
         ("new_test", 1),
         ("extra_test", "hello world"),
         ("all_tests", -1.1),
         ("test", None),
+        ("some_test", 0),
+        ("another_test", "test"),
     ]
     for key, value in assertion_data:
         assert column_name_for_key(table.columns, key).default_value == value
 
 
 def column_name_for_key(columns, key):
     for column in columns:
```

### Comparing `dissect.sql-3.9.dev5/tests/test_row.py` & `dissect_sql-3.9.dev6/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tests/test_sqlite.py` & `dissect_sql-3.9.dev6/tests/test_sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,7 +47,14 @@
     [
         (b"\x04\x00\x1b\x02testing\x059", "utf-8", ([0, 27, 2], [None, "testing", 1337])),
         (b"\x02\x65\x80\x81\x82\x83", "utf-8", ([101], [b"\x80\x81\x82\x83"])),
     ],
 )
 def test_sqlite_read_record(input: bytes, encoding: str, expected_output: tuple[list[int], list[Any]]) -> None:
     assert sqlite3.read_record(BytesIO(input), encoding) == expected_output
+
+
+def test_empty(empty_db: BinaryIO) -> None:
+    s = sqlite3.SQLite3(empty_db)
+
+    assert s.encoding == "utf-8"
+    assert len(list(s.tables())) == 0
```

### Comparing `dissect.sql-3.9.dev5/tests/test_utils.py` & `dissect_sql-3.9.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev5/tox.ini` & `dissect_sql-3.9.dev6/tox.ini`

 * *Files identical despite different names*

