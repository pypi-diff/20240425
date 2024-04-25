# Comparing `tmp/satkit-0.2.6.tar.gz` & `tmp/satkit-0.2.7-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satkit-0.2.6.tar", last modified: Mon Apr  8 15:30:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

