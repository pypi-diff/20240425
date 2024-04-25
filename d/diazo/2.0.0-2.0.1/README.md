# Comparing `tmp/diazo-2.0.0.tar.gz` & `tmp/diazo-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diazo-2.0.0.tar", last modified: Mon Feb 12 15:16:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

