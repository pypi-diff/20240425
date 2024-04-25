# Comparing `tmp/traderusty-0.1.0.tar.gz` & `tmp/traderusty-0.1.1.tar.gz`

## Comparing `traderusty-0.1.0.tar` & `traderusty-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 traderusty-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3000 2024-04-25 01:56:57.000000 traderusty-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-25 01:56:57.000000 traderusty-0.1.0/.gitignore
--rw-r--r--   0     1001      127     2282 2024-04-25 01:56:57.000000 traderusty-0.1.0/Dockerfile
--rw-r--r--   0     1001      127      174 2024-04-25 01:56:57.000000 traderusty-0.1.0/README.md
--rw-r--r--   0     1001      127      109 2024-04-25 01:56:57.000000 traderusty-0.1.0/python/tests/test_all.py
--rw-r--r--   0     1001      127      125 2024-04-25 01:56:57.000000 traderusty-0.1.0/python/traderusty/__init__.py
--rw-r--r--   0     1001      127       64 2024-04-25 01:56:57.000000 traderusty-0.1.0/python/traderusty/traderusty.pyi
--rw-r--r--   0     1001      127      505 2024-04-25 01:56:57.000000 traderusty-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     2605 2024-04-25 01:56:57.000000 traderusty-0.1.0/src/rusty.rs
--rw-r--r--   0     1001      127    65336 2024-04-25 01:56:57.000000 traderusty-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      473 2024-04-25 01:56:57.000000 traderusty-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 traderusty-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 traderusty-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3000 2024-04-25 03:15:40.000000 traderusty-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-25 03:15:40.000000 traderusty-0.1.1/.gitignore
+-rw-r--r--   0     1001      127      152 2024-04-25 03:15:40.000000 traderusty-0.1.1/CHANGELOG.md
+-rw-r--r--   0     1001      127     2282 2024-04-25 03:15:40.000000 traderusty-0.1.1/Dockerfile
+-rw-r--r--   0     1001      127     1065 2024-04-25 03:15:40.000000 traderusty-0.1.1/LICENSE.txt
+-rw-r--r--   0     1001      127      174 2024-04-25 03:15:40.000000 traderusty-0.1.1/README.md
+-rw-r--r--   0     1001      127      109 2024-04-25 03:15:40.000000 traderusty-0.1.1/python/tests/test_all.py
+-rw-r--r--   0     1001      127      125 2024-04-25 03:15:40.000000 traderusty-0.1.1/python/traderusty/__init__.py
+-rw-r--r--   0     1001      127       64 2024-04-25 03:15:40.000000 traderusty-0.1.1/python/traderusty/traderusty.pyi
+-rw-r--r--   0     1001      127      505 2024-04-25 03:15:40.000000 traderusty-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     2659 2024-04-25 03:15:40.000000 traderusty-0.1.1/src/rusty.rs
+-rw-r--r--   0     1001      127    65336 2024-04-25 03:15:40.000000 traderusty-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1438 2024-04-25 03:15:40.000000 traderusty-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 traderusty-0.1.1/PKG-INFO
```

### Comparing `traderusty-0.1.0/.github/workflows/CI.yml` & `traderusty-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.0/.gitignore` & `traderusty-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.0/Dockerfile` & `traderusty-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.0/src/rusty.rs` & `traderusty-0.1.1/src/rusty.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 use std::fs::File;
 use std::io::{self, BufReader, Read};
 use bytecount::count as byte_counter;
 
+const READ_BUFFER_SIZE: usize = 128 * 1024;
+
 /// Counts the number of '\n's in a file as quickly as possible and then
 /// returns the count.
 #[allow(dead_code)]
 pub fn count_file_lines(filename: &str) -> io::Result<usize> {
     let file = File::open(filename)?;
     let mut reader = BufReader::new(file);
-    let mut buffer = vec![0; 65536];    // 64kb at a time
+    let mut buffer = vec![0; READ_BUFFER_SIZE]; // 256kb at a time
     let mut count = 0;
 
     loop {
         let bytes_read = reader.read(&mut buffer)?;
         if bytes_read == 0 {
             break;
         }
```

### Comparing `traderusty-0.1.0/Cargo.lock` & `traderusty-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2082,15 +2082,15 @@
  "tracing-core",
  "tracing-log",
  "tracing-serde",
 ]
 
 [[package]]
 name = "traderusty"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "bytecount",
  "maturin",
  "pyo3",
  "tempfile",
 ]
```

