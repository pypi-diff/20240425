# Comparing `tmp/math_ops_131-1.3.3.tar.gz` & `tmp/math_ops_131-1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_ops_131-1.3.3.tar", last modified: Thu Apr 25 11:49:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

