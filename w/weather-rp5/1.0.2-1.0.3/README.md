# Comparing `tmp/weather_rp5-1.0.2.tar.gz` & `tmp/weather_rp5-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_rp5-1.0.2.tar", last modified: Tue Apr 23 19:47:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

