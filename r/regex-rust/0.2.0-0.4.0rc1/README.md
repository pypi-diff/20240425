# Comparing `tmp/regex_rust-0.2.0.tar.gz` & `tmp/regex_rust-0.4.0rc1-cp310-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

