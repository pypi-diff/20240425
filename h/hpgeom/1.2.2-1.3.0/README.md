# Comparing `tmp/hpgeom-1.2.2.tar.gz` & `tmp/hpgeom-1.3.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpgeom-1.2.2.tar", last modified: Fri Jan 26 05:21:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

