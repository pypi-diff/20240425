# Comparing `tmp/anycrc-0.4.1.tar.gz` & `tmp/anycrc-0.4.2-pp38-pypy38_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.4.1.tar", last modified: Wed Apr 24 13:15:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

