# Comparing `tmp/dhuodata-lib-0.0.8.tar.gz` & `tmp/dhuodata-lib-0.0.9.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.0.8.tar", last modified: Tue Apr 23 18:01:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

