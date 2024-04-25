# Comparing `tmp/tree_sitter_earthfile-0.2.4-cp38-abi3-win_amd64.whl.zip` & `tmp/tree_sitter_earthfile-0.3.0-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 104905 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/__init__.py
--rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/__init__.pyi
--rw-rw-rw-  2.0 fat   523776 b- defN 24-Apr-16 20:15 tree_sitter_earthfile/_binding.pyd
--rw-rw-rw-  2.0 fat      642 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/binding.c
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/py.typed
--rw-rw-rw-  2.0 fat     1397 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/queries/highlights.scm
--rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-16 20:13 tree_sitter_earthfile/queries/injections.scm
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-16 20:15 tree_sitter_earthfile-0.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      987 b- defN 24-Apr-16 20:15 tree_sitter_earthfile-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-16 20:15 tree_sitter_earthfile-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       31 b- defN 24-Apr-16 20:15 tree_sitter_earthfile-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1098 b- defN 24-Apr-16 20:15 tree_sitter_earthfile-0.2.4.dist-info/RECORD
-12 files, 529493 bytes uncompressed, 103013 bytes compressed:  80.5%
+Zip file size: 99323 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/__init__.py
+-rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/__init__.pyi
+-rw-rw-rw-  2.0 fat   477696 b- defN 24-Apr-25 20:09 tree_sitter_earthfile/_binding.pyd
+-rw-rw-rw-  2.0 fat      642 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/binding.c
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/py.typed
+-rw-rw-rw-  2.0 fat     1442 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/queries/highlights.scm
+-rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-25 20:07 tree_sitter_earthfile/queries/injections.scm
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-25 20:09 tree_sitter_earthfile-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      987 b- defN 24-Apr-25 20:09 tree_sitter_earthfile-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-25 20:09 tree_sitter_earthfile-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       31 b- defN 24-Apr-25 20:09 tree_sitter_earthfile-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1098 b- defN 24-Apr-25 20:09 tree_sitter_earthfile-0.3.0.dist-info/RECORD
+12 files, 483458 bytes uncompressed, 97431 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tree_sitter_earthfile/queries/highlights.scm
 Comment: 
 
 Filename: tree_sitter_earthfile/queries/injections.scm
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.4.dist-info/LICENSE
+Filename: tree_sitter_earthfile-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.4.dist-info/METADATA
+Filename: tree_sitter_earthfile-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.4.dist-info/WHEEL
+Filename: tree_sitter_earthfile-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.4.dist-info/top_level.txt
+Filename: tree_sitter_earthfile-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.4.dist-info/RECORD
+Filename: tree_sitter_earthfile-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_earthfile/queries/highlights.scm

```diff
@@ -63,12 +63,13 @@
     (double_quoted_string)
     (single_quoted_string)
 ] @string
 (unquoted_string) @string.special
 (escape_sequence) @constant.character.escape
 
 (variable) @variable
+(secret (identifier) @variable.other.member)
 (expansion ["$" "{" "}" "(" ")"] @punctuation.special)
 (build_arg) @variable
 (options (_) @variable.parameter)
 
 "=" @operator
```

## Comparing `tree_sitter_earthfile-0.2.4.dist-info/LICENSE` & `tree_sitter_earthfile-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tree_sitter_earthfile-0.2.4.dist-info/METADATA` & `tree_sitter_earthfile-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-earthfile
-Version: 0.2.4
+Version: 0.3.0
 Summary: Earthfile grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-earthfile
 Keywords: incremental,parsing,tree-sitter,earthfile
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

## Comparing `tree_sitter_earthfile-0.2.4.dist-info/RECORD` & `tree_sitter_earthfile-0.3.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tree_sitter_earthfile/__init__.py,sha256=b49F9QXcBSzekYK6czZvmdtuGwDStmfTwwwbFGkS8H4,92
 tree_sitter_earthfile/__init__.pyi,sha256=8xf7bY1szgDY9HRJ7FJ326So4SFgMiSRfCB4LADkTpU,27
-tree_sitter_earthfile/_binding.pyd,sha256=D2DuMJo-HdpbdsjXnPJN-Q-RM7KuK8u-FnWcLJsMtp4,523776
+tree_sitter_earthfile/_binding.pyd,sha256=xx4-hhLRDsbJXaoprfoS74IoeeWjuTurMs2Xh0L2OWk,477696
 tree_sitter_earthfile/binding.c,sha256=MKxNXwWUTomdXfVWUkzuE2I7Giioe_EcSNnz2Iw-P9Q,642
 tree_sitter_earthfile/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tree_sitter_earthfile/queries/highlights.scm,sha256=sHHDVqyppK76MTfeSHoaeKUgkEVjJ84jXchDcRWVREE,1397
+tree_sitter_earthfile/queries/highlights.scm,sha256=qhm-jq9Zne_rPb86soKpbPCF_8JR4jAjYULppHDYIRk,1442
 tree_sitter_earthfile/queries/injections.scm,sha256=-GVsiRO-9Cz_5wl71HXOXI7zbMv49V8I1sxJXrizujE,271
-tree_sitter_earthfile-0.2.4.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
-tree_sitter_earthfile-0.2.4.dist-info/METADATA,sha256=sp8aH0q9foHxwVEepnq9Ptf2LIuj0nuwnTEKxqb_n_4,987
-tree_sitter_earthfile-0.2.4.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
-tree_sitter_earthfile-0.2.4.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
-tree_sitter_earthfile-0.2.4.dist-info/RECORD,,
+tree_sitter_earthfile-0.3.0.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
+tree_sitter_earthfile-0.3.0.dist-info/METADATA,sha256=R_9XK1WHV86L-iIGpYv_EgDCa-YcCBc6P3_oGqQav2A,987
+tree_sitter_earthfile-0.3.0.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
+tree_sitter_earthfile-0.3.0.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
+tree_sitter_earthfile-0.3.0.dist-info/RECORD,,
```

