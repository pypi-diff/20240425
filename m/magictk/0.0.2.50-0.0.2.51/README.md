# Comparing `tmp/magictk-0.0.2.50.tar.gz` & `tmp/magictk-0.0.2.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.50.tar", last modified: Wed Apr 24 14:19:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

