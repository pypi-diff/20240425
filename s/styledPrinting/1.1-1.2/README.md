# Comparing `tmp/styledPrinting-1.1.tar.gz` & `tmp/styledPrinting-1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledPrinting-1.1.tar", last modified: Wed Feb 14 16:33:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

