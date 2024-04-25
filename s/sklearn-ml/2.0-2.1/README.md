# Comparing `tmp/sklearn_ml-2.0.tar.gz` & `tmp/sklearn_ml-2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_ml-2.0.tar", last modified: Sun Oct 15 15:44:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

