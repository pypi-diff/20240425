# Comparing `tmp/glasswall-5.2.0.tar.gz` & `tmp/glasswall-5.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glasswall-5.2.0.tar", last modified: Thu Apr 18 09:54:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

