# Comparing `tmp/barkeep-0.1.0.tar.gz` & `tmp/barkeep-0.1.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barkeep-0.1.0.tar", last modified: Mon Feb 19 22:16:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

