# Comparing `tmp/vtzero-0.0.1b3.tar.gz` & `tmp/vtzero-0.0.1b4-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtzero-0.0.1b3.tar", last modified: Tue Oct 25 11:19:51 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

