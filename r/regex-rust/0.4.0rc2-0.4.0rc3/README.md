# Comparing `tmp/regex_rust-0.4.0rc2.tar.gz` & `tmp/regex_rust-0.4.0rc3.tar.gz`

## Comparing `regex_rust-0.4.0rc2.tar` & `regex_rust-0.4.0rc3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 regex_rust-0.4.0rc2/Cargo.toml
--rw-r--r--   0     1001      127    15355 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/.github/workflows/build.yaml
--rw-r--r--   0     1001      127        8 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/.gitignore
--rw-r--r--   0     1001      127      640 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1078 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/LICENSE
--rw-r--r--   0     1001      127     3388 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/README.md
--rw-r--r--   0     1001      127     2365 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/benchmark.py
--rw-r--r--   0     1001      127    12459 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/src/lib.rs
--rw-r--r--   0     1001      127        7 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/tests/requirements.txt
--rw-r--r--   0     1001      127     1411 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/tests/test_regexrs.py
--rw-r--r--   0     1001      127      155 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/tox.ini
--rw-r--r--   0     1001      127     9673 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/Cargo.lock
--rw-r--r--   0     1001      127      924 2024-04-25 05:55:28.000000 regex_rust-0.4.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 regex_rust-0.4.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 regex_rust-0.4.0rc3/Cargo.toml
+-rw-r--r--   0     1001      127    15355 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/.github/workflows/build.yaml
+-rw-r--r--   0     1001      127        8 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/.gitignore
+-rw-r--r--   0     1001      127      640 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1078 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/LICENSE
+-rw-r--r--   0     1001      127     3388 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/README.md
+-rw-r--r--   0     1001      127     2365 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/benchmark.py
+-rw-r--r--   0     1001      127    14196 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/src/lib.rs
+-rw-r--r--   0     1001      127        7 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/tests/requirements.txt
+-rw-r--r--   0     1001      127     1411 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/tests/test_regexrs.py
+-rw-r--r--   0     1001      127      155 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/tox.ini
+-rw-r--r--   0     1001      127     9443 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/Cargo.lock
+-rw-r--r--   0     1001      127      924 2024-04-25 18:59:19.000000 regex_rust-0.4.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 regex_rust-0.4.0rc3/PKG-INFO
```

### Comparing `regex_rust-0.4.0rc2/.github/workflows/build.yaml` & `regex_rust-0.4.0rc3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/.pre-commit-config.yaml` & `regex_rust-0.4.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/LICENSE` & `regex_rust-0.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/README.md` & `regex_rust-0.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/benchmark.py` & `regex_rust-0.4.0rc3/benchmark.py`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/src/lib.rs` & `regex_rust-0.4.0rc3/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use pyo3::prelude::*;
 use pyo3::types::{PyNone, PyTuple};
 use regex;
-use unicode_segmentation::UnicodeSegmentation;
 
 #[pyclass(module = "regexrs")]
 struct Match {
     #[pyo3(get)]
     string: String,
     #[pyo3(get)]
     re: Pattern,
@@ -81,49 +80,85 @@
         Ok(format!("<regexrs.Match object; span=({}, {}), match={:?}>", self.pos, self.endpos, self.string))
     }
 }
 
 #[pyclass(module = "regexrs")]
 #[derive(Clone)]
 struct Pattern {
-    // #[pyo3(get)]
-    // flags: i32,
     regex: regex::Regex,
 }
 
 impl Pattern {
     fn new(pattern: &str) -> Self {
         Pattern {
             regex: regex::Regex::new(pattern).unwrap(),
         }
     }
 }
 
+fn get_byte_to_code_point_and_reverse(haystack: &str) -> (Vec<usize>, Vec<usize>) {
+    // Map UTF-8 byte index to Unicode code point index; the latter is what
+    // Python users expect.
+    let mut byte_to_code_point = vec![usize::MAX; haystack.len() + 1];
+    let mut code_point_to_byte = vec![usize::MAX; haystack.len() + 1];
+    let mut max_codepoint = 0;
+    for (codepoint_off, (byte_off, _)) in haystack.char_indices().enumerate() {
+        byte_to_code_point[byte_off] = codepoint_off;
+        code_point_to_byte[codepoint_off] = byte_off;
+        max_codepoint = codepoint_off;
+    }
+    // End index is exclusive (e.g. 0:3 is first 3 characters), so handle
+    // the case where pattern is at end of string.
+    if !haystack.is_empty() {
+        byte_to_code_point[haystack.len()] = max_codepoint + 1;
+    }
+    (byte_to_code_point, code_point_to_byte)
+}
+
+fn get_byte_to_code_point(haystack: &str) -> Vec<usize> {
+    // Map UTF-8 byte index to Unicode code point index; the latter is what
+    // Python users expect.
+    let mut byte_to_code_point = vec![usize::MAX; haystack.len() + 1];
+    let mut max_codepoint = 0;
+    for (codepoint_off, (byte_off, _)) in haystack.char_indices().enumerate() {
+        byte_to_code_point[byte_off] = codepoint_off;
+        max_codepoint = codepoint_off;
+    }
+    // End index is exclusive (e.g. 0:3 is first 3 characters), so handle
+    // the case where pattern is at end of string.
+    if !haystack.is_empty() {
+        byte_to_code_point[haystack.len()] = max_codepoint + 1;
+    }
+    byte_to_code_point
+}
+
 #[pymethods]
 impl Pattern {
 
     pub fn r#match(&self, string: String, pos: Option<usize>) -> PyResult<Option<Match>> {
-        let p = pos.unwrap_or(0);
+        let (byte_to_code_point, code_point_to_byte) = get_byte_to_code_point_and_reverse(string.as_str());
+        let p = code_point_to_byte[pos.unwrap_or(0)];
         if let Some(caps) = self.regex.captures_at(&string, p) {
             if let Some(matched) = caps.get(0) {
                 if matched.start() == p {
                     // Extract the name of the last matched group
                     let last_group_name = self.regex.capture_names()
                         .filter_map(|name| name) // Skip None values for unnamed groups
                         .filter_map(|name| {
                             // Only consider the group if it has a match
                             caps.name(name).map(|_| name.to_string())
                         })
                         .last(); // Get the last group that had a match
 
+
                     return Ok(Some(Match {
                         string: String::from(matched.as_str()),
                         re: self.clone(),
-                        pos: matched.start(),
-                        endpos: matched.start() + matched.as_str().graphemes(true).count(),
+                        pos: byte_to_code_point[matched.start()],
+                        endpos: byte_to_code_point[matched.end()],
                         lastgroup: last_group_name,
                     }));
                 }
             }
         }
         Ok(None) // No match found or the match does not start at 'p'
     }
@@ -274,20 +309,21 @@
         if let Some(matched) = caps.get(0) {
             // Check that the match starts exactly at the position `p`
             if matched.start() == 0 {
                 let last_group_name = re.capture_names()
                     .filter_map(|name| name)
                     .filter_map(|name| caps.name(name).map(|_| name.to_string()))
                     .last();
+                let byte_to_code_point = get_byte_to_code_point(&string);
 
                 return Ok(Some(Match {
                     string: String::from(matched.as_str()),
                     re: Pattern { regex: re },
-                    pos: matched.start(),
-                    endpos: matched.start() + matched.as_str().graphemes(true).count(),
+                    pos: byte_to_code_point[matched.start()],
+                    endpos: byte_to_code_point[matched.end()],
                     lastgroup: last_group_name,
                 }));
             }
         }
     }
     Ok(None) // No valid match found or the match does not start at 'p'
 }
@@ -333,20 +369,21 @@
     if let Some(caps) = re.captures(&string) {
         if let Some(matched) = caps.get(0) {
             if matched.start() == 0 && matched.end() == string.len() {
                 let last_group_name = re.capture_names()
                     .filter_map(|name| name)
                     .filter_map(|name| caps.name(name).map(|_| name.to_string()))
                     .last();
+                let byte_to_code_point = get_byte_to_code_point(&string);
 
                 return Ok(Some(Match {
                     string: String::from(matched.as_str()),
                     re: Pattern { regex: re },
-                    pos: matched.start(),
-                    endpos: matched.start() + matched.as_str().graphemes(true).count(),
+                    pos: byte_to_code_point[matched.start()],
+                    endpos: byte_to_code_point[matched.end()],
                     lastgroup: last_group_name,
                 }));
             }
         }
     }
     Ok(None)
 }
```

### Comparing `regex_rust-0.4.0rc2/tests/test_regexrs.py` & `regex_rust-0.4.0rc3/tests/test_regexrs.py`

 * *Files identical despite different names*

### Comparing `regex_rust-0.4.0rc2/Cargo.lock` & `regex_rust-0.4.0rc3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -244,15 +244,14 @@
 
 [[package]]
 name = "regexrs"
 version = "0.4.0"
 dependencies = [
  "pyo3",
  "regex",
- "unicode-segmentation",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -283,20 +282,14 @@
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
-name = "unicode-segmentation"
-version = "1.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
-
-[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
```

### Comparing `regex_rust-0.4.0rc2/pyproject.toml` & `regex_rust-0.4.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0", "setuptools"]
 build-backend = 'maturin'
 
 [project]
 name = "regex-rust"
 license = "MIT"
-version = "0.4.0rc2"
+version = "0.4.0rc3"
 authors = [
     {name = "Spencer Phillip Young", email="spencer.young@spyoung.com"}
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
```

### Comparing `regex_rust-0.4.0rc2/PKG-INFO` & `regex_rust-0.4.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: regex-rust
-Version: 0.4.0rc2
+Version: 0.4.0rc3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

