# Comparing `tmp/telegram_sleuth-0.0.1.post5.tar.gz` & `tmp/telegram_sleuth-0.0.1.post6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_sleuth-0.0.1.post5.tar", last modified: Mon Jan  8 00:18:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
