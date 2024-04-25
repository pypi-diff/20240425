# Comparing `tmp/argus_ticket_github-1.0.tar.gz` & `tmp/argus_ticket_github-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus_ticket_github-1.0.tar", last modified: Thu Mar 30 10:52:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

