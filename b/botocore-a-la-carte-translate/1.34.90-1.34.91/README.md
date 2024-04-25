# Comparing `tmp/botocore-a-la-carte-translate-1.34.90.tar.gz` & `tmp/botocore_a_la_carte_translate-1.34.91-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-translate-1.34.90.tar", last modified: Wed Apr 24 01:02:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

