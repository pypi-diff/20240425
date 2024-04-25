# Comparing `tmp/spacy-transformers-1.3.4.tar.gz` & `tmp/spacy_transformers-1.3.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-transformers-1.3.4.tar", last modified: Tue Dec 19 06:29:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

