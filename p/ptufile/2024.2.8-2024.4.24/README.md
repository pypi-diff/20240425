# Comparing `tmp/ptufile-2024.2.8.tar.gz` & `tmp/ptufile-2024.4.24-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptufile-2024.2.8.tar", last modified: Fri Feb  9 01:23:01 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

