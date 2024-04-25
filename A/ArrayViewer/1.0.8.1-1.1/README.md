# Comparing `tmp/ArrayViewer-1.0.8.1.tar.gz` & `tmp/ArrayViewer-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArrayViewer-1.0.8.1.tar", last modified: Wed Oct  4 20:01:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

